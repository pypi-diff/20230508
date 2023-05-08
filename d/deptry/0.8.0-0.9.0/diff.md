# Comparing `tmp/deptry-0.8.0.tar.gz` & `tmp/deptry-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deptry-0.8.0.tar", max compression
+gzip compressed data, was "deptry-0.9.0.tar", max compression
```

## Comparing `deptry-0.8.0.tar` & `deptry-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1070 2023-01-24 08:45:48.048752 deptry-0.8.0/LICENSE
--rw-r--r--   0        0        0     2802 2023-01-24 08:45:48.048752 deptry-0.8.0/README.md
--rw-r--r--   0        0        0       73 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/__init__.py
--rw-r--r--   0        0        0     8182 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/cli.py
--rw-r--r--   0        0        0      293 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/compat.py
--rw-r--r--   0        0        0     1295 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/config.py
--rw-r--r--   0        0        0     5997 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/core.py
--rw-r--r--   0        0        0     4210 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency.py
--rw-r--r--   0        0        0        0 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_getter/__init__.py
--rw-r--r--   0        0        0      890 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_getter/base.py
--rw-r--r--   0        0        0     1741 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_getter/pdm.py
--rw-r--r--   0        0        0     2219 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_getter/pep_621.py
--rw-r--r--   0        0        0     2739 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_getter/poetry.py
--rw-r--r--   0        0        0     4714 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_getter/requirements_txt.py
--rw-r--r--   0        0        0     4263 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/dependency_specification_detector.py
--rw-r--r--   0        0        0        0 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/imports/__init__.py
--rw-r--r--   0        0        0     1074 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/imports/extract.py
--rw-r--r--   0        0        0      247 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/imports/extractors/__init__.py
--rw-r--r--   0        0        0      951 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/imports/extractors/base.py
--rw-r--r--   0        0        0     2004 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/imports/extractors/notebook_import_extractor.py
--rw-r--r--   0        0        0      888 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/imports/extractors/python_import_extractor.py
--rw-r--r--   0        0        0        0 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/issues_finder/__init__.py
--rw-r--r--   0        0        0      513 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/issues_finder/base.py
--rw-r--r--   0        0        0     2754 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/issues_finder/misplaced_dev.py
--rw-r--r--   0        0        0     1234 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/issues_finder/missing.py
--rw-r--r--   0        0        0     2298 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/issues_finder/obsolete.py
--rw-r--r--   0        0        0     1658 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/issues_finder/transitive.py
--rw-r--r--   0        0        0      481 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/json_writer.py
--rw-r--r--   0        0        0     4970 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/module.py
--rw-r--r--   0        0        0     2837 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/python_file_finder.py
--rw-r--r--   0        0        0     4438 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/result_logger.py
--rw-r--r--   0        0        0    15159 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/stdlibs.py
--rw-r--r--   0        0        0      491 2023-01-24 08:45:48.048752 deptry-0.8.0/deptry/utils.py
--rw-r--r--   0        0        0     3065 2023-01-24 08:46:24.692810 deptry-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4036 1970-01-01 00:00:00.000000 deptry-0.8.0/setup.py
--rw-r--r--   0        0        0     4263 1970-01-01 00:00:00.000000 deptry-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-06 10:24:39.581788 deptry-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2802 2023-05-06 10:24:39.581788 deptry-0.9.0/README.md
+-rw-r--r--   0        0        0      109 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/__init__.py
+-rw-r--r--   0        0        0    10935 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/cli.py
+-rw-r--r--   0        0        0     1337 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/config.py
+-rw-r--r--   0        0        0     6864 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/core.py
+-rw-r--r--   0        0        0     4815 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_getter/__init__.py
+-rw-r--r--   0        0        0     1249 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_getter/base.py
+-rw-r--r--   0        0        0     1827 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_getter/pdm.py
+-rw-r--r--   0        0        0     3502 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_getter/pep_621.py
+-rw-r--r--   0        0        0     3248 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_getter/poetry.py
+-rw-r--r--   0        0        0     4846 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_getter/requirements_txt.py
+-rw-r--r--   0        0        0     4221 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/dependency_specification_detector.py
+-rw-r--r--   0        0        0     1042 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/imports/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/imports/extract.py
+-rw-r--r--   0        0        0      283 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/imports/extractors/__init__.py
+-rw-r--r--   0        0        0     1382 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/imports/extractors/base.py
+-rw-r--r--   0        0        0     2154 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/imports/extractors/notebook_import_extractor.py
+-rw-r--r--   0        0        0      977 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/imports/extractors/python_import_extractor.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/issues_finder/__init__.py
+-rw-r--r--   0        0        0      572 2023-05-06 10:24:39.581788 deptry-0.9.0/deptry/issues_finder/base.py
+-rw-r--r--   0        0        0     2810 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/issues_finder/misplaced_dev.py
+-rw-r--r--   0        0        0     1290 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/issues_finder/missing.py
+-rw-r--r--   0        0        0     2354 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/issues_finder/obsolete.py
+-rw-r--r--   0        0        0     1696 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/issues_finder/transitive.py
+-rw-r--r--   0        0        0      481 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/json_writer.py
+-rw-r--r--   0        0        0     4995 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/module.py
+-rw-r--r--   0        0        0     2843 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/python_file_finder.py
+-rw-r--r--   0        0        0     4438 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/result_logger.py
+-rw-r--r--   0        0        0    10238 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/stdlibs.py
+-rw-r--r--   0        0        0      570 2023-05-06 10:24:39.585789 deptry-0.9.0/deptry/utils.py
+-rw-r--r--   0        0        0     3636 2023-05-06 10:25:11.538210 deptry-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 deptry-0.9.0/PKG-INFO
```

### Comparing `deptry-0.8.0/LICENSE` & `deptry-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deptry-0.8.0/README.md` & `deptry-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deptry-0.8.0/deptry/cli.py` & `deptry-0.9.0/deptry/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 from __future__ import annotations
 
 import logging
+from collections import defaultdict
+from importlib.metadata import version
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import click
 
-from deptry.compat import metadata
 from deptry.config import read_configuration_from_pyproject_toml
 from deptry.core import Core
 
+if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+
 DEFAULT_EXCLUDE = ("venv", r"\.venv", r"\.direnv", "tests", r"\.git", r"setup\.py")
 
 
 class CommaSeparatedTupleParamType(click.ParamType):
+    """
+    This class is used to uniformly handle configuration parameters that can be either passed as a comma-separated string,
+    as a list of strings, or as a tuple of strings. For example, the value for a parameter can be a comma-separated string
+    when passed as a command line argument, or as a list of strings when passed through pyproject.toml.
+    """
+
     name = "tuple"
 
     def convert(
         self,
         value: str | list[str] | tuple[str, ...],
         param: click.Parameter | None,
         ctx: click.Context | None,
@@ -27,24 +38,66 @@
             return tuple(value)
         return value
 
 
 COMMA_SEPARATED_TUPLE = CommaSeparatedTupleParamType()
 
 
+class CommaSeparatedMappingParamType(click.ParamType):
+    """
+    This class is used to uniformly handle configuration parameters that can be either passed as a comma-separated pair
+    string, or as a Mapping of strings to tuples of strings. Items in a pair string are separated by an equal sign,
+    where multiple values are separated by a pipe: key1=value1,key2=value2|value3.
+    For example, the value for a parameter can be a comma-separated pair string when passed as a command line argument,
+    or as a mapping of string to tuples of strings when passed through pyproject.toml.
+    """
+
+    name = "mapping"
+
+    def convert(
+        self,
+        # In the mapping value below, although a str is a Sequence[str] itself,
+        # they are treated differently from other sequences of str.
+        value: str | Mapping[str, Sequence[str] | str],
+        param: click.Parameter | None,
+        ctx: click.Context | None,
+    ) -> dict[str, tuple[str, ...]]:
+        converted: dict[str, tuple[str, ...]]
+        if isinstance(value, str):
+            map_: defaultdict[str, list[str]] = defaultdict(list)
+            for item in value.split(","):
+                pair = tuple(item.split("=", 1))
+                if len(pair) != 2:
+                    error_msg = (
+                        f"package name and module names pairs should be concatenated with an equal sign (=): {item}"
+                    )
+                    raise ValueError(error_msg)
+                package_name = pair[0]
+                module_names = pair[1].split("|")
+                map_[package_name].extend(module_names)
+            converted = {k: tuple(v) for k, v in map_.items()}
+        else:
+            converted = {k: (v,) if isinstance(v, str) else tuple(v) for k, v in value.items()}
+
+        return converted
+
+
+COMMA_SEPARATED_MAPPING = CommaSeparatedMappingParamType()
+
+
 def configure_logger(_ctx: click.Context, _param: click.Parameter, value: bool) -> None:
     log_level = logging.DEBUG if value else logging.INFO
     logging.basicConfig(level=log_level, handlers=[logging.StreamHandler()], format="%(message)s")
 
 
 def display_deptry_version(ctx: click.Context, _param: click.Parameter, value: bool) -> None:
     if not value or ctx.resilient_parsing:
         return None
 
-    click.echo(f'deptry {metadata.version("deptry")}')  # type: ignore[no-untyped-call]
+    click.echo(f'deptry {version("deptry")}')
     ctx.exit()
 
 
 @click.command()
 @click.argument("root", type=click.Path(exists=True, path_type=Path))
 @click.option(
     "--verbose",
@@ -191,14 +244,22 @@
 @click.option(
     "--json-output",
     "-o",
     type=str,
     help="""If specified, a summary of the dependency issues found will be written to the output location specified. e.g. `deptry . -o deptry.json`""",
     show_default=True,
 )
+@click.option(
+    "--package-module-name-map",
+    "-pmnm",
+    type=COMMA_SEPARATED_MAPPING,
+    help="""Manually defined module names belonging to packages. For example; `deptry . --package-module-name-map package_1=module_a,package_2=module_b|module_c`.""",
+    default={},
+    show_default=False,
+)
 def deptry(
     root: Path,
     config: Path,
     ignore_obsolete: tuple[str, ...],
     ignore_missing: tuple[str, ...],
     ignore_transitive: tuple[str, ...],
     ignore_misplaced_dev: tuple[str, ...],
@@ -209,14 +270,15 @@
     exclude: tuple[str, ...],
     extend_exclude: tuple[str, ...],
     ignore_notebooks: bool,
     requirements_txt: tuple[str, ...],
     requirements_txt_dev: tuple[str, ...],
     known_first_party: tuple[str, ...],
     json_output: str,
+    package_module_name_map: Mapping[str, Sequence[str]],
 ) -> None:
     """Find dependency issues in your Python project.
 
     [ROOT] is the path to the root directory of the project to be scanned.
     All other arguments should be specified relative to [ROOT].
 
     """
@@ -236,8 +298,9 @@
         skip_missing=skip_missing,
         skip_transitive=skip_transitive,
         skip_misplaced_dev=skip_misplaced_dev,
         requirements_txt=requirements_txt,
         requirements_txt_dev=requirements_txt_dev,
         known_first_party=known_first_party,
         json_output=json_output,
+        package_module_name_map=package_module_name_map,
     ).run()
```

### Comparing `deptry-0.8.0/deptry/config.py` & `deptry-0.9.0/deptry/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import logging
-from pathlib import Path
-from typing import Any
-
-import click
+from typing import TYPE_CHECKING, Any
 
 from deptry.utils import load_pyproject_toml
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    import click
+
 
 def read_configuration_from_pyproject_toml(ctx: click.Context, _param: click.Parameter, value: Path) -> Path | None:
     """
     Callback that, given a click context, overrides the default values with configuration options set in a
     pyproject.toml file.
     Using a callback ensures that the following order is respected for setting an option:
     1. Default value is set
```

### Comparing `deptry-0.8.0/deptry/core.py` & `deptry-0.9.0/deptry/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from __future__ import annotations
 
 import logging
-import os
 import sys
 from dataclasses import dataclass
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from deptry.dependency import Dependency
-from deptry.dependency_getter.base import DependenciesExtract
 from deptry.dependency_getter.pdm import PDMDependencyGetter
 from deptry.dependency_getter.pep_621 import PEP621DependencyGetter
 from deptry.dependency_getter.poetry import PoetryDependencyGetter
 from deptry.dependency_getter.requirements_txt import RequirementsTxtDependencyGetter
 from deptry.dependency_specification_detector import DependencyManagementFormat, DependencySpecificationDetector
+from deptry.exceptions import IncorrectDependencyFormatError, UnsupportedPythonVersionError
 from deptry.imports.extract import get_imported_modules_for_list_of_files
 from deptry.issues_finder.misplaced_dev import MisplacedDevDependenciesFinder
 from deptry.issues_finder.missing import MissingDependenciesFinder
 from deptry.issues_finder.obsolete import ObsoleteDependenciesFinder
 from deptry.issues_finder.transitive import TransitiveDependenciesFinder
 from deptry.json_writer import JsonWriter
-from deptry.module import Module, ModuleBuilder
+from deptry.module import ModuleBuilder
 from deptry.python_file_finder import PythonFileFinder
 from deptry.result_logger import ResultLogger
 from deptry.stdlibs import STDLIBS_PYTHON
 
+if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+    from pathlib import Path
+
+    from deptry.dependency import Dependency
+    from deptry.dependency_getter.base import DependenciesExtract
+    from deptry.module import Module
+
 
 @dataclass
 class Core:
     root: Path
     config: Path
     ignore_obsolete: tuple[str, ...]
     ignore_missing: tuple[str, ...]
@@ -41,14 +47,15 @@
     extend_exclude: tuple[str, ...]
     using_default_exclude: bool
     ignore_notebooks: bool
     requirements_txt: tuple[str, ...]
     requirements_txt_dev: tuple[str, ...]
     known_first_party: tuple[str, ...]
     json_output: str
+    package_module_name_map: Mapping[str, Sequence[str]]
 
     def run(self) -> None:
         self._log_config()
 
         dependency_management_format = DependencySpecificationDetector(
             self.config, requirements_txt=self.requirements_txt
         ).detect()
@@ -95,43 +102,54 @@
             result["misplaced_dev"] = MisplacedDevDependenciesFinder(
                 imported_modules, dependencies, self.ignore_misplaced_dev
             ).find()
         return result
 
     def _get_dependencies(self, dependency_management_format: DependencyManagementFormat) -> DependenciesExtract:
         if dependency_management_format is DependencyManagementFormat.POETRY:
-            return PoetryDependencyGetter(self.config).get()
+            return PoetryDependencyGetter(self.config, self.package_module_name_map).get()
         if dependency_management_format is DependencyManagementFormat.PDM:
-            return PDMDependencyGetter(self.config).get()
+            return PDMDependencyGetter(self.config, self.package_module_name_map).get()
         if dependency_management_format is DependencyManagementFormat.PEP_621:
-            return PEP621DependencyGetter(self.config).get()
+            return PEP621DependencyGetter(self.config, self.package_module_name_map).get()
         if dependency_management_format is DependencyManagementFormat.REQUIREMENTS_TXT:
-            return RequirementsTxtDependencyGetter(self.config, self.requirements_txt, self.requirements_txt_dev).get()
-        raise ValueError("Incorrect dependency manage format. Only poetry, pdm and requirements.txt are supported.")
+            return RequirementsTxtDependencyGetter(
+                self.config, self.package_module_name_map, self.requirements_txt, self.requirements_txt_dev
+            ).get()
+        raise IncorrectDependencyFormatError
 
     def _get_local_modules(self) -> set[str]:
-        directories = [f for f in os.scandir(self.root) if f.is_dir()]
-        guessed_local_modules = {
-            subdirectory.name for subdirectory in directories if "__init__.py" in os.listdir(subdirectory)
-        }
+        """
+        Get all local Python modules from the root directory and `known_first_party` list.
+        A module is considered a local Python module if it matches at least one of those conditions:
+        - it is a directory that contains at least one Python file
+        - it is a Python file that is not named `__init__.py` (since it is a special case)
+        - it is set in the `known_first_party` list
+        """
+        guessed_local_modules = {path.stem for path in self.root.iterdir() if self._is_local_module(path)}
 
         return guessed_local_modules | set(self.known_first_party)
 
     @staticmethod
+    def _is_local_module(path: Path) -> bool:
+        """Guess if a module is a local Python module."""
+        return bool(
+            (path.is_file() and path.name != "__init__.py" and path.suffix == ".py")
+            or (path.is_dir() and list(path.glob("*.py")))
+        )
+
+    @staticmethod
     def _get_stdlib_modules() -> frozenset[str]:
         if sys.version_info[:2] >= (3, 10):
             return sys.stdlib_module_names
 
         try:  # type: ignore[unreachable]
             return STDLIBS_PYTHON[f"{sys.version_info[0]}{sys.version_info[1]}"]
         except KeyError as e:
-            raise ValueError(
-                f"Python version {sys.version_info[0]}.{sys.version_info[1]} is not supported. Only versions >= 3.7 are"
-                " supported."
-            ) from e
+            raise UnsupportedPythonVersionError((sys.version_info[0], sys.version_info[1])) from e
 
     def _log_config(self) -> None:
         logging.debug("Running with the following configuration:")
         for key, value in vars(self).items():
             logging.debug(f"{key}: {value}")
         logging.debug("")
```

### Comparing `deptry-0.8.0/deptry/dependency.py` & `deptry-0.9.0/deptry/dependency.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 from __future__ import annotations
 
 import logging
 import re
-
-from deptry.compat import PackageNotFoundError, metadata
+from contextlib import suppress
+from importlib import metadata
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+    from importlib.metadata import Distribution
 
 
 class Dependency:
     """
     A project's dependency with its associated top-level module names. There are stored in the metadata's top_level.txt.
     An example of this is 'matplotlib' with top-levels: ['matplotlib', 'mpl_toolkits', 'pylab'].
 
     By default, we also add the dependency's name with '-' replaced by '_' to the top-level modules.
     """
 
-    def __init__(self, name: str, conditional: bool = False, optional: bool = False) -> None:
+    def __init__(
+        self, name: str, conditional: bool = False, optional: bool = False, module_names: Sequence[str] | None = None
+    ) -> None:
         """
         Args:
             name: Name of the dependency, as shown in pyproject.toml
             conditional: boolean to indicate if the dependency is conditional, e.g. 'importlib-metadata': {'version': '*', 'python': '<=3.7'}
         """
+        distribution = self.find_distribution(name)
+
         self.name = name
         self.is_conditional = conditional
         self.is_optional = optional
-        self.found = self.find_metadata(name)
-        self.top_levels = self._get_top_levels(name)
-
-    def _get_top_levels(self, name: str) -> set[str]:
-        top_levels = []
+        self.found = distribution is not None
+        self.top_levels = self._get_top_levels(name, distribution, module_names)
 
-        if self.found:
-            top_levels += self._get_top_level_module_names_from_top_level_txt()
-            if not top_levels:
-                top_levels += self._get_top_level_module_names_from_record_file()
-
-        top_levels.append(name.replace("-", "_").lower())
-        return set(top_levels)
+    def _get_top_levels(
+        self, name: str, distribution: Distribution | None, module_names: Sequence[str] | None
+    ) -> set[str]:
+        if module_names is not None:
+            return set(module_names)
+
+        if distribution is not None:
+            with suppress(FileNotFoundError):
+                return self._get_top_level_module_names_from_top_level_txt(distribution)
+
+            with suppress(FileNotFoundError):
+                return self._get_top_level_module_names_from_record_file(distribution)
+
+        # No metadata or other configuration has been found. As a fallback
+        # we'll guess the name.
+        module_name = name.replace("-", "_").lower()
+        logging.warning(
+            f"Assuming the corresponding module name of package {self.name!r} is {module_name!r}. Install the package"
+            " or configure a package_module_name_map entry to override this behaviour."
+        )
+        return {module_name}
 
     def __repr__(self) -> str:
         return f"Dependency '{self.name}'"
 
     def __str__(self) -> str:
         return f"Dependency '{self.name}'{self._string_for_printing()}with top-levels: {self.top_levels}."
 
-    def find_metadata(self, name: str) -> bool:
+    @staticmethod
+    def find_distribution(name: str) -> Distribution | None:
         try:
-            metadata.distribution(name)  # type: ignore[no-untyped-call]
-        except PackageNotFoundError:
-            logging.warning(
-                f"Warning: Package '{name}'{self._string_for_printing()}not found in current environment. Assuming its"
-                f" corresponding module name is '{name.replace('-','_').lower()}'."
-            )
-            return False
-        else:
-            return True
+            return metadata.distribution(name)
+        except metadata.PackageNotFoundError:
+            return None
 
     def _string_for_printing(self) -> str:
         """
         Return 'Conditional', 'Optional' or 'Conditional and optional'
         """
         output_list = []
         if self.is_optional:
@@ -66,53 +81,52 @@
             output_list.append("conditional")
 
         if len(output_list) > 0:
             return f" ({', '.join(output_list)}) "
         else:
             return " "
 
-    def _get_top_level_module_names_from_top_level_txt(self) -> list[str]:
+    @staticmethod
+    def _get_top_level_module_names_from_top_level_txt(distribution: Distribution) -> set[str]:
         """
         top-level.txt is a metadata file added by setuptools that looks as follows:
 
         610faff656c4cfcbb4a3__mypyc
         _black_version
         black
         blackd
         blib2to3
 
         This function extracts these names, if a top-level.txt file exists.
         """
-        metadata_top_levels = metadata.distribution(self.name).read_text("top_level.txt")  # type: ignore[no-untyped-call]
-        if metadata_top_levels:
-            return [x for x in metadata_top_levels.split("\n") if len(x) > 0]
-        else:
-            return []
+        metadata_top_levels = distribution.read_text("top_level.txt")
+        if metadata_top_levels is None:
+            raise FileNotFoundError("top_level.txt")
+
+        return {x for x in metadata_top_levels.splitlines() if x}
 
-    def _get_top_level_module_names_from_record_file(self) -> list[str]:
+    @staticmethod
+    def _get_top_level_module_names_from_record_file(distribution: Distribution) -> set[str]:
         """
         Get the top-level module names from the RECORD file, whose contents usually look as follows:
 
             ...
+            ../../../bin/black,sha256=<HASH>,247
+            __pycache__/_black_version.cpython-311.pyc,,
+            _black_version.py,sha256=<HASH>,19
             black/trans.cpython-39-darwin.so,sha256=<HASH>
             black/trans.py,sha256=<HASH>
             blackd/__init__.py,sha256=<HASH>
             blackd/__main__.py,sha256=<HASH>
             ...
 
-        So if no file top-level.txt is provided, we can try and extract top-levels from this file, in this case black and blackd.
+        So if no file top-level.txt is provided, we can try and extract top-levels from this file, in
+        this case _black_version, black, and blackd.
         """
-        top_levels = []
-        try:
-            metadata_records = metadata.distribution(self.name).read_text("RECORD")  # type: ignore[no-untyped-call]
+        metadata_records = distribution.read_text("RECORD")
+
+        if metadata_records is None:
+            raise FileNotFoundError("RECORD")
 
-            if not metadata_records:
-                return []
-        except Exception:
-            return []
-
-        for line in metadata_records.split("\n"):
-            match = re.match("([a-zA-Z0-9-_]+)/", line)
-            if match:
-                top_levels.append(match.group(1))
+        matches = re.finditer(r"^(?!__)([a-zA-Z0-9-_]+)(?:/|\.py,)", metadata_records, re.MULTILINE)
 
-        return list(set(top_levels))
+        return {x.group(1) for x in matches}
```

### Comparing `deptry-0.8.0/deptry/dependency_getter/base.py` & `deptry-0.9.0/deptry/dependency_getter/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from pathlib import Path
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
-from deptry.dependency import Dependency
+if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+    from pathlib import Path
+
+    from deptry.dependency import Dependency
 
 
 @dataclass
 class DependenciesExtract:
     dependencies: list[Dependency]
     dev_dependencies: list[Dependency]
 
 
 @dataclass
 class DependencyGetter(ABC):
-    """Base class for all dependency getter."""
+    """Base class for all classes that extract a list of project's dependencies from a file.
+
+    Args:
+        config: The path to a configuration file that contains the project's dependencies.
+    """
 
     config: Path
+    package_module_name_map: Mapping[str, Sequence[str]] = field(default_factory=dict)
 
     @abstractmethod
     def get(self) -> DependenciesExtract:
         """Get extracted dependencies and dev dependencies."""
         raise NotImplementedError()
 
     @staticmethod
```

### Comparing `deptry-0.8.0/deptry/dependency_getter/pdm.py` & `deptry-0.9.0/deptry/dependency_getter/pdm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
-from deptry.dependency import Dependency
 from deptry.dependency_getter.base import DependenciesExtract
 from deptry.dependency_getter.pep_621 import PEP621DependencyGetter
 from deptry.utils import load_pyproject_toml
 
+if TYPE_CHECKING:
+    from deptry.dependency import Dependency
+
 
 @dataclass
 class PDMDependencyGetter(PEP621DependencyGetter):
     """
     Class to get dependencies that are specified according to PEP 621 from a `pyproject.toml` file for a project that uses PDM for its dependency management.
     """
 
@@ -43,8 +46,8 @@
         try:
             dev_dependencies_dict: dict[str, str] = pyproject_data["tool"]["pdm"]["dev-dependencies"]
             for deps in dev_dependencies_dict.values():
                 dev_dependency_strings += deps
         except KeyError:
             logging.debug("No section [tool.pdm.dev-dependencies] found in pyproject.toml")
 
-        return self._extract_pep_508_dependencies(dev_dependency_strings)
+        return self._extract_pep_508_dependencies(dev_dependency_strings, self.package_module_name_map)
```

### Comparing `deptry-0.8.0/deptry/dependency_getter/pep_621.py` & `deptry-0.9.0/deptry/dependency_getter/poetry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,83 @@
 from __future__ import annotations
 
-import itertools
-import re
+import contextlib
 from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any
 
 from deptry.dependency import Dependency
 from deptry.dependency_getter.base import DependenciesExtract, DependencyGetter
 from deptry.utils import load_pyproject_toml
 
+if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+
 
 @dataclass
-class PEP621DependencyGetter(DependencyGetter):
+class PoetryDependencyGetter(DependencyGetter):
+    """Extract Poetry dependencies from pyproject.toml."""
+
     def get(self) -> DependenciesExtract:
-        dependencies = [*self._get_dependencies(), *itertools.chain(*self._get_optional_dependencies().values())]
+        dependencies = self._get_poetry_dependencies()
         self._log_dependencies(dependencies)
 
-        return DependenciesExtract(dependencies, [])
+        dev_dependencies = self._get_poetry_dev_dependencies()
+        self._log_dependencies(dev_dependencies, is_dev=True)
 
-    def _get_dependencies(self) -> list[Dependency]:
+        return DependenciesExtract(dependencies, dev_dependencies)
+
+    def _get_poetry_dependencies(self) -> list[Dependency]:
         pyproject_data = load_pyproject_toml(self.config)
-        dependency_strings: list[str] = pyproject_data["project"]["dependencies"]
-        return self._extract_pep_508_dependencies(dependency_strings)
+        dependencies: dict[str, Any] = pyproject_data["tool"]["poetry"]["dependencies"]
+        return self._get_dependencies(dependencies, self.package_module_name_map)
 
-    def _get_optional_dependencies(self) -> dict[str, list[Dependency]]:
+    def _get_poetry_dev_dependencies(self) -> list[Dependency]:
+        """
+        Poetry's development dependencies can be specified under either of the following:
+
+        [tool.poetry.dev-dependencies]
+        [tool.poetry.group.dev.dependencies]
+
+        or both.
+        """
+        dependencies: dict[str, str] = {}
         pyproject_data = load_pyproject_toml(self.config)
 
-        return {
-            group: self._extract_pep_508_dependencies(dependencies)
-            for group, dependencies in pyproject_data["project"].get("optional-dependencies", {}).items()
-        }
+        with contextlib.suppress(KeyError):
+            dependencies = {**pyproject_data["tool"]["poetry"]["dev-dependencies"], **dependencies}
 
-    @classmethod
-    def _extract_pep_508_dependencies(cls, dependencies: list[str]) -> list[Dependency]:
-        extracted_dependencies = []
+        with contextlib.suppress(KeyError):
+            dependencies = {**pyproject_data["tool"]["poetry"]["group"]["dev"]["dependencies"], **dependencies}
 
-        for spec in dependencies:
-            # An example of a spec is `"tomli>=1.1.0; python_version < \"3.11\""`
-            name = cls._find_dependency_name_in(spec)
-            if name:
-                extracted_dependencies.append(
-                    Dependency(name, conditional=cls._is_conditional(spec), optional=cls._is_optional(spec))
-                )
+        return self._get_dependencies(dependencies, self.package_module_name_map)
 
-        return extracted_dependencies
+    @classmethod
+    def _get_dependencies(
+        cls, poetry_dependencies: dict[str, Any], package_module_name_map: Mapping[str, Sequence[str]]
+    ) -> list[Dependency]:
+        dependencies = []
+        for dep, spec in poetry_dependencies.items():
+            # dep is the dependency name, spec is the version specification, e.g. "^0.2.2" or {"*", optional = true}
+            if dep != "python":
+                optional = cls._is_optional(spec)
+                conditional = cls._is_conditional(spec)
+                dependencies.append(
+                    Dependency(
+                        dep, conditional=conditional, optional=optional, module_names=package_module_name_map.get(dep)
+                    )
+                )
 
-    @staticmethod
-    def _is_optional(dependency_specification: str) -> bool:
-        return bool(re.findall(r"\[([a-zA-Z0-9-]+?)\]", dependency_specification))
+        return dependencies
 
     @staticmethod
-    def _is_conditional(dependency_specification: str) -> bool:
-        return ";" in dependency_specification
+    def _is_optional(spec: str | dict[str, Any]) -> bool:
+        """
+        If a dependency specification is of the shape `isodate = {version = "*", optional = true}`, mark it as optional.
+        """
+        return bool(isinstance(spec, dict) and spec.get("optional"))
 
     @staticmethod
-    def _find_dependency_name_in(spec: str) -> str | None:
-        match = re.search("[a-zA-Z0-9-_]+", spec)
-        if match:
-            return match.group(0)
-        return None
+    def _is_conditional(spec: str | dict[str, Any]) -> bool:
+        """
+        If a dependency specification is of the shape `tomli = { version = "^2.0.1", python = "<3.11" }`, mark it as conditional.
+        """
+        return isinstance(spec, dict) and "python" in spec and "version" in spec
```

### Comparing `deptry-0.8.0/deptry/dependency_getter/poetry.py` & `deptry-0.9.0/deptry/dependency_getter/pep_621.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,96 @@
 from __future__ import annotations
 
-import contextlib
+import itertools
+import re
 from dataclasses import dataclass
-from typing import Any
+from typing import TYPE_CHECKING
 
 from deptry.dependency import Dependency
 from deptry.dependency_getter.base import DependenciesExtract, DependencyGetter
 from deptry.utils import load_pyproject_toml
 
+if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+
 
 @dataclass
-class PoetryDependencyGetter(DependencyGetter):
-    """Extract Poetry dependencies from pyproject.toml."""
+class PEP621DependencyGetter(DependencyGetter):
+    """
+    Class to extract dependencies from a pyproject.toml file in which dependencies are specified according to PEP 621. For example:
+
+        [project]
+        ...
+        dependencies = [
+            "httpx",
+            "gidgethub[httpx]>4.0.0",
+            "django>2.1; os_name != 'nt'",
+            "django>2.0; os_name == 'nt'"
+        ]
+
+        [project.optional-dependencies]
+        test = [
+            "pytest < 5.0.0",
+            "pytest-cov[all]"
+        ]
+
+    Note that both dependencies and optional-dependencies are extracted as regular dependencies. Since PEP-621 does not specify
+    a recommended way to extract development dependencies, we do not attempt to extract any from the pyproject.toml file.
+    """
 
     def get(self) -> DependenciesExtract:
-        dependencies = self._get_poetry_dependencies()
+        dependencies = [*self._get_dependencies(), *itertools.chain(*self._get_optional_dependencies().values())]
         self._log_dependencies(dependencies)
 
-        dev_dependencies = self._get_poetry_dev_dependencies()
-        self._log_dependencies(dev_dependencies, is_dev=True)
-
-        return DependenciesExtract(dependencies, dev_dependencies)
+        return DependenciesExtract(dependencies, [])
 
-    def _get_poetry_dependencies(self) -> list[Dependency]:
+    def _get_dependencies(self) -> list[Dependency]:
         pyproject_data = load_pyproject_toml(self.config)
-        dependencies: dict[str, Any] = pyproject_data["tool"]["poetry"]["dependencies"]
-        return self._get_dependencies(dependencies)
-
-    def _get_poetry_dev_dependencies(self) -> list[Dependency]:
-        """
-        These can be either under;
-
-        [tool.poetry.dev-dependencies]
-        [tool.poetry.group.dev.dependencies]
+        dependency_strings: list[str] = pyproject_data["project"]["dependencies"]
+        return self._extract_pep_508_dependencies(dependency_strings, self.package_module_name_map)
 
-        or both.
-        """
-        dependencies: dict[str, str] = {}
+    def _get_optional_dependencies(self) -> dict[str, list[Dependency]]:
         pyproject_data = load_pyproject_toml(self.config)
 
-        with contextlib.suppress(KeyError):
-            dependencies = {**pyproject_data["tool"]["poetry"]["dev-dependencies"], **dependencies}
+        return {
+            group: self._extract_pep_508_dependencies(dependencies, self.package_module_name_map)
+            for group, dependencies in pyproject_data["project"].get("optional-dependencies", {}).items()
+        }
 
-        with contextlib.suppress(KeyError):
-            dependencies = {**pyproject_data["tool"]["poetry"]["group"]["dev"]["dependencies"], **dependencies}
+    @classmethod
+    def _extract_pep_508_dependencies(
+        cls, dependencies: list[str], package_module_name_map: Mapping[str, Sequence[str]]
+    ) -> list[Dependency]:
+        """
+        Given a list of dependency specifications (e.g. "django>2.1; os_name != 'nt'"), convert them to Dependency objects.
+        """
+        extracted_dependencies = []
 
-        return self._get_dependencies(dependencies)
+        for spec in dependencies:
+            # An example of a spec is `"tomli>=1.1.0; python_version < \"3.11\""`
+            name = cls._find_dependency_name_in(spec)
+            if name:
+                extracted_dependencies.append(
+                    Dependency(
+                        name,
+                        conditional=cls._is_conditional(spec),
+                        optional=cls._is_optional(spec),
+                        module_names=package_module_name_map.get(name),
+                    )
+                )
 
-    @classmethod
-    def _get_dependencies(cls, poetry_dependencies: dict[str, Any]) -> list[Dependency]:
-        dependencies = []
-        for dep, spec in poetry_dependencies.items():
-            # dep is the dependency name, spec is the version specification, e.g. "^0.2.2" or {"*", optional = true}
-            if dep != "python":
-                optional = cls._is_optional(spec)
-                conditional = cls._is_conditional(spec)
-                dependencies.append(Dependency(dep, conditional=conditional, optional=optional))
+        return extracted_dependencies
 
-        return dependencies
+    @staticmethod
+    def _is_optional(dependency_specification: str) -> bool:
+        return bool(re.findall(r"\[([a-zA-Z0-9-]+?)\]", dependency_specification))
 
     @staticmethod
-    def _is_optional(spec: str | dict[str, Any]) -> bool:
-        # if of the shape `isodate = {version = "*", optional = true}` mark as optional`
-        return bool(isinstance(spec, dict) and spec.get("optional"))
+    def _is_conditional(dependency_specification: str) -> bool:
+        return ";" in dependency_specification
 
     @staticmethod
-    def _is_conditional(spec: str | dict[str, Any]) -> bool:
-        # if of the shape `tomli = { version = "^2.0.1", python = "<3.11" }`, mark as conditional.
-        return isinstance(spec, dict) and "python" in spec and "version" in spec
+    def _find_dependency_name_in(spec: str) -> str | None:
+        match = re.search("[a-zA-Z0-9-_]+", spec)
+        if match:
+            return match.group(0)
+        return None
```

### Comparing `deptry-0.8.0/deptry/dependency_getter/requirements_txt.py` & `deptry-0.9.0/deptry/dependency_getter/requirements_txt.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,20 @@
         line = self._remove_comments_from(line)
         line = self._remove_newlines_from(line)
         name = self._find_dependency_name_in(line)
         if name:
             line = line.replace(name, "")
             optional = self._check_if_dependency_is_optional(line)
             conditional = self._check_if_dependency_is_conditional(line)
-            return Dependency(name=name, optional=optional, conditional=conditional)
+            return Dependency(
+                name=name,
+                optional=optional,
+                conditional=conditional,
+                module_names=self.package_module_name_map.get(name),
+            )
         else:
             return None
 
     def _find_dependency_name_in(self, line: str) -> str | None:
         """
         Find the dependency name of a dependency specified according to the pip-standards for requirement.txt
         """
```

### Comparing `deptry-0.8.0/deptry/dependency_specification_detector.py` & `deptry-0.9.0/deptry/dependency_specification_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
 import logging
 import os
 from enum import Enum
-from pathlib import Path
+from typing import TYPE_CHECKING
 
+from deptry.exceptions import DependencySpecificationNotFoundError
 from deptry.utils import load_pyproject_toml
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class DependencyManagementFormat(Enum):
     PDM = "pdm"
     PEP_621 = "pep_621"
     POETRY = "poetry"
     REQUIREMENTS_TXT = "requirements_txt"
 
@@ -35,18 +39,16 @@
             return DependencyManagementFormat.POETRY
         if pyproject_toml_found and self._project_uses_pdm():
             return DependencyManagementFormat.PDM
         if pyproject_toml_found and self._project_uses_pep_621():
             return DependencyManagementFormat.PEP_621
         if self._project_uses_requirements_txt():
             return DependencyManagementFormat.REQUIREMENTS_TXT
-        raise FileNotFoundError(
-            "No file called 'pyproject.toml' with a [tool.poetry.dependencies], [tool.pdm] or [project] section or"
-            f" file(s) called '{', '.join(self.requirements_txt)}' found. Exiting."
-        )
+
+        raise DependencySpecificationNotFoundError(self.requirements_txt)
 
     def _project_contains_pyproject_toml(self) -> bool:
         if self.config.exists():
             logging.debug("pyproject.toml found!")
             return True
         else:
             logging.debug("No pyproject.toml found.")
@@ -58,15 +60,15 @@
             pyproject_toml["tool"]["poetry"]["dependencies"]
             logging.debug(
                 "pyproject.toml contains a [tool.poetry.dependencies] section, so Poetry is used to specify the"
                 " project's dependencies."
             )
         except KeyError:
             logging.debug(
-                "pyproject.toml does not contain a [tool.poetry.dependencies] section, so PDM is not used to specify"
+                "pyproject.toml does not contain a [tool.poetry.dependencies] section, so Poetry is not used to specify"
                 " the project's dependencies."
             )
             return False
         else:
             return True
 
     def _project_uses_pdm(self) -> bool:
```

### Comparing `deptry-0.8.0/deptry/imports/extract.py` & `deptry-0.9.0/deptry/imports/extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
 import itertools
 import logging
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from deptry.imports.extractors import NotebookImportExtractor, PythonImportExtractor
-from deptry.imports.extractors.base import ImportExtractor
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from deptry.imports.extractors.base import ImportExtractor
 
 
 def get_imported_modules_for_list_of_files(list_of_files: list[Path]) -> list[str]:
     logging.info(f"Scanning {len(list_of_files)} files...")
 
     modules = sorted(set(itertools.chain.from_iterable(get_imported_modules_from_file(file) for file in list_of_files)))
```

### Comparing `deptry-0.8.0/deptry/imports/extractors/base.py` & `deptry-0.9.0/deptry/imports/extractors/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 from __future__ import annotations
 
 import ast
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import chardet
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @dataclass
 class ImportExtractor(ABC):
+    """
+    Base class for other classes that can be used to extract the imported modules from a file.
+    """
+
     file: Path
 
     @abstractmethod
     def extract_imports(self) -> set[str]:
         raise NotImplementedError()
 
     @staticmethod
     def _extract_imports_from_ast(tree: ast.AST) -> set[str]:
+        """
+        Given an Abstract Syntax Tree, find the imported top-level modules.
+        For example, given the source tree of a file with contents:
+
+            from pandas.tools import scatter_matrix
+
+        Will return the set {"pandas"}.
+        """
+
         imported_modules: set[str] = set()
 
         for node in ast.walk(tree):
             if isinstance(node, ast.Import):
                 imported_modules |= {module.name.split(".")[0] for module in node.names}
             elif isinstance(node, ast.ImportFrom) and node.module and node.level == 0:
                 imported_modules.add(node.module.split(".")[0])
```

### Comparing `deptry-0.8.0/deptry/imports/extractors/notebook_import_extractor.py` & `deptry-0.9.0/deptry/imports/extractors/notebook_import_extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 
 import ast
 import itertools
 import json
 import logging
 import re
 from dataclasses import dataclass
-from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from deptry.imports.extractors.base import ImportExtractor
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @dataclass
 class NotebookImportExtractor(ImportExtractor):
     """Extract import statements from a Jupyter notebook."""
 
     def extract_imports(self) -> set[str]:
+        """Extract the imported top-level modules from all code cells in the Jupyter Notebook."""
         notebook = self._read_ipynb_file(self.file)
         if not notebook:
             return set()
 
         cells = self._keep_code_cells(notebook)
         import_statements = [self._extract_import_statements_from_cell(cell) for cell in cells]
         tree = ast.parse("\n".join(itertools.chain.from_iterable(import_statements)), str(self.file))
         return self._extract_imports_from_ast(tree)
 
     @classmethod
     def _read_ipynb_file(cls, path_to_ipynb: Path) -> dict[str, Any] | None:
         try:
             with open(path_to_ipynb) as ipynb_file:
                 notebook: dict[str, Any] = json.load(ipynb_file)
-        except UnicodeDecodeError:
+        except (UnicodeDecodeError, ValueError):
             try:
                 with open(path_to_ipynb, encoding=cls._get_file_encoding(path_to_ipynb)) as ipynb_file:
                     notebook = json.load(ipynb_file, strict=False)
             except UnicodeDecodeError:
                 logging.warning(f"Warning: File {path_to_ipynb} could not be decoded. Skipping...")
                 return None
         return notebook
```

### Comparing `deptry-0.8.0/deptry/imports/extractors/python_import_extractor.py` & `deptry-0.9.0/deptry/imports/extractors/python_import_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 
 @dataclass
 class PythonImportExtractor(ImportExtractor):
     """Extract import statements from a Python module."""
 
     def extract_imports(self) -> set[str]:
+        """Extract all imported top-level modules from the Python file."""
         try:
             with open(self.file) as python_file:
                 tree = ast.parse(python_file.read(), str(self.file))
-        except UnicodeDecodeError:
+        except (UnicodeDecodeError, ValueError):
             try:
                 with open(self.file, encoding=self._get_file_encoding(self.file)) as python_file:
                     tree = ast.parse(python_file.read(), str(self.file))
             except UnicodeDecodeError:
                 logging.warning(f"Warning: File {self.file} could not be decoded. Skipping...")
                 return set()
```

### Comparing `deptry-0.8.0/deptry/issues_finder/base.py` & `deptry-0.9.0/deptry/issues_finder/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
-from deptry.dependency import Dependency
-from deptry.module import Module
+if TYPE_CHECKING:
+    from deptry.dependency import Dependency
+    from deptry.module import Module
 
 
 @dataclass
 class IssuesFinder(ABC):
     """Base class for all issues finders."""
 
     imported_modules: list[Module]
```

### Comparing `deptry-0.8.0/deptry/issues_finder/misplaced_dev.py` & `deptry-0.9.0/deptry/issues_finder/misplaced_dev.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 from deptry.issues_finder.base import IssuesFinder
-from deptry.module import Module
+
+if TYPE_CHECKING:
+    from deptry.module import Module
 
 
 @dataclass
 class MisplacedDevDependenciesFinder(IssuesFinder):
     """
     Given a list of imported modules and a list of project dependencies, determine which development dependencies
     should actually be regular dependencies.
```

### Comparing `deptry-0.8.0/deptry/issues_finder/missing.py` & `deptry-0.9.0/deptry/issues_finder/missing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 from deptry.issues_finder.base import IssuesFinder
-from deptry.module import Module
+
+if TYPE_CHECKING:
+    from deptry.module import Module
 
 
 @dataclass
 class MissingDependenciesFinder(IssuesFinder):
     """
     Given a list of imported modules and a list of project dependencies, determine which ones are missing.
     """
```

### Comparing `deptry-0.8.0/deptry/issues_finder/obsolete.py` & `deptry-0.9.0/deptry/issues_finder/obsolete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
-from deptry.dependency import Dependency
 from deptry.issues_finder.base import IssuesFinder
 
+if TYPE_CHECKING:
+    from deptry.dependency import Dependency
+
 
 @dataclass
 class ObsoleteDependenciesFinder(IssuesFinder):
     """
     Given a list of imported modules and a list of project dependencies, determine which ones are obsolete.
 
     This is done by checking for each dependency if there is any module of which the metadata field 'Name' is equal to the dependency.
```

### Comparing `deptry-0.8.0/deptry/issues_finder/transitive.py` & `deptry-0.9.0/deptry/issues_finder/transitive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
 from deptry.issues_finder.base import IssuesFinder
-from deptry.module import Module
+
+if TYPE_CHECKING:
+    from deptry.module import Module
 
 
 @dataclass
 class TransitiveDependenciesFinder(IssuesFinder):
     """
     Given a list of imported modules and a list of project dependencies, determine which ones are transitive.
     This is done by elimination; if a module uses an installed package but the package is;
```

### Comparing `deptry-0.8.0/deptry/module.py` & `deptry-0.9.0/deptry/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
+from importlib.metadata import PackageNotFoundError, metadata
+from typing import TYPE_CHECKING
 
-from deptry.compat import PackageNotFoundError, metadata
-from deptry.dependency import Dependency
+if TYPE_CHECKING:
+    from deptry.dependency import Dependency
 
 
 @dataclass
 class Module:
     name: str
     standard_library: bool = False
     local_module: bool = False
@@ -26,15 +28,15 @@
         logging.debug(self.__str__())
         logging.debug("")
 
     def __repr__(self) -> str:
         return f"Module '{self.name}'"
 
     def __str__(self) -> str:
-        return "\n".join("%s: %s" % item for item in vars(self).items())
+        return "\n".join("{}: {}".format(*item) for item in vars(self).items())
 
 
 class ModuleBuilder:
     def __init__(
         self,
         name: str,
         local_modules: set[str],
@@ -86,15 +88,15 @@
         )
 
     def _get_package_name_from_metadata(self) -> str | None:
         """
         Most packages simply have a field called "Name" in their metadata. This method extracts that field.
         """
         try:
-            name: str = metadata.metadata(self.name)["Name"]  # type: ignore[no-untyped-call]
+            name: str = metadata(self.name)["Name"]
         except PackageNotFoundError:
             return None
         else:
             return name
 
     def _get_corresponding_top_levels_from(self, dependencies: list[Dependency]) -> list[str]:
         """
```

### Comparing `deptry-0.8.0/deptry/python_file_finder.py` & `deptry-0.9.0/deptry/python_file_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return bool((self.exclude + self.extend_exclude) and ignore_regex.match(str(directory)))
 
     def _is_file_ignored(
         self, file: Path, file_lookup_suffixes: set[str], ignore_regex: Pattern[str], gitignore_spec: PathSpec | None
     ) -> bool:
         return bool(
             file.suffix not in file_lookup_suffixes
-            or ((self.exclude + self.extend_exclude) and ignore_regex.match(str(file)))
+            or ((self.exclude + self.extend_exclude) and ignore_regex.match(file.as_posix()))
             or (gitignore_spec and gitignore_spec.match_file(file))
         )
 
     def _generate_gitignore_pathspec(self, directory: Path) -> PathSpec | None:
         # If `exclude` is explicitly set, `.gitignore` is not taken into account.
         if not self.using_default_exclude:
             return None
```

### Comparing `deptry-0.8.0/deptry/result_logger.py` & `deptry-0.9.0/deptry/result_logger.py`

 * *Files identical despite different names*

### Comparing `deptry-0.8.0/deptry/stdlibs.py` & `deptry-0.9.0/deptry/stdlibs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,235 +1,16 @@
 """
 DO NOT EDIT THIS FILE MANUALLY.
 It is generated from `scripts/generate_stdlibs.py` script and contains the stdlib modules for Python versions that does
 not support https://docs.python.org/3/library/sys.html#sys.stdlib_module_names (< 3.10).
 The file can be generated again using `python scripts/generate_stdlibs.py`.
 """
+from __future__ import annotations
+
 STDLIBS_PYTHON = {
-    "37": frozenset(
-        {
-            "__future__",
-            "_ast",
-            "_dummy_thread",
-            "_thread",
-            "abc",
-            "aifc",
-            "argparse",
-            "array",
-            "ast",
-            "asynchat",
-            "asyncio",
-            "asyncore",
-            "atexit",
-            "audioop",
-            "base64",
-            "bdb",
-            "binascii",
-            "binhex",
-            "bisect",
-            "builtins",
-            "bz2",
-            "cProfile",
-            "calendar",
-            "cgi",
-            "cgitb",
-            "chunk",
-            "cmath",
-            "cmd",
-            "code",
-            "codecs",
-            "codeop",
-            "collections",
-            "colorsys",
-            "compileall",
-            "concurrent",
-            "configparser",
-            "contextlib",
-            "contextvars",
-            "copy",
-            "copyreg",
-            "crypt",
-            "csv",
-            "ctypes",
-            "curses",
-            "dataclasses",
-            "datetime",
-            "dbm",
-            "decimal",
-            "difflib",
-            "dis",
-            "distutils",
-            "doctest",
-            "dummy_threading",
-            "email",
-            "encodings",
-            "ensurepip",
-            "enum",
-            "errno",
-            "faulthandler",
-            "fcntl",
-            "filecmp",
-            "fileinput",
-            "fnmatch",
-            "formatter",
-            "fractions",
-            "ftplib",
-            "functools",
-            "gc",
-            "getopt",
-            "getpass",
-            "gettext",
-            "glob",
-            "grp",
-            "gzip",
-            "hashlib",
-            "heapq",
-            "hmac",
-            "html",
-            "http",
-            "imaplib",
-            "imghdr",
-            "imp",
-            "importlib",
-            "inspect",
-            "io",
-            "ipaddress",
-            "itertools",
-            "json",
-            "keyword",
-            "lib2to3",
-            "linecache",
-            "locale",
-            "logging",
-            "lzma",
-            "macpath",
-            "mailbox",
-            "mailcap",
-            "marshal",
-            "math",
-            "mimetypes",
-            "mmap",
-            "modulefinder",
-            "msilib",
-            "msvcrt",
-            "multiprocessing",
-            "netrc",
-            "nis",
-            "nntplib",
-            "ntpath",
-            "numbers",
-            "operator",
-            "optparse",
-            "os",
-            "ossaudiodev",
-            "parser",
-            "pathlib",
-            "pdb",
-            "pickle",
-            "pickletools",
-            "pipes",
-            "pkgutil",
-            "platform",
-            "plistlib",
-            "poplib",
-            "posix",
-            "posixpath",
-            "pprint",
-            "profile",
-            "pstats",
-            "pty",
-            "pwd",
-            "py_compile",
-            "pyclbr",
-            "pydoc",
-            "queue",
-            "quopri",
-            "random",
-            "re",
-            "readline",
-            "reprlib",
-            "resource",
-            "rlcompleter",
-            "runpy",
-            "sched",
-            "secrets",
-            "select",
-            "selectors",
-            "shelve",
-            "shlex",
-            "shutil",
-            "signal",
-            "site",
-            "smtpd",
-            "smtplib",
-            "sndhdr",
-            "socket",
-            "socketserver",
-            "spwd",
-            "sqlite3",
-            "sre",
-            "sre_compile",
-            "sre_constants",
-            "sre_parse",
-            "ssl",
-            "stat",
-            "statistics",
-            "string",
-            "stringprep",
-            "struct",
-            "subprocess",
-            "sunau",
-            "symbol",
-            "symtable",
-            "sys",
-            "sysconfig",
-            "syslog",
-            "tabnanny",
-            "tarfile",
-            "telnetlib",
-            "tempfile",
-            "termios",
-            "test",
-            "textwrap",
-            "threading",
-            "time",
-            "timeit",
-            "tkinter",
-            "token",
-            "tokenize",
-            "trace",
-            "traceback",
-            "tracemalloc",
-            "tty",
-            "turtle",
-            "turtledemo",
-            "types",
-            "typing",
-            "unicodedata",
-            "unittest",
-            "urllib",
-            "uu",
-            "uuid",
-            "venv",
-            "warnings",
-            "wave",
-            "weakref",
-            "webbrowser",
-            "winreg",
-            "winsound",
-            "wsgiref",
-            "xdrlib",
-            "xml",
-            "xmlrpc",
-            "zipapp",
-            "zipfile",
-            "zipimport",
-            "zlib",
-        }
-    ),
     "38": frozenset(
         {
             "__future__",
             "_ast",
             "_dummy_thread",
             "_thread",
             "abc",
```

### Comparing `deptry-0.8.0/pyproject.toml` & `deptry-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deptry"
-version = "0.8.0"
+version = "0.9.0"
 description = "A command line utility to check for obsolete, missing and transitive dependencies in a Python project."
 authors = ["Florian Maas <fpgmaas@gmail.com>"]
 maintainers = ["Mathieu Kniewallner <mathieu.kniewallner@gmail.com>"]
 repository = "https://github.com/fpgmaas/deptry"
 documentation = "https://fpgmaas.github.io/deptry/"
 readme = "README.md"
 license = "MIT"
@@ -18,43 +18,62 @@
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 chardet = ">=4.0.0"
 click = "^8.0.0"
-importlib-metadata = { version = "*", python = "<=3.7" }
 pathspec = ">=0.9.0"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
-pre-commit = "^2.20.0"
-pytest = "^7.1.2"
-pytest-cov = "^4.0.0"
-types-chardet = "^5.0.4"
+mypy = "1.2.0"
+pre-commit = "3.3.1"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
+types-chardet = "5.0.4.5"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.0.0"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.9"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target-version = ["py37"]
+target-version = ["py38"]
 preview = true
 
 [tool.coverage.report]
 skip_empty = true
+# Subset of rules from https://pypi.org/project/covdefaults/
+exclude_lines = [
+    # a more strict default pragma
+    "# pragma: no cover\\b",
+
+    # allow defensive code
+    "^\\s*raise AssertionError\\b",
+    "^\\s*raise NotImplementedError\\b",
+    "^\\s*return NotImplemented\\b",
+    "^\\s*raise$",
+
+    # typing-related code
+    "^\\s*if (False|TYPE_CHECKING):",
+    ": \\.\\.\\.(\\s*#.*)?$",
+    "^ +\\.\\.\\.$",
+    "-> ['\"]?NoReturn['\"]?:",
+
+    # non-runnable code
+    "if __name__ == ['\"]__main__['\"]:$",
+]
 
 [tool.coverage.run]
 branch = true
 source = ["deptry"]
 
 [tool.mypy]
 files = ["deptry", "scripts", "tests"]
@@ -71,20 +90,17 @@
 pretty = true
 show_error_codes = true
 
 # Ignore warnings for unused ignores because of https://github.com/python/mypy/issues/8823.
 # In some Python versions, we can end up with backport modules being untyped, while they are typed on others.
 [[tool.mypy.overrides]]
 module = [
-    "deptry.cli",
     "deptry.core",
-    "deptry.dependency",
-    "deptry.module",
     "scripts.generate_stdlibs",
-    "tests.test_core",
+    "tests.unit.test_core",
 ]
 warn_unused_ignores = false
 
 [tool.deptry]
 extend_exclude = [
     "docs",
     "tests",
@@ -92,15 +108,15 @@
 ]
 ignore_missing = ["tomllib"]
 
 [tool.poetry.scripts]
 deptry = "deptry.cli:deptry"
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 fix = true
 select = [
     # flake8-2020
     "YTT",
     # flake8-bandit
     "S",
@@ -112,14 +128,16 @@
     "C4",
     # flake8-debugger
     "T10",
     # flake8-print
     "T20",
     # flake8-simplify
     "SIM",
+    # flake8-type-checking
+    "TCH",
     # isort
     "I",
     # mccabe
     "C90",
     # pycodestyle
     "E", "W",
     # pyflakes
@@ -137,9 +155,15 @@
     # LineTooLong
     "E501",
     # DoNotAssignLambda
     "E731",
 ]
 extend-exclude = ["tests/data/*"]
 
+[tool.ruff.flake8-type-checking]
+strict = true
+
+[tool.ruff.isort]
+required-imports = ["from __future__ import annotations"]
+
 [tool.ruff.per-file-ignores]
-"tests/*" = ["S101"]
+"tests/*" = ["S101", "S603"]
```

### Comparing `deptry-0.8.0/setup.py` & `deptry-0.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: deptry
+Version: 0.9.0
+Summary: A command line utility to check for obsolete, missing and transitive dependencies in a Python project.
+Home-page: https://github.com/fpgmaas/deptry
+License: MIT
+Keywords: dependency,poetry
+Author: Florian Maas
+Author-email: fpgmaas@gmail.com
+Maintainer: Mathieu Kniewallner
+Maintainer-email: mathieu.kniewallner@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: chardet (>=4.0.0)
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: pathspec (>=0.9.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Project-URL: Documentation, https://fpgmaas.github.io/deptry/
+Project-URL: Repository, https://github.com/fpgmaas/deptry
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <img alt="deptry logo" width="460" height="300" src="https://raw.githubusercontent.com/fpgmaas/deptry/main/docs/static/deptry_Logo-01.svg">
+</p>
+
+[![Release](https://img.shields.io/github/v/release/fpgmaas/deptry)](https://pypi.org/project/deptry/)
+[![Build status](https://github.com/fpgmaas/deptry/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/fpgmaas/deptry/actions/workflows/main.yml)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/deptry)](https://pypi.org/project/deptry/)
+[![codecov](https://codecov.io/gh/fpgmaas/deptry/branch/main/graph/badge.svg)](https://codecov.io/gh/fpgmaas/deptry)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/deptry)](https://pypistats.org/packages/deptry)
+[![License](https://img.shields.io/github/license/fpgmaas/deptry)](https://img.shields.io/github/license/fpgmaas/deptry)
+
+_deptry_ is a command line tool to check for issues with dependencies in a Python project, such as obsolete or missing dependencies. It supports the following types of projects:
+
+- Projects that use [Poetry](https://python-poetry.org/) and a corresponding _pyproject.toml_ file
+- Projects that use [PDM](https://pdm.fming.dev/latest/) and a corresponding _pyproject.toml_ file
+- Projects that use a _requirements.txt_ file according to the [pip](https://pip.pypa.io/en/stable/user_guide/) standards
+
+Dependency issues are detected by scanning for imported modules within all Python files in a directory and its subdirectories, and comparing those to the dependencies listed in the project's requirements.
+
+---
+<p align="center">
+  <a href="https://fpgmaas.github.io/deptry">Documentation</a> - <a href="https://fpgmaas.github.io/deptry/contributing/">Contributing</a>
+</p>
+
+---
+
+## Quickstart
+
+### Installation
+
+_deptry_ can be added to your project with
+
+```shell
+poetry add --group dev deptry
+```
+
+or with:
+
+```shell
+<activate virtual environment>
+pip install deptry
+```
+
+> **Warning**: When using pip to install _deptry_, make sure you install it within the virtual environment of your project. Installing _deptry_ globally will not work, since it needs to have access to the metadata of the packages in the virtual environment.
+
+### Prerequisites
+
+_deptry_ should be run within the root directory of the project to be scanned, and the project should be running in its own dedicated virtual environment.
+
+### Usage
+
+To scan your project for dependency issues, run:
+
+```shell
+deptry .
+```
 
-packages = \
-['deptry',
- 'deptry.dependency_getter',
- 'deptry.imports',
- 'deptry.imports.extractors',
- 'deptry.issues_finder']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['chardet>=4.0.0', 'click>=8.0.0,<9.0.0', 'pathspec>=0.9.0']
-
-extras_require = \
-{':python_full_version <= "3.7.0"': ['importlib-metadata'],
- ':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['deptry = deptry.cli:deptry']}
-
-setup_kwargs = {
-    'name': 'deptry',
-    'version': '0.8.0',
-    'description': 'A command line utility to check for obsolete, missing and transitive dependencies in a Python project.',
-    'long_description': '<p align="center">\n  <img alt="deptry logo" width="460" height="300" src="https://raw.githubusercontent.com/fpgmaas/deptry/main/docs/static/deptry_Logo-01.svg">\n</p>\n\n[![Release](https://img.shields.io/github/v/release/fpgmaas/deptry)](https://pypi.org/project/deptry/)\n[![Build status](https://github.com/fpgmaas/deptry/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/fpgmaas/deptry/actions/workflows/main.yml)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/deptry)](https://pypi.org/project/deptry/)\n[![codecov](https://codecov.io/gh/fpgmaas/deptry/branch/main/graph/badge.svg)](https://codecov.io/gh/fpgmaas/deptry)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/deptry)](https://pypistats.org/packages/deptry)\n[![License](https://img.shields.io/github/license/fpgmaas/deptry)](https://img.shields.io/github/license/fpgmaas/deptry)\n\n_deptry_ is a command line tool to check for issues with dependencies in a Python project, such as obsolete or missing dependencies. It supports the following types of projects:\n\n- Projects that use [Poetry](https://python-poetry.org/) and a corresponding _pyproject.toml_ file\n- Projects that use [PDM](https://pdm.fming.dev/latest/) and a corresponding _pyproject.toml_ file\n- Projects that use a _requirements.txt_ file according to the [pip](https://pip.pypa.io/en/stable/user_guide/) standards\n\nDependency issues are detected by scanning for imported modules within all Python files in a directory and its subdirectories, and comparing those to the dependencies listed in the project\'s requirements.\n\n---\n<p align="center">\n  <a href="https://fpgmaas.github.io/deptry">Documentation</a> - <a href="https://fpgmaas.github.io/deptry/contributing/">Contributing</a>\n</p>\n\n---\n\n## Quickstart\n\n### Installation\n\n_deptry_ can be added to your project with\n\n```shell\npoetry add --group dev deptry\n```\n\nor with:\n\n```shell\n<activate virtual environment>\npip install deptry\n```\n\n> **Warning**: When using pip to install _deptry_, make sure you install it within the virtual environment of your project. Installing _deptry_ globally will not work, since it needs to have access to the metadata of the packages in the virtual environment.\n\n### Prerequisites\n\n_deptry_ should be run within the root directory of the project to be scanned, and the project should be running in its own dedicated virtual environment.\n\n### Usage\n\nTo scan your project for dependency issues, run:\n\n```shell\ndeptry .\n```\n\n_deptry_ can be configured by using additional command line arguments, or by adding a `[tool.deptry]` section in _pyproject.toml_.\n\nFor more information, see the [documentation](https://fpgmaas.github.io/deptry/).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
-    'author': 'Florian Maas',
-    'author_email': 'fpgmaas@gmail.com',
-    'maintainer': 'Mathieu Kniewallner',
-    'maintainer_email': 'mathieu.kniewallner@gmail.com',
-    'url': 'https://github.com/fpgmaas/deptry',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+_deptry_ can be configured by using additional command line arguments, or by adding a `[tool.deptry]` section in _pyproject.toml_.
 
+For more information, see the [documentation](https://fpgmaas.github.io/deptry/).
+
+---
+
+Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,51 +1,53 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['deptry',
-'deptry.dependency_getter', 'deptry.imports', 'deptry.imports.extractors',
-'deptry.issues_finder'] package_data = \ {'': ['*']} install_requires = \
-['chardet>=4.0.0', 'click>=8.0.0,<9.0.0', 'pathspec>=0.9.0'] extras_require = \
-{':python_full_version <= "3.7.0"': ['importlib-metadata'], ':python_version <
-"3.11"': ['tomli>=2.0.1,<3.0.0']} entry_points = \ {'console_scripts': ['deptry
-= deptry.cli:deptry']} setup_kwargs = { 'name': 'deptry', 'version': '0.8.0',
-'description': 'A command line utility to check for obsolete, missing and
-transitive dependencies in a Python project.', 'long_description': '
-                              \n [deptry logo]\n
-\n\n[![Release](https://img.shields.io/github/v/release/fpgmaas/deptry)](https:
-//pypi.org/project/deptry/)\n[![Build status](https://github.com/fpgmaas/
-deptry/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/
-fpgmaas/deptry/actions/workflows/main.yml)\n[![Supported Python versions]
-(https://img.shields.io/pypi/pyversions/deptry)](https://pypi.org/project/
-deptry/)\n[![codecov](https://codecov.io/gh/fpgmaas/deptry/branch/main/graph/
-badge.svg)](https://codecov.io/gh/fpgmaas/deptry)\n[![PyPI - Downloads](https:/
-/img.shields.io/pypi/dm/deptry)](https://pypistats.org/packages/deptry)\n[!
+Metadata-Version: 2.1 Name: deptry Version: 0.9.0 Summary: A command line
+utility to check for obsolete, missing and transitive dependencies in a Python
+project. Home-page: https://github.com/fpgmaas/deptry License: MIT Keywords:
+dependency,poetry Author: Florian Maas Author-email: fpgmaas@gmail.com
+Maintainer: Mathieu Kniewallner Maintainer-email: mathieu.kniewallner@gmail.com
+Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Quality Assurance Requires-Dist: chardet (>=4.0.0) Requires-
+Dist: click (>=8.0.0,<9.0.0) Requires-Dist: pathspec (>=0.9.0) Requires-Dist:
+tomli (>=2.0.1,<3.0.0) ; python_version < "3.11" Project-URL: Documentation,
+https://fpgmaas.github.io/deptry/ Project-URL: Repository, https://github.com/
+fpgmaas/deptry Description-Content-Type: text/markdown
+                                 [deptry logo]
+[![Release](https://img.shields.io/github/v/release/fpgmaas/deptry)](https://
+pypi.org/project/deptry/) [![Build status](https://github.com/fpgmaas/deptry/
+actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/fpgmaas/
+deptry/actions/workflows/main.yml) [![Supported Python versions](https://
+img.shields.io/pypi/pyversions/deptry)](https://pypi.org/project/deptry/) [!
+[codecov](https://codecov.io/gh/fpgmaas/deptry/branch/main/graph/badge.svg)]
+(https://codecov.io/gh/fpgmaas/deptry) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/deptry)](https://pypistats.org/packages/deptry) [!
 [License](https://img.shields.io/github/license/fpgmaas/deptry)](https://
-img.shields.io/github/license/fpgmaas/deptry)\n\n_deptry_ is a command line
-tool to check for issues with dependencies in a Python project, such as
-obsolete or missing dependencies. It supports the following types of projects:
-\n\n- Projects that use [Poetry](https://python-poetry.org/) and a
-corresponding _pyproject.toml_ file\n- Projects that use [PDM](https://
-pdm.fming.dev/latest/) and a corresponding _pyproject.toml_ file\n- Projects
-that use a _requirements.txt_ file according to the [pip](https://pip.pypa.io/
-en/stable/user_guide/) standards\n\nDependency issues are detected by scanning
-for imported modules within all Python files in a directory and its
-subdirectories, and comparing those to the dependencies listed in the
-project\'s requirements.\n\n---\n
-                       \n Documentation - Contributing\n
-\n\n---\n\n## Quickstart\n\n### Installation\n\n_deptry_ can be added to your
-project with\n\n```shell\npoetry add --group dev deptry\n```\n\nor with:
-\n\n```shell\n\npip install deptry\n```\n\n> **Warning**: When using pip to
-install _deptry_, make sure you install it within the virtual environment of
-your project. Installing _deptry_ globally will not work, since it needs to
-have access to the metadata of the packages in the virtual environment.\n\n###
-Prerequisites\n\n_deptry_ should be run within the root directory of the
-project to be scanned, and the project should be running in its own dedicated
-virtual environment.\n\n### Usage\n\nTo scan your project for dependency
-issues, run:\n\n```shell\ndeptry .\n```\n\n_deptry_ can be configured by using
-additional command line arguments, or by adding a `[tool.deptry]` section in
-_pyproject.toml_.\n\nFor more information, see the [documentation](https://
-fpgmaas.github.io/deptry/).\n\n---\n\nRepository initiated with [fpgmaas/
-cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
-'author': 'Florian Maas', 'author_email': 'fpgmaas@gmail.com', 'maintainer':
-'Mathieu Kniewallner', 'maintainer_email': 'mathieu.kniewallner@gmail.com',
-'url': 'https://github.com/fpgmaas/deptry', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'entry_points': entry_points,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+img.shields.io/github/license/fpgmaas/deptry) _deptry_ is a command line tool
+to check for issues with dependencies in a Python project, such as obsolete or
+missing dependencies. It supports the following types of projects: - Projects
+that use [Poetry](https://python-poetry.org/) and a corresponding
+_pyproject.toml_ file - Projects that use [PDM](https://pdm.fming.dev/latest/
+) and a corresponding _pyproject.toml_ file - Projects that use a
+_requirements.txt_ file according to the [pip](https://pip.pypa.io/en/stable/
+user_guide/) standards Dependency issues are detected by scanning for imported
+modules within all Python files in a directory and its subdirectories, and
+comparing those to the dependencies listed in the project's requirements. ---
+                         Documentation - Contributing
+--- ## Quickstart ### Installation _deptry_ can be added to your project with
+```shell poetry add --group dev deptry ``` or with: ```shell  pip install
+deptry ``` > **Warning**: When using pip to install _deptry_, make sure you
+install it within the virtual environment of your project. Installing _deptry_
+globally will not work, since it needs to have access to the metadata of the
+packages in the virtual environment. ### Prerequisites _deptry_ should be run
+within the root directory of the project to be scanned, and the project should
+be running in its own dedicated virtual environment. ### Usage To scan your
+project for dependency issues, run: ```shell deptry . ``` _deptry_ can be
+configured by using additional command line arguments, or by adding a `
+[tool.deptry]` section in _pyproject.toml_. For more information, see the
+[documentation](https://fpgmaas.github.io/deptry/). --- Repository initiated
+with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-
+poetry).
```

