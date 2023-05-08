# Comparing `tmp/edk2-pytool-extensions-0.9.4.tar.gz` & `tmp/edk2-pytool-extensions-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/edk2-pytool-extensions-0.9.4.tar", last modified: Fri Aug  9 18:14:41 2019, max compression
+gzip compressed data, was "dist/edk2-pytool-extensions-0.9.5.tar", last modified: Mon Aug 12 05:39:30 2019, max compression
```

## Comparing `edk2-pytool-extensions-0.9.4.tar` & `edk2-pytool-extensions-0.9.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/
--rw-r--r--   0 vsts      (1001) docker     (117)     3209 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/BasicDevTests.py
--rw-r--r--   0 vsts      (1001) docker     (117)      761 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/ConfirmVersionAndTag.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2726 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (117)      135 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (117)     7672 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/docs/
--rw-r--r--   0 vsts      (1001) docker     (117)     2601 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/developing.md
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/docs/features/
--rw-r--r--   0 vsts      (1001) docker     (117)     1050 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/features/feature_extdep.md
--rw-r--r--   0 vsts      (1001) docker     (117)     3514 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/features/feature_invocables.md
--rw-r--r--   0 vsts      (1001) docker     (117)      826 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/features/feature_plugin_manager.md
--rw-r--r--   0 vsts      (1001) docker     (117)    10703 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/features/feature_sde.md
--rw-r--r--   0 vsts      (1001) docker     (117)     1838 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/publishing.md
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/docs/usability/
--rw-r--r--   0 vsts      (1001) docker     (117)     8880 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/usability/using_extdep.md
--rw-r--r--   0 vsts      (1001) docker     (117)      869 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/usability/using_logging.md
--rw-r--r--   0 vsts      (1001) docker     (117)     3199 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/usability/using_nuget_publishing.md
--rw-r--r--   0 vsts      (1001) docker     (117)     8091 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/usability/using_omnicache.md
--rw-r--r--   0 vsts      (1001) docker     (117)     7937 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/usability/using_plugin_manager.md
--rw-r--r--   0 vsts      (1001) docker     (117)     6952 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/usability/using_settings_manager.md
--rw-r--r--   0 vsts      (1001) docker     (117)     7320 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/docs/using.md
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (117)     7672 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)     2747 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      399 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (117)       34 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (117)       12 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5136 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/base_abstract_invocable.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/bin/
--rw-r--r--   0 vsts      (1001) docker     (117)  5734488 2019-08-09 18:12:42.000000 edk2-pytool-extensions-0.9.4/edk2toolext/bin/NuGet.exe
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/bin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1465 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/bin/nuget.py
--rw-r--r--   0 vsts      (1001) docker     (117)       60 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/bin/readme.md
--rw-r--r--   0 vsts      (1001) docker     (117)    10146 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/config_validator.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8385 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/edk2_git.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6964 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/edk2_invocable.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9283 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/edk2_logging.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9741 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/conf_mgmt.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4502 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/environment_descriptor_files.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4141 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/git_dependency.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6591 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/nuget_dependency.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6887 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/web_dependency.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6275 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/external_dependency.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5018 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/multiple_workspace.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2980 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugin_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4421 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/ci_build_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (117)      721 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/dsc_processor_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (117)      713 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/uefi_build_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2379 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/uefi_helper_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9589 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/repo_resolver.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11710 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/self_describing_environment.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10174 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/shell_environment.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20462 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/uefi_build.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5700 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/var_dict.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2509 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/environment/version_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13503 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_ci_build.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3820 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_ci_setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5574 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_platform_build.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8583 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3009 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_update.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20449 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/nuget_publishing.py
--rw-r--r--   0 vsts      (1001) docker     (117)    15784 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/omnicache.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/
--rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5798 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_config_validator.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2186 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_edk2_logging.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12313 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_git_dependency.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4674 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_omnicache.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9811 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_repo_resolver.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2822 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_self_describing_environment.py
--rw-r--r--   0 vsts      (1001) docker     (117)    18719 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_shell_environment.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6545 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_var_dict.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14307 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_web_dependency.py
--rw-r--r--   0 vsts      (1001) docker     (117)       38 2019-08-09 18:14:41.000000 edk2-pytool-extensions-0.9.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (117)     2636 2019-08-09 18:12:25.000000 edk2-pytool-extensions-0.9.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/
+-rw-r--r--   0 vsts      (1001) docker     (117)     3209 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/BasicDevTests.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      761 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/ConfirmVersionAndTag.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2726 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (117)      135 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (117)     8043 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/docs/
+-rw-r--r--   0 vsts      (1001) docker     (117)     2601 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/developing.md
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/docs/features/
+-rw-r--r--   0 vsts      (1001) docker     (117)     1050 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/features/feature_extdep.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     3514 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/features/feature_invocables.md
+-rw-r--r--   0 vsts      (1001) docker     (117)      826 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/features/feature_plugin_manager.md
+-rw-r--r--   0 vsts      (1001) docker     (117)    10703 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/features/feature_sde.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     1838 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/publishing.md
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/docs/usability/
+-rw-r--r--   0 vsts      (1001) docker     (117)     8880 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/usability/using_extdep.md
+-rw-r--r--   0 vsts      (1001) docker     (117)      869 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/usability/using_logging.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     3199 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/usability/using_nuget_publishing.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     8091 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/usability/using_omnicache.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     7937 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/usability/using_plugin_manager.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     6952 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/usability/using_settings_manager.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     7320 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/docs/using.md
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (117)     8043 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)     2747 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)      399 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)       34 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)       12 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5136 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/base_abstract_invocable.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/bin/
+-rw-r--r--   0 vsts      (1001) docker     (117)  5734488 2019-08-12 05:37:33.000000 edk2-pytool-extensions-0.9.5/edk2toolext/bin/NuGet.exe
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/bin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1465 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/bin/nuget.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       60 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/bin/readme.md
+-rw-r--r--   0 vsts      (1001) docker     (117)    10146 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/config_validator.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8385 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/edk2_git.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6964 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/edk2_invocable.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9283 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/edk2_logging.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9741 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/conf_mgmt.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4502 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/environment_descriptor_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4141 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/git_dependency.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6591 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/nuget_dependency.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6887 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/web_dependency.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6275 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/external_dependency.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5018 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/multiple_workspace.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2980 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugin_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4630 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/ci_build_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      721 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/dsc_processor_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      713 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/uefi_build_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2379 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/uefi_helper_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9589 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/repo_resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11710 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/self_describing_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10174 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/shell_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20462 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/uefi_build.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6080 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/var_dict.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2509 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/environment/version_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13779 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_ci_build.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3820 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_ci_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5574 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_platform_build.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8583 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3009 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_update.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20449 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/nuget_publishing.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    15784 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/omnicache.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/
+-rw-r--r--   0 vsts      (1001) docker     (117)       93 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5798 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_config_validator.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2186 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_edk2_logging.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    12313 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_git_dependency.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4674 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_omnicache.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9811 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_repo_resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2822 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_self_describing_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    18719 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_shell_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7433 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_var_dict.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14307 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_web_dependency.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       38 2019-08-12 05:39:30.000000 edk2-pytool-extensions-0.9.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (117)     2636 2019-08-12 05:37:14.000000 edk2-pytool-extensions-0.9.5/setup.py
```

### Comparing `edk2-pytool-extensions-0.9.4/BasicDevTests.py` & `edk2-pytool-extensions-0.9.5/BasicDevTests.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/ConfirmVersionAndTag.py` & `edk2-pytool-extensions-0.9.5/ConfirmVersionAndTag.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/LICENSE` & `edk2-pytool-extensions-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/PKG-INFO` & `edk2-pytool-extensions-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edk2-pytool-extensions
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python tools supporting UEFI EDK2 firmware development
 Home-page: https://github.com/tianocore/edk2-pytool-extensions
 Author: Tianocore Edk2-PyTool-Extensions team
 Author-email: sean.brogan@microsoft.com
 License: BSD-2-Clause-Patent
 Description: # Tianocore Edk2 PyTool Extensions (edk2toolext)
         
@@ -44,14 +44,22 @@
         
             ```python
             from edk2toolext.<module> import <class>
             ```
         
         ## Release Version History
         
+        ### Version 0.9.5
+        
+        * Features:
+          * Issue 27 - Add Api to allow override of var_dict entry
+          * Change CIBuild plugins to allow detection of skipping using newly defined return code
+        * Bugs
+          * Issue 27 - When a build variable is updated with same value but different attributes those attributes are not set.
+        
         ### Version 0.9.4
         
         * Bugs
           * Issue 14 - XML log created by Stuart_ci_build has incorrect fields
         
         ### Version 0.9.3
```

### Comparing `edk2-pytool-extensions-0.9.4/docs/developing.md` & `edk2-pytool-extensions-0.9.5/docs/developing.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/features/feature_extdep.md` & `edk2-pytool-extensions-0.9.5/docs/features/feature_extdep.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/features/feature_invocables.md` & `edk2-pytool-extensions-0.9.5/docs/features/feature_invocables.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/features/feature_plugin_manager.md` & `edk2-pytool-extensions-0.9.5/docs/features/feature_plugin_manager.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/features/feature_sde.md` & `edk2-pytool-extensions-0.9.5/docs/features/feature_sde.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/publishing.md` & `edk2-pytool-extensions-0.9.5/docs/publishing.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/usability/using_extdep.md` & `edk2-pytool-extensions-0.9.5/docs/usability/using_extdep.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/usability/using_logging.md` & `edk2-pytool-extensions-0.9.5/docs/usability/using_logging.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/usability/using_nuget_publishing.md` & `edk2-pytool-extensions-0.9.5/docs/usability/using_nuget_publishing.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/usability/using_omnicache.md` & `edk2-pytool-extensions-0.9.5/docs/usability/using_omnicache.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/usability/using_plugin_manager.md` & `edk2-pytool-extensions-0.9.5/docs/usability/using_plugin_manager.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/usability/using_settings_manager.md` & `edk2-pytool-extensions-0.9.5/docs/usability/using_settings_manager.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/docs/using.md` & `edk2-pytool-extensions-0.9.5/docs/using.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/PKG-INFO` & `edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edk2-pytool-extensions
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python tools supporting UEFI EDK2 firmware development
 Home-page: https://github.com/tianocore/edk2-pytool-extensions
 Author: Tianocore Edk2-PyTool-Extensions team
 Author-email: sean.brogan@microsoft.com
 License: BSD-2-Clause-Patent
 Description: # Tianocore Edk2 PyTool Extensions (edk2toolext)
         
@@ -44,14 +44,22 @@
         
             ```python
             from edk2toolext.<module> import <class>
             ```
         
         ## Release Version History
         
+        ### Version 0.9.5
+        
+        * Features:
+          * Issue 27 - Add Api to allow override of var_dict entry
+          * Change CIBuild plugins to allow detection of skipping using newly defined return code
+        * Bugs
+          * Issue 27 - When a build variable is updated with same value but different attributes those attributes are not set.
+        
         ### Version 0.9.4
         
         * Bugs
           * Issue 14 - XML log created by Stuart_ci_build has incorrect fields
         
         ### Version 0.9.3
```

### Comparing `edk2-pytool-extensions-0.9.4/edk2_pytool_extensions.egg-info/SOURCES.txt` & `edk2-pytool-extensions-0.9.5/edk2_pytool_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/base_abstract_invocable.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/base_abstract_invocable.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/bin/NuGet.exe` & `edk2-pytool-extensions-0.9.5/edk2toolext/bin/NuGet.exe`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/bin/nuget.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/bin/nuget.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/config_validator.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/config_validator.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/edk2_git.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/edk2_git.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/edk2_invocable.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/edk2_invocable.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/edk2_logging.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/edk2_logging.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/conf_mgmt.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/conf_mgmt.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/environment_descriptor_files.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/environment_descriptor_files.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/git_dependency.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/git_dependency.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/nuget_dependency.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/nuget_dependency.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/extdeptypes/web_dependency.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/extdeptypes/web_dependency.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/external_dependency.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/external_dependency.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/multiple_workspace.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/multiple_workspace.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugin_manager.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/ci_build_plugin.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/ci_build_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,22 @@
     #
     #   - package is the edk2 path to package.  This means workspace/packagepath relative.
     #   - edk2path object configured with workspace and packages path
     #   - PkgConfig Object (dict) for the pkg
     #   - EnvConfig Object
     #   - Plugin Manager Instance
     #   - Plugin Helper Obj Instance
-    #   - Junit Logger
+    #   - tc - test case that needs state configured for reporting by plugin.
     #   - output_stream the StringIO output stream from this plugin via logging
+    #
+    #   Returns  >0 : number of errors found
+    #             0 : passed successfully
+    #            -1 : skipped for missing prereq
+    #
+    #
     def RunBuildPlugin(self, packagename, Edk2pathObj, pkgconfig, environment, PLM, PLMHelper, tc, output_stream):
         pass
 
     ##
     # Return tuple (string, string) that is the (test case name, test case base class name)
     #
     #
```

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/dsc_processor_plugin.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/dsc_processor_plugin.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/uefi_build_plugin.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/uefi_build_plugin.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/plugintypes/uefi_helper_plugin.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/plugintypes/uefi_helper_plugin.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/repo_resolver.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/repo_resolver.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/self_describing_environment.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/self_describing_environment.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/shell_environment.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/shell_environment.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/uefi_build.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/uefi_build.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/var_dict.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/var_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,31 @@
             print("Value overridable", file=f)
         print("**********************", file=f)
     #
     # Function used to override the value if option allows it
     #
 
     def SetValue(self, value, comment, overridable=False):
-        if (value == self.Value):
+        if (value == self.Value) and (overridable == self.Overrideable):
             return True
 
         if(not self.Overrideable):
             logging.debug("Can't set value [%s] as it isn't overrideable. Previous comment %s" % (
                 value, self.Comment))
             return False
 
         self.Value = value
         self.Comment = comment
         self.Overrideable = overridable
         return True
 
+    def AllowOverride(self):
+        self.Overrideable = True
+        return True
+
     def GetValue(self):
         return self.Value
 
 
 class VarDict(object):
     def __init__(self):
         self.Logger = logging.getLogger("EnvDict")
@@ -91,14 +95,23 @@
             # new entry
             en = EnvEntry(value, comment, overridable)
             self.Dstore[key] = en
             return True
 
         return en.SetValue(value, comment, overridable)
 
+    def AllowOverride(self, k):
+        key = k.upper()
+        en = self.GetEntry(key)
+        if(en is not None):
+            self.Logger.warn("Allowing Override for key %s" % k)
+            en.AllowOverride()
+            return True
+        return False
+
     #
     # function used to get a build var value for given key and buildtype
     #
     # if BuildType is None
     # Build vars are defined by vars that start with BLD_
     #  BLD_*_<YOUR KEY HERE> means all build types
     #  BLD_DEBUG_<YOUR KEY HERE> means build of debug type
```

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/environment/version_aggregator.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/environment/version_aggregator.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_ci_build.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_ci_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,36 +136,39 @@
         for dependency in self.PlatformSettings.GetDependencies():
             pplist.append(dependency["Path"])
 
         # make Edk2Path object to handle all path operations
         try:
             edk2path = Edk2Path(self.GetWorkspaceRoot(), pplist)
         except Exception as e:
-            logging.error("You need to run stewart_ci_setup to resolve all repos.")
+            logging.error("Src Tree is invalid.  Did you Setup correctly?")
             raise e
 
         logging.info(f"Running CI Build: {self.PlatformSettings.GetName()}")
         logging.info(f"WorkSpace: {self.GetWorkspaceRoot()}")
         logging.info(f"Package Path: {self.PlatformSettings.GetPackagesPath()}")
         # logging.info("mu_build version: {0}".format(pkg_resources.get_distribution("mu_build").version))
         # logging.info("mu_python_library version: " + pkg_resources.get_distribution("mu_python_library").version)
         # logging.info("mu_environment version: " + pkg_resources.get_distribution("mu_environment").version)
         # Bring up the common minimum environment.
-        logging.log(edk2_logging.SECTION, "Getting Enviroment")
+        logging.log(edk2_logging.SECTION, "Getting Environment")
         (build_env, shell_env) = self_describing_environment.BootstrapEnvironment(
             self.GetWorkspaceRoot(), self.GetActiveScopes())
         env = shell_environment.GetBuildVars()
 
         # Bind our current execution environment into the shell vars.
         ph = os.path.dirname(sys.executable)
         if " " in ph:
             ph = '"' + ph + '"'
         shell_env.set_shell_var("PYTHON_HOME", ph)
         # PYTHON_COMMAND is required to be set for using edk2 python builds.
-        # todo: work with edk2 to remove the bat file and move to native python calls
+        # todo: work with edk2 to remove the bat file and move to native python calls.
+        #       This would be better in an edk2 plugin so that it could be modified/controlled
+        #       more easily
+        #
         pc = sys.executable
         if " " in pc:
             pc = '"' + pc + '"'
         shell_env.set_shell_var("PYTHON_COMMAND", pc)
 
         archSupported = " ".join(self.PlatformSettings.GetArchSupported())
         env.SetValue("TARGET_ARCH", archSupported, "from PlatformSettings.GetArchSupported()")
@@ -273,24 +276,26 @@
                             logging.critical("EXCEPTION: {0}".format(exp))
                             exceptionPrint = traceback.format_exception(type(exp), exp, exc_traceback)
                             logging.critical(" ".join(exceptionPrint))
                             tc.SetError("Exception: {0}".format(
                                 exp), "UNEXPECTED EXCEPTION")
                             rc = 1
 
-                        if(rc != 0):
+                        if(rc > 0):
                             failure_num += 1
                             if(rc is None):
                                 logging.error(
-                                    "--->Test Failed: %s returned NoneType" % Descriptor.Name)
+                                    f"--->Test Failed: {Descriptor.Name} {target} returned NoneType")
                             else:
                                 logging.error(
-                                    "--->Test Failed: %s returned %d" % (Descriptor.Name, rc))
+                                    f"--->Test Failed: {Descriptor.Name} {target} returned {rc}")
+                        elif(rc < 0):
+                            logging.warn(f"--->Test Skipped: in plugin! {Descriptor.Name} {target}")
                         else:
-                            edk2_logging.log_progress(f"--->Test Success {Descriptor.Name} {target}")
+                            edk2_logging.log_progress(f"--->Test Success: {Descriptor.Name} {target}")
 
                     # revert to the checkpoint we created previously
                     shell_environment.RevertBuildVars()
                     # remove the logger
                     edk2_logging.remove_output_stream(plugin_output_stream)
                 # finished target loop
             # Finished plugin loop
```

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_ci_setup.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_ci_setup.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_platform_build.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_platform_build.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_setup.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_setup.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/invocables/edk2_update.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/invocables/edk2_update.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/nuget_publishing.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/nuget_publishing.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/omnicache.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/omnicache.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_config_validator.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_edk2_logging.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_edk2_logging.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_git_dependency.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_git_dependency.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_omnicache.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_omnicache.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_repo_resolver.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_repo_resolver.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_self_describing_environment.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_self_describing_environment.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_shell_environment.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_shell_environment.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_var_dict.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_var_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,31 @@
         v = var_dict.VarDict()
         v.SetValue("test1", "value1", "test 1 comment", True)
         ## confirm override == true
         v.SetValue("test1", "value2", "test for override")
         vv = v.GetValue("test1")
         self.assertEqual("value2", vv)
 
+    def test_var_dict_can_change_override_state_with_same_set(self):
+        v = var_dict.VarDict()
+        v.SetValue("test1", "value1", "test 1 comment", True)
+        v.SetValue("test1", "value1", "Change override to false", False)
+        v.SetValue("test1", "value2", "this should fail", False)
+        self.assertNotEqual(v.GetValue("test1"), "value2")
+
+    def test_var_dict_can_change_override_state_with_allow_override(self):
+        v = var_dict.VarDict()
+        v.SetValue("test1", "value1", "test 1 comment", False)
+        v.AllowOverride("test1")
+        v.SetValue("test1", "value2", "this should be allowed", False)
+        self.assertEqual(v.GetValue("test1"), "value2")
+        ## since override was set to False should not change again
+        v.SetValue("test1", "value3", "this should not be allowed", False)
+        self.assertEqual(v.GetValue("test1"), "value2")
+
     def test_var_dict_key_not_case_sensitive(self):
         v = var_dict.VarDict()
         v.SetValue("test1", "value1", "test 1 comment")
         ## confirm case sensitivity
         vv = v.GetValue("TEST1")
         self.assertEqual("value1", vv)
```

### Comparing `edk2-pytool-extensions-0.9.4/edk2toolext/tests/test_web_dependency.py` & `edk2-pytool-extensions-0.9.5/edk2toolext/tests/test_web_dependency.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-extensions-0.9.4/setup.py` & `edk2-pytool-extensions-0.9.5/setup.py`

 * *Files identical despite different names*

