# Comparing `tmp/cdktf-cdk8s-0.5.6.tar.gz` & `tmp/cdktf-cdk8s-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdk8s-0.5.6.tar", last modified: Fri Mar 24 08:40:25 2023, max compression
+gzip compressed data, was "cdktf-cdk8s-0.5.7.tar", last modified: Mon May  8 14:57:34 2023, max compression
```

## Comparing `cdktf-cdk8s-0.5.6.tar` & `cdktf-cdk8s-0.5.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)    33009 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   364945 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/_jsii/cdktf-cdk8s@0.5.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:40:12.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:40:25.328567 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-24 08:40:24.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-24 08:40:25.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:40:24.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-24 08:40:25.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-24 08:40:25.000000 cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:34.752257 cdktf-cdk8s-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 14:57:34.752257 cdktf-cdk8s-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:57:34.752257 cdktf-cdk8s-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:34.748257 cdktf-cdk8s-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:34.748257 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)    34263 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:34.752257 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   360026 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/_jsii/cdktf-cdk8s@0.5.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:57:23.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:34.752257 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 14:57:34.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 14:57:34.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:57:34.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 14:57:34.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 14:57:34.000000 cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/top_level.txt
```

### Comparing `cdktf-cdk8s-0.5.6/LICENSE` & `cdktf-cdk8s-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.5.6/PKG-INFO` & `cdktf-cdk8s-0.5.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdk8s
-Version: 0.5.6
+Version: 0.5.7
 Summary: A compatibility layer for using cdk8s constructs within Terraform CDK.
 Home-page: https://github.com/cdktf/cdktf-cdk8s.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-cdk8s.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -57,9 +57,7 @@
   }
 }
 
 const app = new App();
 new MyStack(app, "cdktf-cdk8s");
 app.synth();
 ```
-
-
```

### Comparing `cdktf-cdk8s-0.5.6/README.md` & `cdktf-cdk8s-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.5.6/setup.py` & `cdktf-cdk8s-0.5.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdk8s",
-    "version": "0.5.6",
+    "version": "0.5.7",
     "description": "A compatibility layer for using cdk8s constructs within Terraform CDK.",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-cdk8s.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -22,39 +22,40 @@
     },
     "packages": [
         "cdktf_cdk8s",
         "cdktf_cdk8s._jsii"
     ],
     "package_data": {
         "cdktf_cdk8s._jsii": [
-            "cdktf-cdk8s@0.5.6.jsii.tgz"
+            "cdktf-cdk8s@0.5.7.jsii.tgz"
         ],
         "cdktf_cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdk8s>=2.1.6",
-        "cdktf-cdktf-provider-kubernetes>=5.0.0",
-        "cdktf>=0.15.0",
-        "constructs>=10.0.107, <11.0.0",
-        "jsii>=1.73.0, <2.0.0",
+        "cdktf-cdktf-provider-kubernetes>=6.0.0",
+        "cdktf>=0.16.0",
+        "constructs>=10.0.25, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-cdk8s-0.5.6/src/cdktf_cdk8s/__init__.py` & `cdktf-cdk8s-0.5.7/src/cdktf_cdk8s/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,33 +90,33 @@
         token: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param cdk8s_app: 
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#alias KubernetesProvider#alias}
-        :param client_certificate: PEM-encoded client certificate for TLS authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#client_certificate KubernetesProvider#client_certificate}
-        :param client_key: PEM-encoded client certificate key for TLS authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#client_key KubernetesProvider#client_key}
-        :param cluster_ca_certificate: PEM-encoded root certificates bundle for TLS authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#cluster_ca_certificate KubernetesProvider#cluster_ca_certificate}
-        :param config_context: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context KubernetesProvider#config_context}.
-        :param config_context_auth_info: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context_auth_info KubernetesProvider#config_context_auth_info}.
-        :param config_context_cluster: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context_cluster KubernetesProvider#config_context_cluster}.
-        :param config_path: Path to the kube config file. Can be set with KUBE_CONFIG_PATH. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_path KubernetesProvider#config_path}
-        :param config_paths: A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_paths KubernetesProvider#config_paths}
-        :param exec: exec block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#exec KubernetesProvider#exec}
-        :param experiments: experiments block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#experiments KubernetesProvider#experiments}
-        :param host: The hostname (in form of URI) of Kubernetes master. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#host KubernetesProvider#host}
-        :param ignore_annotations: List of Kubernetes metadata annotations to ignore across all resources handled by this provider for situations where external systems are managing certain resource annotations. Each item is a regular expression. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#ignore_annotations KubernetesProvider#ignore_annotations}
-        :param ignore_labels: List of Kubernetes metadata labels to ignore across all resources handled by this provider for situations where external systems are managing certain resource labels. Each item is a regular expression. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#ignore_labels KubernetesProvider#ignore_labels}
-        :param insecure: Whether server should be accessed without verifying the TLS certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#insecure KubernetesProvider#insecure}
-        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#password KubernetesProvider#password}
-        :param proxy_url: URL to the proxy to be used for all API requests. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#proxy_url KubernetesProvider#proxy_url}
-        :param token: Token to authenticate an service account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#token KubernetesProvider#token}
-        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#username KubernetesProvider#username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#alias KubernetesProvider#alias}
+        :param client_certificate: PEM-encoded client certificate for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#client_certificate KubernetesProvider#client_certificate}
+        :param client_key: PEM-encoded client certificate key for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#client_key KubernetesProvider#client_key}
+        :param cluster_ca_certificate: PEM-encoded root certificates bundle for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#cluster_ca_certificate KubernetesProvider#cluster_ca_certificate}
+        :param config_context: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context KubernetesProvider#config_context}.
+        :param config_context_auth_info: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context_auth_info KubernetesProvider#config_context_auth_info}.
+        :param config_context_cluster: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context_cluster KubernetesProvider#config_context_cluster}.
+        :param config_path: Path to the kube config file. Can be set with KUBE_CONFIG_PATH. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_path KubernetesProvider#config_path}
+        :param config_paths: A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_paths KubernetesProvider#config_paths}
+        :param exec: exec block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#exec KubernetesProvider#exec}
+        :param experiments: experiments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#experiments KubernetesProvider#experiments}
+        :param host: The hostname (in form of URI) of Kubernetes master. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#host KubernetesProvider#host}
+        :param ignore_annotations: List of Kubernetes metadata annotations to ignore across all resources handled by this provider for situations where external systems are managing certain resource annotations. Each item is a regular expression. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#ignore_annotations KubernetesProvider#ignore_annotations}
+        :param ignore_labels: List of Kubernetes metadata labels to ignore across all resources handled by this provider for situations where external systems are managing certain resource labels. Each item is a regular expression. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#ignore_labels KubernetesProvider#ignore_labels}
+        :param insecure: Whether server should be accessed without verifying the TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#insecure KubernetesProvider#insecure}
+        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#password KubernetesProvider#password}
+        :param proxy_url: URL to the proxy to be used for all API requests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#proxy_url KubernetesProvider#proxy_url}
+        :param token: Token to authenticate an service account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#token KubernetesProvider#token}
+        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#username KubernetesProvider#username}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c1318c333a56de3bcab994349ad716a730c79b7743c7f471bcd586a5025ca0ab)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = CDK8sProviderConfig(
             cdk8s_app=cdk8s_app,
@@ -196,33 +196,33 @@
         password: typing.Optional[builtins.str] = None,
         proxy_url: typing.Optional[builtins.str] = None,
         token: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
         cdk8s_app: _cdk8s_d3d9af27.App,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#alias KubernetesProvider#alias}
-        :param client_certificate: PEM-encoded client certificate for TLS authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#client_certificate KubernetesProvider#client_certificate}
-        :param client_key: PEM-encoded client certificate key for TLS authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#client_key KubernetesProvider#client_key}
-        :param cluster_ca_certificate: PEM-encoded root certificates bundle for TLS authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#cluster_ca_certificate KubernetesProvider#cluster_ca_certificate}
-        :param config_context: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context KubernetesProvider#config_context}.
-        :param config_context_auth_info: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context_auth_info KubernetesProvider#config_context_auth_info}.
-        :param config_context_cluster: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context_cluster KubernetesProvider#config_context_cluster}.
-        :param config_path: Path to the kube config file. Can be set with KUBE_CONFIG_PATH. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_path KubernetesProvider#config_path}
-        :param config_paths: A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_paths KubernetesProvider#config_paths}
-        :param exec: exec block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#exec KubernetesProvider#exec}
-        :param experiments: experiments block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#experiments KubernetesProvider#experiments}
-        :param host: The hostname (in form of URI) of Kubernetes master. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#host KubernetesProvider#host}
-        :param ignore_annotations: List of Kubernetes metadata annotations to ignore across all resources handled by this provider for situations where external systems are managing certain resource annotations. Each item is a regular expression. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#ignore_annotations KubernetesProvider#ignore_annotations}
-        :param ignore_labels: List of Kubernetes metadata labels to ignore across all resources handled by this provider for situations where external systems are managing certain resource labels. Each item is a regular expression. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#ignore_labels KubernetesProvider#ignore_labels}
-        :param insecure: Whether server should be accessed without verifying the TLS certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#insecure KubernetesProvider#insecure}
-        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#password KubernetesProvider#password}
-        :param proxy_url: URL to the proxy to be used for all API requests. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#proxy_url KubernetesProvider#proxy_url}
-        :param token: Token to authenticate an service account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#token KubernetesProvider#token}
-        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#username KubernetesProvider#username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#alias KubernetesProvider#alias}
+        :param client_certificate: PEM-encoded client certificate for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#client_certificate KubernetesProvider#client_certificate}
+        :param client_key: PEM-encoded client certificate key for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#client_key KubernetesProvider#client_key}
+        :param cluster_ca_certificate: PEM-encoded root certificates bundle for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#cluster_ca_certificate KubernetesProvider#cluster_ca_certificate}
+        :param config_context: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context KubernetesProvider#config_context}.
+        :param config_context_auth_info: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context_auth_info KubernetesProvider#config_context_auth_info}.
+        :param config_context_cluster: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context_cluster KubernetesProvider#config_context_cluster}.
+        :param config_path: Path to the kube config file. Can be set with KUBE_CONFIG_PATH. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_path KubernetesProvider#config_path}
+        :param config_paths: A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_paths KubernetesProvider#config_paths}
+        :param exec: exec block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#exec KubernetesProvider#exec}
+        :param experiments: experiments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#experiments KubernetesProvider#experiments}
+        :param host: The hostname (in form of URI) of Kubernetes master. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#host KubernetesProvider#host}
+        :param ignore_annotations: List of Kubernetes metadata annotations to ignore across all resources handled by this provider for situations where external systems are managing certain resource annotations. Each item is a regular expression. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#ignore_annotations KubernetesProvider#ignore_annotations}
+        :param ignore_labels: List of Kubernetes metadata labels to ignore across all resources handled by this provider for situations where external systems are managing certain resource labels. Each item is a regular expression. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#ignore_labels KubernetesProvider#ignore_labels}
+        :param insecure: Whether server should be accessed without verifying the TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#insecure KubernetesProvider#insecure}
+        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#password KubernetesProvider#password}
+        :param proxy_url: URL to the proxy to be used for all API requests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#proxy_url KubernetesProvider#proxy_url}
+        :param token: Token to authenticate an service account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#token KubernetesProvider#token}
+        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#username KubernetesProvider#username}
         :param cdk8s_app: 
         '''
         if isinstance(exec, dict):
             exec = _cdktf_cdktf_provider_kubernetes_provider_b14d7399.KubernetesProviderExec(**exec)
         if isinstance(experiments, dict):
             experiments = _cdktf_cdktf_provider_kubernetes_provider_b14d7399.KubernetesProviderExperiments(**experiments)
         if __debug__:
@@ -289,178 +289,178 @@
         if username is not None:
             self._values["username"] = username
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#alias KubernetesProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#alias KubernetesProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded client certificate for TLS authentication.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#client_certificate KubernetesProvider#client_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#client_certificate KubernetesProvider#client_certificate}
         '''
         result = self._values.get("client_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_key(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded client certificate key for TLS authentication.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#client_key KubernetesProvider#client_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#client_key KubernetesProvider#client_key}
         '''
         result = self._values.get("client_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cluster_ca_certificate(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded root certificates bundle for TLS authentication.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#cluster_ca_certificate KubernetesProvider#cluster_ca_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#cluster_ca_certificate KubernetesProvider#cluster_ca_certificate}
         '''
         result = self._values.get("cluster_ca_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_context(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context KubernetesProvider#config_context}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context KubernetesProvider#config_context}.'''
         result = self._values.get("config_context")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_context_auth_info(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context_auth_info KubernetesProvider#config_context_auth_info}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context_auth_info KubernetesProvider#config_context_auth_info}.'''
         result = self._values.get("config_context_auth_info")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_context_cluster(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_context_cluster KubernetesProvider#config_context_cluster}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_context_cluster KubernetesProvider#config_context_cluster}.'''
         result = self._values.get("config_context_cluster")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_path(self) -> typing.Optional[builtins.str]:
         '''Path to the kube config file. Can be set with KUBE_CONFIG_PATH.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_path KubernetesProvider#config_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_path KubernetesProvider#config_path}
         '''
         result = self._values.get("config_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_paths(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#config_paths KubernetesProvider#config_paths}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#config_paths KubernetesProvider#config_paths}
         '''
         result = self._values.get("config_paths")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def exec(
         self,
     ) -> typing.Optional[_cdktf_cdktf_provider_kubernetes_provider_b14d7399.KubernetesProviderExec]:
         '''exec block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#exec KubernetesProvider#exec}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#exec KubernetesProvider#exec}
         '''
         result = self._values.get("exec")
         return typing.cast(typing.Optional[_cdktf_cdktf_provider_kubernetes_provider_b14d7399.KubernetesProviderExec], result)
 
     @builtins.property
     def experiments(
         self,
     ) -> typing.Optional[_cdktf_cdktf_provider_kubernetes_provider_b14d7399.KubernetesProviderExperiments]:
         '''experiments block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#experiments KubernetesProvider#experiments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#experiments KubernetesProvider#experiments}
         '''
         result = self._values.get("experiments")
         return typing.cast(typing.Optional[_cdktf_cdktf_provider_kubernetes_provider_b14d7399.KubernetesProviderExperiments], result)
 
     @builtins.property
     def host(self) -> typing.Optional[builtins.str]:
         '''The hostname (in form of URI) of Kubernetes master.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#host KubernetesProvider#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#host KubernetesProvider#host}
         '''
         result = self._values.get("host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ignore_annotations(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of Kubernetes metadata annotations to ignore across all resources handled by this provider for situations where external systems are managing certain resource annotations.
 
         Each item is a regular expression.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#ignore_annotations KubernetesProvider#ignore_annotations}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#ignore_annotations KubernetesProvider#ignore_annotations}
         '''
         result = self._values.get("ignore_annotations")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def ignore_labels(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of Kubernetes metadata labels to ignore across all resources handled by this provider for situations where external systems are managing certain resource labels.
 
         Each item is a regular expression.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#ignore_labels KubernetesProvider#ignore_labels}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#ignore_labels KubernetesProvider#ignore_labels}
         '''
         result = self._values.get("ignore_labels")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether server should be accessed without verifying the TLS certificate.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#insecure KubernetesProvider#insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#insecure KubernetesProvider#insecure}
         '''
         result = self._values.get("insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#password KubernetesProvider#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#password KubernetesProvider#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def proxy_url(self) -> typing.Optional[builtins.str]:
         '''URL to the proxy to be used for all API requests.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#proxy_url KubernetesProvider#proxy_url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#proxy_url KubernetesProvider#proxy_url}
         '''
         result = self._values.get("proxy_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''Token to authenticate an service account.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#token KubernetesProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#token KubernetesProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
         '''The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/kubernetes#username KubernetesProvider#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/kubernetes/2.19.0/docs#username KubernetesProvider#username}
         '''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cdk8s_app(self) -> _cdk8s_d3d9af27.App:
         result = self._values.get("cdk8s_app")
```

### Comparing `cdktf-cdk8s-0.5.6/src/cdktf_cdk8s.egg-info/PKG-INFO` & `cdktf-cdk8s-0.5.7/src/cdktf_cdk8s.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdk8s
-Version: 0.5.6
+Version: 0.5.7
 Summary: A compatibility layer for using cdk8s constructs within Terraform CDK.
 Home-page: https://github.com/cdktf/cdktf-cdk8s.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-cdk8s.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -57,9 +57,7 @@
   }
 }
 
 const app = new App();
 new MyStack(app, "cdktf-cdk8s");
 app.synth();
 ```
-
-
```

