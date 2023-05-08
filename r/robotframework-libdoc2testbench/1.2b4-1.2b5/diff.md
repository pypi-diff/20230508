# Comparing `tmp/robotframework-libdoc2testbench-1.2b4.tar.gz` & `tmp/robotframework-libdoc2testbench-1.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-libdoc2testbench-1.2b4.tar", last modified: Fri Apr 21 08:33:05 2023, max compression
+gzip compressed data, was "robotframework-libdoc2testbench-1.2b5.tar", last modified: Thu May  4 14:45:55 2023, max compression
```

## Comparing `robotframework-libdoc2testbench-1.2b4.tar` & `robotframework-libdoc2testbench-1.2b5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.082648 robotframework-libdoc2testbench-1.2b4/
--rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b4/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)      182 2022-02-01 11:40:46.000000 robotframework-libdoc2testbench-1.2b4/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:33:05.082358 robotframework-libdoc2testbench-1.2b4/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     6163 2022-02-01 11:41:54.000000 robotframework-libdoc2testbench-1.2b4/README.md
--rw-r--r--   0 rener      (502) wheel        (0)     1671 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b4/Setup.py
--rwxr-xr-x   0 rener      (502) wheel        (0)      171 2023-04-21 08:20:32.000000 robotframework-libdoc2testbench-1.2b4/createPip_whl_tar.sh
--rw-r--r--   0 rener      (502) wheel        (0)     1431 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b4/pyproject.toml
--rw-r--r--   0 rener      (502) wheel        (0)       38 2023-04-21 08:33:05.082740 robotframework-libdoc2testbench-1.2b4/setup.cfg
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.075831 robotframework-libdoc2testbench-1.2b4/src/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.079561 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/
--rw-r--r--   0 rener      (502) wheel        (0)    10474 2023-04-21 08:32:19.000000 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)      852 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__main__.py
--rw-r--r--   0 rener      (502) wheel        (0)    22962 2023-04-21 08:32:08.000000 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/testbenchwriter.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.081945 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)      545 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)      118 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)       53 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       17 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-04 14:45:55.121784 robotframework-libdoc2testbench-1.2b5/
+-rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b5/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)      182 2022-02-01 11:40:46.000000 robotframework-libdoc2testbench-1.2b5/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-05-04 14:45:55.121610 robotframework-libdoc2testbench-1.2b5/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     6163 2022-02-01 11:41:54.000000 robotframework-libdoc2testbench-1.2b5/README.md
+-rw-r--r--   0 rener      (502) wheel        (0)     1671 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b5/Setup.py
+-rwxr-xr-x   0 rener      (502) wheel        (0)      171 2023-04-21 08:20:32.000000 robotframework-libdoc2testbench-1.2b5/createPip_whl_tar.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     2196 2023-05-04 14:23:12.000000 robotframework-libdoc2testbench-1.2b5/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)       38 2023-05-04 14:45:55.121821 robotframework-libdoc2testbench-1.2b5/setup.cfg
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-04 14:45:55.118982 robotframework-libdoc2testbench-1.2b5/src/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-04 14:45:55.120450 robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/
+-rw-r--r--   0 rener      (502) wheel        (0)    10860 2023-05-04 14:45:40.000000 robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)      852 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/__main__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    23017 2023-05-04 14:42:54.000000 robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/testbenchwriter.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-04 14:45:55.121411 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-05-04 14:45:55.000000 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      545 2023-05-04 14:45:55.000000 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-05-04 14:45:55.000000 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      118 2023-05-04 14:45:55.000000 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       53 2023-05-04 14:45:55.000000 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       17 2023-05-04 14:45:55.000000 robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/top_level.txt
```

### Comparing `robotframework-libdoc2testbench-1.2b4/LICENSE` & `robotframework-libdoc2testbench-1.2b5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b4/PKG-INFO` & `robotframework-libdoc2testbench-1.2b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-libdoc2testbench
-Version: 1.2b4
+Version: 1.2b5
 Summary: Robot Framework Libdoc Extension that generates imbus TestBench Library import formats.
 Home-page: https://github.com/imbus/robotframework-libdoc2testbench
 Author: imbus AG | Maximilian Birkenhagen
 Author-email: maximilian.birkenhagen@imbus.de
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-libdoc2testbench-1.2b4/README.md` & `robotframework-libdoc2testbench-1.2b5/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b4/Setup.py` & `robotframework-libdoc2testbench-1.2b5/Setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__init__.py` & `robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,40 +9,61 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import argparse
-import os
 import re
 import shutil
 import sys
+from enum import Enum
 from pathlib import Path
 from zipfile import ZipFile
 
 from robot.libdocpkg import LibraryDocumentation
 from robot.libdocpkg.robotbuilder import LibraryDoc
+from robot.running.arguments.argumentspec import ArgInfo
+from robot.utils import safe_str
 from robot.version import get_full_version as robot_version_print
 
 from .testbenchwriter import Libdoc2TestBenchWriter
 
-__version__ = "1.2b4"
+__version__ = "1.2b5"
+
+
+
+
+def default_repr(self):
+    if self.default is self.NOTSET:
+        return None
+    if (
+        isinstance(self.default, (bool, int, float)) or self.default is None
+    ):
+        return f"${{{self.default}}}"
+    if self.default == "":  # noqa: PLC1901
+        return "${Empty}"
+    if isinstance(self.default, Enum):
+        return self.default.name
+    return safe_str(self.default)
+
+
+ArgInfo.default_repr = property(default_repr)
 
 
 def start_libdoc2testbench():
     """Command line entry point for the Libdoc2TestBench module."""
     parser = argparse.ArgumentParser(
         description="""Robot Framework Libdoc Extension that generates imbus
                     TestBench Library import formats. The easiest way to run
                     Libdoc2TestBench is just using the `Libdoc2TestBench`
                     command and giving it one resource or library to generate
                     a zip-file at the current location.
                     """,
-        usage=f"Libdoc2TestBench <LIBRARY> <output.zip>",
+        usage="Libdoc2TestBench <LIBRARY> <output.zip>",
         prog='Libdoc2TestBench',
         epilog='Example: Libdoc2TestBench Browser My-Browser-Dump.zip',
     )
     parser.add_argument(
         "library_or_resource", help="RF library or resource", nargs='?', default=None
     )
     parser.add_argument(
@@ -153,15 +174,14 @@
     attachment: bool,
 ):
     # Init attachments_path, for handling a resource
     attachments_path = None
 
     # Holds the last generated primary key by the testbenchwriter.
     # This is used as part of the exit message on successful conversion.
-    last_issued_pk = None
 
     libraries, resources = get_libdoc_lists(
         lib_or_res, lib_name, lib_version, docformat, specdocformat
     )
 
     # If set, create necessary subdirectories
     if temp_path:
@@ -177,33 +197,30 @@
     if project_dump_path.is_file():
         user_input = input('project-dump.xml already exists... overwrite? y/n? \n')
         if user_input.lower() not in ['y', 'yes']:
             sys.exit('Stopped execution - file was not changed.')
 
     if not outfile_path:
         lib_lists = libraries + resources
-        if len(lib_lists) == 1:
-            outfile_path = lib_lists[0].name
-        else:
-            outfile_path = 'project-dump'
+        outfile_path = lib_lists[0].name if len(lib_lists) == 1 else "project-dump"
 
     if xml_flag:
         outfile_path = (
             outfile_path
-            if os.path.splitext(outfile_path)[1].lower() == '.xml'
+            if Path(outfile_path).suffix.lower() == ".xml"
             else f"{outfile_path}.xml"
         )
     else:
         outfile_path = (
             outfile_path
-            if os.path.splitext(outfile_path)[1].lower() == '.zip'
+            if Path(outfile_path).suffix.lower() == '.zip'
             else f"{outfile_path}.zip"
         )
 
-    with open(project_dump_path, "w", encoding='UTF-8') as outfile:
+    with Path(project_dump_path).open( "w", encoding='UTF-8') as outfile:
         # The write method returns the last issued primary key.
         Libdoc2TestBenchWriter().write(
             libraries,
             resources,
             outfile,
             repo_id,
             library_root,
@@ -212,39 +229,39 @@
         )
 
         # If a file exists at the output path - get permission to overwrite.
         if Path(outfile_path).is_file():
             user_input = input(f'{outfile_path} already exists... overwrite? y/n? \n')
             if user_input.lower() not in ['y', 'yes']:
                 sys.exit('Stopped execution - file was not changed.')
-            os.remove(outfile_path)
+            Path(outfile_path).unlink()
 
         if xml_flag:
             # Put XML-file in output_path and leave attachments behind
-            os.rename(project_dump_path, outfile_path)
+            Path(project_dump_path).rename(outfile_path)
         else:
             # Build the zip file and clean up.
             write_zip_file(outfile_path, project_dump_path, resources, attachment)
-            os.remove(project_dump_path)
+            Path(project_dump_path).unlink()
             if attachments_path:
                 shutil.rmtree(attachments_path)
 
     absolute_outfile_path = Path(outfile_path).resolve()
     print(f"Successfully written TestBench project dump to: \n{absolute_outfile_path}")
 
 
 def get_libdoc_lists(lib_or_res, lib_name, lib_version, docformat, specdocformat):
     resources = []
     libraries = []
-    if os.path.exists(lib_or_res):
-        with open(lib_or_res, "r", encoding='UTF-8') as library_list:
+    if Path(lib_or_res).exists():
+        with Path(lib_or_res).open(encoding='UTF-8') as library_list:
             first_line = library_list.readline()
             if re.fullmatch(r'\*+\s*import\s?list(\s?\**)\n?', first_line, re.IGNORECASE):
                 for line in library_list.read().splitlines():
-                    if not line.strip().startswith('#') and not len(line.strip()) == 0:
+                    if not line.strip().startswith('#') and len(line.strip()) != 0:
                         libdoc = create_libdoc(
                             line.strip(), lib_name, lib_version, docformat, specdocformat
                         )
                         if libdoc.type == 'RESOURCE':
                             resources.append(libdoc)
                         else:
                             libraries.append(libdoc)
@@ -270,22 +287,20 @@
 
 def create_libdoc(lib_or_res, lib_name, lib_version, docformat, specdocformat) -> LibraryDoc:
     try:
         libdoc = LibraryDocumentation(lib_or_res, lib_name, lib_version, docformat)
         if specdocformat == 'HTML':
             libdoc.convert_docs_to_html()
         return libdoc
-    except:
+    except Exception:
         sys.exit(f"The requested module {lib_or_res} could not be found.")
 
 
 def write_zip_file(outfile_path, project_dump_path, resources, attachment):
     with ZipFile(outfile_path, 'w') as zip_file:
         zip_file.write(project_dump_path, 'project-dump.xml')
 
         # If there are attachments, add them to the zip-file.
         if resources and attachment:
-            # zip_file.write('attachments)
             for libdoc in resources:
-                if os.path.exists(libdoc.source):
-                    file = os.path.split(libdoc.source)[-1]
-                    zip_file.write(libdoc.source, "attachments/" + file)
+                if Path(libdoc.source).exists():
+                    zip_file.write(libdoc.source, "attachments/" + Path(libdoc.source).name)
```

### Comparing `robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__main__.py` & `robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/testbenchwriter.py` & `robotframework-libdoc2testbench-1.2b5/src/Libdoc2TestBench/testbenchwriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 #  This code contains derived code from Robot Framework Core Project
 #  under Apache 2.0 License.
 #  https://github.com/robotframework/robotframework
 
 import enum
 import os
-from datetime import datetime
+from datetime import datetime, timezone
 from hashlib import sha1
 from pathlib import Path
 from typing import Dict, List, Optional, Set
 
 from robot.libdocpkg.robotbuilder import LibraryDoc
 from robot.running.arguments.argumentspec import ArgInfo
 from robot.utils import XmlWriter
@@ -123,15 +123,15 @@
 
     # Created when first evoked by self.write
     pk_generator = None
 
     # Values used to fill project view fields.
     testobject_state = ProjectStates.active.value
     testobject_desc = "Robot Framework Import"
-    created_time = f"{datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')} +0000"
+    created_time = datetime.now(tz=timezone.utc).strftime('%Y-%m-%d %H:%M:%S %z')
     libdoc_name = None  # set-up in write() method.
     attachment_reference_pk = {}  # Needed for resource files - holds exactly one pk
 
     # Attributes used in the header of the xml-file
     xml_attributes = {'version': "3.0", 'build-number': "230202/6a0c", 'repository': "iTB_RF"}
 
     # Values used to fill imbus TestBench project settings.
@@ -295,55 +295,58 @@
         writer.start('test-elements')
 
     def _start_root_subdivision(self, writer, name, description):
         # Start RF/Resource subdivison
         writer.start('element', {'type': ElementTypes.subdivision.value})
         writer.element('pk', self.pk_generator.get_pk())
         writer.element('name', name)
-        writer.element('uid', self._generate_UID('SD', name))
+        writer.element('uid', self._generate_uid('SD', name))
         writer.element('locker', '')
         writer.element('description', description)
         writer.element('html-description', '')
         writer.element('historyPK', '-1')
         writer.element('identicalVersionPK', '-1')
         writer.element('references', '')
 
     def _start_library_subdivision(self, libdoc, writer):
         writer.start('element', {'type': ElementTypes.subdivision.value})
         writer.element('pk', self.pk_generator.get_pk())
         writer.element('name', libdoc.name)
-        writer.element('uid', self._generate_UID('SD', libdoc.name))
+        writer.element('uid', self._generate_uid('SD', libdoc.name))
         writer.element('locker', '')
         writer.element(
             'html-description',
             f"<html><p> Import of {libdoc.name} {libdoc.version}</p>{libdoc.doc}</html>",
         )
         writer.element('historyPK', '-1')
         writer.element('identicalVersionPK', '-1')
         writer.element('references', '')
 
     def _get_argument_name_prefix(self, argument_kind: str) -> str:
         if argument_kind == ArgInfo.VAR_POSITIONAL:
             return "* "
-        elif argument_kind == ArgInfo.VAR_NAMED:
+        if argument_kind == ArgInfo.VAR_NAMED:
             return "** "
-        elif argument_kind == ArgInfo.NAMED_ONLY:
+        if argument_kind == ArgInfo.NAMED_ONLY:
             return "- "
         return ""
 
     def _write_interactions(self, libdoc, writer, attachment=False):
         libdoc_dic = libdoc.to_dictionary()
         for keyword in libdoc_dic["keywords"]:
             writer.start('element', {'type': ElementTypes.interaction.value})
             writer.element('pk', self.pk_generator.get_pk())
             writer.element('name', keyword['name'])
-            writer.element('uid', self._generate_UID('IA', keyword['name'], libdoc.name))
+            writer.element('uid', self._generate_uid('IA', keyword['name'], libdoc.name))
             writer.element('locker', '')
             writer.element('status', '3')
-            writer.element('html-description', f"<html>{keyword['doc'].replace('<br>', '<br/>').replace('<hr>', '<br>')}</html>")
+            writer.element(
+                'html-description',
+                f"<html>{keyword['doc'].replace('<br>', '<br/>').replace('<hr>', '<br>')}</html>",
+            )
             writer.element('historyPK', '-1')
             writer.element('identicalVersionPK', '-1')
             writer.start('references')
 
             if attachment:
                 writer.element(
                     'reference-ref', attrs={'pk': self.attachment_reference_pk[libdoc.name]}
@@ -368,15 +371,15 @@
                 writer.element('datatype-ref', '', {'pk': typ_pk})
                 writer.element('definition-type', '0')
                 writer.element('use-type', '1')
                 writer.element('datatype-name', type_name)
                 default_value = arg.get('defaultValue')
                 if default_value is None:
                     default_value = self._get_arg_kind_default_value(argument_kind)
-                if default_value is not None:
+                else:
                     writer.start('default-value', {'type': 'representative'})
                     writer.element('type', '1')
                     representative_pk = Element.all_elements.get(
                         f"{type_name}.{default_value}", '-1'
                     )
                     writer.element('representative-ref', '', {'pk': representative_pk})
                     writer.element('representative-name', default_value)
@@ -384,15 +387,15 @@
                 writer.end('parameter')
             writer.end('parameters')
             writer.end('element')  # close interaction tag
 
     def _get_arg_kind_default_value(self, argument_kind: str) -> Optional[str]:
         if argument_kind == ArgInfo.VAR_POSITIONAL:
             return "@{EMPTY}"
-        elif argument_kind == ArgInfo.VAR_NAMED:
+        if argument_kind == ArgInfo.VAR_NAMED:
             return "&{EMPTY}"
         return None
 
     def _get_datatype_name(self, argument: Dict[str, str]) -> str:
         for argument_type in argument.get('typedocs', {}).values():
             if argument_type in self.enum_types or argument_type in self.typed_dicts:
                 return argument_type
@@ -439,15 +442,15 @@
             datatype_documentation = self._get_datatype_documentation(datatype_name, libdoc_dic)
             datatype = datatypes.get(datatype_name) or DataType(
                 self.pk_generator, datatype_name, datatype_documentation
             )
             default_value = argument.get('defaultValue')
             if default_value is None:
                 default_value = self._get_arg_kind_default_value(argument_kind)
-            for idx, type_name in enumerate(argument.get('typedocs', {}).keys()):
+            for type_name in argument.get('typedocs', {}):
                 members = set()
                 if type_name == "bool":
                     members = {'True', 'False', '${True}', '${False}'}
                     datatype.add_equivalence_class(type_name, members)
                 elif type_name in self.enum_types:
                     members_list = next(
                         filter(
@@ -463,29 +466,32 @@
                 datatype.add_equivalence_class(datatype_name, {default_value})
             datatype.add_equivalence_class(datatype_name)
             datatypes[datatype_name] = datatype
 
         writer.start('element', {'type': ElementTypes.subdivision.value})
         writer.element('pk', self.pk_generator.get_pk())
         writer.element('name', '_Datatypes')
-        writer.element('uid', self._generate_UID('SD', '_Datatypes', libdoc.name))
+        writer.element('uid', self._generate_uid('SD', '_Datatypes', libdoc.name))
         writer.element('locker', '')
         writer.element('status', '3')
         writer.element('html-description', '')
         writer.element('historyPK', '-1')
         writer.element('identicalVersionPK', '-1')
         writer.element('references', '')
 
         for datatype_idx, data_type in enumerate(datatypes.values()):
             writer.start('element', {'type': ElementTypes.datatype.value})
             writer.element('pk', data_type.pk)
             writer.element('name', data_type.get_name())
-            writer.element('uid', self._generate_UID('DT', data_type.name, libdoc.name))
+            writer.element('uid', self._generate_uid('DT', data_type.name, libdoc.name))
             writer.element('locker', '')
-            writer.element('html-description', data_type.html_desc.replace('<br>', '<br/>').replace('<hr>', '<br>'))
+            writer.element(
+                'html-description',
+                data_type.html_desc.replace('<br>', '<br/>').replace('<hr>', '<br>'),
+            )
             writer.element('historyPK', '-1')
             writer.element('identicalVersionPK', '-1')
             writer.start('equivalence-classes')
             for ec_name, ec_members in data_type.equivalence_classes.items():
                 writer.start('equivalence-class')
                 writer.element('pk', self.pk_generator.get_pk())
                 writer.element('name', ec_name)
@@ -525,15 +531,15 @@
         writer.start('referenced-user-names')
         writer.end('referenced-user-names')
         writer.element('errors', '')
         writer.element('warnings', '')
         writer.end('project-dump')
         writer.close()
 
-    def _generate_UID(self, element_type: str, element_name: str, lib_name: str = "") -> str:
+    def _generate_uid(self, element_type: str, element_name: str, lib_name: str = "") -> str:
         # UIDs format:
         # Prefix: RepositoryID-AbreviationElementType-
         # Root: first 10 characters of sha1Hash of LibraryName.ElementName
         repository_id = self.xml_attributes.get('repository', 'itb')
 
         # robustify element name regarding smaller changes
         element_name = element_name.replace('_', '')
```

### Comparing `robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/PKG-INFO` & `robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-libdoc2testbench
-Version: 1.2b4
+Version: 1.2b5
 Summary: Robot Framework Libdoc Extension that generates imbus TestBench Library import formats.
 Home-page: https://github.com/imbus/robotframework-libdoc2testbench
 Author: imbus AG | Maximilian Birkenhagen
 Author-email: maximilian.birkenhagen@imbus.de
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt` & `robotframework-libdoc2testbench-1.2b5/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

