# Comparing `tmp/mocker-builder-0.1.4.tar.gz` & `tmp/mocker-builder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mocker-builder-0.1.4.tar", last modified: Thu Apr  6 11:02:33 2023, max compression
+gzip compressed data, was "dist/mocker-builder-0.1.5.tar", last modified: Mon May  8 19:15:37 2023, max compression
```

## Comparing `mocker-builder-0.1.4.tar` & `mocker-builder-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/PKG-INFO
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    21572 2023-03-30 13:19:39.000000 mocker-builder-0.1.4/README.md
-drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder/
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       77 2022-10-09 14:25:42.000000 mocker-builder-0.1.4/mocker_builder/__init__.py
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    30157 2023-04-06 10:57:12.000000 mocker-builder-0.1.4/mocker_builder/mocker_builder.py
-drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder.egg-info/
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder.egg-info/PKG-INFO
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)      267 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)        1 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       45 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder.egg-info/requires.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       15 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/mocker_builder.egg-info/top_level.txt
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       38 2023-04-06 11:02:33.000000 mocker-builder-0.1.4/setup.cfg
--rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)     1704 2023-03-24 10:06:37.000000 mocker-builder-0.1.4/setup.py
+drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/PKG-INFO
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    21572 2023-03-30 13:19:39.000000 mocker-builder-0.1.5/README.md
+drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder/
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       77 2022-10-09 14:25:42.000000 mocker-builder-0.1.5/mocker_builder/__init__.py
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    30235 2023-05-08 19:05:16.000000 mocker-builder-0.1.5/mocker_builder/mocker_builder.py
+drwxrwxr-x   0 tiago.cunha  (1001) tiago.cunha  (1001)        0 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)    27218 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)      267 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)        1 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       45 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/requires.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       15 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/mocker_builder.egg-info/top_level.txt
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)       38 2023-05-08 19:15:37.000000 mocker-builder-0.1.5/setup.cfg
+-rw-rw-r--   0 tiago.cunha  (1001) tiago.cunha  (1001)     1704 2023-03-24 10:06:37.000000 mocker-builder-0.1.5/setup.py
```

### Comparing `mocker-builder-0.1.4/PKG-INFO` & `mocker-builder-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-builder
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library to build mock tests dynamicaly using the mocker feature from pytest-mock lib
 Home-page: https://github.com/tgc77/mocker_builder
 Author: Tiago G Cunha
 Author-email: tikx.batera@gmail.com
 License: MIT
 Project-URL: Documentation, https://mocker-builder.readthedocs.io
 Project-URL: Source, https://github.com/tgc77/mocker_builder
```

### Comparing `mocker-builder-0.1.4/README.md` & `mocker-builder-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mocker-builder-0.1.4/mocker_builder/mocker_builder.py` & `mocker-builder-0.1.5/mocker_builder/mocker_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 NewCallableType = TypeVar('NewCallableType', bound=Optional[Callable])
 ReturnValueType = TypeVar('ReturnValueType', bound=Optional[Any])
 SideEffectType = TypeVar('SideEffectType', bound=Optional[Union[Callable, List]])
 MockMetadataKwargsType = TypeVar('MockMetadataKwargsType', bound=Dict[str, Any])
 FixtureType = TypeVar('FixtureType', bound=Callable[..., object])
 _Patch = TypeVar('_Patch', bound=_PatchType)
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 
 class MockerBuilderWarning:
     """Base class for all warnings emitted by mocker-builder"""
 
     @staticmethod
     def warn(message: str):
@@ -287,18 +287,19 @@
         self,
         mock_metadata_kwargs: MockMetadataKwargsType
     ):
         kwargs = {}
         for attr in self._mock_keys_validate:
             value = mock_metadata_kwargs.get(attr)
             if value:
-                if isinstance(value, dict):
-                    for key, data in value.items():
-                        kwargs.update({key: data})
-                    continue
+                if attr in ['mock_configure', 'mock_kwargs']:
+                    if isinstance(value, dict):
+                        for key, data in value.items():
+                            kwargs.update({key: data})
+                        continue
                 kwargs.update({attr: value})
         self._mock_metadata.patch_kwargs = kwargs
 
     def __apply_bypass_methods_return_value(self):
         if self._mock_metadata.target_path.rsplit('.', 1)[-1] in self._bypass_methods:
             self._mock_metadata.return_value = None
```

### Comparing `mocker-builder-0.1.4/mocker_builder.egg-info/PKG-INFO` & `mocker-builder-0.1.5/mocker_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-builder
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library to build mock tests dynamicaly using the mocker feature from pytest-mock lib
 Home-page: https://github.com/tgc77/mocker_builder
 Author: Tiago G Cunha
 Author-email: tikx.batera@gmail.com
 License: MIT
 Project-URL: Documentation, https://mocker-builder.readthedocs.io
 Project-URL: Source, https://github.com/tgc77/mocker_builder
```

### Comparing `mocker-builder-0.1.4/setup.py` & `mocker-builder-0.1.5/setup.py`

 * *Files identical despite different names*

