# Comparing `tmp/animo_trainer-0.1.8.tar.gz` & `tmp/animo_trainer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animo_trainer-0.1.8.tar", last modified: Tue Mar 21 21:41:47 2023, max compression
+gzip compressed data, was "animo_trainer-0.1.9.tar", last modified: Thu Mar 23 22:25:21 2023, max compression
```

## Comparing `animo_trainer-0.1.8.tar` & `animo_trainer-0.1.9.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.693035 animo_trainer-0.1.8/
--rw-rw-rw-   0        0        0       68 2023-03-20 18:37:35.000000 animo_trainer-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      106 2023-03-20 18:37:35.000000 animo_trainer-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      772 2023-03-21 21:41:47.692035 animo_trainer-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-03-21 16:09:40.000000 animo_trainer-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.225342 animo_trainer-0.1.8/animo_trainer/
--rw-rw-rw-   0        0        0       32 2023-03-21 19:45:58.000000 animo_trainer-0.1.8/animo_trainer/__init__.py
--rw-rw-rw-   0        0        0     5580 2023-03-17 21:48:34.000000 animo_trainer-0.1.8/animo_trainer/animo_env.py
--rw-rw-rw-   0        0        0      558 2023-03-17 21:48:34.000000 animo_trainer-0.1.8/animo_trainer/animo_stats_writers.py
--rw-rw-rw-   0        0        0     2939 2023-03-21 20:44:18.000000 animo_trainer-0.1.8/animo_trainer/animo_torch_model_saver.py
--rw-rw-rw-   0        0        0    12163 2023-03-21 21:06:57.000000 animo_trainer-0.1.8/animo_trainer/animo_trainer_controller.py
--rw-rw-rw-   0        0        0     5748 2023-03-21 21:20:59.000000 animo_trainer-0.1.8/animo_trainer/animo_training_session.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.305498 animo_trainer-0.1.8/animo_trainer/lib/
--rw-rw-rw-   0        0        0     2984 2023-03-21 17:13:52.000000 animo_trainer-0.1.8/animo_trainer/lib/AnimoData.deps.json
--rw-rw-rw-   0        0        0    17920 2023-03-21 21:41:34.000000 animo_trainer-0.1.8/animo_trainer/lib/AnimoData.dll
--rw-rw-rw-   0        0        0    13660 2023-03-21 21:41:34.000000 animo_trainer-0.1.8/animo_trainer/lib/AnimoData.pdb
--rw-rw-rw-   0        0        0     2609 2023-03-21 17:13:52.000000 animo_trainer-0.1.8/animo_trainer/lib/AnimoSimulation.deps.json
--rw-rw-rw-   0        0        0   204800 2023-03-21 17:13:52.000000 animo_trainer-0.1.8/animo_trainer/lib/AnimoSimulation.dll
--rw-rw-rw-   0        0        0   100340 2023-03-21 17:13:52.000000 animo_trainer-0.1.8/animo_trainer/lib/AnimoSimulation.pdb
--rw-rw-rw-   0        0        0   695336 2021-03-17 20:03:36.000000 animo_trainer-0.1.8/animo_trainer/lib/Newtonsoft.Json.dll
--rw-rw-rw-   0        0        0   163464 2018-05-15 13:29:44.000000 animo_trainer-0.1.8/animo_trainer/lib/System.Numerics.Vectors.dll
--rw-rw-rw-   0        0        0     2069 2023-03-21 21:06:32.000000 animo_trainer-0.1.8/animo_trainer/main.py
--rw-rw-rw-   0        0        0      941 2023-03-17 21:48:34.000000 animo_trainer-0.1.8/animo_trainer/typed_numpy.py
--rw-rw-rw-   0        0        0       21 2023-03-21 21:36:16.000000 animo_trainer-0.1.8/animo_trainer/version.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.248348 animo_trainer-0.1.8/animo_trainer.egg-info/
--rw-rw-rw-   0        0        0      772 2023-03-21 21:41:47.000000 animo_trainer-0.1.8/animo_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4246 2023-03-21 21:41:47.000000 animo_trainer-0.1.8/animo_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 21:41:47.000000 animo_trainer-0.1.8/animo_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-21 21:41:47.000000 animo_trainer-0.1.8/animo_trainer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-03-21 21:41:47.000000 animo_trainer-0.1.8/animo_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-21 21:41:47.000000 animo_trainer-0.1.8/animo_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-21 21:41:47.693035 animo_trainer-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      955 2023-03-21 19:45:58.000000 animo_trainer-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.306498 animo_trainer-0.1.8/tests/
--rw-rw-rw-   0        0        0     2289 2023-03-17 18:40:23.000000 animo_trainer-0.1.8/tests/test_simulate.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.310499 animo_trainer-0.1.8/typings/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.317501 animo_trainer-0.1.8/typings/Internal/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.186334 animo_trainer-0.1.8/typings/Internal/Runtime/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.323026 animo_trainer-0.1.8/typings/Internal/Runtime/CompilerServices/
--rw-rw-rw-   0        0        0    10883 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/Internal/Runtime/CompilerServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.329021 animo_trainer-0.1.8/typings/Internal/Runtime/InteropServices/
--rw-rw-rw-   0        0        0     2615 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/Internal/Runtime/InteropServices/__init__.pyi
--rw-rw-rw-   0        0        0      392 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/Internal/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.186334 animo_trainer-0.1.8/typings/Microsoft/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.187333 animo_trainer-0.1.8/typings/Microsoft/Win32/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.335022 animo_trainer-0.1.8/typings/Microsoft/Win32/SafeHandles/
--rw-rw-rw-   0        0        0     1444 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/Microsoft/Win32/SafeHandles/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.336022 animo_trainer-0.1.8/typings/System/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.343024 animo_trainer-0.1.8/typings/System/Buffers/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.351025 animo_trainer-0.1.8/typings/System/Buffers/Binary/
--rw-rw-rw-   0        0        0     8554 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Buffers/Binary/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.358027 animo_trainer-0.1.8/typings/System/Buffers/Text/
--rw-rw-rw-   0        0        0     5939 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Buffers/Text/__init__.pyi
--rw-rw-rw-   0        0        0     8522 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Buffers/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.189335 animo_trainer-0.1.8/typings/System/CodeDom/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.364030 animo_trainer-0.1.8/typings/System/CodeDom/Compiler/
--rw-rw-rw-   0        0        0     5807 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/CodeDom/Compiler/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.365028 animo_trainer-0.1.8/typings/System/Collections/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.372031 animo_trainer-0.1.8/typings/System/Collections/Concurrent/
--rw-rw-rw-   0        0        0     2896 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Collections/Concurrent/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.373031 animo_trainer-0.1.8/typings/System/Collections/Generic/
--rw-rw-rw-   0        0        0    62665 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Collections/Generic/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.379032 animo_trainer-0.1.8/typings/System/Collections/ObjectModel/
--rw-rw-rw-   0        0        0     2798 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Collections/ObjectModel/__init__.pyi
--rw-rw-rw-   0        0        0    14037 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Collections/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.385033 animo_trainer-0.1.8/typings/System/ComponentModel/
--rw-rw-rw-   0        0        0     2389 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/ComponentModel/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.192335 animo_trainer-0.1.8/typings/System/Configuration/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.390035 animo_trainer-0.1.8/typings/System/Configuration/Assemblies/
--rw-rw-rw-   0        0        0      981 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Configuration/Assemblies/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.397037 animo_trainer-0.1.8/typings/System/Diagnostics/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.403047 animo_trainer-0.1.8/typings/System/Diagnostics/CodeAnalysis/
--rw-rw-rw-   0        0        0     7493 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Diagnostics/CodeAnalysis/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.410041 animo_trainer-0.1.8/typings/System/Diagnostics/Contracts/
--rw-rw-rw-   0        0        0    10649 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Diagnostics/Contracts/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.416042 animo_trainer-0.1.8/typings/System/Diagnostics/SymbolStore/
--rw-rw-rw-   0        0        0      298 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Diagnostics/SymbolStore/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.423044 animo_trainer-0.1.8/typings/System/Diagnostics/Tracing/
--rw-rw-rw-   0        0        0    21263 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Diagnostics/Tracing/__init__.pyi
--rw-rw-rw-   0        0        0    18735 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Diagnostics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.432047 animo_trainer-0.1.8/typings/System/Globalization/
--rw-rw-rw-   0        0        0    68863 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Globalization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.442048 animo_trainer-0.1.8/typings/System/IO/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.449050 animo_trainer-0.1.8/typings/System/IO/Enumeration/
--rw-rw-rw-   0        0        0     7685 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/IO/Enumeration/__init__.pyi
--rw-rw-rw-   0        0        0   102670 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/IO/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.454051 animo_trainer-0.1.8/typings/System/Net/
--rw-rw-rw-   0        0        0     1130 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Net/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.462052 animo_trainer-0.1.8/typings/System/Numerics/
--rw-rw-rw-   0        0        0    74395 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Numerics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.470024 animo_trainer-0.1.8/typings/System/Reflection/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.479026 animo_trainer-0.1.8/typings/System/Reflection/Emit/
--rw-rw-rw-   0        0        0    93675 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Reflection/Emit/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.486027 animo_trainer-0.1.8/typings/System/Reflection/Metadata/
--rw-rw-rw-   0        0        0      837 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Reflection/Metadata/__init__.pyi
--rw-rw-rw-   0        0        0   100095 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Reflection/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.492029 animo_trainer-0.1.8/typings/System/Resources/
--rw-rw-rw-   0        0        0     7254 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Resources/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.498031 animo_trainer-0.1.8/typings/System/Runtime/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.509038 animo_trainer-0.1.8/typings/System/Runtime/CompilerServices/
--rw-rw-rw-   0        0        0    74279 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Runtime/CompilerServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.514038 animo_trainer-0.1.8/typings/System/Runtime/ConstrainedExecution/
--rw-rw-rw-   0        0        0     1312 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/ConstrainedExecution/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.520039 animo_trainer-0.1.8/typings/System/Runtime/ExceptionServices/
--rw-rw-rw-   0        0        0     1054 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/ExceptionServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.530041 animo_trainer-0.1.8/typings/System/Runtime/InteropServices/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.537043 animo_trainer-0.1.8/typings/System/Runtime/InteropServices/ComTypes/
--rw-rw-rw-   0        0        0    29019 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Runtime/InteropServices/ComTypes/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.542044 animo_trainer-0.1.8/typings/System/Runtime/InteropServices/ObjectiveC/
--rw-rw-rw-   0        0        0     2322 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Runtime/InteropServices/ObjectiveC/__init__.pyi
--rw-rw-rw-   0        0        0    89234 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Runtime/InteropServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.549045 animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.560048 animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/Arm/
--rw-rw-rw-   0        0        0   376194 2023-03-21 21:41:37.000000 animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/Arm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.569052 animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/X86/
--rw-rw-rw-   0        0        0   197416 2023-03-21 21:41:38.000000 animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/X86/__init__.pyi
--rw-rw-rw-   0        0        0    53007 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.575054 animo_trainer-0.1.8/typings/System/Runtime/Loader/
--rw-rw-rw-   0        0        0     2563 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/Loader/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.579055 animo_trainer-0.1.8/typings/System/Runtime/Remoting/
--rw-rw-rw-   0        0        0      192 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/Remoting/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.580055 animo_trainer-0.1.8/typings/System/Runtime/Serialization/
--rw-rw-rw-   0        0        0    10688 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/Serialization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.585056 animo_trainer-0.1.8/typings/System/Runtime/Versioning/
--rw-rw-rw-   0        0        0     5655 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/Versioning/__init__.pyi
--rw-rw-rw-   0        0        0     4296 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Runtime/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.592057 animo_trainer-0.1.8/typings/System/Security/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.597058 animo_trainer-0.1.8/typings/System/Security/Cryptography/
--rw-rw-rw-   0        0        0     1211 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Security/Cryptography/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.603023 animo_trainer-0.1.8/typings/System/Security/Permissions/
--rw-rw-rw-   0        0        0     5712 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Security/Permissions/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.608015 animo_trainer-0.1.8/typings/System/Security/Principal/
--rw-rw-rw-   0        0        0     1308 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Security/Principal/__init__.pyi
--rw-rw-rw-   0        0        0    12014 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Security/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.616018 animo_trainer-0.1.8/typings/System/Text/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.622018 animo_trainer-0.1.8/typings/System/Text/Unicode/
--rw-rw-rw-   0        0        0      618 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Text/Unicode/__init__.pyi
--rw-rw-rw-   0        0        0    60174 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Text/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.632021 animo_trainer-0.1.8/typings/System/Threading/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.642023 animo_trainer-0.1.8/typings/System/Threading/Tasks/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.648024 animo_trainer-0.1.8/typings/System/Threading/Tasks/Sources/
--rw-rw-rw-   0        0        0     4015 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Threading/Tasks/Sources/__init__.pyi
--rw-rw-rw-   0        0        0    86620 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Threading/Tasks/__init__.pyi
--rw-rw-rw-   0        0        0    75007 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/Threading/__init__.pyi
--rw-rw-rw-   0        0        0   875103 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/System/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.206337 animo_trainer-0.1.8/typings/TransformsAI/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.214340 animo_trainer-0.1.8/typings/TransformsAI/Animo/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.649025 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.650025 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Database/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.651026 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Database/Tables/
--rw-rw-rw-   0        0        0     4883 2023-03-17 18:08:14.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Database/Tables/__init__.pyi
--rw-rw-rw-   0        0        0     3274 2023-03-17 18:08:14.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Database/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.652026 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Models/
--rw-rw-rw-   0        0        0     7158 2023-03-17 18:08:14.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Models/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.653026 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Utility/
--rw-rw-rw-   0        0        0     1350 2023-03-17 18:08:14.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Utility/__init__.pyi
--rw-rw-rw-   0        0        0     8174 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.655027 animo_trainer-0.1.8/typings/TransformsAI/Animo/Grid/
--rw-rw-rw-   0        0        0    15552 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Grid/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.210340 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.656027 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Observations/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.657027 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Observations/Primitives/
--rw-rw-rw-   0        0        0     3923 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Observations/Primitives/__init__.pyi
--rw-rw-rw-   0        0        0     4928 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Observations/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.658027 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Rewards/
--rw-rw-rw-   0        0        0    17004 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Rewards/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.659027 animo_trainer-0.1.8/typings/TransformsAI/Animo/Numerics/
--rw-rw-rw-   0        0        0     7549 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Numerics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.660028 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.661028 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/Items/
--rw-rw-rw-   0        0        0    71861 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/Items/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.668029 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/NPCs/
--rw-rw-rw-   0        0        0    14026 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/NPCs/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.675031 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/Resolutions/
--rw-rw-rw-   0        0        0     1936 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/Resolutions/__init__.pyi
--rw-rw-rw-   0        0        0    15145 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.676031 animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.677032 animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/Events/
--rw-rw-rw-   0        0        0     8314 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/Events/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.685033 animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/Intents/
--rw-rw-rw-   0        0        0     2146 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/Intents/__init__.pyi
--rw-rw-rw-   0        0        0      648 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-03-21 21:41:47.691036 animo_trainer-0.1.8/typings/TransformsAI/Animo/Tools/
--rw-rw-rw-   0        0        0     5634 2023-03-21 21:41:35.000000 animo_trainer-0.1.8/typings/TransformsAI/Animo/Tools/__init__.pyi
--rw-rw-rw-   0        0        0      146 2023-03-17 21:48:34.000000 animo_trainer-0.1.8/typings/clr.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.576696 animo_trainer-0.1.9/
+-rw-rw-rw-   0        0        0       68 2023-03-20 18:37:35.000000 animo_trainer-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      106 2023-03-20 18:37:35.000000 animo_trainer-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      772 2023-03-23 22:25:21.575696 animo_trainer-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-03-22 01:40:08.000000 animo_trainer-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.242620 animo_trainer-0.1.9/animo_trainer/
+-rw-rw-rw-   0        0        0       32 2023-03-22 01:40:08.000000 animo_trainer-0.1.9/animo_trainer/__init__.py
+-rw-rw-rw-   0        0        0     5580 2023-03-17 21:48:34.000000 animo_trainer-0.1.9/animo_trainer/animo_env.py
+-rw-rw-rw-   0        0        0      558 2023-03-17 21:48:34.000000 animo_trainer-0.1.9/animo_trainer/animo_stats_writers.py
+-rw-rw-rw-   0        0        0     2939 2023-03-22 01:40:08.000000 animo_trainer-0.1.9/animo_trainer/animo_torch_model_saver.py
+-rw-rw-rw-   0        0        0    12163 2023-03-22 01:40:08.000000 animo_trainer-0.1.9/animo_trainer/animo_trainer_controller.py
+-rw-rw-rw-   0        0        0     5748 2023-03-22 01:40:08.000000 animo_trainer-0.1.9/animo_trainer/animo_training_session.py
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.302635 animo_trainer-0.1.9/animo_trainer/lib/
+-rw-rw-rw-   0        0        0     2984 2023-03-21 17:13:52.000000 animo_trainer-0.1.9/animo_trainer/lib/AnimoData.deps.json
+-rw-rw-rw-   0        0        0    17920 2023-03-21 21:41:34.000000 animo_trainer-0.1.9/animo_trainer/lib/AnimoData.dll
+-rw-rw-rw-   0        0        0    13660 2023-03-21 21:41:34.000000 animo_trainer-0.1.9/animo_trainer/lib/AnimoData.pdb
+-rw-rw-rw-   0        0        0     2609 2023-03-21 17:13:52.000000 animo_trainer-0.1.9/animo_trainer/lib/AnimoSimulation.deps.json
+-rw-rw-rw-   0        0        0   204800 2023-03-21 17:13:52.000000 animo_trainer-0.1.9/animo_trainer/lib/AnimoSimulation.dll
+-rw-rw-rw-   0        0        0   100340 2023-03-21 17:13:52.000000 animo_trainer-0.1.9/animo_trainer/lib/AnimoSimulation.pdb
+-rw-rw-rw-   0        0        0   695336 2021-03-17 20:03:36.000000 animo_trainer-0.1.9/animo_trainer/lib/Newtonsoft.Json.dll
+-rw-rw-rw-   0        0        0   163464 2018-05-15 13:29:44.000000 animo_trainer-0.1.9/animo_trainer/lib/System.Numerics.Vectors.dll
+-rw-rw-rw-   0        0        0     3877 2023-03-23 22:18:54.000000 animo_trainer-0.1.9/animo_trainer/main.py
+-rw-rw-rw-   0        0        0      941 2023-03-17 21:48:34.000000 animo_trainer-0.1.9/animo_trainer/typed_numpy.py
+-rw-rw-rw-   0        0        0       21 2023-03-23 16:28:10.000000 animo_trainer-0.1.9/animo_trainer/version.py
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.267627 animo_trainer-0.1.9/animo_trainer.egg-info/
+-rw-rw-rw-   0        0        0      772 2023-03-23 22:25:21.000000 animo_trainer-0.1.9/animo_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4246 2023-03-23 22:25:21.000000 animo_trainer-0.1.9/animo_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-23 22:25:21.000000 animo_trainer-0.1.9/animo_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-03-23 22:25:21.000000 animo_trainer-0.1.9/animo_trainer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-03-23 22:25:21.000000 animo_trainer-0.1.9/animo_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-03-23 22:25:21.000000 animo_trainer-0.1.9/animo_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-23 22:25:21.576696 animo_trainer-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      955 2023-03-22 01:40:08.000000 animo_trainer-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.304635 animo_trainer-0.1.9/tests/
+-rw-rw-rw-   0        0        0     2289 2023-03-17 18:40:23.000000 animo_trainer-0.1.9/tests/test_simulate.py
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.305635 animo_trainer-0.1.9/typings/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.311637 animo_trainer-0.1.9/typings/Internal/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.195610 animo_trainer-0.1.9/typings/Internal/Runtime/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.317638 animo_trainer-0.1.9/typings/Internal/Runtime/CompilerServices/
+-rw-rw-rw-   0        0        0    10883 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/Internal/Runtime/CompilerServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.324640 animo_trainer-0.1.9/typings/Internal/Runtime/InteropServices/
+-rw-rw-rw-   0        0        0     2615 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/Internal/Runtime/InteropServices/__init__.pyi
+-rw-rw-rw-   0        0        0      392 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/Internal/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.196610 animo_trainer-0.1.9/typings/Microsoft/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.196610 animo_trainer-0.1.9/typings/Microsoft/Win32/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.325639 animo_trainer-0.1.9/typings/Microsoft/Win32/SafeHandles/
+-rw-rw-rw-   0        0        0     1444 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/Microsoft/Win32/SafeHandles/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.326640 animo_trainer-0.1.9/typings/System/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.328640 animo_trainer-0.1.9/typings/System/Buffers/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.335642 animo_trainer-0.1.9/typings/System/Buffers/Binary/
+-rw-rw-rw-   0        0        0     8554 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Buffers/Binary/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.341642 animo_trainer-0.1.9/typings/System/Buffers/Text/
+-rw-rw-rw-   0        0        0     5939 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Buffers/Text/__init__.pyi
+-rw-rw-rw-   0        0        0     8522 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Buffers/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.198611 animo_trainer-0.1.9/typings/System/CodeDom/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.347645 animo_trainer-0.1.9/typings/System/CodeDom/Compiler/
+-rw-rw-rw-   0        0        0     5807 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/CodeDom/Compiler/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.349645 animo_trainer-0.1.9/typings/System/Collections/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.354645 animo_trainer-0.1.9/typings/System/Collections/Concurrent/
+-rw-rw-rw-   0        0        0     2896 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Collections/Concurrent/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.356646 animo_trainer-0.1.9/typings/System/Collections/Generic/
+-rw-rw-rw-   0        0        0    62665 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Collections/Generic/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.357646 animo_trainer-0.1.9/typings/System/Collections/ObjectModel/
+-rw-rw-rw-   0        0        0     2798 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Collections/ObjectModel/__init__.pyi
+-rw-rw-rw-   0        0        0    14037 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Collections/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.363649 animo_trainer-0.1.9/typings/System/ComponentModel/
+-rw-rw-rw-   0        0        0     2389 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/ComponentModel/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.201612 animo_trainer-0.1.9/typings/System/Configuration/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.364648 animo_trainer-0.1.9/typings/System/Configuration/Assemblies/
+-rw-rw-rw-   0        0        0      981 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Configuration/Assemblies/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.371650 animo_trainer-0.1.9/typings/System/Diagnostics/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.378652 animo_trainer-0.1.9/typings/System/Diagnostics/CodeAnalysis/
+-rw-rw-rw-   0        0        0     7493 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Diagnostics/CodeAnalysis/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.379652 animo_trainer-0.1.9/typings/System/Diagnostics/Contracts/
+-rw-rw-rw-   0        0        0    10649 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Diagnostics/Contracts/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.385652 animo_trainer-0.1.9/typings/System/Diagnostics/SymbolStore/
+-rw-rw-rw-   0        0        0      298 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Diagnostics/SymbolStore/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.393655 animo_trainer-0.1.9/typings/System/Diagnostics/Tracing/
+-rw-rw-rw-   0        0        0    21263 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Diagnostics/Tracing/__init__.pyi
+-rw-rw-rw-   0        0        0    18735 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Diagnostics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.394655 animo_trainer-0.1.9/typings/System/Globalization/
+-rw-rw-rw-   0        0        0    68863 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Globalization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.395655 animo_trainer-0.1.9/typings/System/IO/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.402656 animo_trainer-0.1.9/typings/System/IO/Enumeration/
+-rw-rw-rw-   0        0        0     7685 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/IO/Enumeration/__init__.pyi
+-rw-rw-rw-   0        0        0   102670 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/IO/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.408659 animo_trainer-0.1.9/typings/System/Net/
+-rw-rw-rw-   0        0        0     1130 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Net/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.410659 animo_trainer-0.1.9/typings/System/Numerics/
+-rw-rw-rw-   0        0        0    74395 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Numerics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.411659 animo_trainer-0.1.9/typings/System/Reflection/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.422661 animo_trainer-0.1.9/typings/System/Reflection/Emit/
+-rw-rw-rw-   0        0        0    93675 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Reflection/Emit/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.428662 animo_trainer-0.1.9/typings/System/Reflection/Metadata/
+-rw-rw-rw-   0        0        0      837 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Reflection/Metadata/__init__.pyi
+-rw-rw-rw-   0        0        0   100095 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Reflection/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.435665 animo_trainer-0.1.9/typings/System/Resources/
+-rw-rw-rw-   0        0        0     7254 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Resources/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.442665 animo_trainer-0.1.9/typings/System/Runtime/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.443666 animo_trainer-0.1.9/typings/System/Runtime/CompilerServices/
+-rw-rw-rw-   0        0        0    74279 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Runtime/CompilerServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.445666 animo_trainer-0.1.9/typings/System/Runtime/ConstrainedExecution/
+-rw-rw-rw-   0        0        0     1312 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/ConstrainedExecution/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.451668 animo_trainer-0.1.9/typings/System/Runtime/ExceptionServices/
+-rw-rw-rw-   0        0        0     1054 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/ExceptionServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.452668 animo_trainer-0.1.9/typings/System/Runtime/InteropServices/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.453669 animo_trainer-0.1.9/typings/System/Runtime/InteropServices/ComTypes/
+-rw-rw-rw-   0        0        0    29019 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Runtime/InteropServices/ComTypes/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.460669 animo_trainer-0.1.9/typings/System/Runtime/InteropServices/ObjectiveC/
+-rw-rw-rw-   0        0        0     2322 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Runtime/InteropServices/ObjectiveC/__init__.pyi
+-rw-rw-rw-   0        0        0    89234 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Runtime/InteropServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.468671 animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.479675 animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/Arm/
+-rw-rw-rw-   0        0        0   376194 2023-03-21 21:41:37.000000 animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/Arm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.489676 animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/X86/
+-rw-rw-rw-   0        0        0   197416 2023-03-21 21:41:38.000000 animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/X86/__init__.pyi
+-rw-rw-rw-   0        0        0    53007 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.496677 animo_trainer-0.1.9/typings/System/Runtime/Loader/
+-rw-rw-rw-   0        0        0     2563 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/Loader/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.497678 animo_trainer-0.1.9/typings/System/Runtime/Remoting/
+-rw-rw-rw-   0        0        0      192 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/Remoting/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.498679 animo_trainer-0.1.9/typings/System/Runtime/Serialization/
+-rw-rw-rw-   0        0        0    10688 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/Serialization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.504680 animo_trainer-0.1.9/typings/System/Runtime/Versioning/
+-rw-rw-rw-   0        0        0     5655 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/Versioning/__init__.pyi
+-rw-rw-rw-   0        0        0     4296 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Runtime/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.506680 animo_trainer-0.1.9/typings/System/Security/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.511682 animo_trainer-0.1.9/typings/System/Security/Cryptography/
+-rw-rw-rw-   0        0        0     1211 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Security/Cryptography/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.513682 animo_trainer-0.1.9/typings/System/Security/Permissions/
+-rw-rw-rw-   0        0        0     5712 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Security/Permissions/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.514682 animo_trainer-0.1.9/typings/System/Security/Principal/
+-rw-rw-rw-   0        0        0     1308 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Security/Principal/__init__.pyi
+-rw-rw-rw-   0        0        0    12014 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Security/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.515683 animo_trainer-0.1.9/typings/System/Text/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.521685 animo_trainer-0.1.9/typings/System/Text/Unicode/
+-rw-rw-rw-   0        0        0      618 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Text/Unicode/__init__.pyi
+-rw-rw-rw-   0        0        0    60174 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Text/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.522684 animo_trainer-0.1.9/typings/System/Threading/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.524684 animo_trainer-0.1.9/typings/System/Threading/Tasks/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.525685 animo_trainer-0.1.9/typings/System/Threading/Tasks/Sources/
+-rw-rw-rw-   0        0        0     4015 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Threading/Tasks/Sources/__init__.pyi
+-rw-rw-rw-   0        0        0    86620 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Threading/Tasks/__init__.pyi
+-rw-rw-rw-   0        0        0    75007 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/Threading/__init__.pyi
+-rw-rw-rw-   0        0        0   875103 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/System/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.218615 animo_trainer-0.1.9/typings/TransformsAI/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.225617 animo_trainer-0.1.9/typings/TransformsAI/Animo/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.526686 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.532686 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Database/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.538687 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Database/Tables/
+-rw-rw-rw-   0        0        0     4883 2023-03-17 18:08:14.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Database/Tables/__init__.pyi
+-rw-rw-rw-   0        0        0     3274 2023-03-17 18:08:14.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Database/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.544690 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Models/
+-rw-rw-rw-   0        0        0     7158 2023-03-17 18:08:14.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Models/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.550691 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Utility/
+-rw-rw-rw-   0        0        0     1350 2023-03-17 18:08:14.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Utility/__init__.pyi
+-rw-rw-rw-   0        0        0     8174 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.551690 animo_trainer-0.1.9/typings/TransformsAI/Animo/Grid/
+-rw-rw-rw-   0        0        0    15552 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Grid/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.222616 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.552692 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Observations/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.553692 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Observations/Primitives/
+-rw-rw-rw-   0        0        0     3923 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Observations/Primitives/__init__.pyi
+-rw-rw-rw-   0        0        0     4928 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Observations/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.554691 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Rewards/
+-rw-rw-rw-   0        0        0    17004 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Rewards/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.555691 animo_trainer-0.1.9/typings/TransformsAI/Animo/Numerics/
+-rw-rw-rw-   0        0        0     7549 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Numerics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.556691 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.557692 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/Items/
+-rw-rw-rw-   0        0        0    71861 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/Items/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.564694 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/NPCs/
+-rw-rw-rw-   0        0        0    14026 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/NPCs/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.565694 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/Resolutions/
+-rw-rw-rw-   0        0        0     1936 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/Resolutions/__init__.pyi
+-rw-rw-rw-   0        0        0    15145 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.566694 animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.567694 animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/Events/
+-rw-rw-rw-   0        0        0     8314 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/Events/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.568694 animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/Intents/
+-rw-rw-rw-   0        0        0     2146 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/Intents/__init__.pyi
+-rw-rw-rw-   0        0        0      648 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-03-23 22:25:21.574697 animo_trainer-0.1.9/typings/TransformsAI/Animo/Tools/
+-rw-rw-rw-   0        0        0     5634 2023-03-21 21:41:35.000000 animo_trainer-0.1.9/typings/TransformsAI/Animo/Tools/__init__.pyi
+-rw-rw-rw-   0        0        0      146 2023-03-17 21:48:34.000000 animo_trainer-0.1.9/typings/clr.pyi
```

### Comparing `animo_trainer-0.1.8/PKG-INFO` & `animo_trainer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animo_trainer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Animo Trainer
 Home-page: https://transforms.ai/
 Author: Transitional Forms
 Author-email: dante@transforms.ai
 License: Copyright (c) 2023 Transitional Forms Inc. All Rights Reserved.
 Requires-Python: >=3.9,<3.10
 License-File: LICENSE.txt
```

### Comparing `animo_trainer-0.1.8/animo_trainer/animo_env.py` & `animo_trainer-0.1.9/animo_trainer/animo_env.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/animo_stats_writers.py` & `animo_trainer-0.1.9/animo_trainer/animo_stats_writers.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/animo_torch_model_saver.py` & `animo_trainer-0.1.9/animo_trainer/animo_torch_model_saver.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/animo_trainer_controller.py` & `animo_trainer-0.1.9/animo_trainer/animo_trainer_controller.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/animo_training_session.py` & `animo_trainer-0.1.9/animo_trainer/animo_training_session.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/AnimoData.deps.json` & `animo_trainer-0.1.9/animo_trainer/lib/AnimoData.deps.json`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/AnimoData.dll` & `animo_trainer-0.1.9/animo_trainer/lib/AnimoData.dll`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/AnimoData.pdb` & `animo_trainer-0.1.9/animo_trainer/lib/AnimoData.pdb`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/AnimoSimulation.deps.json` & `animo_trainer-0.1.9/animo_trainer/lib/AnimoSimulation.deps.json`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/AnimoSimulation.dll` & `animo_trainer-0.1.9/animo_trainer/lib/AnimoSimulation.dll`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/AnimoSimulation.pdb` & `animo_trainer-0.1.9/animo_trainer/lib/AnimoSimulation.pdb`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/Newtonsoft.Json.dll` & `animo_trainer-0.1.9/animo_trainer/lib/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/lib/System.Numerics.Vectors.dll` & `animo_trainer-0.1.9/animo_trainer/lib/System.Numerics.Vectors.dll`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer/typed_numpy.py` & `animo_trainer-0.1.9/animo_trainer/typed_numpy.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/animo_trainer.egg-info/PKG-INFO` & `animo_trainer-0.1.9/animo_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animo-trainer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Animo Trainer
 Home-page: https://transforms.ai/
 Author: Transitional Forms
 Author-email: dante@transforms.ai
 License: Copyright (c) 2023 Transitional Forms Inc. All Rights Reserved.
 Requires-Python: >=3.9,<3.10
 License-File: LICENSE.txt
```

### Comparing `animo_trainer-0.1.8/animo_trainer.egg-info/SOURCES.txt` & `animo_trainer-0.1.9/animo_trainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/setup.py` & `animo_trainer-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/tests/test_simulate.py` & `animo_trainer-0.1.9/tests/test_simulate.py`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/Internal/Runtime/CompilerServices/__init__.pyi` & `animo_trainer-0.1.9/typings/Internal/Runtime/CompilerServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/Internal/Runtime/InteropServices/__init__.pyi` & `animo_trainer-0.1.9/typings/Internal/Runtime/InteropServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/Microsoft/Win32/SafeHandles/__init__.pyi` & `animo_trainer-0.1.9/typings/Microsoft/Win32/SafeHandles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Buffers/Binary/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Buffers/Binary/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Buffers/Text/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Buffers/Text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Buffers/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Buffers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/CodeDom/Compiler/__init__.pyi` & `animo_trainer-0.1.9/typings/System/CodeDom/Compiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Collections/Concurrent/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Collections/Concurrent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Collections/Generic/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Collections/Generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Collections/ObjectModel/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Collections/ObjectModel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Collections/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Collections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/ComponentModel/__init__.pyi` & `animo_trainer-0.1.9/typings/System/ComponentModel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Configuration/Assemblies/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Configuration/Assemblies/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Diagnostics/CodeAnalysis/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Diagnostics/CodeAnalysis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Diagnostics/Contracts/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Diagnostics/Contracts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Diagnostics/Tracing/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Diagnostics/Tracing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Diagnostics/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Diagnostics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Globalization/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Globalization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/IO/Enumeration/__init__.pyi` & `animo_trainer-0.1.9/typings/System/IO/Enumeration/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/IO/__init__.pyi` & `animo_trainer-0.1.9/typings/System/IO/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Net/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Net/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Numerics/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Numerics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Reflection/Emit/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Reflection/Emit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Reflection/Metadata/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Reflection/Metadata/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Reflection/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Reflection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Resources/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Resources/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/CompilerServices/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/CompilerServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/ConstrainedExecution/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/ConstrainedExecution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/ExceptionServices/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/ExceptionServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/InteropServices/ComTypes/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/InteropServices/ComTypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/InteropServices/ObjectiveC/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/InteropServices/ObjectiveC/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/InteropServices/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/InteropServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/Arm/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/Arm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/X86/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/X86/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/Intrinsics/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/Intrinsics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/Loader/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/Loader/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/Serialization/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/Serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/Versioning/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/Versioning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Runtime/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Security/Cryptography/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Security/Cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Security/Permissions/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Security/Permissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Security/Principal/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Security/Principal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Security/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Text/Unicode/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Text/Unicode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Text/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Threading/Tasks/Sources/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Threading/Tasks/Sources/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Threading/Tasks/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Threading/Tasks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/Threading/__init__.pyi` & `animo_trainer-0.1.9/typings/System/Threading/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/System/__init__.pyi` & `animo_trainer-0.1.9/typings/System/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Database/Tables/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Database/Tables/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Database/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Database/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Models/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/Utility/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/Utility/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Data/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Grid/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Grid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Observations/Primitives/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Observations/Primitives/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Observations/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Observations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Learning/Rewards/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Learning/Rewards/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Numerics/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Numerics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/Items/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/Items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/NPCs/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/NPCs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/Resolutions/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/Resolutions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Objects/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Objects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/Events/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/Events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/Intents/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/Intents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Simulation/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Simulation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `animo_trainer-0.1.8/typings/TransformsAI/Animo/Tools/__init__.pyi` & `animo_trainer-0.1.9/typings/TransformsAI/Animo/Tools/__init__.pyi`

 * *Files identical despite different names*

