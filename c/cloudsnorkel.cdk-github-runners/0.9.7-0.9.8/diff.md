# Comparing `tmp/cloudsnorkel.cdk-github-runners-0.9.7.tar.gz` & `tmp/cloudsnorkel.cdk-github-runners-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.7.tar", last modified: Thu Apr 27 21:25:04 2023, max compression
+gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.8.tar", last modified: Tue May  2 23:01:49 2023, max compression
```

## Comparing `cloudsnorkel.cdk-github-runners-0.9.7.tar` & `cloudsnorkel.cdk-github-runners-0.9.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.204815 cloudsnorkel.cdk-github-runners-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-27 21:25:04.204815 cloudsnorkel.cdk-github-runners-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:25:04.204815 cloudsnorkel.cdk-github-runners-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.196815 cloudsnorkel.cdk-github-runners-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.196815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.200815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/
--rw-r--r--   0 runner    (1001) docker     (123)   563192 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.200815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1998045 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.200815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:01:49.069050 cloudsnorkel.cdk-github-runners-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-05-02 23:01:49.069050 cloudsnorkel.cdk-github-runners-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:01:49.069050 cloudsnorkel.cdk-github-runners-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:01:49.061050 cloudsnorkel.cdk-github-runners-0.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:01:49.061050 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:01:49.065050 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)   566084 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:01:49.065050 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2347586 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:01:33.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:01:49.065050 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-05-02 23:01:49.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-02 23:01:49.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:01:49.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 23:01:49.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 23:01:49.000000 cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/LICENSE` & `cloudsnorkel.cdk-github-runners-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.7
+Version: 0.9.8
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/README.md` & `cloudsnorkel.cdk-github-runners-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/setup.py` & `cloudsnorkel.cdk-github-runners-0.9.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudsnorkel.cdk-github-runners",
-    "version": "0.9.7",
+    "version": "0.9.8",
     "description": "CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.",
     "license": "Apache-2.0",
     "url": "https://github.com/CloudSnorkel/cdk-github-runners.git",
     "long_description_content_type": "text/markdown",
     "author": "Amir Szekely<amir@cloudsnorkel.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudsnorkel.cdk_github_runners",
         "cloudsnorkel.cdk_github_runners._jsii"
     ],
     "package_data": {
         "cloudsnorkel.cdk_github_runners._jsii": [
-            "cdk-github-runners@0.9.7.jsii.tgz"
+            "cdk-github-runners@0.9.8.jsii.tgz"
         ],
         "cloudsnorkel.cdk_github_runners": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/__init__.py` & `cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel/cdk_github_runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,43 +623,49 @@
 @jsii.data_type(
     jsii_type="@cloudsnorkel/cdk-github-runners.ApiGatewayAccessProps",
     jsii_struct_bases=[],
     name_mapping={
         "allowed_ips": "allowedIps",
         "allowed_security_groups": "allowedSecurityGroups",
         "allowed_vpc": "allowedVpc",
+        "allowed_vpc_endpoints": "allowedVpcEndpoints",
     },
 )
 class ApiGatewayAccessProps:
     def __init__(
         self,
         *,
         allowed_ips: typing.Optional[typing.Sequence[builtins.str]] = None,
         allowed_security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         allowed_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+        allowed_vpc_endpoints: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.IVpcEndpoint]] = None,
     ) -> None:
         '''
         :param allowed_ips: (experimental) List of IP addresses in CIDR notation that are allowed to access the API Gateway. If not specified on public API Gateway, all IP addresses are allowed. If not specified on private API Gateway, no IP addresses are allowed (but specified security groups are).
         :param allowed_security_groups: (experimental) List of security groups that are allowed to access the API Gateway. Only works for private API Gateways with {@link allowedVpc}.
-        :param allowed_vpc: (experimental) Creates a private API Gateway and allows access from the specified VPC.
+        :param allowed_vpc: (experimental) Create a private API Gateway and allow access from the specified VPC.
+        :param allowed_vpc_endpoints: (experimental) Create a private API Gateway and allow access from the specified VPC endpoints. Use this to make use of existing VPC endpoints. The VPC endpoint must point to ``ec2.InterfaceVpcEndpointAwsService.APIGATEWAY``. No other settings are supported when using this option.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0230281aea2f0096e32af8e4f02c3c351aada0957c217590514bfc5f6f656b0e)
             check_type(argname="argument allowed_ips", value=allowed_ips, expected_type=type_hints["allowed_ips"])
             check_type(argname="argument allowed_security_groups", value=allowed_security_groups, expected_type=type_hints["allowed_security_groups"])
             check_type(argname="argument allowed_vpc", value=allowed_vpc, expected_type=type_hints["allowed_vpc"])
+            check_type(argname="argument allowed_vpc_endpoints", value=allowed_vpc_endpoints, expected_type=type_hints["allowed_vpc_endpoints"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if allowed_ips is not None:
             self._values["allowed_ips"] = allowed_ips
         if allowed_security_groups is not None:
             self._values["allowed_security_groups"] = allowed_security_groups
         if allowed_vpc is not None:
             self._values["allowed_vpc"] = allowed_vpc
+        if allowed_vpc_endpoints is not None:
+            self._values["allowed_vpc_endpoints"] = allowed_vpc_endpoints
 
     @builtins.property
     def allowed_ips(self) -> typing.Optional[typing.List[builtins.str]]:
         '''(experimental) List of IP addresses in CIDR notation that are allowed to access the API Gateway.
 
         If not specified on public API Gateway, all IP addresses are allowed.
 
@@ -681,21 +687,36 @@
         :stability: experimental
         '''
         result = self._values.get("allowed_security_groups")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
 
     @builtins.property
     def allowed_vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
-        '''(experimental) Creates a private API Gateway and allows access from the specified VPC.
+        '''(experimental) Create a private API Gateway and allow access from the specified VPC.
 
         :stability: experimental
         '''
         result = self._values.get("allowed_vpc")
         return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
 
+    @builtins.property
+    def allowed_vpc_endpoints(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.IVpcEndpoint]]:
+        '''(experimental) Create a private API Gateway and allow access from the specified VPC endpoints.
+
+        Use this to make use of existing VPC endpoints. The VPC endpoint must point to ``ec2.InterfaceVpcEndpointAwsService.APIGATEWAY``.
+
+        No other settings are supported when using this option.
+
+        :stability: experimental
+        '''
+        result = self._values.get("allowed_vpc_endpoints")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.IVpcEndpoint]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1535,21 +1556,21 @@
         webhook_access: typing.Optional["LambdaAccess"] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param allow_public_subnet: (experimental) Allow management functions to run in public subnets. Lambda Functions in a public subnet can NOT access the internet. Default: false
         :param extra_certificates: (experimental) Path to a directory containing a file named certs.pem containing any additional certificates required to trust GitHub Enterprise Server. Use this when GitHub Enterprise Server certificates are self-signed. You may also want to use custom images for your runner providers that contain the same certificates. See {@link CodeBuildImageBuilder.addCertificates }:: const imageBuilder = CodeBuildRunnerProvider.imageBuilder(this, 'Image Builder with Certs'); imageBuilder.addComponent(RunnerImageComponent.extraCertificates('path-to-my-extra-certs-folder/certs.pem', 'private-ca'); const provider = new CodeBuildRunnerProvider(this, 'CodeBuild', { imageBuilder: imageBuilder, }); new GitHubRunners( this, 'runners', { providers: [provider], extraCertificates: 'path-to-my-extra-certs-folder', } );
-        :param idle_timeout: (experimental) Time to wait before stopping a runner that remains idle. If the user cancelled the job, or if another runner stole it, this stops the runner to avoid wasting resources. Default: 10 minutes
+        :param idle_timeout: (experimental) Time to wait before stopping a runner that remains idle. If the user cancelled the job, or if another runner stole it, this stops the runner to avoid wasting resources. Default: 5 minutes
         :param log_options: (experimental) Logging options for the state machine that manages the runners. Default: no logs
         :param providers: (experimental) List of runner providers to use. At least one provider is required. Provider will be selected when its label matches the labels requested by the workflow job. Default: CodeBuild, Lambda and Fargate runners with all the defaults (no VPC or default account VPC)
         :param security_group: (experimental) Security group attached to all management functions. Use this with to provide access to GitHub Enterprise Server hosted inside a VPC.
         :param setup_access: (experimental) Access configuration for the setup function. Once you finish the setup process, you can set this to ``LambdaAccess.noAccess()`` to remove access to the setup function. You can also use ``LambdaAccess.apiGateway({ allowedIps: ['my-ip/0']})`` to limit access to your IP only. Default: LambdaAccess.lambdaUrl()
         :param status_access: (experimental) Access configuration for the status function. This function returns a lot of sensitive information about the runner, so you should only allow access to it from trusted IPs, if at all. Default: LambdaAccess.noAccess()
-        :param vpc: (experimental) VPC used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC.
+        :param vpc: (experimental) VPC used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC. Make sure the selected VPC and subnets have access to the following with either NAT Gateway or VPC Endpoints: - GitHub Enterprise Server - Secrets Manager - SQS - Step Functions - CloudFormation (status function only) - EC2 (status function only) - ECR (status function only)
         :param vpc_subnets: (experimental) VPC subnets used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC.
         :param webhook_access: (experimental) Access configuration for the webhook function. This function is called by GitHub when a new workflow job is scheduled. For an extra layer of security, you can set this to ``LambdaAccess.apiGateway({ allowedIps: LambdaAccess.githubWebhookIps() })``. You can also set this to ``LambdaAccess.privateApiGateway()`` if your GitHub Enterprise Server is hosted in a VPC. This will create an API Gateway endpoint that's only accessible from within the VPC. *WARNING*: changing access type may change the URL. When the URL changes, you must update GitHub as well. Default: LambdaAccess.lambdaUrl()
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c1a45de07d09ed9f4fd0b9051aeff4571ceda633f49c0b30a5058ad6d72fad18)
@@ -1835,21 +1856,21 @@
         vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
         webhook_access: typing.Optional["LambdaAccess"] = None,
     ) -> None:
         '''(experimental) Properties for GitHubRunners.
 
         :param allow_public_subnet: (experimental) Allow management functions to run in public subnets. Lambda Functions in a public subnet can NOT access the internet. Default: false
         :param extra_certificates: (experimental) Path to a directory containing a file named certs.pem containing any additional certificates required to trust GitHub Enterprise Server. Use this when GitHub Enterprise Server certificates are self-signed. You may also want to use custom images for your runner providers that contain the same certificates. See {@link CodeBuildImageBuilder.addCertificates }:: const imageBuilder = CodeBuildRunnerProvider.imageBuilder(this, 'Image Builder with Certs'); imageBuilder.addComponent(RunnerImageComponent.extraCertificates('path-to-my-extra-certs-folder/certs.pem', 'private-ca'); const provider = new CodeBuildRunnerProvider(this, 'CodeBuild', { imageBuilder: imageBuilder, }); new GitHubRunners( this, 'runners', { providers: [provider], extraCertificates: 'path-to-my-extra-certs-folder', } );
-        :param idle_timeout: (experimental) Time to wait before stopping a runner that remains idle. If the user cancelled the job, or if another runner stole it, this stops the runner to avoid wasting resources. Default: 10 minutes
+        :param idle_timeout: (experimental) Time to wait before stopping a runner that remains idle. If the user cancelled the job, or if another runner stole it, this stops the runner to avoid wasting resources. Default: 5 minutes
         :param log_options: (experimental) Logging options for the state machine that manages the runners. Default: no logs
         :param providers: (experimental) List of runner providers to use. At least one provider is required. Provider will be selected when its label matches the labels requested by the workflow job. Default: CodeBuild, Lambda and Fargate runners with all the defaults (no VPC or default account VPC)
         :param security_group: (experimental) Security group attached to all management functions. Use this with to provide access to GitHub Enterprise Server hosted inside a VPC.
         :param setup_access: (experimental) Access configuration for the setup function. Once you finish the setup process, you can set this to ``LambdaAccess.noAccess()`` to remove access to the setup function. You can also use ``LambdaAccess.apiGateway({ allowedIps: ['my-ip/0']})`` to limit access to your IP only. Default: LambdaAccess.lambdaUrl()
         :param status_access: (experimental) Access configuration for the status function. This function returns a lot of sensitive information about the runner, so you should only allow access to it from trusted IPs, if at all. Default: LambdaAccess.noAccess()
-        :param vpc: (experimental) VPC used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC.
+        :param vpc: (experimental) VPC used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC. Make sure the selected VPC and subnets have access to the following with either NAT Gateway or VPC Endpoints: - GitHub Enterprise Server - Secrets Manager - SQS - Step Functions - CloudFormation (status function only) - EC2 (status function only) - ECR (status function only)
         :param vpc_subnets: (experimental) VPC subnets used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC.
         :param webhook_access: (experimental) Access configuration for the webhook function. This function is called by GitHub when a new workflow job is scheduled. For an extra layer of security, you can set this to ``LambdaAccess.apiGateway({ allowedIps: LambdaAccess.githubWebhookIps() })``. You can also set this to ``LambdaAccess.privateApiGateway()`` if your GitHub Enterprise Server is hosted in a VPC. This will create an API Gateway endpoint that's only accessible from within the VPC. *WARNING*: changing access type may change the URL. When the URL changes, you must update GitHub as well. Default: LambdaAccess.lambdaUrl()
 
         :stability: experimental
         '''
         if isinstance(log_options, dict):
             log_options = LogOptions(**log_options)
@@ -1934,15 +1955,15 @@
 
     @builtins.property
     def idle_timeout(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) Time to wait before stopping a runner that remains idle.
 
         If the user cancelled the job, or if another runner stole it, this stops the runner to avoid wasting resources.
 
-        :default: 10 minutes
+        :default: 5 minutes
 
         :stability: experimental
         '''
         result = self._values.get("idle_timeout")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
@@ -2006,17 +2027,25 @@
         :stability: experimental
         '''
         result = self._values.get("status_access")
         return typing.cast(typing.Optional["LambdaAccess"], result)
 
     @builtins.property
     def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
-        '''(experimental) VPC used for all management functions.
+        '''(experimental) VPC used for all management functions. Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC.
 
-        Use this with GitHub Enterprise Server hosted that's inaccessible from outside the VPC.
+        Make sure the selected VPC and subnets have access to the following with either NAT Gateway or VPC Endpoints:
+
+        - GitHub Enterprise Server
+        - Secrets Manager
+        - SQS
+        - Step Functions
+        - CloudFormation (status function only)
+        - EC2 (status function only)
+        - ECR (status function only)
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
 
     @builtins.property
@@ -2980,14 +3009,15 @@
     @builtins.classmethod
     def api_gateway(
         cls,
         *,
         allowed_ips: typing.Optional[typing.Sequence[builtins.str]] = None,
         allowed_security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         allowed_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+        allowed_vpc_endpoints: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.IVpcEndpoint]] = None,
     ) -> "LambdaAccess":
         '''(experimental) Provide access using API Gateway.
 
         This is the most secure option, but requires additional configuration. It allows you to limit access to specific IP addresses and even to a specific VPC.
 
         To limit access to GitHub.com use::
 
@@ -2997,22 +3027,24 @@
 
         Alternatively, get and manually update the list manually with::
 
            curl https://api.github.com/meta | jq .hooks
 
         :param allowed_ips: (experimental) List of IP addresses in CIDR notation that are allowed to access the API Gateway. If not specified on public API Gateway, all IP addresses are allowed. If not specified on private API Gateway, no IP addresses are allowed (but specified security groups are).
         :param allowed_security_groups: (experimental) List of security groups that are allowed to access the API Gateway. Only works for private API Gateways with {@link allowedVpc}.
-        :param allowed_vpc: (experimental) Creates a private API Gateway and allows access from the specified VPC.
+        :param allowed_vpc: (experimental) Create a private API Gateway and allow access from the specified VPC.
+        :param allowed_vpc_endpoints: (experimental) Create a private API Gateway and allow access from the specified VPC endpoints. Use this to make use of existing VPC endpoints. The VPC endpoint must point to ``ec2.InterfaceVpcEndpointAwsService.APIGATEWAY``. No other settings are supported when using this option.
 
         :stability: experimental
         '''
         props = ApiGatewayAccessProps(
             allowed_ips=allowed_ips,
             allowed_security_groups=allowed_security_groups,
             allowed_vpc=allowed_vpc,
+            allowed_vpc_endpoints=allowed_vpc_endpoints,
         )
 
         return typing.cast("LambdaAccess", jsii.sinvoke(cls, "apiGateway", [props]))
 
     @jsii.member(jsii_name="githubWebhookIps")
     @builtins.classmethod
     def github_webhook_ips(cls) -> typing.List[builtins.str]:
@@ -9945,14 +9977,15 @@
     pass
 
 def _typecheckingstub__0230281aea2f0096e32af8e4f02c3c351aada0957c217590514bfc5f6f656b0e(
     *,
     allowed_ips: typing.Optional[typing.Sequence[builtins.str]] = None,
     allowed_security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     allowed_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    allowed_vpc_endpoints: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.IVpcEndpoint]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__197fbc91031fbef228119c4ea4b7d54d7ee7ae2efdfedf7354f2313378ee5db9(
     instance_type: _aws_cdk_aws_ec2_ceddda9d.InstanceType,
 ) -> None:
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.7
+Version: 0.9.8
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt` & `cloudsnorkel.cdk-github-runners-0.9.8/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
 src/cloudsnorkel/cdk_github_runners/__init__.py
 src/cloudsnorkel/cdk_github_runners/py.typed
 src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
-src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.7.jsii.tgz
+src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.8.jsii.tgz
```

