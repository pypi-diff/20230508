# Comparing `tmp/low-cost-ecs-0.0.8.tar.gz` & `tmp/low-cost-ecs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "low-cost-ecs-0.0.8.tar", last modified: Sun Sep 11 08:21:34 2022, max compression
+gzip compressed data, was "low-cost-ecs-0.0.9.tar", last modified: Sun Sep 11 08:38:10 2022, max compression
```

## Comparing `low-cost-ecs-0.0.8.tar` & `low-cost-ecs-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6381 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/src/low_cost_ecs/
--rw-r--r--   0 runner    (1001) docker     (121)    37018 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/src/low_cost_ecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/src/low_cost_ecs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/src/low_cost_ecs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39188 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/src/low_cost_ecs/_jsii/low-cost-ecs@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 08:21:22.000000 low-cost-ecs-0.0.8/src/low_cost_ecs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:21:34.591037 low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6381 2022-09-11 08:21:34.000000 low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-11 08:21:34.000000 low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 08:21:34.000000 low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-11 08:21:34.000000 low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-11 08:21:34.000000 low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6416 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5507 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/src/low_cost_ecs/
+-rw-r--r--   0 runner    (1001) docker     (121)    37053 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/src/low_cost_ecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/src/low_cost_ecs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/src/low_cost_ecs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39221 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/src/low_cost_ecs/_jsii/low-cost-ecs@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 08:37:56.000000 low-cost-ecs-0.0.9/src/low_cost_ecs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 08:38:10.516977 low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6416 2022-09-11 08:38:09.000000 low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-11 08:38:10.000000 low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 08:38:09.000000 low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-11 08:38:10.000000 low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-11 08:38:10.000000 low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/top_level.txt
```

### Comparing `low-cost-ecs-0.0.8/LICENSE` & `low-cost-ecs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `low-cost-ecs-0.0.8/PKG-INFO` & `low-cost-ecs-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: low-cost-ecs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easy and low-cost ECS on EC2 server without a load balancer
 Home-page: https://github.com/rajyan/low-cost-ecs.git
 Author: Yohta Kimura<kitakita7617@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rajyan/low-cost-ecs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -27,20 +27,20 @@
 [![Release](https://github.com/rajyan/low-cost-ecs/workflows/release/badge.svg)](https://github.com/rajyan/low-cost-ecs/actions/workflows/release.yml)
 [<img src="https://constructs.dev/badge?package=low-cost-ecs" width="150">](https://constructs.dev/packages/low-cost-ecs)
 
 # Low-Cost ECS
 
 A CDK construct that provides easy and [low-cost](#cost) ECS on EC2 server setup without a load balancer.
 
-**This construct is for development purposes only** see [Limitations](#limitations).
+**This construct is for development purposes only**. See [Limitations](#limitations).
 
 # Try it out!
 
-The easiest way to see what this construct creates is to clone this repository and deploying a sample server.
-Edit settings in `bin/low-cost-ecs.ts` and deploy cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
+The easiest way to see what this construct creates is to clone this repository and deploy the sample server.
+Edit settings in `bin/low-cost-ecs.ts` and deploy the cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
 
 ```
 git clone https://github.com/rajyan/low-cost-ecs.git
 # edit settings in bin/low-cost-ecs.ts
 npx cdk deploy
 ```
 
@@ -75,24 +75,24 @@
             serverTaskDefinition: serverTaskDefinition
         });
     }
 }
 ```
 
 The required fields are `hostedZoneDomain` and `email`.
-You can configure your server task definition, and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
+You can configure your server task definition and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
 
 # Why
 
 ECS may often seem expensive when used for personal development purposes, because of the cost of the load balancer.
-The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mapping,
+The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mappings and so on,
 but it is over-featured for running 1 ECS service.
 
-However, to run an ECS sever without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
-This construct aims to automate these works and deploy resources to run a low-cost ECS server.
+However, to run an ECS server without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
+This construct aims to automate these works and to make it easy to deploy resources to run a low-cost ECS server.
 
 # Overview
 
 Resources generated in this stack
 
 * Route53 A record
 
@@ -100,15 +100,15 @@
 * Certificate State Machine
 
   * Install and renew certificates to EFS using [certbot-dns-route53](https://certbot-dns-route53.readthedocs.io/en/stable/)
   * Scheduled automated renewal every 60 days
   * Email notification on certbot task failure
 * ECS on EC2 host instance
 
-  * ECS-optimized Amazon Linux 2 AMI instance auto scaling group
+  * ECS-optimized Amazon Linux 2 AMI instance auto-scaling group
   * Automatically associated with Elastic IP on instance initialization
 * ECS Service
 
   * TLS/SSL certificate installation on default container startup
   * Certificate EFS mounted on `/etc/letsencrypt`
 * Others
 
@@ -161,10 +161,11 @@
 --interactive
 ```
 
 # Limitations
 
 The ECS service occupies the host port, only one service can be run at a time.
 The old task must be terminated before the new task launches, and this causes downtime on release.
+
 Also, if you make changes that require recreating service, you may need to manually terminate the task of old the service.
```

### Comparing `low-cost-ecs-0.0.8/README.md` & `low-cost-ecs-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 [![Release](https://github.com/rajyan/low-cost-ecs/workflows/release/badge.svg)](https://github.com/rajyan/low-cost-ecs/actions/workflows/release.yml)
 [<img src="https://constructs.dev/badge?package=low-cost-ecs" width="150">](https://constructs.dev/packages/low-cost-ecs)
 
 # Low-Cost ECS
 
 A CDK construct that provides easy and [low-cost](#cost) ECS on EC2 server setup without a load balancer.
 
-**This construct is for development purposes only** see [Limitations](#limitations).
+**This construct is for development purposes only**. See [Limitations](#limitations).
 
 # Try it out!
 
-The easiest way to see what this construct creates is to clone this repository and deploying a sample server.
-Edit settings in `bin/low-cost-ecs.ts` and deploy cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
+The easiest way to see what this construct creates is to clone this repository and deploy the sample server.
+Edit settings in `bin/low-cost-ecs.ts` and deploy the cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
 
 ```
 git clone https://github.com/rajyan/low-cost-ecs.git
 # edit settings in bin/low-cost-ecs.ts
 npx cdk deploy
 ```
 
@@ -51,24 +51,24 @@
             serverTaskDefinition: serverTaskDefinition
         });
     }
 }
 ```
 
 The required fields are `hostedZoneDomain` and `email`.
-You can configure your server task definition, and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
+You can configure your server task definition and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
 
 # Why
 
 ECS may often seem expensive when used for personal development purposes, because of the cost of the load balancer.
-The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mapping,
+The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mappings and so on,
 but it is over-featured for running 1 ECS service.
 
-However, to run an ECS sever without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
-This construct aims to automate these works and deploy resources to run a low-cost ECS server.
+However, to run an ECS server without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
+This construct aims to automate these works and to make it easy to deploy resources to run a low-cost ECS server.
 
 # Overview
 
 Resources generated in this stack
 
 * Route53 A record
 
@@ -76,15 +76,15 @@
 * Certificate State Machine
 
   * Install and renew certificates to EFS using [certbot-dns-route53](https://certbot-dns-route53.readthedocs.io/en/stable/)
   * Scheduled automated renewal every 60 days
   * Email notification on certbot task failure
 * ECS on EC2 host instance
 
-  * ECS-optimized Amazon Linux 2 AMI instance auto scaling group
+  * ECS-optimized Amazon Linux 2 AMI instance auto-scaling group
   * Automatically associated with Elastic IP on instance initialization
 * ECS Service
 
   * TLS/SSL certificate installation on default container startup
   * Certificate EFS mounted on `/etc/letsencrypt`
 * Others
 
@@ -137,8 +137,9 @@
 --interactive
 ```
 
 # Limitations
 
 The ECS service occupies the host port, only one service can be run at a time.
 The old task must be terminated before the new task launches, and this causes downtime on release.
+
 Also, if you make changes that require recreating service, you may need to manually terminate the task of old the service.
```

### Comparing `low-cost-ecs-0.0.8/setup.py` & `low-cost-ecs-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "low-cost-ecs",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Easy and low-cost ECS on EC2 server without a load balancer",
     "license": "MIT",
     "url": "https://github.com/rajyan/low-cost-ecs.git",
     "long_description_content_type": "text/markdown",
     "author": "Yohta Kimura<kitakita7617@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "low_cost_ecs",
         "low_cost_ecs._jsii"
     ],
     "package_data": {
         "low_cost_ecs._jsii": [
-            "low-cost-ecs@0.0.8.jsii.tgz"
+            "low-cost-ecs@0.0.9.jsii.tgz"
         ],
         "low_cost_ecs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `low-cost-ecs-0.0.8/src/low_cost_ecs/__init__.py` & `low-cost-ecs-0.0.9/src/low_cost_ecs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [![Release](https://github.com/rajyan/low-cost-ecs/workflows/release/badge.svg)](https://github.com/rajyan/low-cost-ecs/actions/workflows/release.yml)
 [<img src="https://constructs.dev/badge?package=low-cost-ecs" width="150">](https://constructs.dev/packages/low-cost-ecs)
 
 # Low-Cost ECS
 
 A CDK construct that provides easy and [low-cost](#cost) ECS on EC2 server setup without a load balancer.
 
-**This construct is for development purposes only** see [Limitations](#limitations).
+**This construct is for development purposes only**. See [Limitations](#limitations).
 
 # Try it out!
 
-The easiest way to see what this construct creates is to clone this repository and deploying a sample server.
-Edit settings in `bin/low-cost-ecs.ts` and deploy cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
+The easiest way to see what this construct creates is to clone this repository and deploy the sample server.
+Edit settings in `bin/low-cost-ecs.ts` and deploy the cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
 
 ```
 git clone https://github.com/rajyan/low-cost-ecs.git
 # edit settings in bin/low-cost-ecs.ts
 npx cdk deploy
 ```
 
@@ -52,24 +52,24 @@
             serverTaskDefinition: serverTaskDefinition
         });
     }
 }
 ```
 
 The required fields are `hostedZoneDomain` and `email`.
-You can configure your server task definition, and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
+You can configure your server task definition and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
 
 # Why
 
 ECS may often seem expensive when used for personal development purposes, because of the cost of the load balancer.
-The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mapping,
+The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mappings and so on,
 but it is over-featured for running 1 ECS service.
 
-However, to run an ECS sever without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
-This construct aims to automate these works and deploy resources to run a low-cost ECS server.
+However, to run an ECS server without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
+This construct aims to automate these works and to make it easy to deploy resources to run a low-cost ECS server.
 
 # Overview
 
 Resources generated in this stack
 
 * Route53 A record
 
@@ -77,15 +77,15 @@
 * Certificate State Machine
 
   * Install and renew certificates to EFS using [certbot-dns-route53](https://certbot-dns-route53.readthedocs.io/en/stable/)
   * Scheduled automated renewal every 60 days
   * Email notification on certbot task failure
 * ECS on EC2 host instance
 
-  * ECS-optimized Amazon Linux 2 AMI instance auto scaling group
+  * ECS-optimized Amazon Linux 2 AMI instance auto-scaling group
   * Automatically associated with Elastic IP on instance initialization
 * ECS Service
 
   * TLS/SSL certificate installation on default container startup
   * Certificate EFS mounted on `/etc/letsencrypt`
 * Others
 
@@ -138,14 +138,15 @@
 --interactive
 ```
 
 # Limitations
 
 The ECS service occupies the host port, only one service can be run at a time.
 The old task must be terminated before the new task launches, and this causes downtime on release.
+
 Also, if you make changes that require recreating service, you may need to manually terminate the task of old the service.
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
```

### Comparing `low-cost-ecs-0.0.8/src/low_cost_ecs.egg-info/PKG-INFO` & `low-cost-ecs-0.0.9/src/low_cost_ecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: low-cost-ecs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easy and low-cost ECS on EC2 server without a load balancer
 Home-page: https://github.com/rajyan/low-cost-ecs.git
 Author: Yohta Kimura<kitakita7617@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rajyan/low-cost-ecs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -27,20 +27,20 @@
 [![Release](https://github.com/rajyan/low-cost-ecs/workflows/release/badge.svg)](https://github.com/rajyan/low-cost-ecs/actions/workflows/release.yml)
 [<img src="https://constructs.dev/badge?package=low-cost-ecs" width="150">](https://constructs.dev/packages/low-cost-ecs)
 
 # Low-Cost ECS
 
 A CDK construct that provides easy and [low-cost](#cost) ECS on EC2 server setup without a load balancer.
 
-**This construct is for development purposes only** see [Limitations](#limitations).
+**This construct is for development purposes only**. See [Limitations](#limitations).
 
 # Try it out!
 
-The easiest way to see what this construct creates is to clone this repository and deploying a sample server.
-Edit settings in `bin/low-cost-ecs.ts` and deploy cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
+The easiest way to see what this construct creates is to clone this repository and deploy the sample server.
+Edit settings in `bin/low-cost-ecs.ts` and deploy the cdk construct. [Public hosted zone](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html) is required.
 
 ```
 git clone https://github.com/rajyan/low-cost-ecs.git
 # edit settings in bin/low-cost-ecs.ts
 npx cdk deploy
 ```
 
@@ -75,24 +75,24 @@
             serverTaskDefinition: serverTaskDefinition
         });
     }
 }
 ```
 
 The required fields are `hostedZoneDomain` and `email`.
-You can configure your server task definition, and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
+You can configure your server task definition and other props. Read [`LowCostECSProps` documentation](https://github.com/rajyan/low-cost-ecs/blob/main/API.md#low-cost-ecs.LowCostECSProps) for details.
 
 # Why
 
 ECS may often seem expensive when used for personal development purposes, because of the cost of the load balancer.
-The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mapping,
+The application load balancer is a great service because it is easy to set up managed ACM certificates, it scales, and has dynamic port mappings and so on,
 but it is over-featured for running 1 ECS service.
 
-However, to run an ECS sever without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
-This construct aims to automate these works and deploy resources to run a low-cost ECS server.
+However, to run an ECS server without a load balancer, you need to associate an Elastic IP to the host instance and install your certificate by yourself.
+This construct aims to automate these works and to make it easy to deploy resources to run a low-cost ECS server.
 
 # Overview
 
 Resources generated in this stack
 
 * Route53 A record
 
@@ -100,15 +100,15 @@
 * Certificate State Machine
 
   * Install and renew certificates to EFS using [certbot-dns-route53](https://certbot-dns-route53.readthedocs.io/en/stable/)
   * Scheduled automated renewal every 60 days
   * Email notification on certbot task failure
 * ECS on EC2 host instance
 
-  * ECS-optimized Amazon Linux 2 AMI instance auto scaling group
+  * ECS-optimized Amazon Linux 2 AMI instance auto-scaling group
   * Automatically associated with Elastic IP on instance initialization
 * ECS Service
 
   * TLS/SSL certificate installation on default container startup
   * Certificate EFS mounted on `/etc/letsencrypt`
 * Others
 
@@ -161,10 +161,11 @@
 --interactive
 ```
 
 # Limitations
 
 The ECS service occupies the host port, only one service can be run at a time.
 The old task must be terminated before the new task launches, and this causes downtime on release.
+
 Also, if you make changes that require recreating service, you may need to manually terminate the task of old the service.
```

