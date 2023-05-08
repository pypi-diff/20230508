# Comparing `tmp/pycons3rt3-0.0.8.tar.gz` & `tmp/pycons3rt3-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycons3rt3-0.0.8.tar", last modified: Fri Feb 12 16:27:52 2021, max compression
+gzip compressed data, was "dist/pycons3rt3-0.0.9.tar", last modified: Mon Jun  7 15:55:03 2021, max compression
```

## Comparing `pycons3rt3-0.0.8.tar` & `pycons3rt3-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-02-12 16:27:52.695972 pycons3rt3-0.0.8/
--rwxr-xr-x   0 yennaco    (501) staff       (20)      167 2019-04-06 00:04:44.000000 pycons3rt3-0.0.8/AUTHORS.txt
--rw-r--r--   0 yennaco    (501) staff       (20)     1298 2021-02-12 16:25:34.000000 pycons3rt3-0.0.8/CHANGES.txt
--rw-r--r--   0 yennaco    (501) staff       (20)    35128 2018-07-24 19:14:20.000000 pycons3rt3-0.0.8/LICENSE
--rw-r--r--   0 yennaco    (501) staff       (20)      130 2019-04-07 02:25:57.000000 pycons3rt3-0.0.8/MANIFEST.in
--rw-r--r--   0 yennaco    (501) staff       (20)    12205 2021-02-12 16:27:52.695701 pycons3rt3-0.0.8/PKG-INFO
--rw-r--r--   0 yennaco    (501) staff       (20)     9048 2019-12-12 16:15:30.000000 pycons3rt3-0.0.8/README.md
-drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-02-12 16:27:52.689691 pycons3rt3-0.0.8/pycons3rt3/
--rw-r--r--   0 yennaco    (501) staff       (20)        6 2021-02-12 16:25:33.000000 pycons3rt3-0.0.8/pycons3rt3/VERSION.txt
--rwxr-xr-x   0 yennaco    (501) staff       (20)     1433 2020-09-28 22:13:00.000000 pycons3rt3-0.0.8/pycons3rt3/__init__.py
--rwxr-xr-x   0 yennaco    (501) staff       (20)     9782 2019-08-21 19:44:05.000000 pycons3rt3-0.0.8/pycons3rt3/aliasip.py
--rw-r--r--   0 yennaco    (501) staff       (20)    36898 2020-11-18 23:05:40.000000 pycons3rt3-0.0.8/pycons3rt3/asset.py
--rw-r--r--   0 yennaco    (501) staff       (20)     8151 2021-01-21 22:51:59.000000 pycons3rt3-0.0.8/pycons3rt3/aws_metadata.py
--rw-r--r--   0 yennaco    (501) staff       (20)     1802 2020-08-31 18:46:30.000000 pycons3rt3-0.0.8/pycons3rt3/awsutil.py
--rwxr-xr-x   0 yennaco    (501) staff       (20)    61679 2021-01-16 19:33:10.000000 pycons3rt3-0.0.8/pycons3rt3/bash.py
--rw-r--r--   0 yennaco    (501) staff       (20)    12835 2020-06-09 22:50:31.000000 pycons3rt3-0.0.8/pycons3rt3/cloud.py
--rw-r--r--   0 yennaco    (501) staff       (20)     4548 2020-11-07 00:15:09.000000 pycons3rt3-0.0.8/pycons3rt3/cons3rt.py
--rw-r--r--   0 yennaco    (501) staff       (20)   241992 2021-01-19 22:59:02.000000 pycons3rt3-0.0.8/pycons3rt3/cons3rtapi.py
--rw-r--r--   0 yennaco    (501) staff       (20)    32585 2021-01-15 17:02:39.000000 pycons3rt3-0.0.8/pycons3rt3/cons3rtcli.py
--rw-r--r--   0 yennaco    (501) staff       (20)    77591 2020-12-20 07:35:33.000000 pycons3rt3-0.0.8/pycons3rt3/cons3rtclient.py
--rw-r--r--   0 yennaco    (501) staff       (20)     8466 2020-11-12 22:49:37.000000 pycons3rt3-0.0.8/pycons3rt3/cons3rtconfig.py
--rwxr-xr-x   0 yennaco    (501) staff       (20)    44292 2020-12-20 04:04:20.000000 pycons3rt3-0.0.8/pycons3rt3/deployment.py
--rw-r--r--   0 yennaco    (501) staff       (20)      626 2019-05-13 17:37:12.000000 pycons3rt3-0.0.8/pycons3rt3/dyndict.py
--rw-r--r--   0 yennaco    (501) staff       (20)   236122 2021-01-07 21:25:47.000000 pycons3rt3-0.0.8/pycons3rt3/ec2util.py
--rw-r--r--   0 yennaco    (501) staff       (20)    20126 2020-11-03 06:17:27.000000 pycons3rt3-0.0.8/pycons3rt3/elbv2util.py
--rw-r--r--   0 yennaco    (501) staff       (20)     3631 2020-12-15 00:09:25.000000 pycons3rt3-0.0.8/pycons3rt3/exceptions.py
--rw-r--r--   0 yennaco    (501) staff       (20)    25907 2020-12-20 07:25:57.000000 pycons3rt3-0.0.8/pycons3rt3/httpclient.py
--rw-r--r--   0 yennaco    (501) staff       (20)    18093 2020-07-14 14:26:30.000000 pycons3rt3-0.0.8/pycons3rt3/images.py
--rwxr-xr-x   0 yennaco    (501) staff       (20)     5035 2020-09-28 23:36:54.000000 pycons3rt3-0.0.8/pycons3rt3/logify.py
--rw-r--r--   0 yennaco    (501) staff       (20)    27118 2020-10-22 21:40:23.000000 pycons3rt3-0.0.8/pycons3rt3/mailchimp.py
--rwxr-xr-x   0 yennaco    (501) staff       (20)    24309 2019-08-17 04:08:47.000000 pycons3rt3-0.0.8/pycons3rt3/nexus.py
--rw-r--r--   0 yennaco    (501) staff       (20)     7248 2020-11-12 19:47:45.000000 pycons3rt3-0.0.8/pycons3rt3/openssl.py
--rw-r--r--   0 yennaco    (501) staff       (20)    20263 2020-11-18 22:40:34.000000 pycons3rt3-0.0.8/pycons3rt3/ostemplates.py
--rw-r--r--   0 yennaco    (501) staff       (20)     4857 2020-08-17 21:15:26.000000 pycons3rt3-0.0.8/pycons3rt3/osutil.py
--rw-r--r--   0 yennaco    (501) staff       (20)     1731 2020-04-19 22:39:12.000000 pycons3rt3-0.0.8/pycons3rt3/password.py
--rw-r--r--   0 yennaco    (501) staff       (20)     2980 2021-01-15 16:51:56.000000 pycons3rt3-0.0.8/pycons3rt3/pycons3rtlibs.py
--rw-r--r--   0 yennaco    (501) staff       (20)    10332 2020-08-05 01:14:50.000000 pycons3rt3-0.0.8/pycons3rt3/pygit.py
--rw-r--r--   0 yennaco    (501) staff       (20)     6070 2019-08-17 12:08:48.000000 pycons3rt3-0.0.8/pycons3rt3/pyjavakeys.py
--rw-r--r--   0 yennaco    (501) staff       (20)    33457 2020-09-28 16:15:20.000000 pycons3rt3-0.0.8/pycons3rt3/rdsutil.py
--rw-r--r--   0 yennaco    (501) staff       (20)     9205 2020-08-07 18:04:42.000000 pycons3rt3-0.0.8/pycons3rt3/reports.py
--rw-r--r--   0 yennaco    (501) staff       (20)    19012 2021-01-26 22:05:58.000000 pycons3rt3-0.0.8/pycons3rt3/route53util.py
--rw-r--r--   0 yennaco    (501) staff       (20)    26436 2020-05-12 15:54:46.000000 pycons3rt3-0.0.8/pycons3rt3/s3util.py
--rw-r--r--   0 yennaco    (501) staff       (20)     1987 2020-06-09 22:20:17.000000 pycons3rt3-0.0.8/pycons3rt3/scenario.py
--rw-r--r--   0 yennaco    (501) staff       (20)    11027 2021-01-15 15:47:52.000000 pycons3rt3-0.0.8/pycons3rt3/service_runner.py
--rwxr-xr-x   0 yennaco    (501) staff       (20)    12763 2020-02-24 23:14:17.000000 pycons3rt3-0.0.8/pycons3rt3/slack.py
--rw-r--r--   0 yennaco    (501) staff       (20)    18536 2020-12-10 18:39:50.000000 pycons3rt3-0.0.8/pycons3rt3/ssh.py
--rw-r--r--   0 yennaco    (501) staff       (20)     1250 2020-12-15 00:14:00.000000 pycons3rt3-0.0.8/pycons3rt3/stsutil.py
--rw-r--r--   0 yennaco    (501) staff       (20)      974 2019-08-16 22:25:09.000000 pycons3rt3-0.0.8/pycons3rt3/test_exceptions.py
--rw-r--r--   0 yennaco    (501) staff       (20)     2659 2019-08-17 18:56:23.000000 pycons3rt3-0.0.8/pycons3rt3/windows.py
-drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-02-12 16:27:52.693159 pycons3rt3-0.0.8/pycons3rt3.egg-info/
--rw-r--r--   0 yennaco    (501) staff       (20)    12205 2021-02-12 16:27:52.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/PKG-INFO
--rw-r--r--   0 yennaco    (501) staff       (20)     1376 2021-02-12 16:27:52.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/SOURCES.txt
--rw-r--r--   0 yennaco    (501) staff       (20)        1 2021-02-12 16:27:52.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/dependency_links.txt
--rw-r--r--   0 yennaco    (501) staff       (20)      194 2021-02-12 16:27:52.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/entry_points.txt
--rw-r--r--   0 yennaco    (501) staff       (20)      114 2021-02-12 16:27:52.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/requires.txt
--rw-r--r--   0 yennaco    (501) staff       (20)       11 2021-02-12 16:27:52.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/top_level.txt
--rw-r--r--   0 yennaco    (501) staff       (20)        1 2019-08-16 22:03:03.000000 pycons3rt3-0.0.8/pycons3rt3.egg-info/zip-safe
-drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-02-12 16:27:52.695052 pycons3rt3-0.0.8/sample-configs/
--rw-r--r--   0 yennaco    (501) staff       (20)      233 2021-01-04 17:25:00.000000 pycons3rt3-0.0.8/sample-configs/sample-cert-auth-config.json
--rw-r--r--   0 yennaco    (501) staff       (20)     1496 2020-11-18 22:53:42.000000 pycons3rt3-0.0.8/sample-configs/sample-multi-site.json
--rw-r--r--   0 yennaco    (501) staff       (20)      225 2020-11-18 22:48:18.000000 pycons3rt3-0.0.8/sample-configs/sample-user-auth-config.json
--rw-r--r--   0 yennaco    (501) staff       (20)       38 2021-02-12 16:27:52.696061 pycons3rt3-0.0.8/setup.cfg
--rwxr-xr-x   0 yennaco    (501) staff       (20)     1621 2020-09-28 17:29:05.000000 pycons3rt3-0.0.8/setup.py
+drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-06-07 15:55:03.036795 pycons3rt3-0.0.9/
+-rwxr-xr-x   0 yennaco    (501) staff       (20)      167 2019-04-06 00:04:44.000000 pycons3rt3-0.0.9/AUTHORS.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)     1995 2021-06-07 15:54:24.000000 pycons3rt3-0.0.9/CHANGES.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)    35128 2018-07-24 19:14:20.000000 pycons3rt3-0.0.9/LICENSE
+-rw-r--r--   0 yennaco    (501) staff       (20)      130 2019-04-07 02:25:57.000000 pycons3rt3-0.0.9/MANIFEST.in
+-rw-r--r--   0 yennaco    (501) staff       (20)    12205 2021-06-07 15:55:03.036545 pycons3rt3-0.0.9/PKG-INFO
+-rw-r--r--   0 yennaco    (501) staff       (20)     9048 2019-12-12 16:15:30.000000 pycons3rt3-0.0.9/README.md
+drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-06-07 15:55:03.028339 pycons3rt3-0.0.9/pycons3rt3/
+-rw-r--r--   0 yennaco    (501) staff       (20)        6 2021-06-07 15:53:58.000000 pycons3rt3-0.0.9/pycons3rt3/VERSION.txt
+-rwxr-xr-x   0 yennaco    (501) staff       (20)     1433 2020-09-28 22:13:00.000000 pycons3rt3-0.0.9/pycons3rt3/__init__.py
+-rwxr-xr-x   0 yennaco    (501) staff       (20)     9782 2019-08-21 19:44:05.000000 pycons3rt3-0.0.9/pycons3rt3/aliasip.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     3556 2021-04-02 16:51:42.000000 pycons3rt3-0.0.9/pycons3rt3/ansiblevault.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    39154 2021-05-24 15:28:36.000000 pycons3rt3-0.0.9/pycons3rt3/asset.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     8151 2021-01-21 22:51:59.000000 pycons3rt3-0.0.9/pycons3rt3/aws_metadata.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     1802 2020-08-31 18:46:30.000000 pycons3rt3-0.0.9/pycons3rt3/awsutil.py
+-rwxr-xr-x   0 yennaco    (501) staff       (20)    61809 2021-04-16 23:25:34.000000 pycons3rt3-0.0.9/pycons3rt3/bash.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    12835 2020-06-09 22:50:31.000000 pycons3rt3-0.0.9/pycons3rt3/cloud.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     4806 2021-03-26 14:16:04.000000 pycons3rt3-0.0.9/pycons3rt3/cons3rt.py
+-rw-r--r--   0 yennaco    (501) staff       (20)   241315 2021-05-24 15:28:35.000000 pycons3rt3-0.0.9/pycons3rt3/cons3rtapi.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    39011 2021-03-26 14:33:40.000000 pycons3rt3-0.0.9/pycons3rt3/cons3rtcli.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    77591 2020-12-20 07:35:33.000000 pycons3rt3-0.0.9/pycons3rt3/cons3rtclient.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     8466 2020-11-12 22:49:37.000000 pycons3rt3-0.0.9/pycons3rt3/cons3rtconfig.py
+-rwxr-xr-x   0 yennaco    (501) staff       (20)    44292 2020-12-20 04:04:20.000000 pycons3rt3-0.0.9/pycons3rt3/deployment.py
+-rw-r--r--   0 yennaco    (501) staff       (20)      626 2019-05-13 17:37:12.000000 pycons3rt3-0.0.9/pycons3rt3/dyndict.py
+-rw-r--r--   0 yennaco    (501) staff       (20)   253108 2021-04-08 15:23:12.000000 pycons3rt3-0.0.9/pycons3rt3/ec2util.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    20126 2020-11-03 06:17:27.000000 pycons3rt3-0.0.9/pycons3rt3/elbv2util.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     3832 2021-03-24 04:51:22.000000 pycons3rt3-0.0.9/pycons3rt3/exceptions.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    26053 2021-03-23 21:29:22.000000 pycons3rt3-0.0.9/pycons3rt3/httpclient.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    32857 2021-04-06 16:22:36.000000 pycons3rt3-0.0.9/pycons3rt3/iamutil.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    29186 2021-03-26 14:43:55.000000 pycons3rt3-0.0.9/pycons3rt3/images.py
+-rwxr-xr-x   0 yennaco    (501) staff       (20)     5035 2020-09-28 23:36:54.000000 pycons3rt3-0.0.9/pycons3rt3/logify.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    27118 2020-10-22 21:40:23.000000 pycons3rt3-0.0.9/pycons3rt3/mailchimp.py
+-rwxr-xr-x   0 yennaco    (501) staff       (20)    24309 2019-08-17 04:08:47.000000 pycons3rt3-0.0.9/pycons3rt3/nexus.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     7288 2021-04-02 16:15:43.000000 pycons3rt3-0.0.9/pycons3rt3/openssl.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    20200 2021-03-23 21:20:01.000000 pycons3rt3-0.0.9/pycons3rt3/ostemplates.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     4857 2020-08-17 21:15:26.000000 pycons3rt3-0.0.9/pycons3rt3/osutil.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     1731 2020-04-19 22:39:12.000000 pycons3rt3-0.0.9/pycons3rt3/password.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     2980 2021-01-15 16:51:56.000000 pycons3rt3-0.0.9/pycons3rt3/pycons3rtlibs.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    12002 2021-05-04 15:29:18.000000 pycons3rt3-0.0.9/pycons3rt3/pygit.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     6070 2019-08-17 12:08:48.000000 pycons3rt3-0.0.9/pycons3rt3/pyjavakeys.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    33457 2020-09-28 16:15:20.000000 pycons3rt3-0.0.9/pycons3rt3/rdsutil.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     9205 2020-08-07 18:04:42.000000 pycons3rt3-0.0.9/pycons3rt3/reports.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    19026 2021-04-09 21:11:02.000000 pycons3rt3-0.0.9/pycons3rt3/route53util.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    15281 2021-03-23 21:52:36.000000 pycons3rt3-0.0.9/pycons3rt3/s3organizer.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    40751 2021-04-06 17:34:31.000000 pycons3rt3-0.0.9/pycons3rt3/s3util.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     1987 2020-06-09 22:20:17.000000 pycons3rt3-0.0.9/pycons3rt3/scenario.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    11027 2021-01-15 15:47:52.000000 pycons3rt3-0.0.9/pycons3rt3/service_runner.py
+-rwxr-xr-x   0 yennaco    (501) staff       (20)    12763 2020-02-24 23:14:17.000000 pycons3rt3-0.0.9/pycons3rt3/slack.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    18536 2020-12-10 18:39:50.000000 pycons3rt3-0.0.9/pycons3rt3/ssh.py
+-rw-r--r--   0 yennaco    (501) staff       (20)    14335 2021-04-06 16:08:24.000000 pycons3rt3-0.0.9/pycons3rt3/stsutil.py
+-rw-r--r--   0 yennaco    (501) staff       (20)      974 2019-08-16 22:25:09.000000 pycons3rt3-0.0.9/pycons3rt3/test_exceptions.py
+-rw-r--r--   0 yennaco    (501) staff       (20)     2659 2019-08-17 18:56:23.000000 pycons3rt3-0.0.9/pycons3rt3/windows.py
+drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-06-07 15:55:03.032551 pycons3rt3-0.0.9/pycons3rt3.egg-info/
+-rw-r--r--   0 yennaco    (501) staff       (20)    12205 2021-06-07 15:55:02.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/PKG-INFO
+-rw-r--r--   0 yennaco    (501) staff       (20)     1451 2021-06-07 15:55:02.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/SOURCES.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)        1 2021-06-07 15:55:02.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/dependency_links.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)      236 2021-06-07 15:55:02.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/entry_points.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)      114 2021-06-07 15:55:02.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/requires.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)       11 2021-06-07 15:55:02.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/top_level.txt
+-rw-r--r--   0 yennaco    (501) staff       (20)        1 2019-08-16 22:03:03.000000 pycons3rt3-0.0.9/pycons3rt3.egg-info/zip-safe
+drwxr-xr-x   0 yennaco    (501) staff       (20)        0 2021-06-07 15:55:03.035410 pycons3rt3-0.0.9/sample-configs/
+-rw-r--r--   0 yennaco    (501) staff       (20)      233 2021-01-04 17:25:00.000000 pycons3rt3-0.0.9/sample-configs/sample-cert-auth-config.json
+-rw-r--r--   0 yennaco    (501) staff       (20)     1496 2020-11-18 22:53:42.000000 pycons3rt3-0.0.9/sample-configs/sample-multi-site.json
+-rw-r--r--   0 yennaco    (501) staff       (20)      225 2020-11-18 22:48:18.000000 pycons3rt3-0.0.9/sample-configs/sample-user-auth-config.json
+-rw-r--r--   0 yennaco    (501) staff       (20)       38 2021-06-07 15:55:03.036882 pycons3rt3-0.0.9/setup.cfg
+-rwxr-xr-x   0 yennaco    (501) staff       (20)     1678 2021-03-23 21:52:36.000000 pycons3rt3-0.0.9/setup.py
```

### Comparing `pycons3rt3-0.0.8/LICENSE` & `pycons3rt3-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/PKG-INFO` & `pycons3rt3-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycons3rt3
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python3 library for CONS3RT assets and API calls
 Home-page: https://github.com/cons3rt/pycons3rt3
 Author: Joe Yennaco
 Author-email: joe.yennaco@jackpinetech.com
 License: GNU GPL v3
 Description: # pycons3rt3
```

### Comparing `pycons3rt3-0.0.8/README.md` & `pycons3rt3-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/__init__.py` & `pycons3rt3-0.0.9/pycons3rt3/__init__.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/aliasip.py` & `pycons3rt3-0.0.9/pycons3rt3/aliasip.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/asset.py` & `pycons3rt3-0.0.9/pycons3rt3/asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,69 @@
         self.asset_id = asset_id
         self.site_url = site_url
 
     def __str__(self):
         return str(self.asset_dir_path)
 
 
+def download_asset(asset_id, download_dir):
+    """Downloads the specified asset ID to the specified download directory
+
+    :param asset_id: (int) ID of the asset
+    :param download_dir: (str) path of the directory to download to
+    :return: (str) path to the downloaded asset or None
+    """
+    log = logging.getLogger(mod_logger + '.validate_asset_structure')
+    c = Cons3rtApi()
+    try:
+        asset_zip = c.download_asset(asset_id=asset_id, background=False, dest_dir=download_dir, suppress_status=False,
+                                     overwrite=True)
+    except Cons3rtApiError as exc:
+        msg = 'Problem downloading asset ID [{i}] to download directory [{d}]\n{e}\n{t}'.format(
+            i=str(asset_id), d=download_dir, e=str(exc), t=traceback.format_exc())
+        log.error(msg)
+        return
+    return asset_zip
+
+
+def download_cli(args):
+    """Handles the asset download subcommand
+
+    :param args: ArgParse
+    :return: (int) 0 if successful, non-zero otherwise
+    """
+    # Determine and validate the asset ID
+    if args.id:
+        asset_id = args.id
+    else:
+        print('ERROR: Please provide the asset ID to download as the --id parameter')
+        return 1
+    if not isinstance(asset_id, int):
+        try:
+            asset_id = int(asset_id)
+        except ValueError:
+            print('ERROR: Please provide the --id args as an integer asset ID')
+            return 1
+
+    # Determine and validate the download directory
+    if args.dest_dir:
+        download_dir = args.dest_dir
+    else:
+        download_dir = os.path.join(os.path.expanduser('~'), 'Downloads')
+    if not os.path.isdir(download_dir):
+        print('ERROR: Download directory not found: {d}'.format(d=download_dir))
+        return 1
+    downloaded_asset = download_asset(asset_id=asset_id, download_dir=download_dir)
+    if not downloaded_asset:
+        print('ERROR: Problem downloading asset ID [{i}] to directory: {d}'.format(i=str(asset_id), d=download_dir))
+        return 2
+    print('Asset ID [{i}] downloaded successfully to: {z}'.format(i=str(asset_id), z=downloaded_asset))
+    return 0
+
+
 def ignore_by_extension(item_path):
     if not os.path.isfile(item_path):
         return False
     for ignore_file_extension in ignore_file_extensions:
         if item_path.endswith('.{e}'.format(e=ignore_file_extension)):
             return True
     return False
@@ -858,21 +913,22 @@
     parser.add_argument('--asset_dir', help='Path to the asset to import')
     parser.add_argument('--asset_subtype', help='Asset subtype to query on')
     parser.add_argument('--asset_type', help='Set to: containers, software')
     parser.add_argument('--category_ids', help='List of category IDs to filter on')
     parser.add_argument('--community', help='Include to retrieve community assets', action='store_true')
     parser.add_argument('--dest_dir', help='Destination directory for the asset zip (default is Downloads)')
     parser.add_argument('--expanded', help='Include to retrieve expanded info on assets', action='store_true')
+    parser.add_argument('--id', help='Asset ID to download')
     parser.add_argument('--keep', help='Include to keep the asset zip file after import/update', action='store_true')
     parser.add_argument('--latest', help='Include to only return the latest with the highest ID', action='store_true')
     parser.add_argument('--name', help='Asset name to filter on')
     parser.add_argument('--visibility', help='Set to the desired visibility')
     args = parser.parse_args()
 
-    valid_commands = ['create', 'import', 'query', 'queryids', 'update', 'validate']
+    valid_commands = ['create', 'download', 'import', 'query', 'queryids', 'update', 'validate']
     valid_commands_str = ','.join(valid_commands)
 
     # Get the command
     command = args.command.strip().lower()
 
     # Ensure the command is valid
     if command not in valid_commands:
@@ -934,14 +990,16 @@
         keep = True
 
     # Process the command
     res = 0
 
     if command == 'create':
         res = create(asset_dir=asset_dir, dest_dir=dest_dir)
+    elif command == 'download':
+        res = download_cli(args)
     elif command == 'import':
         res = import_update(asset_dir=asset_dir, dest_dir=dest_dir, import_only=True, visibility=visibility,
                             log_level='WARNING')
     elif command == 'query':
         res = query_assets_args(args)
     elif command == 'queryids':
         res = query_assets_args(args, id_only=True)
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/aws_metadata.py` & `pycons3rt3-0.0.9/pycons3rt3/aws_metadata.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/awsutil.py` & `pycons3rt3-0.0.9/pycons3rt3/awsutil.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/bash.py` & `pycons3rt3-0.0.9/pycons3rt3/bash.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,15 +454,19 @@
             continue
         try:
             env[entry[0]] = entry[1]
         except IndexError as exc:
             log.warning('Problem setting environment variable, skipping: {p}\n{e}'.format(p=env_var, e=str(exc)))
             continue
         log.debug('Added environment variable {p}={v}'.format(p=entry[0], v=entry[1]))
-    os.environ.update(env)
+    try:
+        os.environ.update(env)
+    except OSError as exc:
+        msg = 'Problem updating the environment'
+        raise CommandError(msg) from exc
     return env
 
 
 def source_env():
     """Sources environment variable files
 
     :return: None
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/cloud.py` & `pycons3rt3-0.0.9/pycons3rt3/cloud.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/cons3rt.py` & `pycons3rt3-0.0.9/pycons3rt3/cons3rt.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 """
 
 import sys
 import argparse
 
 from .cons3rtconfig import manual_config
-from .cons3rtcli import CloudCli, CloudspaceCli, ProjectCli, RunCli, TeamCli
+from .cons3rtcli import CloudCli, CloudspaceCli, DeploymentCli, ProjectCli, RunCli, TeamCli
 
 # Commands for setting up the cons3rtapi configuration
 setup_command_options = [
     'setup',
     'config',
     'configure'
 ]
 
 # List of valid CLI commands
 valid_commands = setup_command_options + [
     'cloud',
     'cloudspace',
+    'deployment',
     'project',
     'run',
     'team'
 ]
 
 # String representation of valid commands
 valid_commands_str = 'Valid commands: {c}'.format(c=', '.join(valid_commands))
@@ -38,14 +39,21 @@
 def cloudspace_cli(args, subcommands):
     c = CloudspaceCli(args, subcommands)
     if c.process_args():
         return 0
     return 1
 
 
+def deployment_cli(args, subcommands):
+    c = DeploymentCli(args, subcommands)
+    if c.process_args():
+        return 0
+    return 1
+
+
 def project_cli(args, subcommands):
     c = ProjectCli(args, subcommands)
     if c.process_args():
         return 0
     return 1
 
 
@@ -109,14 +117,16 @@
 
     if args.command in setup_command_options:
         manual_config()
     elif args.command == 'cloud':
         return cloud_cli(args, subcommands)
     elif args.command == 'cloudspace':
         return cloudspace_cli(args, subcommands)
+    elif args.command == 'deployment':
+        return deployment_cli(args, subcommands)
     elif args.command == 'project':
         return project_cli(args, subcommands)
     elif args.command == 'run':
         return run_cli(args, subcommands)
     elif args.command == 'team':
         return team_cli(args, subcommands)
     else:
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/cons3rtapi.py` & `pycons3rt3-0.0.9/pycons3rt3/cons3rtapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -2870,15 +2870,15 @@
         except Cons3rtApiError as exc:
             msg = 'Problem listing unregistered templates in VR ID {i}'.format(i=str(vr_id))
             raise Cons3rtApiError(msg) from exc
         return unregistered_templates
 
     def create_template_registration(self, vr_id, template_name, operating_system=None, display_name=None,
                                      cons3rt_agent_installed=True, container_capable=False, default_username=None,
-                                     default_password=None, has_gpu=False, license_str=None, note=None, max_cpus=20,
+                                     default_password=None, license_str=None, note=None, max_cpus=20,
                                      max_ram_mb=131072, root_disk_size_mb=102400, additional_disks=None,
                                      linux_package_manager=None, power_on_delay_override=None, powershell_version=None,
                                      linux_service_management=None):
         """Creates a template registration in the provided virtualization realm ID
 
         NOTE: This does not support special permissions
 
@@ -2886,15 +2886,14 @@
         :param template_name: (str) actual name of the template in the virtualization realm (or cons3rttemplatename tag)
         :param operating_system: (str) operating system type
         :param display_name: (str) optional display name for the template
         :param cons3rt_agent_installed: (bool) set True if cons3rt agent is installed
         :param container_capable: (bool) Set true if the OS can launch containers
         :param default_username: (str) Default template username
         :param default_password: (str) Default template password
-        :param has_gpu: (bool) Set true if this template supports GPU
         :param license_str: (str) Optional license info
         :param note: (str) Optional note
         :param max_cpus: (int) Maximum number of CPUs for the template
         :param max_ram_mb: (int) Maximum amount of RAM for the template in MB
         :param root_disk_size_mb: (int) Size of the root disk in MB
         :param additional_disks: (list) of additional disks (dict), must have capacityInMegabytes (int)
         :param linux_package_manager: (str) package manager for linux distros
@@ -2943,15 +2942,15 @@
                 disks.append(additional_disk)
 
         template = OperatingSystemTemplate(template_name=template_name, operating_system_type=operating_system)
         try:
             template_data = template.generate_registration_data(
                 display_name=display_name, cons3rt_agent_installed=cons3rt_agent_installed,
                 container_capable=container_capable, default_username=default_username,
-                default_password=default_password, has_gpu=has_gpu, license_str=license_str, note=note,
+                default_password=default_password, license_str=license_str, note=note,
                 max_cpus=max_cpus, max_ram_mb=max_ram_mb, disks=disks, linux_package_manager=linux_package_manager,
                 power_on_delay_override=power_on_delay_override, powershell_version=powershell_version,
                 linux_service_management=linux_service_management
             )
         except InvalidOperatingSystemTemplate as exc:
             msg = 'Problem generating registration data\n{e}'.format(e=str(exc))
             raise Cons3rtApiError(msg) from exc
@@ -3079,22 +3078,21 @@
         except Cons3rtApiError as exc:
             msg = 'Problem creating template subscription in VR ID {i} for template registration ID: {r}'.format(
                 r=str(template_registration_id), i=str(vr_id))
             raise Cons3rtApiError(msg) from exc
         return is_success
 
     def update_template_subscription(self, vr_id, template_subscription_id, offline, state='IN_DEVELOPMENT',
-                                     allow_gpu=False, max_cpus=20, max_ram_mb=131072):
+                                     max_cpus=20, max_ram_mb=131072):
         """Updates template subscription data in the provided virtualization realm ID
 
         :param vr_id: (int) ID of the virtualization realm
         :param template_subscription_id: (int) ID of the template subscription
         :param offline: (bool) Set True to set the template to offline, False for online
         :param state: (str) Subscription state
-        :param allow_gpu: (bool) Set True to allow GPU bindings for this template subscription
         :param max_cpus: (int) Set to the maximum number of CPUs allowed
         :param max_ram_mb: (int) Set to the maximum RAM in megabytes allowed
         :return: (dict) of template subscription data
         :raises: Cons3rtApiError
         """
         log = logging.getLogger(self.cls_logger + '.update_template_subscription')
 
@@ -3121,19 +3119,14 @@
             raise Cons3rtApiError(msg)
 
         # Ensure state is a string
         if not isinstance(state, str):
             msg = 'state arg must be a str, found: {t}'.format(t=state.__class__.__name__)
             raise Cons3rtApiError(msg)
 
-        # Ensure allow_gpu is a bool
-        if not isinstance(allow_gpu, bool):
-            msg = 'allow_gpu arg must be an bool, found: {t}'.format(t=allow_gpu.__class__.__name__)
-            raise Cons3rtApiError(msg)
-
         # Ensure the max_cpus is an int
         if not isinstance(max_cpus, int):
             try:
                 max_cpus = int(max_cpus)
             except ValueError as exc:
                 msg = 'max_cpus arg must be an Integer, found: {t}'.format(
                     t=max_cpus.__class__.__name__)
@@ -3153,15 +3146,14 @@
         if state not in valid_states:
             msg = 'Invalid state [{s}], expected: {e}'.format(s=state, e=','.join(valid_states))
             raise Cons3rtApiError(msg)
 
         # Validate the subscription data
         subscription_data = {
             'state': state,
-            'allowGpuUsage': allow_gpu,
             'maxNumCpus': max_cpus,
             'maxRamInMegabytes': max_ram_mb
         }
 
         # Update the template subscription
         log.info('Updating template subscription ID {r} in VR ID {i} with offline set to: {o} with payload: {p}'.format(
             r=str(template_subscription_id), i=str(vr_id), o=str(offline), p=str(subscription_data)))
@@ -3590,15 +3582,15 @@
 
         :param asset_id: (int) asset ID
         :param background: (bool) set True to download in the background and receive an email when ready
         :param dest_dir: (str) path to the destination directory
         :param overwrite (bool) set True to overwrite the existing file
         :param suppress_status: (bool) Set to True to suppress printing download status
         :return: (str) path to the downloaded asset zip
-        :raises: Cons3rtClientError
+        :raises: Cons3rtApiError
         """
         log = logging.getLogger(self.cls_logger + '.download_asset')
         if not dest_dir:
             dest_dir = os.path.expanduser('~')
         download_file = os.path.join(dest_dir, 'asset-{i}.zip'.format(i=str(asset_id)))
         log.info('Attempting to download asset ID: {a}'.format(a=str(asset_id)))
         try:
@@ -3607,15 +3599,15 @@
                 background=background,
                 download_file=download_file,
                 overwrite=overwrite,
                 suppress_status=suppress_status
             )
         except Cons3rtClientError as exc:
             msg = 'Problem downloading asset ID: {a}'.format(a=str(asset_id))
-            raise Cons3rtClientError(msg) from exc
+            raise Cons3rtApiError(msg) from exc
         log.info('Completed download of asset ID {a} to: {d}'.format(a=str(asset_id), d=download_file))
         return asset_zip
 
     def get_my_run_id(self):
         """From deployment properties on this host, gets the run ID
 
         cons3rt.deploymentRun.id
@@ -4991,34 +4983,30 @@
                 raise Cons3rtApiError(msg) from exc
 
             if not online:
                 log.info('Template [{n}] will not set online in VR ID: {i}'.format(n=template_name, i=str(vr_id)))
                 continue
 
             # TODO when Tracker 4459 is fixed, include the reg_details['templateData']['maxCpu']
-            has_gpu = False
             max_ram_mb = 131072
             max_cpus = 16
             if 'templateData' in reg_details.keys():
-                if 'HasGpu' in reg_details['templateData']:
-                    has_gpu = reg_details['templateData']['HasGpu']
                 if 'maxRamInMegabytes' in reg_details['templateData']:
                     max_ram_mb = reg_details['templateData']['maxRamInMegabytes']
                 if 'maxNumCpus' in reg_details['templateData']:
                     max_cpus = reg_details['templateData']['maxNumCpus']
 
             log.info('Setting template {n} online in VR ID: {i}'.format(n=template_name, i=str(vr_id)))
 
             try:
                 self.update_template_subscription(
                     vr_id=vr_id,
                     template_subscription_id=subscription['id'],
                     offline=False,
                     state='IN_DEVELOPMENT',
-                    allow_gpu=has_gpu,
                     max_cpus=max_cpus,
                     max_ram_mb=max_ram_mb
                 )
             except Cons3rtApiError as exc:
                 msg = 'Problem setting template [{n}] online in VR ID: {i}'.format(n=template_name, i=str(vr_id))
                 raise Cons3rtApiError(msg) from exc
         log.info('Completed sharing and subscribing template [{n}] from VR ID: {i}'.format(
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/cons3rtcli.py` & `pycons3rt3-0.0.9/pycons3rt3/cons3rtcli.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,30 @@
 
     @staticmethod
     def err(msg):
         print('ERROR: {m}'.format(m=msg))
         traceback.print_exc()
 
     @staticmethod
+    def print_deployments(deployment_list):
+        msg = 'ID\tName\n'
+        for deployment in deployment_list:
+            if 'id' in deployment:
+                msg += str(deployment['id'])
+            else:
+                msg += '      '
+            msg += '\t'
+            if 'name' in deployment:
+                msg += deployment['name']
+            else:
+                msg += '                '
+            msg += '\n'
+        print(msg)
+
+    @staticmethod
     def print_drs(dr_list):
         msg = 'ID\tName\t\t\t\t\t\tStatus\t\tProject\t\tCreator\n'
         for dr_info in dr_list:
 
             if 'id' in dr_info:
                 msg += str(dr_info['id'])
             else:
@@ -566,14 +582,156 @@
         elif self.args.all:
             self.c5t.share_templates_to_vrs_by_name(
                 provider_vr_id=self.args.provider_id,
                 vr_ids=self.ids
             )
 
 
+class DeploymentCli(Cons3rtCli):
+
+    def __init__(self, args, subcommands):
+        Cons3rtCli.__init__(self, args=args, subcommands=subcommands)
+        self.valid_subcommands = [
+            'list',
+            'run'
+        ]
+
+    def process_args(self):
+        if not self.validate_args():
+            return False
+        if not self.process_subcommands():
+            return False
+        return True
+
+    def process_subcommands(self):
+        if not self.subcommands:
+            return True
+        if len(self.subcommands) < 1:
+            return True
+        if self.subcommands[0] not in self.valid_subcommands:
+            self.err('Unrecognized command: {c}'.format(c=self.subcommands[0]))
+            return False
+        if self.subcommands[0] == 'list':
+            try:
+                self.list_deployments()
+            except Cons3rtCliError:
+                return False
+        if self.subcommands[0] == 'run':
+            try:
+                self.run()
+            except Cons3rtCliError:
+                return False
+        return True
+
+    def run(self):
+        if not self.ids:
+            msg = '--id or --ids arg required to specify the deployment ID(s)'
+            self.err(msg)
+            raise Cons3rtCliError(msg)
+        if len(self.subcommands) > 1:
+            run_subcommand = self.subcommands[1]
+            if run_subcommand == 'delete':
+                self.delete_runs_for_deployments()
+                return
+            elif run_subcommand == 'list':
+                self.list_runs_for_deployments()
+                return
+            elif run_subcommand == 'release':
+                self.release_runs()
+                return
+            else:
+                self.err('Unrecognized command: {c}'.format(c=run_subcommand))
+            return False
+
+    def list_deployments(self):
+        deployments = []
+        try:
+            deployments += self.c5t.list_deployments()
+        except Cons3rtApiError as exc:
+            msg = 'There was a problem listing deployments\n{e}'.format(e=str(exc))
+            self.err(msg)
+            raise Cons3rtCliError(msg) from exc
+        print('Found {n} deployments'.format(n=str(len(deployments))))
+        if len(deployments) > 0:
+            deployments = self.sort_by_id(deployments)
+            self.print_deployments(deployment_list=deployments)
+
+    def list_runs_for_deployments(self):
+        runs = []
+        for deployment_id in self.ids:
+            try:
+                runs += self.c5t.list_deployment_runs_for_deployment(deployment_id=deployment_id)
+            except Cons3rtApiError as exc:
+                msg = 'Problem listing deployment runs for deployment ID: {i}'.format(i=deployment_id)
+                self.err(msg)
+                raise Cons3rtCliError(msg) from exc
+        if len(runs) > 0:
+            runs = self.sort_by_id(runs)
+            self.print_drs(dr_list=runs)
+        print('Total number of runs found: {n}'.format(n=str(len(runs))))
+        return runs
+
+    def delete_runs_for_deployments(self):
+        runs = self.list_runs_for_deployments()
+        inactive_run_ids = []
+        for run in runs:
+            if 'id' not in run.keys():
+                print('WARN: id not found in run: {r}'.format(r=str(run)))
+                continue
+            if 'deploymentRunStatus' not in run.keys():
+                print('WARN: deploymentRunStatus not found in run: {r}'.format(r=str(run)))
+                continue
+            if run['deploymentRunStatus'] in ['CANCELED', 'COMPLETED', 'TESTED']:
+                inactive_run_ids.append(run['id'])
+        if len(inactive_run_ids) > 0:
+            inactive_run_ids = self.sort_by_id(inactive_run_ids)
+        else:
+            print('No inactive runs to delete for deployment IDs: [{i}]'.format(
+                i=','.join(map(str, self.ids))))
+            return
+        print('Deleting [{n}] inactive runs: [{i}]'.format(
+            n=str(len(inactive_run_ids)), i=','.join(map(str, inactive_run_ids))))
+        for inactive_run_id in inactive_run_ids:
+            print('Deleting inactive deployment run: {i}'.format(i=inactive_run_id))
+            self.c5t.delete_inactive_run(dr_id=inactive_run_id)
+
+    def release_runs(self):
+        runs = self.list_runs_for_deployments()
+        active_run_ids = []
+        if len(runs) > 0:
+            runs = self.sort_by_id(runs)
+        else:
+            print('No runs found to release')
+            return
+        for run in runs:
+            if 'id' not in run.keys():
+                print('WARN: id not found in run: {r}'.format(r=str(run)))
+                continue
+            if 'deploymentRunStatus' not in run.keys():
+                print('WARN: deploymentRunStatus not found in run: {r}'.format(r=str(run)))
+                continue
+            if run['deploymentRunStatus'] in ['RESERVED']:
+                active_run_ids.append(run['id'])
+        if len(active_run_ids) > 0:
+            active_run_ids = self.sort_by_id(active_run_ids)
+        else:
+            print('No active runs to release for deployment IDs: [{i}]'.format(
+                i=','.join(map(str, self.ids))))
+            return
+        print('Releasing [{n}] active runs: [{i}]'.format(
+            n=str(len(active_run_ids)), i=','.join(map(str, active_run_ids))))
+        proceed = input('These runs will not be recoverable, proceed with release? (y/n) ')
+        if not proceed:
+            return
+        if proceed != 'y':
+            return
+        for active_run_id in active_run_ids:
+            self.c5t.release_deployment_run(dr_id=active_run_id)
+
+
 class ProjectCli(Cons3rtCli):
 
     def __init__(self, args, subcommands):
         Cons3rtCli.__init__(self, args=args, subcommands=subcommands)
         self.valid_subcommands = [
             'list',
             'run'
@@ -682,34 +840,42 @@
 
     def delete_runs(self):
         runs = []
         for project_id in self.ids:
             runs += self.list_runs_for_project(project_id=project_id, search_type='SEARCH_INACTIVE')
         if len(runs) > 0:
             runs = self.sort_by_id(runs)
+        else:
+            print('No inactive runs to delete for project IDs: [{i}]'.format(
+                i=','.join(map(str, self.ids))))
+            return
         print('Total number of inactive runs found to delete: {n}'.format(n=str(len(runs))))
         for run in runs:
             self.c5t.delete_inactive_run(dr_id=run['id'])
 
     def release_runs(self):
         runs = []
         for project_id in self.ids:
             runs += self.list_runs_for_project(project_id=project_id, search_type='SEARCH_ACTIVE')
         if len(runs) > 0:
             runs = self.sort_by_id(runs)
         else:
-            print('No runs found to release')
+            print('No inactive runs to release for project IDs: [{i}]'.format(
+                i=','.join(map(str, self.ids))))
             return
-        print('Total number of inactive runs found to release: {n}'.format(n=str(len(runs))))
+        print('Total number of active runs found to release: {n}'.format(n=str(len(runs))))
         proceed = input('These runs will not be recoverable, proceed with release? (y/n) ')
         if not proceed:
             return
         if proceed != 'y':
             return
         for run in runs:
+            if 'id' not in run.keys():
+                print('WARNING: id not found in run: {r}'.format(r=str(run)))
+                continue
             self.c5t.release_deployment_run(dr_id=run['id'])
 
 
 class RunCli(Cons3rtCli):
 
     def __init__(self, args, subcommands):
         Cons3rtCli.__init__(self, args=args, subcommands=subcommands)
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/cons3rtclient.py` & `pycons3rt3-0.0.9/pycons3rt3/cons3rtclient.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/cons3rtconfig.py` & `pycons3rt3-0.0.9/pycons3rt3/cons3rtconfig.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/deployment.py` & `pycons3rt3-0.0.9/pycons3rt3/deployment.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/dyndict.py` & `pycons3rt3-0.0.9/pycons3rt3/dyndict.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/ec2util.py` & `pycons3rt3-0.0.9/pycons3rt3/ec2util.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,21 @@
 
 nat_default_size = 't3.micro'
 
 
 class EC2Util(object):
     """Utility for interacting with the AWS API
     """
-    def __init__(self, region_name=None, aws_access_key_id=None, aws_secret_access_key=None, skip_is_aws=False):
+    def __init__(self, region_name=None, aws_access_key_id=None, aws_secret_access_key=None, aws_session_token=None,
+                 skip_is_aws=False):
         self.cls_logger = mod_logger + '.EC2Util'
         try:
             self.client = get_ec2_client(region_name=region_name, aws_access_key_id=aws_access_key_id,
-                                         aws_secret_access_key=aws_secret_access_key)
+                                         aws_secret_access_key=aws_secret_access_key,
+                                         aws_session_token=aws_session_token)
         except ClientError as exc:
             msg = 'Unable to create an EC2 client'
             raise EC2UtilError(msg) from exc
         self.region = self.client.meta.region_name
         self.is_aws = False
         self.instance_id = None
         self.vpc_id = None
@@ -84,27 +86,27 @@
             elapsed_time = round(time.time() - start_time, 1)
             if elapsed_time > timeout_sec:
                 log.warning('Resource ID {i} has not passed instance status checks after {t} seconds'.format(
                     i=resource_id, t=str(timeout_sec)))
                 return False
             try:
                 if resource_id.startswith('i-'):
-                    self.client.describe_instances(InstanceIds=[resource_id])
+                    get_instance(client=self.client, instance_id=resource_id)
                 elif resource_id.startswith('subnet-'):
                     self.client.describe_subnets(SubnetIds=[resource_id])
                 elif resource_id.startswith('sg-'):
                     self.client.describe_security_groups(GroupIds=[resource_id])
                 elif resource_id.startswith('rtb-'):
                     self.client.describe_route_tables(RouteTableIds=[resource_id])
                 elif resource_id.startswith('acl-'):
                     self.client.describe_network_acls(NetworkAclIds=[resource_id])
                 elif resource_id.startswith('vpc-'):
                     self.client.describe_vpcs(VpcIds=[resource_id])
                 elif resource_id.startswith('igw-'):
-                    self.client.describe_vpcs(InternetGatewayIds=[resource_id])
+                    self.client.describe_internet_gateways(InternetGatewayIds=[resource_id])
                 else:
                     log.warning('Resource type not supported for this method: {r}'.format(r=resource_id))
                     return False
             except ClientError as exc:
                 log.info('Resource ID not found: {i}\n{e}'.format(i=resource_id, e=str(exc)))
                 continue
             else:
@@ -178,37 +180,29 @@
         log = logging.getLogger(self.cls_logger + '.get_vpc_id')
 
         # Exit if not running on AWS
         if not self.is_aws:
             log.info('This machine is not running in AWS, exiting...')
             return
 
-        if self.instance_id is None:
-            log.error('Unable to get the Instance ID for this machine')
+        if not self.instance_id:
+            log.warning('Unable to get the Instance ID for this machine')
             return
         log.info('Found Instance ID: {i}'.format(i=self.instance_id))
 
         log.info('Querying AWS to get the VPC ID...')
         try:
-            response = self.client.describe_instances(
-                    DryRun=False,
-                    InstanceIds=[self.instance_id])
+            instance = get_instance(client=self.client, instance_id=self.instance_id)
         except ClientError as exc:
-            log.error('Unable to query AWS to get info for instance {i}\n{e}'.format(
-                    i=self.instance_id, e=str(exc)))
-            return
-
-        # Get the VPC ID from the response
-        try:
-            vpc_id = response['Reservations'][0]['Instances'][0]['VpcId']
-        except KeyError:
-            log.error('Unable to get VPC ID from response: {r}'.format(r=response))
+            log.warning('Unable to query AWS to get info for instance {i}\n{e}'.format(i=self.instance_id, e=str(exc)))
             return
-        log.info('Found VPC ID: {v}'.format(v=vpc_id))
-        return vpc_id
+        if 'VpcId' in instance.keys():
+            log.info('Found VPC ID: {v}'.format(v=instance['VpcId']))
+            return instance['VpcId']
+        log.warning('Unable to get VPC ID from instance: {i}'.format(i=str(instance)))
 
     def list_available_regions(self):
         """Returns a list of available regions for this client
 
         :return: (list) available regions
         :raises: EC2UtilError
         """
@@ -1192,46 +1186,30 @@
         :param interface: Integer associated to the interface/device number
         :return: String Elastic Network Interface ID or None if not found
         :raises OSError, AWSAPIError, EC2UtilError
         """
         log = logging.getLogger(self.cls_logger + '.get_eni_id')
 
         # Get the instance-id
-        if self.instance_id is None:
-            msg = 'Instance ID not found for this machine'
-            log.error(msg)
+        if not self.instance_id:
+            msg = 'Instance ID not found for this machine, unable to determine ENI ID'
             raise OSError(msg)
-        log.info('Found instance ID: {i}'.format(i=self.instance_id))
-
-        log.debug('Querying EC2 instances...')
-        try:
-            response = self.client.describe_instances(
-                    DryRun=False,
-                    InstanceIds=[self.instance_id]
-            )
-        except ClientError as exc:
-            msg = 'Unable to query EC2 for instances'
-            log.error(msg)
-            raise AWSAPIError(msg) from exc
-        log.debug('Found instance info: {r}'.format(r=response))
+        log.info('Querying instance ID [{i}] to look for ENIs...'.format(i=self.instance_id))
+        instance = get_instance(client=self.client, instance_id=self.instance_id)
 
         # Find the ENI ID
         log.info('Looking for the ENI ID to alias...')
         eni_id = None
         try:
-            for reservation in response['Reservations']:
-                for instance in reservation['Instances']:
-                    if instance['InstanceId'] == self.instance_id:
-                        for network_interface in instance['NetworkInterfaces']:
-                            if network_interface['Attachment']['DeviceIndex'] == interface:
-                                eni_id = network_interface['NetworkInterfaceId']
+            for network_interface in instance['NetworkInterfaces']:
+                if network_interface['Attachment']['DeviceIndex'] == interface:
+                    eni_id = network_interface['NetworkInterfaceId']
         except KeyError as exc:
-            msg = 'ENI ID not found in AWS response for interface: {i}'.format(i=interface)
+            msg = 'Unable ot find ENI ID instance data: {i}'.format(i=str(instance))
             raise EC2UtilError(msg) from exc
-
         log.info('Found ENI ID: {e}'.format(e=eni_id))
         return eni_id
 
     def add_secondary_ip(self, ip_address, interface=1):
         """Adds an IP address as a secondary IP address
 
         :param ip_address: String IP address to add as a secondary IP
@@ -1576,34 +1554,35 @@
         if code != 200:
             msg = 'attach_network_interface returned invalid code: {c}'.format(c=code)
             log.error(msg)
             raise AWSAPIError(msg)
         log.info('Successfully attached ENI ID {eni} to EC2 instance ID {i}'.format(
                 eni=eni_id, i=self.instance_id))
 
-    def get_elastic_ips(self):
+    def get_elastic_ips(self, instance_id=None):
         """Returns the elastic IP info for this instance any are
         attached
 
         :return: (dict) Info about the Elastic IPs
-        :raises AWSAPIError
+        :raises EC2UtilError
         """
         log = logging.getLogger(self.cls_logger + '.get_elastic_ips')
-        instance_id = get_instance_id()
-        if instance_id is None:
-            log.error('Unable to get the Instance ID for this machine')
-            return
-        log.info('Found Instance ID: {i}'.format(i=instance_id))
+
+        # Ensure instance_id is set
+        if not instance_id:
+            if self.instance_id:
+                instance_id = self.instance_id
+            else:
+                instance_id = get_instance_id()
+        if not instance_id:
+            msg = 'Unable to determine instance ID to query for elastic IPs'
+            raise EC2UtilError(msg)
 
         log.info('Querying AWS for info about instance ID {i}...'.format(i=instance_id))
-        try:
-            instance_info = self.client.describe_instances(DryRun=False, InstanceIds=[instance_id])
-        except ClientError as exc:
-            msg = 'Unable to query AWS to get info for instance {i}'.format(i=instance_id)
-            raise AWSAPIError(msg) from exc
+        instance_info = get_instance(client=self.client, instance_id=self.instance_id)
 
         # Get the list of Public/Elastic IPs for this instance
         public_ips = []
         for network_interface in instance_info['Reservations'][0]['Instances'][0]['NetworkInterfaces']:
             network_interface_id = network_interface['NetworkInterfaceId']
             log.info('Checking ENI: {n}...'.format(n=network_interface_id))
             try:
@@ -1623,19 +1602,19 @@
 
         # Get info for each Public/Elastic IP
         try:
             address_info = self.client.describe_addresses(DryRun=False, PublicIps=public_ips)
         except ClientError as exc:
             msg = 'Unable to query AWS to get info for addresses {p}'.format(p=public_ips)
             log.error(msg)
-            raise AWSAPIError(msg) from exc
+            raise EC2UtilError(msg) from exc
         if not address_info:
             msg = 'No address info return for Public IPs: {p}'.format(p=public_ips)
             log.error(msg)
-            raise AWSAPIError(msg)
+            raise EC2UtilError(msg)
         return address_info
 
     def disassociate_elastic_ips(self):
         """For each attached Elastic IP, disassociate it
 
         :return: None
         :raises AWSAPIError
@@ -2575,52 +2554,41 @@
 
     def get_ec2_instances(self):
         """Describes the EC2 instances
 
         :return: dict containing EC2 instance data
         :raises: EC2UtilError
         """
-        log = logging.getLogger(self.cls_logger + '.get_ec2_instances')
-        log.info('Describing EC2 instances...')
-        try:
-            response = self.client.describe_instances()
-        except ClientError as exc:
-            msg = 'There was a problem describing EC2 instances'
-            raise EC2UtilError(msg) from exc
-        return response
+        return list_instances(client=self.client)
 
     def get_ebs_volumes(self):
         """Describes the EBS volumes
 
         :return: dict containing EBS volume data
         :raises EC2UtilError
         """
-        log = logging.getLogger(self.cls_logger + '.get_ebs_volumes')
-        log.info('Describing EBS volumes...')
-        try:
-            response = self.client.describe_volumes()
-        except ClientError as exc:
-            msg = 'There was a problem describing EBS volumes'
-            raise EC2UtilError(msg) from exc
-        return response
+        return list_volumes(client=self.client)
 
     def get_vpcs(self):
         """Describes the VPCs
 
         :return: dict containing VPC data
         :raises: EC2UtilError
         """
         log = logging.getLogger(self.cls_logger + '.get_vpcs')
         log.info('Describing VPCs...')
         try:
             response = self.client.describe_vpcs()
         except ClientError as exc:
             msg = 'There was a problem describing VPCs'
             raise EC2UtilError(msg) from exc
-        return response
+        if 'Vpcs' not in response.keys():
+            msg = 'Vpcs not found in response: {d}'.format(d=str(response))
+            raise EC2UtilError(msg)
+        return response['Vpcs']
 
     def retrieve_vpc(self, vpc_id):
         """Retrieve info on the provided VPC ID
 
         :param vpc_id: (str) ID of the VPC
         :return: (dict) info on the VPC
         :raises: EC2UtilError
@@ -2668,61 +2636,61 @@
                 cidr_blocks.append(cidr_block_assoc_set['CidrBlock'])
         return cidr_blocks
 
     def get_vpc_id_by_name(self, vpc_name):
         """Return the VPC ID matching the provided name or None if not found
 
         :param vpc_name: (str) name of the VPC
-        :return: (id) of the VPC or None if not found
+        :return: (dict) VPC data if found, or None if not found
         """
         log = logging.getLogger(self.cls_logger + '.get_vpc_id_by_name')
         log.info('Getting a list of VPCS...')
         try:
             vpcs = self.get_vpcs()
         except EC2UtilError as exc:
             raise EC2UtilError('Problem listing VPCs') from exc
 
         # Ensure VPCs were found
-        if 'Vpcs' not in vpcs.keys():
+        if len(vpcs) < 1:
             log.info('No VPCs found')
             return
 
         # Check eac VPC for matching name
-        log.info('Found [{n}] VPCs'.format(n=str(len(vpcs['Vpcs']))))
-        for vpc in vpcs['Vpcs']:
+        log.info('Found [{n}] VPCs'.format(n=str(len(vpcs))))
+        for vpc in vpcs:
             if 'VpcId' not in vpc.keys():
                 continue
             if 'Tags' not in vpc.keys():
                 continue
             for tag in vpc['Tags']:
                 if tag['Key'] == 'Name' and tag['Value'] == vpc_name:
                     log.info('Found VPC with name [{n}] has ID: {i}'.format(n=vpc_name, i=vpc['VpcId']))
-                    return vpc['VpcId']
+                    return vpc
         log.info('VPC with name {n} not found'.format(n=vpc_name))
 
     def create_vpc(self, vpc_name, cidr_block, amazon_ipv6_cidr=False, instance_tenancy='default', dry_run=False):
         """Creates a VPC with the provided name
 
         :param vpc_name: (str) desired VPC name
         :param cidr_block: (str) desired CIDR block for the VPC
         :param instance_tenancy: (str) default or dedicated
         :param amazon_ipv6_cidr: (bool) Set true to request an Amazon IPv6 CIDR block
         :param dry_run: (bool) Set true to dry run the call
-        :return: (str) VPC ID
+        :return: (dict) VPC data (see boto3 docs)
         """
         log = logging.getLogger(self.cls_logger + '.create_vpc')
 
         # Check for an existing VPC with the desired name
         try:
-            vpc_id = self.get_vpc_id_by_name(vpc_name=vpc_name)
+            existing_vpc = self.get_vpc_id_by_name(vpc_name=vpc_name)
         except EC2UtilError as exc:
             raise EC2UtilError('Problem checking for existing VPCs') from exc
-        if vpc_id:
-            log.info('Found existing VPC named {n} with ID: {i}'.format(n=vpc_name, i=vpc_id))
-            return vpc_id
+        if existing_vpc:
+            log.info('Found existing VPC named {n} with ID: {i}'.format(n=vpc_name, i=existing_vpc['VpcId']))
+            return existing_vpc
 
         # Create the VPC
         try:
             response = self.client.create_vpc(
                 CidrBlock=cidr_block,
                 AmazonProvidedIpv6CidrBlock=amazon_ipv6_cidr,
                 InstanceTenancy=instance_tenancy,
@@ -2745,15 +2713,15 @@
         if not self.ensure_exists(resource_id=vpc_id):
             raise EC2UtilError('Created VPC ID not found after timeout: {i}'.format(i=vpc_id))
 
         # Apply the name tag
         if not self.create_name_tag(resource_id=vpc_id, resource_name=vpc_name):
             raise EC2UtilError('Problem setting name tag for VPC ID: {i}'.format(i=vpc_id))
         log.info('Successfully created VPC name {n} with ID: {n}'.format(n=vpc_name, i=vpc_id))
-        return vpc_id
+        return response['Vpc']
 
     def add_vpc_cidr(self, vpc_id, cidr, amazon_ipv6_cidr=False):
         """Adds the provided CIDR block to the VPC
 
         :param vpc_id: (str) ID of the VPC
         :param cidr: (str) CIDR block to add
         :param amazon_ipv6_cidr: (bool)
@@ -2773,26 +2741,42 @@
             raise EC2UtilError(msg) from exc
 
     def create_usable_vpc(self, vpc_name, cidr_block):
         """Creates a VPC with a subnet that routes to an Internet Gateway, and default Network ACL and routes
 
         :param vpc_name: (str) name of the VPC
         :param cidr_block: (str) desired CIDR block
-        :return: (str) ID of the VPC that was created or configured
+        :return: (tuple) (str) ID of the VPC that was created or configured, (str) ID of the Internet Gateway
         """
         log = logging.getLogger(self.cls_logger + '.create_usable_vpc')
 
         # Create a VPC
         try:
-            vpc_id = self.create_vpc(vpc_name=vpc_name, cidr_block=cidr_block)
+            vpc = self.create_vpc(vpc_name=vpc_name, cidr_block=cidr_block)
         except EC2UtilError as exc:
             raise EC2UtilError('Problem creating a VPC') from exc
-        log.info('Created VPC ID: {i}'.format(i=vpc_id))
+        log.info('Created (or found existing) VPC ID: {i}'.format(i=vpc['VpcId']))
+
+        # Check if the VPC already has an internet gateway
+        try:
+            igs = list_internet_gateways(client=self.client)
+        except EC2UtilError as exc:
+            msg = 'Problem listing internet gateways'
+            raise EC2UtilError(msg) from exc
+
+        for ig in igs:
+            if 'Attachments' in ig.keys():
+                for attachment in ig['Attachments']:
+                    if attachment['VpcId'] == vpc['VpcId']:
+                        log.info('VPC [{v}] already has attached Internet gateway [{i}]'.format(
+                            v=vpc['VpcId'], i=ig['InternetGatewayId']))
+                        return vpc['VpcId'], ig['InternetGatewayId']
 
         # Create an Internet Gateway
+        log.info('Existing attached internet gateway not found for VPC [{v}], creating one...'.format(v=vpc['VpcId']))
         try:
             internet_gateway = self.client.create_internet_gateway(DryRun=False)
         except ClientError as exc:
             raise EC2UtilError('Problem creating Internet Gateway') from exc
 
         if 'InternetGateway' not in internet_gateway:
             raise EC2UtilError('Internet gateway was not created')
@@ -2812,20 +2796,21 @@
             raise EC2UtilError('Problem creating name tag for Internet gateway: {i}'.format(i=ig_id))
 
         # Attach the Internet gateway
         try:
             self.client.attach_internet_gateway(
                 DryRun=False,
                 InternetGatewayId=ig_id,
-                VpcId=vpc_id
+                VpcId=vpc['VpcId']
             )
         except ClientError as exc:
-            raise EC2UtilError('Problem attaching Internet gateway {i} to VPC {v}'.format(i=ig_id, v=vpc_id)) from exc
-        log.info('Successfully attach Internet gateway {i} to VPC: {v}'.format(i=ig_id, v=vpc_id))
-        return vpc_id
+            msg = 'Problem attaching Internet gateway {i} to VPC {v}'.format(i=ig_id, v=vpc['VpcId'])
+            raise EC2UtilError(msg) from exc
+        log.info('Successfully attach Internet gateway {i} to VPC: {v}'.format(i=ig_id, v=vpc['VpcId']))
+        return vpc['VpcId'], ig_id
 
     def enable_vpc_dns(self, vpc_id):
         """Sets the EnableDnsHostnames and EnableDnsSupport values to True for the VPC ID
 
         modify_vpc_attribute
 
         :param vpc_id: (str) ID of the VPC
@@ -2858,14 +2843,27 @@
         :param vpc_id: (str) VPC ID
         :param cidr: (str) subnet CIDR block
         :param availability_zone: (str) availability zone
         :return: (str) subnet ID
         :raises: EC2UtilError
         """
         log = logging.getLogger(self.cls_logger + '.create_subnet')
+
+        # Checking for existing Subnet in VOC
+        try:
+            existing_vpc_subnets = self.list_subnets(vpc_id=vpc_id)
+        except EC2UtilError as exc:
+            log.warning('Unable to list existing subnets in VPC [{v}]\n{e}'.format(v=vpc_id, e=str(exc)))
+        else:
+            for existing_vpc_subnet in existing_vpc_subnets:
+                if existing_vpc_subnet['CidrBlock'] == cidr:
+                    log.info('Found existing subnet [{s}] for VPC [{v}] with CIDR [{c}]'.format(
+                        s=existing_vpc_subnet['SubnetId'], v=vpc_id, c=cidr))
+                    return existing_vpc_subnet['SubnetId']
+
         log.info('Creating subnet in with name [{n}] in VPC ID [{v}] with CIDR: {c}'.format(
             n=name, v=vpc_id, c=cidr))
         try:
             log.info('Requesting subnet in availability zone: {z}'.format(z=availability_zone))
             if availability_zone:
                 response = self.client.create_subnet(CidrBlock=cidr, VpcId=vpc_id, DryRun=False,
                                                      AvailabilityZone=availability_zone)
@@ -4762,14 +4760,19 @@
             attachment['ResourceType'] = self.resource_type
         if self.resource_id:
             attachment['ResourceId'] = self.resource_id
         json_output['TransitGatewayAttachments'] = [attachment]
         return json_output
 
 
+############################################################################
+# Method for getting an EC2 client
+############################################################################
+
+
 def get_ec2_client(region_name=None, aws_access_key_id=None, aws_secret_access_key=None, aws_session_token=None):
     """Gets an EC2 client
 
     :return: boto3.client object
     :raises: AWSAPIError
     """
     return get_boto3_client(service='ec2', region_name=region_name, aws_access_key_id=aws_access_key_id,
@@ -5003,14 +5006,19 @@
                         route_type=route_type,
                         state=state
                     )
                 )
     return transit_routes_list
 
 
+############################################################################
+# Method for retrieving AWS Service IP addresses
+############################################################################
+
+
 def get_aws_service_ips(regions=None, include_elastic_ips=False, ipv6=False):
     """Returns a list of AWS service IP addresses
 
     Ref: https://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html#aws-ip-egress-control
 
     :param regions: (list) region IDs to include in the results (e.g. [us-gov-west-1, us-gov-east-1])
                            use the region 'GLOBAL' to include global non-region-specific ranges
@@ -5076,14 +5084,19 @@
         if candidate_ip_range in region_ips:
             region_filtered_ip_ranges.append(candidate_ip_range)
     log.info('Found {n} matching IP ranges in regions: {r}'.format(
         n=str(len(region_filtered_ip_ranges)), r=','.join(regions)))
     return region_filtered_ip_ranges
 
 
+############################################################################
+# Method for retrieving AWS Red Hat Update Server RHUI3 IP addresses
+############################################################################
+
+
 def get_aws_rhui3_ips(regions=None):
     """Returns the list of Red Hat RHUI3 IP addresses
 
     Note: GovCloud uses the US-based servers
 
     :param regions: (list) region IDs to include in the results (e.g. [us-gov-west-1, us-gov-east-1])
     :return: (list) of IP addresses
@@ -5115,7 +5128,437 @@
         for rhui3_region_ip in rhui3_region_ips:
             if validate_ip_address(rhui3_region_ip):
                 log.info('Found RHUI3 IP address for region {r}: {i}'.format(r=region, i=rhui3_region_ip))
                 rhui3_ips.append(rhui3_region_ip)
             else:
                 log.error('Invalid RHUI3 IP address returned for region {r}: {i}'.format(r=region, i=rhui3_region_ip))
     return rhui3_ips
+
+
+############################################################################
+# Methods for retrieving EC2 Instances
+############################################################################
+
+
+def list_instances_with_token(client, max_results=100, continuation_token=None):
+    """Returns a list of instances using the provided token and owner ID
+
+    :param client: boto3.client object
+    :param max_results: (int) max results to query on
+    :param continuation_token: (str) token to query on
+    :return: (dict) response object containing response data
+    """
+    if continuation_token:
+        return client.describe_instances(
+            DryRun=False,
+            MaxResults=max_results,
+            NextToken=continuation_token
+        )
+    else:
+        return client.describe_instances(
+            DryRun=False,
+            MaxResults=max_results
+        )
+
+
+def list_instances(client):
+    """Gets a list of EC2 instances in this account/region
+
+    :param client: boto3.client object
+    :return: (list)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.list_instances')
+    log.info('Getting a list of EC2 instances...')
+    instances = []
+    continuation_token = None
+    next_query = True
+    max_results = 100
+    while True:
+        if not next_query:
+            break
+        try:
+            response = list_instances_with_token(
+                client=client,
+                max_results=max_results,
+                continuation_token=continuation_token
+            )
+        except ClientError as exc:
+            msg = 'Problem querying for EC2 instances'
+            raise EC2UtilError(msg) from exc
+        if 'Reservations' not in response.keys():
+            log.warning('Reservations not found in response: {r}'.format(r=str(response.keys())))
+            return instances
+        if 'NextToken' not in response.keys():
+            next_query = False
+        else:
+            continuation_token = response['NextToken']
+        for reservation in response['Reservations']:
+            if 'Instances' not in reservation.keys():
+                log.warning('Instances not found in reservation: {r}'.format(r=str(reservation)))
+                continue
+            instances += reservation['Instances']
+    log.info('Found {n} EC2 instances'.format(n=str(len(instances))))
+    return instances
+
+
+def list_instance_names(client):
+    """Gets a list of EC2 instances that have name tags, and returns the list of names
+
+    :param client: boto3.client object
+    :return: (list) of (str) "Name" tag values, if any
+    """
+    log = logging.getLogger(mod_logger + '.list_instance_names')
+    instance_names = []
+    instances = list_instances(client=client)
+    log.info('Looking for instances with the Name tag set...')
+    for instance in instances:
+        if 'Tags' not in instance.keys():
+            continue
+        for tag in instance['Tags']:
+            if tag['Key'] == 'Name':
+                instance_names.append(tag['Value'])
+                log.info('Found instance with Name tag: {v}'.format(v=tag['Value']))
+    return instance_names
+
+
+def get_instance(client, instance_id):
+    """Returns detailed info about the instance ID
+
+    :param client: boto3.client object
+    :param instance_id: (str) ID of the snapshot to retrieve
+    :return: (dict) data about the snapshot (see boto3 docs)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.get_instance')
+    log.info('Getting info about instance ID: {i}'.format(i=instance_id))
+    try:
+        response = client.describe_instances(DryRun=False, SnapshotIds=[instance_id])
+    except ClientError as exc:
+        msg = 'Unable to describe instance ID: {a}'.format(a=instance_id)
+        raise EC2UtilError(msg) from exc
+    if 'Reservations' not in response.keys():
+        msg = 'Reservations not found in response: {r}'.format(r=str(response))
+        raise EC2UtilError(msg)
+    reservations = response['Reservations']
+    if not isinstance(reservations, list):
+        msg = 'Expected Reservations to be a list, found: {t}'.format(t=reservations.__class__.__name__)
+        raise EC2UtilError(msg)
+    instances = []
+    for reservation in reservations:
+        if 'Instances' not in reservation.keys():
+            msg = 'Instances not found in reservation: {r}'.format(r=str(reservation))
+            raise EC2UtilError(msg)
+        if not isinstance(reservation['Instances'], list):
+            msg = 'Expected Instances to be a list, found: {t}'.format(t=reservation['Instances'].__class__.__name__)
+            raise EC2UtilError(msg)
+        instances += reservation['Instances']
+    if len(instances) != 1:
+        msg = 'Expected to find 1 instance, found: {n}'.format(n=str(len(instances)))
+        raise EC2UtilError(msg)
+    return instances[0]
+
+
+############################################################################
+# Methods for retrieving EC2 Snapshots
+############################################################################
+
+
+def list_snapshots_with_token(client, owner_id, max_results=100, continuation_token=None):
+    """Returns a list of snapshots using the provided token and owner ID
+
+    :param client: boto3.client object
+    :param owner_id: (str) owner ID for the account
+    :param max_results: (int) max results to query on
+    :param continuation_token: (str) token to query on
+    :return: (dict) response object containing response data
+    """
+    if continuation_token:
+        return client.describe_snapshots(
+            DryRun=False,
+            MaxResults=max_results,
+            NextToken=continuation_token,
+            OwnerIds=[owner_id]
+        )
+    else:
+        return client.describe_snapshots(
+            DryRun=False,
+            MaxResults=max_results,
+            OwnerIds=[owner_id]
+        )
+
+
+def list_snapshots(client, owner_id):
+    """Gets a list of EC2 snapshots in this account/region
+
+    :param client: boto3.client object
+    :param owner_id: (str) ID of the account to search
+    :return: (list)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.list_snapshots')
+    log.info('Getting a list of EC2 snapshots in account ID: {i}'.format(i=owner_id))
+    snapshots = []
+    continuation_token = None
+    next_query = True
+    max_results = 100
+    while True:
+        if not next_query:
+            break
+        try:
+            response = list_snapshots_with_token(
+                client=client,
+                owner_id=owner_id,
+                max_results=max_results,
+                continuation_token=continuation_token
+            )
+        except ClientError as exc:
+            msg = 'Problem querying for EC2 snapshots'
+            raise EC2UtilError(msg) from exc
+        if 'Snapshots' not in response.keys():
+            log.warning('Snapshots not found in response: {r}'.format(r=str(response.keys())))
+            return snapshots
+        if 'NextToken' not in response.keys():
+            next_query = False
+        else:
+            continuation_token = response['NextToken']
+        snapshots += response['Snapshots']
+    log.info('Found {n} EC2 snapshots'.format(n=str(len(snapshots))))
+    return snapshots
+
+
+def get_snapshot(client, snapshot_id):
+    """Returns detailed info about the snapshot ID
+
+    :param client: boto3.client object
+    :param snapshot_id: (str) ID of the snapshot to retrieve
+    :return: (dict) data about the snapshot (see boto3 docs)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.get_snapshot')
+    log.info('Getting info about snapshot ID: {i}'.format(i=snapshot_id))
+    try:
+        response = client.describe_snapshots(DryRun=False, SnapshotIds=[snapshot_id])
+    except ClientError as exc:
+        msg = 'Unable to describe snapshot ID: {a}'.format(a=snapshot_id)
+        raise EC2UtilError(msg) from exc
+    if 'Snapshots' not in response:
+        msg = 'Snapshots not found in response: {r}'.format(r=str(response))
+        raise EC2UtilError(msg)
+    snapshots = response['Snapshots']
+    if not isinstance(snapshots, list):
+        msg = 'Expected Snapshots to be a list, found: {t}'.format(t=snapshots.__class__.__name__)
+        raise EC2UtilError(msg)
+    if len(snapshots) != 1:
+        msg = 'Expected to find 1 snapshot, found: {n}'.format(n=str(len(snapshots)))
+        raise EC2UtilError(msg)
+    return snapshots[0]
+
+
+############################################################################
+# Methods for retrieving EC2 AMIs / Images
+############################################################################
+
+
+def list_images(client, owner_id):
+    """Gets a list of EC2 snapshots in this account/region
+
+    :param client: boto3.client object
+    :param owner_id: (str) ID of the account to search
+    :return: (list)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.list_images')
+    log.info('Getting a list of EC2 images/AMIs in account ID: {i}'.format(i=owner_id))
+    try:
+        response = client.describe_images(
+            DryRun=False,
+            Owners=[owner_id]
+        )
+    except ClientError as exc:
+        msg = 'Problem querying for EC2 images'
+        raise EC2UtilError(msg) from exc
+    if 'Images' not in response.keys():
+        msg = 'Images not found in response: {r}'.format(r=str(response.keys()))
+        raise EC2UtilError(msg)
+    images = response['Images']
+    log.info('Found {n} EC2 images'.format(n=str(len(images))))
+    return images
+
+
+def get_image(client, ami_id):
+    """Returns detailed info about the AMI ID
+
+    :param client: boto3.client object
+    :param ami_id: (str) ID of the AMI to retrieve
+    :return: (dict) data about the AMI (see boto3 docs)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.get_image')
+    log.info('Getting info about AMI ID: {i}'.format(i=ami_id))
+    try:
+        response = client.describe_images(DryRun=False, ImageIds=[ami_id])
+    except ClientError as exc:
+        msg = 'Unable to describe image ID: {a}'.format(a=ami_id)
+        raise EC2UtilError(msg) from exc
+    if 'Images' not in response:
+        msg = 'Images not found in response: {r}'.format(r=str(response))
+        raise EC2UtilError(msg)
+    if len(response['Images']) != 1:
+        msg = 'Expected to find 1 image, found {n} in response: {r}'.format(
+            n=str(len(response['Images'])), r=str(response))
+        raise EC2UtilError(msg)
+    return response['Images'][0]
+
+
+############################################################################
+# Methods for retrieving EC2 Volumes
+############################################################################
+
+
+def list_volumes_with_token(client, max_results=100, continuation_token=None):
+    """Returns a list of volumes using the provided token
+
+    :param client: boto3.client object
+    :param max_results: (int) max results to query on
+    :param continuation_token: (str) token to query on
+    :return: (dict) response object containing response data
+    """
+    if continuation_token:
+        return client.describe_volumes(
+            DryRun=False,
+            MaxResults=max_results,
+            NextToken=continuation_token
+        )
+    else:
+        return client.describe_volumes(
+            DryRun=False,
+            MaxResults=max_results
+        )
+
+
+def list_volumes(client):
+    """Gets a list of EC2 volumes in this account/region
+
+    :param client: boto3.client object
+    :return: (list)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.list_volumes')
+    log.info('Getting a list of EC2 volumes...')
+    volumes = []
+    continuation_token = None
+    next_query = True
+    max_results = 100
+    while True:
+        if not next_query:
+            break
+        try:
+            response = list_volumes_with_token(
+                client=client,
+                max_results=max_results,
+                continuation_token=continuation_token
+            )
+        except ClientError as exc:
+            msg = 'Problem querying for EC2 volumes'
+            raise EC2UtilError(msg) from exc
+        if 'Volumes' not in response.keys():
+            log.warning('Volumes not found in response: {r}'.format(r=str(response.keys())))
+            return volumes
+        if 'NextToken' not in response.keys():
+            next_query = False
+        else:
+            continuation_token = response['NextToken']
+        volumes += response['Volumes']
+    log.info('Found {n} EC2 volumes'.format(n=str(len(volumes))))
+    return volumes
+
+
+def get_volume(client, volume_id):
+    """Returns detailed info about the volume ID
+
+    :param client: boto3.client object
+    :param volume_id: (str) ID of the volume to retrieve
+    :return: (dict) data about the volume (see boto3 docs)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.get_volume')
+    log.info('Getting info about volume ID: {i}'.format(i=volume_id))
+    try:
+        response = client.describe_volumes(DryRun=False, VolumeIds=[volume_id])
+    except ClientError as exc:
+        msg = 'Unable to describe volume ID: {a}'.format(a=volume_id)
+        raise EC2UtilError(msg) from exc
+    if 'Volumes' not in response:
+        msg = 'Volumes not found in response: {r}'.format(r=str(response))
+        raise EC2UtilError(msg)
+    volumes = response['Volumes']
+    if not isinstance(volumes, list):
+        msg = 'Expected Volumes to be a list, found: {t}'.format(t=volumes.__class__.__name__)
+        raise EC2UtilError(msg)
+    if len(volumes) != 1:
+        msg = 'Expected to find 1 volume, found: {n}'.format(n=str(len(volumes)))
+        raise EC2UtilError(msg)
+    return volumes[0]
+
+
+############################################################################
+# Methods for retrieving internet gateways
+############################################################################
+
+
+def list_internet_gateways_with_token(client, max_results=100, continuation_token=None):
+    """Returns a list of internet gateways using the provided token
+
+    :param client: boto3.client object
+    :param max_results: (int) max results to query on
+    :param continuation_token: (str) token to query on
+    :return: (dict) response object containing response data
+    """
+    if continuation_token:
+        return client.describe_internet_gateways(
+            DryRun=False,
+            MaxResults=max_results,
+            NextToken=continuation_token
+        )
+    else:
+        return client.describe_internet_gateways(
+            DryRun=False,
+            MaxResults=max_results
+        )
+
+
+def list_internet_gateways(client):
+    """Gets a list of internet gateways in this account/region
+
+    :param client: boto3.client object
+    :return: (list)
+    :raises: EC2UtilError
+    """
+    log = logging.getLogger(mod_logger + '.list_internet_gateways')
+    log.info('Getting a list of internet gateways...')
+    internet_gateways = []
+    continuation_token = None
+    next_query = True
+    max_results = 100
+    while True:
+        if not next_query:
+            break
+        try:
+            response = list_internet_gateways_with_token(
+                client=client,
+                max_results=max_results,
+                continuation_token=continuation_token
+            )
+        except ClientError as exc:
+            msg = 'Problem querying for internet gateways'
+            raise EC2UtilError(msg) from exc
+        if 'InternetGateways' not in response.keys():
+            log.warning('InternetGateways not found in response: {r}'.format(r=str(response.keys())))
+            return internet_gateways
+        if 'NextToken' not in response.keys():
+            next_query = False
+        else:
+            continuation_token = response['NextToken']
+        internet_gateways += response['InternetGateways']
+    log.info('Found {n} internet gateways'.format(n=str(len(internet_gateways))))
+    return internet_gateways
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/elbv2util.py` & `pycons3rt3-0.0.9/pycons3rt3/elbv2util.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/exceptions.py` & `pycons3rt3-0.0.9/pycons3rt3/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,28 +143,36 @@
 
 
 class EC2UtilError(Exception):
     """There was a problem with an AWS EC2 operation"""
 
 
 class ElbUtilError(Exception):
-    """There was a problem with an AWS EC2 operation"""
+    """There was a problem with an AWS ELB operation"""
+
+
+class IamUtilError(Exception):
+    """There was a problem with an AWS IAM operation"""
 
 
 class ImageUtilError(Exception):
-    """There was a problem with an AWS AMI operation"""
+    """There was a problem with an AWS EC2 AMI/snapshot/volume operation"""
 
 
 class RdsUtilError(Exception):
     """There was a problem with an AWS RDS operation"""
 
 
 class Route53UtilError(Exception):
     """There was a problem with an AWS Route53 operation"""
 
 
+class S3OrganizationError(Exception):
+    """Handles Errors deleting and organizing S3"""
+
+
 class S3UtilError(Exception):
     """There was a problem with an AWS S3 operation"""
 
 
 class StsUtilError(Exception):
     """There was a problem with an AWS STS operation"""
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/httpclient.py` & `pycons3rt3-0.0.9/pycons3rt3/httpclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,17 @@
         # Otherwise use data provided as content
         elif content_data:
             content = content_data
 
         # Add content type if content was provided
         if content:
             headers['Content-Type'] = '{t}'.format(t=content_type)
+            log.debug('Making POST with content:\n{c}'.format(c=str(content)))
+        else:
+            log.debug('Making POST with no content')
 
         # Make the POST request
         attempt_num = 1
         err_msg_tally = ''
         while True:
             if attempt_num >= self.max_retry_attempts:
                 msg = 'Max attempts exceeded: {n}\n{e}'.format(n=str(self.max_retry_attempts), e=err_msg_tally)
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/logify.py` & `pycons3rt3-0.0.9/pycons3rt3/logify.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/mailchimp.py` & `pycons3rt3-0.0.9/pycons3rt3/mailchimp.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/nexus.py` & `pycons3rt3-0.0.9/pycons3rt3/nexus.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/openssl.py` & `pycons3rt3-0.0.9/pycons3rt3/openssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,39 +70,39 @@
             f=decrypted_file, p=password_file)) from exc
     if result['code'] != 0:
         raise CommandError('openssl exited with code: {c}'.format(c=str(result['code'])))
     log.info('Created decrypted file: {d}'.format(d=decrypted_file))
     return True
 
 
-def openssl_smime_decrypt(encrypted_file, decrypted_file, key_file):
+def openssl_smime_decrypt(encrypted_file, decrypted_file, password_file):
     """Decrypts a file using openssl smime and a password file
 
     # From Otto
     openssl smime -decrypt -md sha512 -binary -in $DIR/cons3rt-otto.enc -inform DER -out $DIR/cons3rt-otto.txt
     -inkey $DIR/`basename $ENC_CRT`.key
 
     :param encrypted_file: (str) path to encrypted file
     :param decrypted_file: (str) path to decrypted file
-    :param key_file: (str) path to the key file for decryption
+    :param password_file: (str) path to the key file for decryption
     :return: True (if successful)
     :raises: CommandError
     """
     log = logging.getLogger(mod_logger + '.openssl_smime_decrypt')
-    if not os.path.isfile(key_file):
-        raise CommandError('Key file not found: {f}'.format(f=key_file))
+    if not os.path.isfile(password_file):
+        raise CommandError('Password file not found: {f}'.format(f=password_file))
     if not os.path.isfile(encrypted_file):
         raise CommandError('Encrypted file not found: {f}'.format(f=encrypted_file))
     command = ['openssl', 'smime', '-decrypt', '-md', 'sha512', '-binary', '-in', encrypted_file, '-inform', 'DER',
-               '-out', decrypted_file, '-inkey', key_file]
+               '-out', decrypted_file, '-inkey', password_file]
     try:
         result = run_command(command, timeout_sec=10.0)
     except CommandError as exc:
-        raise CommandError('Problem decrypting file {f} with key file: {p}'.format(
-            f=decrypted_file, p=key_file)) from exc
+        raise CommandError('Problem decrypting file {f} with password file: {p}'.format(
+            f=decrypted_file, p=password_file)) from exc
     if result['code'] != 0:
         raise CommandError('openssl exited with code: {c}'.format(c=str(result['code'])))
     log.info('Created decrypted file: {d}'.format(d=decrypted_file))
     return True
 
 
 def openssl_encrypt(decrypted_file, password_file, encrypted_file=None):
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/ostemplates.py` & `pycons3rt3-0.0.9/pycons3rt3/ostemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 class OperatingSystemTemplate(object):
 
     def __init__(self, template_name, operating_system_type):
         self.template_name = template_name
         self.operating_system_type = operating_system_type
         self.registration_data = {}
         self.required_args = [
-            'cons3rt_agent_installed', 'container_capable', 'has_gpu', 'max_cpus', 'max_ram_mb'
+            'cons3rt_agent_installed', 'container_capable', 'max_cpus', 'max_ram_mb'
         ]
         self.root_disk_size = 102400
         self.additional_disks = []
         self.disks = []
         self.remote_access_templates = []
 
     def is_valid_operating_system_type(self):
@@ -322,15 +322,14 @@
         # Build the template registration data
         template_data = {
             'displayName': self.template_name,
             'virtRealmTemplateName': self.template_name,
             'operatingSystem': self.operating_system_type,
             'cons3rtAgentInstalled': kwargs['cons3rt_agent_installed'],
             'containerCapable': kwargs['container_capable'],
-            'hasGpu': kwargs['has_gpu'],
             'maxNumCpus': kwargs['max_cpus'],
             'maxRamInMegabytes': kwargs['max_ram_mb'],
             'disks': self.disks
         }
 
         # Add registration data that can be enumerated
         template_data['packageManagementType'] = OperatingSystemType.get_linux_package_manager(
@@ -388,15 +387,15 @@
         for required_arg in self.required_args:
             if required_arg not in kwargs.keys():
                 missing_required_args.append(required_arg)
         if len(missing_required_args) > 0:
             msg = 'Missing required args: {a}'.format(a=','.join(missing_required_args))
             raise InvalidOperatingSystemTemplate(msg)
 
-        arg_bools = ['cons3rt_agent_installed', 'container_capable', 'has_gpu']
+        arg_bools = ['cons3rt_agent_installed', 'container_capable']
         for arg_bool in arg_bools:
             if not kwargs[arg_bool]:
                 continue
             if arg_bool in kwargs.keys():
                 if not isinstance(kwargs[arg_bool], bool):
                     msg = '{b} must be a bool, found: {t}'.format(b=arg_bool, t=type(kwargs[arg_bool]).__name__)
                     raise InvalidOperatingSystemTemplate(msg)
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/osutil.py` & `pycons3rt3-0.0.9/pycons3rt3/osutil.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/password.py` & `pycons3rt3-0.0.9/pycons3rt3/password.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/pycons3rtlibs.py` & `pycons3rt3-0.0.9/pycons3rt3/pycons3rtlibs.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/pygit.py` & `pycons3rt3-0.0.9/pycons3rt3/pygit.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """Module: pygit
 
 This module provides utilities for performing git operations
 
 """
 import logging
+import shutil
 import os
 import time
 
 from .logify import Logify
 from .bash import run_command, mkdir_p
 from .exceptions import CommandError, PyGitError
 
@@ -35,14 +36,50 @@
         raise PyGitError('Unable to find the git executable') from exc
     git_cmd = result['output']
     if not os.path.isfile(git_cmd):
         raise PyGitError('Could not find git command: {g}'.format(g=git_cmd))
     return git_cmd
 
 
+def git_status(git_repo_dir):
+    """Determines whether the git repo is in a good state
+
+    :param git_repo_dir: (str) path to the git clone directory
+    :return: True if git status returns 0, False otherwise
+    """
+    log = logging.getLogger(mod_logger + '.git_status')
+
+    # Get the git command executable
+    try:
+        git_cmd = get_git_cmd()
+    except PyGitError as exc:
+        log.error('git command not found, cannot run git status\n{e}'.format(e=str(exc)))
+        return False
+    command = [git_cmd, 'status']
+    cwd = os.getcwd()
+    os.chdir(git_repo_dir)
+
+    # Run git status and check the exit code
+    log.info('Running git status on directory: {d}'.format(d=git_repo_dir))
+    success = False
+    try:
+        result = run_command(command)
+    except CommandError as exc:
+        log.error('There was a problem running the git command: {c}\n{e}'.format(c=command, e=str(exc)))
+    else:
+        if result['code'] != 0:
+            log.warning('The git command {g} failed and returned exit code: {c}\n{o}'.format(
+                g=command, c=result['code'], o=result['output']))
+        else:
+            log.info('git status returned successfully with output: {o}'.format(o=result['output']))
+            success = True
+    os.chdir(cwd)
+    return success
+
+
 def git_clone(url, clone_dir, branch='master', username=None, password=None, max_retries=10, retry_sec=30,
               git_cmd=None, git_lfs=False):
     """Clones a git url
 
     :param url: (str) Git URL in https or ssh
     :param clone_dir: (str) Path to the desired destination dir
     :param branch: (str) branch to clone
@@ -87,56 +124,70 @@
     # Find the git command
     if git_cmd is None:
         try:
             git_cmd = get_git_cmd()
         except PyGitError as exc:
             raise PyGitError('git command not found, cannot run clone') from exc
 
-    # Build a git clone or git pull command based on the existence of the clone directory
-    if os.path.isdir(os.path.join(clone_dir, '.git')):
-        log.debug('Git repo directory already exists, updating repo in: {d}'.format(d=clone_dir))
-        os.chdir(clone_dir)
-        command = [git_cmd, 'pull']
+    # Build a git clone or git pull command based on the existence of the clone directory and if it had a good
+    # previous clone
+    do_empty = False
+    pull = False
+    if os.path.isdir(clone_dir):
+        if git_status(git_repo_dir=clone_dir):
+            pull = True
+        else:
+            do_empty = True
     else:
         # Create a subdirectory to clone into
         log.debug('Creating the repo directory: {d}'.format(d=clone_dir))
         try:
             mkdir_p(clone_dir)
         except CommandError as exc:
             msg = 'Unable to create source directory: {d}'.format(d=clone_dir)
             raise PyGitError(msg) from exc
 
-        # Create the git clone command
+    # Create the git clone command
+    if pull:
+        os.chdir(clone_dir)
+        command = [git_cmd, 'pull']
+    else:
         if git_lfs:
             command = [git_cmd, 'lfs']
         else:
             command = [git_cmd]
         command += ['clone', '-b', branch, clone_url, clone_dir]
 
     # Run the git command
     log.info('Running git command: {c}'.format(c=command))
     for i in range(max_retries):
         attempt_num = i + 1
-        log.info('Attempt #{n} to git clone the repository...'.format(n=attempt_num))
+        log.info('Attempt #{n} of {m} to git clone the repository...'.format(n=str(attempt_num), m=str(max_retries)))
+
+        # Empty the directory if it has contents but not a good clone
+        if not pull and os.path.isdir(clone_dir):
+            log.info('Removing existing directory: {d}'.format(d=clone_dir))
+            shutil.rmtree(clone_dir)
+
         try:
             result = run_command(command)
         except CommandError as exc:
             log.warning('There was a problem running the git command: {c}\n{e}'.format(c=command, e=str(exc)))
         else:
             if result['code'] != 0:
                 log.warning('The git command {g} failed and returned exit code: {c}\n{o}'.format(
                     g=command, c=result['code'], o=result['output']))
             else:
-                log.info('Successfully cloned/updated GIT repo: {u}'.format(u=url))
+                log.info('Successfully cloned/pulled git repo: {u}'.format(u=url))
                 return
         if attempt_num == max_retries:
-            msg = 'Attempted unsuccessfully to clone the git repo after {n} attempts'.format(n=attempt_num)
+            msg = 'Attempted unsuccessfully to clone/pull the git repo after {n} attempts'.format(n=attempt_num)
             log.error(msg)
             raise PyGitError(msg)
-        log.info('Waiting to retry the git clone in {t} seconds...'.format(t=retry_sec))
+        log.info('Waiting to retry the git clone/pull in {t} seconds...'.format(t=retry_sec))
         time.sleep(retry_sec)
 
 
 def git_pull(git_repo_dir):
     """Pulls the latest got on the current branch
 
     :param git_repo_dir: (str) path to the git repo directory
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/pyjavakeys.py` & `pycons3rt3-0.0.9/pycons3rt3/pyjavakeys.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/rdsutil.py` & `pycons3rt3-0.0.9/pycons3rt3/rdsutil.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/reports.py` & `pycons3rt3-0.0.9/pycons3rt3/reports.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/route53util.py` & `pycons3rt3-0.0.9/pycons3rt3/route53util.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             else:
                 hosted_zone = create_public_hosted_zone(
                     client=self.client, domain=self.domain
                 )
         except Route53UtilError as exc:
             msg = 'Problem creating hosted zone: {d}'.format(d=self.domain)
             raise Route53UtilError(msg) from exc
-        self.hosted_zone_id = hosted_zone['HostedZone']['Id']
+        self.hosted_zone_id = hosted_zone['Id']
         return hosted_zone
 
     def delete_record(self, record_type, name, value):
         """Returns a formatted simple record for adding to Route53
 
         :param record_type: (str) type of record (see boto3 docs)
         :param name: (str) name of the record to create (e.g. www)
@@ -282,15 +282,15 @@
     if 'HostedZone' not in response.keys():
         msg = 'HostedZone not found in response: {r}'.format(r=str(response))
         raise Route53UtilError(msg)
     if 'Id' not in response['HostedZone'].keys():
         msg = 'Id not found in HostedZone data: {d}'.format(d=str(response['HostedZone']))
         raise Route53UtilError(msg)
     log.info('Created private hosted zone: {d}'.format(d=domain))
-    return response
+    return response['HostedZone']
 
 
 def create_public_hosted_zone(client, domain, comment=''):
     """Creates a public hosted zone
 
     :param client: Route53 client object
     :param domain: (str) domain name / FQDN
@@ -316,15 +316,15 @@
     if 'HostedZone' not in response.keys():
         msg = 'HostedZone not found in response: {r}'.format(r=str(response))
         raise Route53UtilError(msg)
     if 'Id' not in response['HostedZone'].keys():
         msg = 'Id not found in HostedZone data: {d}'.format(d=str(response['HostedZone']))
         raise Route53UtilError(msg)
     log.info('Created public hosted zone: {d}'.format(d=domain))
-    return response
+    return response['HostedZone']
 
 
 def create_simple_change_record(record_type, name, value, action='UPSERT', time_to_live=300):
     """Returns a formatted simple record for adding to Route53
     
     :param record_type: (str) type of record (see boto3 docs)
     :param name: (str) name of the record to create (e.g. www)
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/s3util.py` & `pycons3rt3-0.0.9/pycons3rt3/s3util.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,26 +10,28 @@
     S3Util: Provides a set of useful utilities for accessing S3 buckets
         in for finding, downloading and uploading objects.
 
     S3UtilError: Custom exception for raised when there is a problem
         connecting to S3, or a problem with a download or upload
         operation.
 """
+import json
 import logging
 import re
 import os
 import socket
 import threading
 import time
 
 import boto3
 from botocore.client import ClientError
 from botocore.exceptions import EndpointConnectionError
 from s3transfer.exceptions import RetriesExceededError
 
+from .awsutil import get_boto3_client
 from .logify import Logify
 from .exceptions import S3UtilError
 
 __author__ = 'Joe Yennaco'
 
 
 # Set up logger name for this module
@@ -457,14 +459,112 @@
         except ClientError as exc:
             log.debug('Unable to copy key [{k}] to bucket: {b}\n{e}'.format(k=current_key, b=target_bucket, e=str(exc)))
             return False
         log.debug('Successfully copied key [{k}] to bucket {b}: {n}'.format(k=current_key, b=target_bucket, n=new_key))
         return True
 
 
+############################################################################
+# Methods for blocking public access
+############################################################################
+
+
+def block_public_access(client, bucket_name, block_public_acls=True, ignore_public_acls=True, block_public_policy=True,
+                        restrict_public_buckets=True):
+    """Enabled bucket encryption
+
+    :param client: boto3.client
+    :param bucket_name: (str) bucket name
+    :param block_public_acls: (bool) Specifies whether Amazon S3 should block public access control lists (ACLs) for
+        this bucket and objects in this bucket
+    :param ignore_public_acls: (bool) Specifies whether Amazon S3 should ignore public ACLs for this bucket and
+        objects in this bucket
+    :param block_public_policy: (bool) Specifies whether Amazon S3 should block public bucket policies for this bucket
+    :param restrict_public_buckets: (bool) Specifies whether Amazon S3 should restrict public bucket policies for this
+        bucket
+    :return: None
+    :raises: S3UtilError
+    """
+    log = logging.getLogger(mod_logger + '.block_public_access')
+    msg = 'For bucket [{n}], setting Block Public ACLs to [{b}], Ignore Public ACLs to [{i}], BlockPublic Policy to ' \
+          '[{c}], and Restrict Public Buckets to [{r}]'.format(n=bucket_name, b=block_public_acls, i=ignore_public_acls,
+                                                               c=block_public_policy, r=restrict_public_buckets)
+    log.info(msg)
+    try:
+        client.put_public_access_block(
+            Bucket=bucket_name,
+            PublicAccessBlockConfiguration={
+                'BlockPublicAcls': block_public_acls,
+                'IgnorePublicAcls': ignore_public_acls,
+                'BlockPublicPolicy': block_public_policy,
+                'RestrictPublicBuckets': restrict_public_buckets
+            }
+        )
+    except ClientError as exc:
+        msg = 'Problem setting block public access on [{n}]'.format(n=bucket_name)
+        raise S3UtilError(msg) from exc
+
+
+############################################################################
+# Methods for creating S3 buckets
+############################################################################
+
+
+def create_bucket(client, bucket_name, region='us-east-1'):
+    """Creates the specified bucket, if it already exists returns it
+
+    Default configuration is set up
+
+    :param client: boto3.client object
+    :param bucket_name: (str) bucket name
+    :param region: (str) region to create the bucket in
+    :return: (dict) role data (specified in boto3)
+    :raises: IamUtilError
+    """
+    log = logging.getLogger(mod_logger + '.create_bucket')
+    log.info('Attempting to create bucket [{n}]'.format(n=bucket_name))
+
+    # Checking for existing bucket
+    bucket_data = None
+    existing_buckets = list_buckets(client=client)
+    for existing_bucket in existing_buckets:
+        if 'Name' not in existing_bucket.keys():
+            log.warning('Name not found in bucket: {r}'.format(r=str(existing_bucket)))
+            continue
+        if bucket_name == existing_bucket['Name']:
+            bucket_data = existing_bucket
+    if bucket_data:
+        log.info('Found existing bucket [{n}]'.format(n=bucket_name))
+        return bucket_data
+    log.info('Attempting to create bucket [{n}]'.format(n=bucket_name))
+    try:
+        response = client.create_bucket(
+            Bucket=bucket_name,
+            CreateBucketConfiguration={
+                'LocationConstraint': region
+            }
+        )
+    except ClientError as exc:
+        msg = 'Problem creating bucket [{n}]'.format(n=bucket_name)
+        raise S3UtilError(msg) from exc
+    if 'Location' not in response.keys():
+        msg = 'Location not found in response: {d}'.format(d=str(response))
+        raise S3UtilError(msg)
+    log.info('Created new bucket: [{n}]'.format(n=bucket_name))
+    return {
+        'Name': bucket_name,
+        'Location': response['Location']
+    }
+
+
+############################################################################
+# Methods for downloading objects
+############################################################################
+
+
 def download(download_info):
     """Module  method for downloading from S3
 
     This public module method takes a key and the full path to
     the destination directory, assumes that the args have been
     validated by the public caller methods, and attempts to
     download the specified key to the dest_dir.
@@ -562,14 +662,217 @@
                 continue
         else:
             log.info('Successfully downloaded {k} from S3 bucket {b} to: {d}'.format(
                     k=key, b=bucket_name, d=destination))
             return destination
 
 
+############################################################################
+# Methods for enabling default encryption
+############################################################################
+
+
+def enable_bucket_encryption(client, bucket_name, kms_id=None):
+    """Enabled bucket encryption
+
+    :param client: boto3.client
+    :param bucket_name: (str) bucket name
+    :param kms_id: (str) AWS Key Management Service (KMS) customer master key ID to use for the default encryption.
+        You can specify the key ID or the Amazon Resource Name (ARN) of the CMK. However, if you are using encryption
+        with cross-account operations, you must use a fully qualified CMK ARN. For more information, see Using
+        encryption for cross-account operations.
+    :return: None
+    :raises: S3UtilError
+    """
+    log = logging.getLogger(mod_logger + '.enable_bucket_encryption')
+
+    if kms_id:
+        rule = {
+            'ApplyServerSideEncryptionByDefault': {
+                'SSEAlgorithm': 'aws:kms',
+                'KMSMasterKeyID': kms_id
+            }
+        }
+        msg = 'Enabling default encryption on [{n}] with KMS ID  [{k}]'.format(n=bucket_name, k=kms_id)
+    else:
+        rule = {
+            'ApplyServerSideEncryptionByDefault': {
+                'SSEAlgorithm': 'AES256',
+            }
+        }
+        msg = 'Enabling default encryption on [{n}] with AES256'.format(n=bucket_name)
+    rules = [rule]
+    log.info(msg)
+    try:
+        client.put_bucket_encryption(
+            Bucket=bucket_name,
+            ServerSideEncryptionConfiguration={'Rules': rules}
+        )
+    except ClientError as exc:
+        msg = 'Problem enabling bucket encryption on [{n}]'.format(n=bucket_name)
+        raise S3UtilError(msg) from exc
+
+
+############################################################################
+# Methods for enabling logging
+############################################################################
+
+
+def enable_bucket_logging(client, bucket_name, target_bucket, prefix):
+    """Enable bucket logging
+
+    :param client: boto3.client
+    :param bucket_name: (str) bucket name
+    :param target_bucket: (str) target bucket name
+    :param prefix: (str) prefix to append to logs stored in the target bucket
+    :return: None
+    :raises: S3UtilError
+    """
+    log = logging.getLogger(mod_logger + '.enable_bucket_logging')
+    log.info('Enabling logging on bucket [{n}] to target bucket [{t}] with prefix [{p}]'.format(
+        n=bucket_name, t=target_bucket, p=prefix))
+    try:
+        client.put_bucket_logging(
+            Bucket=bucket_name,
+            BucketLoggingStatus={
+                'LoggingEnabled': {
+                    'TargetBucket': target_bucket,
+                    'TargetPrefix': prefix
+                }
+            }
+        )
+    except ClientError as exc:
+        msg = 'Problem enabling bucket logging on [{n}]'.format(n=bucket_name)
+        raise S3UtilError(msg) from exc
+
+
+def enable_bucket_log_delivery(client, target_bucket_name):
+    """Adds an ACL to allow log delivery to the provided target bucket.  Once configured, other buckets can
+    send logs to this bucket
+
+    :param client: boto3.client
+    :param target_bucket_name: (str) bucket name of the logging target
+    :return: None
+    :raises: S3UtilError
+    """
+    log = logging.getLogger(mod_logger + '.enable_bucket_log_delivery')
+    log.info('Enabling log delivery on target bucket [{n}]'.format(n=target_bucket_name))
+
+    # Get the current ACL
+    try:
+        response = client.get_bucket_acl(Bucket=target_bucket_name)
+    except ClientError as exc:
+        msg = 'Problem getting ACL for bucket [{n}]'.format(n=target_bucket_name)
+        raise S3UtilError(msg) from exc
+    if 'Grants' not in response.keys():
+        msg = 'Grants not found in response: {d}'.format(d=str(response))
+        raise S3UtilError(msg)
+    if 'Owner' not in response.keys():
+        msg = 'Owner not found in response: {d}'.format(d=str(response))
+        raise S3UtilError(msg)
+    existing_grants = response['Grants']
+    owner = response['Owner']
+
+    # Determine the log delivery URI based on region
+    log_delivery_uri = 'http://acs.amazonaws.com/groups/s3/LogDelivery'
+
+    new_grants = [
+        {
+            'Grantee': {
+                'URI': log_delivery_uri,
+                'Type': 'Group'
+            },
+            'Permission': 'WRITE'
+        },
+        {
+            'Grantee': {
+                'URI': log_delivery_uri,
+                'Type': 'Group'
+            },
+            'Permission': 'READ_ACP'
+        }
+    ]
+
+    # Append existing ACL
+    new_grants += existing_grants
+
+    # Update the bucket ACL
+    try:
+        client.put_bucket_acl(
+            Bucket=target_bucket_name,
+            AccessControlPolicy={
+                'Grants': new_grants,
+                'Owner': owner
+            }
+        )
+    except ClientError as exc:
+        msg = 'Problem enabling bucket logging on [{n}]'.format(n=target_bucket_name)
+        raise S3UtilError(msg) from exc
+
+
+############################################################################
+# Methods for enabling versioning
+############################################################################
+
+
+def enable_bucket_versioning(client, bucket_name, enable=True, mfa_delete=False, mfa_device=None):
+    """Enable bucket versioning
+
+    :param client: boto3.client
+    :param bucket_name: (str) bucket name
+    :param enable: (bool) Set True to enable, False to suspend versioning
+    :param mfa_delete: (bool) Set True to force MFA for object deletion
+    :param mfa_device: (str) ARN of the MFA device for this request
+    :return: None
+    :raises: S3UtilError
+    """
+    log = logging.getLogger(mod_logger + '.enable_bucket_versioning')
+    log.info('Enabling versioning on bucket: {n}'.format(n=bucket_name))
+
+    status = 'Suspended'
+    if enable:
+        status = 'Enabled'
+
+    mfa_status = 'Disabled'
+    if mfa_delete:
+        mfa_status = 'Enabled'
+
+    mfa_str = None
+    if mfa_device:
+        mfa_totp = input('Enter your MFA code for [{d}]: '.format(d=mfa_device))
+        mfa_str = '{d} {c}'.format(d=mfa_device, c=mfa_totp)
+
+    try:
+        if mfa_str:
+            client.put_bucket_versioning(
+                Bucket=bucket_name,
+                VersioningConfiguration={
+                    'MFADelete': mfa_status,
+                    'Status': status
+                },
+                MFA=mfa_str
+            )
+        else:
+            client.put_bucket_versioning(
+                Bucket=bucket_name,
+                VersioningConfiguration={
+                    'MFADelete': mfa_status,
+                    'Status': status
+                }
+            )
+    except ClientError as exc:
+        msg = 'Problem enabling bucket versioning on [{n}]'.format(n=bucket_name)
+        raise S3UtilError(msg) from exc
+
+
+############################################################################
+# Methods for finding objects
+############################################################################
+
+
 def find_bucket_keys(bucket_name, regex, region_name=None, aws_access_key_id=None, aws_secret_access_key=None):
     """Finds a list of S3 keys matching the passed regex
 
     Given a regular expression, this method searches the S3 bucket
     for matching keys, and returns an array of strings for matched
     keys, an empty array if non are found.
 
@@ -600,14 +903,93 @@
         match = re.search(regex, item.key)
         if match:
             matched_keys.append(item.key)
     log.info('Found matching keys: {k}'.format(k=matched_keys))
     return matched_keys
 
 
+############################################################################
+# Getting a boto3 client object for S3
+############################################################################
+
+
+def get_s3_client(region_name=None, aws_access_key_id=None, aws_secret_access_key=None, aws_session_token=None):
+    """Gets an S3 client
+
+    :return: boto3.client object
+    :raises: AWSAPIError
+    """
+    return get_boto3_client(service='s3', region_name=region_name, aws_access_key_id=aws_access_key_id,
+                            aws_secret_access_key=aws_secret_access_key, aws_session_token=aws_session_token)
+
+
+############################################################################
+# Listing S3 buckets
+############################################################################
+
+
+def list_buckets(client):
+    """Returns a list of S3 buckets
+
+    :param client: boto3.client
+    :return: (list) of (dict) S3 buckets (see boto3 docs
+    """
+    log = logging.getLogger(mod_logger + '.list_buckets')
+    log.info('Attempting to list S3 buckets...')
+    try:
+        response = client.list_buckets()
+    except ClientError as exc:
+        msg = 'Problem listing S3 buckets'
+        raise S3UtilError(msg) from exc
+    if 'Buckets' not in response.keys():
+        msg = 'Buckets not found in response: {d}'.format(d=str(response))
+        raise S3UtilError(msg)
+    return response['Buckets']
+
+
+############################################################################
+# Methods for setting bucket policy
+############################################################################
+
+
+def set_bucket_policy(client, bucket_name, policy_document):
+    """Set the bucket policy to the provided
+
+    :param client: boto3.client
+    :param bucket_name: (str) bucket name
+    :param policy_document: (str) path to JSON policy file
+    :return: None
+    :raises: S3UtilError
+    """
+    log = logging.getLogger(mod_logger + '.set_bucket_policy')
+    log.info('Setting policy on bucket [{n}] to policy document [{d}]'.format(
+        n=bucket_name, d=policy_document))
+
+    # Ensure the file exists
+    if not os.path.isfile(policy_document):
+        raise S3UtilError('Policy document not found: {f}'.format(f=policy_document))
+    try:
+        with open(policy_document, 'r') as f:
+            policy_document_data = json.load(f)
+    except(OSError, IOError) as exc:
+        raise S3UtilError('Unable to read policy file: {f}'.format(f=policy_document)) from exc
+    log.info('Loading policy from file: {f}'.format(f=policy_document))
+    json_policy_data = json.dumps(policy_document_data)
+
+    # Replace account ID in the policy
+    json_policy_data = json_policy_data.replace('REPLACE_ACCOUNT_ID', '12345')
+
+    try:
+        client.put_bucket_policy(Bucket=bucket_name, Policy=json_policy_data)
+    except ClientError as exc:
+        msg = 'Problem setting bucket policy for [{n}] to [{d}] with contents:\n{c}'.format(
+            n=bucket_name, d=policy_document, c=json_policy_data)
+        raise S3UtilError(msg) from exc
+
+
 def main():
     """Sample usage for this python module
 
     This main method simply illustrates sample usage for this python
     module.
 
     :return: None
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3/scenario.py` & `pycons3rt3-0.0.9/pycons3rt3/scenario.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/service_runner.py` & `pycons3rt3-0.0.9/pycons3rt3/service_runner.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/slack.py` & `pycons3rt3-0.0.9/pycons3rt3/slack.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/ssh.py` & `pycons3rt3-0.0.9/pycons3rt3/ssh.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/test_exceptions.py` & `pycons3rt3-0.0.9/pycons3rt3/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3/windows.py` & `pycons3rt3-0.0.9/pycons3rt3/windows.py`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/pycons3rt3.egg-info/PKG-INFO` & `pycons3rt3-0.0.9/pycons3rt3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycons3rt3
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python3 library for CONS3RT assets and API calls
 Home-page: https://github.com/cons3rt/pycons3rt3
 Author: Joe Yennaco
 Author-email: joe.yennaco@jackpinetech.com
 License: GNU GPL v3
 Description: # pycons3rt3
```

### Comparing `pycons3rt3-0.0.8/pycons3rt3.egg-info/SOURCES.txt` & `pycons3rt3-0.0.9/pycons3rt3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 pycons3rt3/VERSION.txt
 pycons3rt3/__init__.py
 pycons3rt3/aliasip.py
+pycons3rt3/ansiblevault.py
 pycons3rt3/asset.py
 pycons3rt3/aws_metadata.py
 pycons3rt3/awsutil.py
 pycons3rt3/bash.py
 pycons3rt3/cloud.py
 pycons3rt3/cons3rt.py
 pycons3rt3/cons3rtapi.py
@@ -19,28 +20,30 @@
 pycons3rt3/cons3rtconfig.py
 pycons3rt3/deployment.py
 pycons3rt3/dyndict.py
 pycons3rt3/ec2util.py
 pycons3rt3/elbv2util.py
 pycons3rt3/exceptions.py
 pycons3rt3/httpclient.py
+pycons3rt3/iamutil.py
 pycons3rt3/images.py
 pycons3rt3/logify.py
 pycons3rt3/mailchimp.py
 pycons3rt3/nexus.py
 pycons3rt3/openssl.py
 pycons3rt3/ostemplates.py
 pycons3rt3/osutil.py
 pycons3rt3/password.py
 pycons3rt3/pycons3rtlibs.py
 pycons3rt3/pygit.py
 pycons3rt3/pyjavakeys.py
 pycons3rt3/rdsutil.py
 pycons3rt3/reports.py
 pycons3rt3/route53util.py
+pycons3rt3/s3organizer.py
 pycons3rt3/s3util.py
 pycons3rt3/scenario.py
 pycons3rt3/service_runner.py
 pycons3rt3/slack.py
 pycons3rt3/ssh.py
 pycons3rt3/stsutil.py
 pycons3rt3/test_exceptions.py
```

### Comparing `pycons3rt3-0.0.8/sample-configs/sample-multi-site.json` & `pycons3rt3-0.0.9/sample-configs/sample-multi-site.json`

 * *Files identical despite different names*

### Comparing `pycons3rt3-0.0.8/setup.py` & `pycons3rt3-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,20 @@
     include_package_data=True,
     license='GNU GPL v3',
     packages=find_packages(),
     zip_safe=True,
     install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'pycons3rt_setup = pycons3rt3.osutil:main',
             'asset = pycons3rt3.asset:main',
-            'slack = pycons3rt3.slack:main',
+            'cons3rt = pycons3rt3.cons3rt:main',
+            's3organizer = pycons3rt3.s3organizer:main',
             'deployment = pycons3rt3.deployment:main',
-            'cons3rt = pycons3rt3.cons3rt:main'
+            'pycons3rt_setup = pycons3rt3.osutil:main',
+            'slack = pycons3rt3.slack:main'
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent'
     ]
 )
```

