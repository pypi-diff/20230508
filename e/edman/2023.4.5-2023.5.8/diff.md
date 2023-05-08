# Comparing `tmp/edman-2023.4.5.tar.gz` & `tmp/edman-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2023.4.5.tar", last modified: Wed Apr  5 05:03:14 2023, max compression
+gzip compressed data, was "edman-2023.5.8.tar", last modified: Mon May  8 02:04:22 2023, max compression
```

## Comparing `edman-2023.4.5.tar` & `edman-2023.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:03:14.919325 edman-2023.4.5/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.4.5/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-04-13 07:00:02.000000 edman-2023.4.5/MANIFEST.in
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-04-05 05:03:14.919325 edman-2023.4.5/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.4.5/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:03:14.909325 edman-2023.4.5/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2022-04-13 07:00:02.000000 edman-2023.4.5/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.4.5/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.4.5/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.4.5/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.4.5/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    20001 2023-04-05 05:00:36.000000 edman-2023.4.5/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.4.5/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10113 2023-04-05 05:00:36.000000 edman-2023.4.5/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.4.5/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:03:14.919325 edman-2023.4.5/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-04-05 05:03:14.000000 edman-2023.4.5/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      470 2023-04-05 05:03:14.000000 edman-2023.4.5/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-04-05 05:03:14.000000 edman-2023.4.5/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-04-05 05:03:14.000000 edman-2023.4.5/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        6 2023-04-05 05:03:14.000000 edman-2023.4.5/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      707 2023-04-05 05:03:14.919325 edman-2023.4.5/setup.cfg
--rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2022-04-13 07:00:02.000000 edman-2023.4.5/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:03:14.919325 edman-2023.4.5/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.4.5/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    87007 2023-03-09 05:51:32.000000 edman-2023.4.5/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    36057 2023-04-05 05:00:36.000000 edman-2023.4.5/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.4.5/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.4.5/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.4.5/tests/test_utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-04-13 07:00:02.000000 edman-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:22.028113 edman-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.8/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    21800 2023-05-08 02:02:11.000000 edman-2023.5.8/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.8/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      470 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        6 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      707 2023-05-08 02:04:22.028113 edman-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2022-04-13 07:00:02.000000 edman-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.8/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    36850 2023-05-08 02:02:11.000000 edman-2023.5.8/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.8/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.8/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_utils.py
```

### Comparing `edman-2023.4.5/LICENSE.txt` & `edman-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/PKG-INFO` & `edman-2023.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.4.5
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Home-page: https://github.com/ryde/edman
 Author: Masaki Ohno
 Author-email: masakio@post.kek.jp
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
```

### Comparing `edman-2023.4.5/README.rst` & `edman-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman/config.py` & `edman-2023.5.8/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman/convert.py` & `edman-2023.5.8/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman/db.py` & `edman-2023.5.8/edman/db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman/exceptions.py` & `edman-2023.5.8/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman/file.py` & `edman-2023.5.8/edman/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import copy
 import gzip
 from tempfile import TemporaryDirectory, NamedTemporaryFile
 import datetime
 import zipfile
-from typing import Union, Tuple, Iterator, List
+from typing import Union, Tuple, Iterator, List, Any
 from pathlib import Path
 import gridfs
 from gridfs.errors import NoFile, GridFSError
 import jmespath
 from bson import ObjectId
 from edman.utils import Utils
 from edman.exceptions import (EdmanFormatError, EdmanDbProcessError,
@@ -43,78 +43,14 @@
             try:
                 with file.open('rb') as f:
                     fp = f.read()
             except IOError:
                 raise
             yield file.name, fp
 
-    def add_file_reference(self, collection: str, oid: Union[ObjectId, str],
-                           file_path: Tuple[Path], structure: str,
-                           query=None, compress=False) -> bool:
-        """
-        ドキュメントにファイルリファレンスを追加する
-        ファイルのインサート処理、圧縮処理なども行う
-
-        :param str collection:
-        :param oid:
-        :type oid: ObjectId or str
-        :param tuple file_path:
-        :param str structure:
-        :param query:
-        :type query: list or None
-        :param bool compress: default False
-        :return:
-        :rtype: bool
-        """
-
-        oid = Utils.conv_objectid(oid)
-
-        # ドキュメント存在確認&対象ドキュメント取得
-        doc = self.db[collection].find_one({'_id': oid})
-        if doc is None:
-            raise EdmanInternalError('対象のドキュメントが存在しません')
-
-        if structure == 'emb':
-            # クエリーがドキュメントのキーとして存在するかチェック
-            if not Utils.query_check(query, doc):
-                raise EdmanFormatError('対象のドキュメントに対してクエリーが一致しません.')
-
-        # ファイルのインサート
-        inserted_file_oids = []
-        for file in self.file_gen(file_path):
-            file_obj = file[1]
-            metadata = {'filename': file[0]}
-
-            if compress:
-                file_obj = gzip.compress(file_obj,
-                                         compresslevel=self.comp_level)
-                metadata.update({'compress': 'gzip'})
-
-            inserted_file_oids.append(self.fs.put(file_obj, **metadata))
-
-        if structure == 'ref':
-            new_doc = self.file_list_attachment(doc, inserted_file_oids)
-        elif structure == 'emb':
-            try:
-                new_doc = Utils.doc_traverse(doc, inserted_file_oids, query,
-                                             self.file_list_attachment)
-            except Exception:
-                raise
-        else:
-            raise EdmanFormatError('構造はrefかembが必要です')
-
-        # ドキュメント差し替え
-        replace_result = self.db[collection].replace_one({'_id': oid}, new_doc)
-
-        if replace_result.modified_count == 1:
-            return True
-        else:  # 差し替えができなかった時は添付ファイルは削除
-            self.fs_delete(inserted_file_oids)
-            return False
-
     def delete(self, delete_oid: ObjectId, collection: str,
                oid: Union[ObjectId, str], structure: str, query=None) -> bool:
         """
         該当のoidをファイルリファレンスから削除し、GridFSからファイルを削除
 
         :param ObjectId delete_oid:
         :param str collection:
@@ -236,57 +172,150 @@
                 fs_out = self.fs.get(file_oid)
             except gridfs.errors.NoFile:
                 continue
             else:
                 result.update({file_oid: fs_out.filename})
         return result
 
-    def download(self, oid: ObjectId, path: Union[str, Path]) -> bool:
+    def download(self, file_oid: list[ObjectId],
+                 path: Union[str, Path]) -> bool:
         """
         Gridfsからデータをダウンロードし、ファイルに保存
         metadataに圧縮指定があれば伸長する
 
-        :param ObjectId oid:
+        :param list file_oid:
+        :param path:
+        :type path: str or Path
+        :return: result
+        :rtype: bool
+        """
+        # 定型的な前処理があればここに追加する
+        return self._grid_out(file_oid, path)
+
+    def _grid_out(self, file_oid_list: List[ObjectId],
+                  path: Union[str, Path]) -> bool:
+        """
+        Gridfsからデータを取得し、ファイルに保存
+        metadataに圧縮指定があれば伸長する
+        複数のファイルを指定すると、複数のファイルが作成される
+
+        :param list file_oid_list:
         :param path:
         :type path: str or Path
         :return: result
         :rtype: bool
         """
-        result = False
 
         # パスがstrならpathlibにする
         p = Path(path) if isinstance(path, str) else path
 
         # パスが正しいか検証
         if not p.exists():
             raise FileNotFoundError
+        # ファイルが存在するか検証
+        if False in map(self.fs.exists, file_oid_list):
+            raise EdmanDbProcessError('指定のファイルはDBに存在しません')
+        else:
+            # ダウンロード処理
+            results = []
+            for file_oid in file_oid_list:
+                fs_out = self.fs.get(file_oid)
+                save_path = p / fs_out.filename
+                try:
+                    with save_path.open('wb') as f:
+                        tmp = fs_out.read()
+                        if hasattr(fs_out,
+                                   'compress') and fs_out.compress == 'gzip':
+                            tmp = gzip.decompress(tmp)
+                        f.write(tmp)
+                        f.flush()
+                        os.fsync(f.fileno())
+                except IOError:
+                    raise
+                results.append(save_path.exists())
+        return all(results)
+
+    def upload(self, collection: str, oid: Union[ObjectId, str],
+               file_path: Tuple[Tuple[Any, bool]], structure: str,
+               query=None) -> bool:
+        """
+        ドキュメントにファイルリファレンスを追加する
+        ファイルのインサート処理、圧縮処理なども行う
+        :param str collection:
+        :param oid:
+        :type oid: ObjectId or str
+        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパスと圧縮可否のタプル
+        :param str structure:
+        :param query:
+        :type query: list or None
+        :return:
+        :rtype: bool
+        """
+
+        oid = Utils.conv_objectid(oid)
+
+        # ドキュメント存在確認&対象ドキュメント取得
+        doc = self.db[collection].find_one({'_id': oid})
+        if doc is None:
+            raise EdmanInternalError('対象のドキュメントが存在しません')
+        if structure == 'emb':
+            # クエリーがドキュメントのキーとして存在するかチェック
+            if not Utils.query_check(query, doc):
+                raise EdmanFormatError('対象のドキュメントに対してクエリーが一致しません.')
 
-        # ダウンロード処理
-        if self.fs.exists(oid):
-            fs_out = self.fs.get(oid)
-            save_path = p / fs_out.filename
+        # ファイルのインサート
+        inserted_file_oids = self.grid_in(file_path)
+        if structure == 'ref':
+            new_doc = self.file_list_attachment(doc, inserted_file_oids)
+        elif structure == 'emb':
             try:
-                with save_path.open('wb') as f:
-                    tmp = fs_out.read()
-                    if hasattr(fs_out,
-                               'compress') and fs_out.compress == 'gzip':
-                        tmp = gzip.decompress(tmp)
-                    f.write(tmp)
-                    f.flush()
-                    os.fsync(f.fileno())
-            except IOError:
+                new_doc = Utils.doc_traverse(doc, inserted_file_oids, query,
+                                             self.file_list_attachment)
+            except Exception:
                 raise
+        else:
+            raise EdmanFormatError('構造はrefかembが必要です')
 
-            if save_path.exists():
-                result = True
+        # ドキュメント差し替え
+        replace_result = self.db[collection].replace_one({'_id': oid}, new_doc)
 
-        else:
-            raise EdmanDbProcessError('指定のファイルはDBに存在しません')
+        if replace_result.modified_count == 1:
+            return True
+        else:  # 差し替えができなかった時は添付ファイルは削除
+            self.fs_delete(inserted_file_oids)
+            return False
 
-        return result
+    def grid_in(self, files: Tuple[Tuple[Any, bool]]) -> list[Any]:
+        """
+        Gridfsへ複数のデータをアップロードし
+        compressに圧縮指定があればgzipで圧縮する
+
+        :param tuple files:
+        :return: inserted
+        :rtype: list
+        """
+        inserted = []
+        for file, compress in files:
+            try:
+                with file.open('rb') as f:
+                    fb = f.read()
+                    if compress:
+                        fb = gzip.compress(fb, compresslevel=self.comp_level)
+                        compress = 'gzip'
+                    else:
+                        compress = None
+                    metadata = {'filename': os.path.basename(f.name),
+                                'compress': compress}
+            except (IOError, OSError) as e:
+                raise EdmanDbProcessError(e)
+            try:
+                inserted.append(self.fs.put(fb, **metadata))
+            except GridFSError as e:
+                raise EdmanDbProcessError(e)
+        return inserted
 
     def file_list_attachment(self, doc: dict,
                              files_oid: List[ObjectId]) -> dict:
         """
         辞書データにファイルのoidを挿入する
         docにself.file_refがあれば、追加する処理
         oidが重複していないものだけ追加
@@ -386,15 +415,20 @@
                     try:
                         content = self.fs.get(file_ref)
                     except NoFile:
                         raise EdmanDbProcessError('指定の関連ファイルが存在しません')
                     except GridFSError:
                         raise
                     else:
-                        filepath = os.path.join(dir_path, content.name)
+                        # 圧縮設定の場合はその拡張子を追加
+                        if content.compress is not None:
+                            filename = content.name + '.' + content.compress
+                        else:
+                            filename = content.name
+                        filepath = os.path.join(dir_path, filename)
                     try:
                         with open(filepath, 'wb') as f:
                             f.write(content.read())
                     except (FileNotFoundError, IOError):
                         EdmanInternalError('ファイルを保存することが出来ませんでした')
                     except GridFSError:
                         raise
```

### Comparing `edman-2023.4.5/edman/json_manager.py` & `edman-2023.5.8/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman/search.py` & `edman-2023.5.8/edman/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,17 +134,14 @@
         result = None
         try:
             docs = list(self.connected_db[collection].find(query))
         except errors.OperationFailure:
             raise EdmanDbProcessError('ドキュメントが取得できませんでした')
         else:
             if len(docs):
-                # 複数ドキュメントの場合は選択処理へ
-                # doc = docs[0] if len(docs) == 1 else self._self_data_select(docs)
-                # result = {collection: docs[0]}
                 result = {collection: docs[0]}
         return result
 
     def _get_parent(self, self_doc: dict, depth: int) -> Union[dict, None]:
         """
         | 親となるドキュメントを取得
         | depthで深度を設定し、階層分取得する
```

### Comparing `edman-2023.4.5/edman/utils.py` & `edman-2023.5.8/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/edman.egg-info/PKG-INFO` & `edman-2023.5.8/edman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.4.5
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Home-page: https://github.com/ryde/edman
 Author: Masaki Ohno
 Author-email: masakio@post.kek.jp
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
```

### Comparing `edman-2023.4.5/setup.cfg` & `edman-2023.5.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edman
-version = 2023.4.5
+version = 2023.5.8
 author = Masaki Ohno
 author_email = masakio@post.kek.jp
 license = MIT License
 description = KEK IMSS SBRC/PF Experimental Data Management System
 url = https://github.com/ryde/edman
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `edman-2023.4.5/tests/test_convert.py` & `edman-2023.5.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/tests/test_db.py` & `edman-2023.5.8/tests/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,32 @@
         self.date = self.config.date
         self.file = self.config.file
 
     # def tearDown(self):
     #     # DB破棄
     #     pass
 
+    @staticmethod
+    def make_txt_files(dir_path, name='file_dl_list', suffix='.txt',
+                       text='test', qty=1):
+        # 添付ファイル用テキストファイル作成
+        p = Path(dir_path)
+        if qty == 1:
+            filename = name + suffix
+            save_path = p / filename
+            with save_path.open('w') as f:
+                f.write(text)
+        else:
+            for i in range(qty):
+                filename = name + str(i) + suffix
+                save_path = p / filename
+                with save_path.open('w') as f:
+                    f.write(text + str(i))
+        return sorted(p.glob(name + '*' + suffix))
+
     def test_insert(self):
         if not self.db_server_connect:
             return
 
         data = [
             {'collection1': [
                 {'name': 'IBM 5100', 'value': 100},
@@ -1229,47 +1247,31 @@
                 ],
                 'type': 'R'
             }
         }
         convert = Convert()
         converted_edman = convert.dict_to_edman(data, mode='ref')
         inserted_report = self.db.insert(converted_edman)
-        # print('inserted_report', inserted_report)
 
         target_collection = 'st2'
-        # ファイルリファレンスをアタッチ
         file = File(self.testdb)
         attached_file_oid = inserted_report[0]['engine'][0]
-        # print('file_oid', file_oid)
 
         with tempfile.TemporaryDirectory() as tmp_dir:
-            p = Path(tmp_dir)
-            filename_list = []
-            name = 'file_ref.txt'
-            filename_list.append(name)
-            save_path = p / name
-            with save_path.open('w') as f:
-                test_var = 'test ref'
-                f.write(test_var)
-                # ここはfileクラスのメソッドは利用せずにgridfsでインサートしたほうが良いかも？
-                file.add_file_reference('engine', attached_file_oid,
-                                        (save_path,),
-                                        'ref')
+            p_files = self.make_txt_files(tmp_dir, name='file_ref',text='test ref')
+            for p_file in p_files:
+                file.upload('engine', attached_file_oid,((p_file,False),),'ref')
 
         oid = inserted_report[1][target_collection][1]
-        # print(target_collection, oid)
         new_collection = 'new_collection'
         actual = self.db.structure(target_collection, oid,
                                    structure_mode='emb',
                                    new_collection=new_collection)
-        # print('actual', actual)
         find_result = self.testdb[new_collection].find_one(
             {'_id': actual[0][new_collection][0]})
-        # print('find_result', find_result['engine'][0])
-
         self.assertTrue(
             True if self.file in find_result['engine'][0] else False)
 
         # _ed_fileとidを除いたデータが入力値と一致するか
         del find_result['engine'][0][self.file]
         del find_result['_id']
         self.assertEqual(data['sample']['st2'][1], find_result)
@@ -1280,15 +1282,14 @@
                 'name': 'NSX',
                 'power': 280
             }
         }
         convert = Convert()
         converted_edman = convert.dict_to_edman(data, mode='ref')
         inserted_report = self.db.insert(converted_edman)
-        # print(inserted_report)
         oid = inserted_report[0]['sample'][0]
         new_collection = 'new_collection'
         actual = self.db.structure('sample', oid,
                                    structure_mode='emb',
                                    new_collection=new_collection)
         # print(actual)
         find_result = self.testdb[new_collection].find_one(
@@ -1322,27 +1323,23 @@
         converted_edman = convert.dict_to_edman(data, mode='emb')
         inserted_report = self.db.insert(converted_edman)
         oid = inserted_report[0]['sample2'][0]
         new_collection = 'new_collection'
         actual = self.db.structure('sample2', oid,
                                    structure_mode='ref',
                                    new_collection=new_collection)
-        # print('actual', actual)
         actual2 = self.db.structure('new_collection',
                                     actual[0]['new_collection'][0],
                                     structure_mode='emb',
                                     new_collection='new_collection2')
-        # print('actual2', actual2)
 
         result = self.testdb['new_collection2'].find_one(
             {'_id': actual2[0]['new_collection2'][0]})
         del result['_id']
         self.assertDictEqual(result, data['sample2'])
-        # print(result)
-        # print(data['sample2'])
 
     def test_get_child_all(self):
         if not self.db_server_connect:
             return
 
         db = self.client[self.test_ini['db']]
         parent_id = ObjectId()
```

### Comparing `edman-2023.4.5/tests/test_file.py` & `edman-2023.5.8/tests/test_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,232 +123,14 @@
             actual = []
             # files = tuple(sorted(p.glob('gen_test*.txt')))
             for idx, f in enumerate(self.file.file_gen(tuple(files))):
                 filename, filedata = f
                 actual.append((filename, filedata.decode()))
             self.assertListEqual(sorted(actual), sorted(expected))
 
-    def test_add_file_reference(self):
-        if not self.db_server_connect:
-            return
-
-        # refの場合
-        # refデータ入力
-        ref_json = {
-            "structure_1": [
-                {
-                    "position": "top",
-                    "username": "ryde",
-                    "structure_2": [
-                        {
-                            "maker": "Ferrari",
-                            "carname": "F355",
-                            "power": 380,
-                            "float_val": 4453.456
-                        },
-                        {
-                            "maker": "HONDA",
-                            "carname": "NSX",
-                            "power": 280,
-                            "float_val": 321.56,
-                            "start_date": {"#date": "1981-04-23"},
-                            "structure_3_1": [
-                                {
-                                    "filename": "test1.txt",
-                                    "name": "添付ファイル1"
-                                },
-                                {
-                                    "filename": "test2.txt",
-                                    "name": "添付ファイル2"
-                                }
-                            ],
-                            "structure_3_2": [
-                                {
-                                    "filename": "test3.txt",
-                                    "name": "添付ファイル3",
-                                    "structure_4": {
-                                        "filename": "test4.txt",
-                                        "name": "添付ファイル4",
-                                        "structure_5": [
-                                            {
-                                                "url": "example2.com",
-                                                "name": "テストURL2"
-                                            },
-                                            {
-                                                "url": "example3.com",
-                                                "name": "テストURL3"
-                                            }
-                                        ]
-                                    },
-                                    "structure_6": [
-                                        {
-                                            "url": "example_x.com",
-                                            "name": "テストURL_x"
-                                        },
-                                        {
-                                            "url": "example_y.com",
-                                            "name": "テストURL_y"
-                                        }
-                                    ],
-                                    "structure_5": {
-                                        "url": "example.com",
-                                        "name": "テストURL1",
-                                        "structure_5": {
-                                            "url": "example4.com",
-                                            "name": "テストURL4"
-                                        }
-                                    }
-                                }
-                            ]
-                        }
-                    ]
-                }
-            ]
-        }
-        convert = Convert()
-        converted_edman = convert.dict_to_edman(ref_json, mode='ref')
-        insert_result = self.db.insert(converted_edman)
-
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            files = self.make_txt_files(tmp_dir, name='insert_file_ref_test',
-                                        qty=2)
-            expected = []
-            for file_path in files:
-                with file_path.open() as f:
-                    expected.append((file_path.name, f.read()))
-
-            # メソッド実行
-            collection = 'structure_5'
-            oid = [i[collection][0] for i in insert_result if collection in i][
-                0]
-            insert_file_result = self.file.add_file_reference(collection, oid,
-                                                              tuple(files),
-                                                              'ref',
-                                                              compress=True)
-
-            # DBからデータ取得
-            query = {'_id': oid}
-            result = self.testdb[collection].find_one(query)
-
-            # 取得したデータからgridfsのファイルを取得
-            actual = []
-            self.fs = gridfs.GridFS(self.testdb)
-            for file_oid in result[self.config.file]:
-                data = self.fs.get(file_oid)
-                d = data.read()
-                if hasattr(data, 'compress') and data.compress == 'gzip':
-                    d = gzip.decompress(d)
-                actual.append((data.filename, d.decode()))
-
-            # テスト
-            self.assertTrue(insert_file_result)
-            self.assertListEqual(sorted(actual), sorted(expected))
-
-        # embの場合
-        data = {
-            "position": "top",
-            "structure_2": [
-                {
-                    "maker": "Ferrari",
-                    "carname": "F355",
-                    "power": 380,
-                    "float_val": 4453.456
-                },
-                {
-                    "maker": "HONDA",
-                    "carname": "NSX",
-                    "power": 280,
-                    "float_val": 321.56,
-                    "structure_3_1": [
-                        {
-                            "filename": "test1.txt",
-                            "name": "添付ファイル1"
-                        },
-                        {
-                            "filename": "test2.txt",
-                            "name": "添付ファイル2"
-                        }
-                    ],
-                    "structure_3_2": [
-                        {
-                            "filename": "test3.txt",
-                            "name": "添付ファイル3",
-                            "structure_4": {
-                                "filename": "test4.txt",
-                                "name": "添付ファイル4",
-                                "structure_5": [
-                                    {
-                                        "url": "example2.com",
-                                        "name": "テストURL2"
-                                    },
-                                    {
-                                        "url": "example3.com",
-                                        "name": "テストURL3"
-                                    }
-                                ]
-                            },
-                            "structure_6": [
-                                {
-                                    "url": "example_x.com",
-                                    "name": "テストURL_x"
-                                },
-                                {
-                                    "url": "example_y.com",
-                                    "name": "テストURL_y"
-                                }
-                            ],
-                            "structure_5": {
-                                "url": "example.com",
-                                "name": "テストURL1",
-                                "structure_5": {
-                                    "url": "example4.com",
-                                    "name": "テストURL4"
-                                }
-                            }
-                        }
-                    ]
-                }
-            ]
-        }
-        insert_result = self.testdb['structure_emb'].insert_one(data)
-
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            files_obj = self.make_txt_files(tmp_dir, name='emb_test', qty=2)
-            expected = []
-            for file_path in files_obj:
-                with file_path.open() as f:
-                    expected.append(f.read())
-
-            collection = 'structure_emb'
-            oid = insert_result.inserted_id
-            query = ['structure_2', '1']
-
-            # メソッド実行
-            insert_file_emb_result = self.file.add_file_reference(
-                collection, oid, tuple(files_obj), 'emb', query, compress=True)
-            # ドキュメントをfindして出す
-            result = self.testdb[collection].find_one({'_id': oid})
-
-            # gridfsからデータ取得
-            out_data = []
-            self.fs = gridfs.GridFS(self.testdb)
-            for oid in result['structure_2'][1][self.config.file]:
-                data = self.fs.get(oid)
-                f_data = data.read()
-                if hasattr(data, 'compress') and data.compress == 'gzip':
-                    f_data = gzip.decompress(f_data)
-
-                out_data.append(f_data.decode())
-
-            # DBデータとファイルのデータに差異はないか
-            self.assertListEqual(sorted(expected), sorted(out_data))
-
-            # メソッド成功時のフラグ
-            self.assertTrue(insert_file_emb_result)
-
     def test_file_list_attachment(self):
 
         # _ed_fileがなかった場合
         doc = {'name': 'NSX', 'ddd': 'aaa'}
         files_oid = [ObjectId(), ObjectId()]
         actual = self.file.file_list_attachment(doc, files_oid)
         expected = {'name': 'NSX', 'ddd': 'aaa', self.config.file: files_oid}
@@ -405,55 +187,14 @@
                         self.fs.put(f.read(), filename=str(i.name)))
 
             self.file.fs_delete(fs_oids)
             for i in fs_oids:
                 with self.subTest(i=i):
                     self.assertFalse(self.fs.exists(i))
 
-    def test_download(self):
-        if not self.db_server_connect:
-            return
-
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            files = self.make_txt_files(tmp_dir, name='file_dl', qty=2)
-
-            # ファイル読み込み、ファイルをgridfsに入れる
-            files_oid = []
-            self.fs = gridfs.GridFS(self.testdb)
-            test_vars = {}
-            for filename in files:
-                with filename.open('rb') as f:
-                    content = f.read()
-                    file_obj = gzip.compress(content, compresslevel=6)
-                    files_oid.append(
-                        self.fs.put(file_obj, filename=filename.name,
-                                    compress='gzip'))
-                    test_vars.update({filename.name: content.decode()})
-            files_list_dic = dict(zip(files_oid, [i.name for i in files]))
-
-        with tempfile.TemporaryDirectory() as tmp_dl_dir:
-            path = Path(tmp_dl_dir)
-
-            # 正常テスト
-            expected = {}
-            for oid, file_name in files_list_dic.items():
-                if self.file.download(oid, path):
-                    if path.exists():
-                        expected.update({oid: file_name})
-            self.assertDictEqual(files_list_dic, expected)
-
-            # files_list_dicファイルの中身が同じかテスト
-            for name, txt in test_vars.items():
-                dl_path = path / name
-                with dl_path.open('rb') as f:
-                    raw_data = f.read()
-                    dl_data = raw_data.decode()
-                    with self.subTest(name=name):
-                        self.assertEqual(dl_data, txt)
-
     def test_get_file_names(self):
         if not self.db_server_connect:
             return
 
         with tempfile.TemporaryDirectory() as tmp_dir:
             files = self.make_txt_files(tmp_dir, name='file_names', qty=2)
 
@@ -730,17 +471,17 @@
             file_dl_list = self.make_txt_files(tmp_dl_dir, name=input_filename,
                                                text=test_var)
 
             # ファイル読み込み、ファイルをgridfsに入れる
             files_oid = []
             self.fs = gridfs.GridFS(self.testdb)
             for filename in file_dl_list:
+                metadata = {'filename': filename.name, 'compress': None}
                 with filename.open('rb') as f:
-                    files_oid.append(
-                        self.fs.put(f.read(), filename=filename.name))
+                    files_oid.append(self.fs.put(f.read(), **metadata))
 
             # docをDBに入れる
             parent_id = ObjectId()
             doc_id = ObjectId()
             child_id = ObjectId()
             parent_col = 'parent_col'
             doc_col = 'doc_col'
@@ -818,26 +559,20 @@
     def test_get_fileref_and_generate_dl_list(self):
 
         if not self.db_server_connect:
             return
 
         # DBにdocsと添付ファイルを挿入する
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
-            p = Path(tmp_dl_dir)
-            filename_list = []
             name = 'file_dl_list.txt'
-            filename_list.append(name)
-            save_path = p / name
-            with save_path.open('w') as f:
-                test_var = 'test'
-                f.write(test_var)
             # ファイル読み込み、ファイルをgridfsに入れる
             files_oid = []
             self.fs = gridfs.GridFS(self.testdb)
-            for filename in sorted(p.glob('file_dl_list*.txt')):
+            input_filename = os.path.splitext(os.path.basename(name))[0]
+            for filename in self.make_txt_files(tmp_dl_dir, input_filename):
                 with filename.open('rb') as f:
                     files_oid.append(
                         self.fs.put(f.read(), filename=filename.name))
             # docをDBに入れる
             child_oid = ObjectId()
             doc = {'name': 'test1',
                    self.config.file: files_oid,
@@ -887,7 +622,292 @@
         filename = 2545
         now = datetime.datetime.now()
         name = now.strftime('%Y%m%d%H%M%S')
         filename_str = str(filename)
         expected = name + filename_str + '.zip'
         actual = self.file.generate_zip_filename(filename)
         self.assertEqual(expected, actual)
+
+    def test_grid_out(self):
+        if not self.db_server_connect:
+            return
+
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            files = self.make_txt_files(tmp_dir, name='file_dl', qty=2)
+
+            # ファイル読み込み、ファイルをgridfsに入れる
+            files_oid = []
+            self.fs = gridfs.GridFS(self.testdb)
+            test_vars = {}
+            for filename in files:
+                with filename.open('rb') as f:
+                    content = f.read()
+                    file_obj = gzip.compress(content, compresslevel=6)
+                    files_oid.append(
+                        self.fs.put(file_obj, filename=filename.name,
+                                    compress='gzip'))
+                    test_vars.update({filename.name: content.decode()})
+
+        with tempfile.TemporaryDirectory() as tmp_dl_dir:
+            path = Path(tmp_dl_dir)
+
+            grid_out_result = self.file._grid_out(files_oid, tmp_dl_dir)
+            # 実行結果
+            self.assertTrue(grid_out_result)
+
+            # DB送信前のファイル名＆ファイルの中身と、ダウンロード後のファイル名&ファイルの中身を比較する
+            expected = {}
+            for dl_file in path.glob('*.txt'):
+                with dl_file.open() as f:
+                    expected.update({dl_file.name: f.read()})
+            self.assertDictEqual(test_vars, expected)
+
+    def test_upload(self):
+        if not self.db_server_connect:
+            return
+
+        # refの場合
+        # refデータ入力
+        ref_json = {
+            "structure_1": [
+                {
+                    "position": "top",
+                    "username": "ryde",
+                    "structure_2": [
+                        {
+                            "maker": "Ferrari",
+                            "carname": "F355",
+                            "power": 380,
+                            "float_val": 4453.456
+                        },
+                        {
+                            "maker": "HONDA",
+                            "carname": "NSX",
+                            "power": 280,
+                            "float_val": 321.56,
+                            "start_date": {"#date": "1981-04-23"},
+                            "structure_3_1": [
+                                {
+                                    "filename": "test1.txt",
+                                    "name": "添付ファイル1"
+                                },
+                                {
+                                    "filename": "test2.txt",
+                                    "name": "添付ファイル2"
+                                }
+                            ],
+                            "structure_3_2": [
+                                {
+                                    "filename": "test3.txt",
+                                    "name": "添付ファイル3",
+                                    "structure_4": {
+                                        "filename": "test4.txt",
+                                        "name": "添付ファイル4",
+                                        "structure_5": [
+                                            {
+                                                "url": "example2.com",
+                                                "name": "テストURL2"
+                                            },
+                                            {
+                                                "url": "example3.com",
+                                                "name": "テストURL3"
+                                            }
+                                        ]
+                                    },
+                                    "structure_6": [
+                                        {
+                                            "url": "example_x.com",
+                                            "name": "テストURL_x"
+                                        },
+                                        {
+                                            "url": "example_y.com",
+                                            "name": "テストURL_y"
+                                        }
+                                    ],
+                                    "structure_5": {
+                                        "url": "example.com",
+                                        "name": "テストURL1",
+                                        "structure_5": {
+                                            "url": "example4.com",
+                                            "name": "テストURL4"
+                                        }
+                                    }
+                                }
+                            ]
+                        }
+                    ]
+                }
+            ]
+        }
+        convert = Convert()
+        converted_edman = convert.dict_to_edman(ref_json, mode='ref')
+        insert_result = self.db.insert(converted_edman)
+
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            files = self.make_txt_files(tmp_dir, name='insert_file_ref_test',
+                                        qty=2)
+            expected = []
+            for file_path in files:
+                with file_path.open() as f:
+                    expected.append((file_path.name, f.read()))
+
+            # メソッド実行
+            collection = 'structure_5'
+            oid = [i[collection][0] for i in insert_result if collection in i][
+                0]
+            p_files = tuple([(i, True) for i in files])
+            insert_file_result = self.file.upload(collection, oid,
+                                                  p_files,
+                                                  'ref')
+
+            # DBからデータ取得
+            query = {'_id': oid}
+            result = self.testdb[collection].find_one(query)
+
+            # 取得したデータからgridfsのファイルを取得
+            actual = []
+            self.fs = gridfs.GridFS(self.testdb)
+            for file_oid in result[self.config.file]:
+                data = self.fs.get(file_oid)
+                d = data.read()
+                if hasattr(data, 'compress') and data.compress == 'gzip':
+                    d = gzip.decompress(d)
+                actual.append((data.filename, d.decode()))
+
+            # テスト
+            self.assertTrue(insert_file_result)
+            self.assertListEqual(sorted(actual), sorted(expected))
+
+        # embの場合
+        data = {
+            "position": "top",
+            "structure_2": [
+                {
+                    "maker": "Ferrari",
+                    "carname": "F355",
+                    "power": 380,
+                    "float_val": 4453.456
+                },
+                {
+                    "maker": "HONDA",
+                    "carname": "NSX",
+                    "power": 280,
+                    "float_val": 321.56,
+                    "structure_3_1": [
+                        {
+                            "filename": "test1.txt",
+                            "name": "添付ファイル1"
+                        },
+                        {
+                            "filename": "test2.txt",
+                            "name": "添付ファイル2"
+                        }
+                    ],
+                    "structure_3_2": [
+                        {
+                            "filename": "test3.txt",
+                            "name": "添付ファイル3",
+                            "structure_4": {
+                                "filename": "test4.txt",
+                                "name": "添付ファイル4",
+                                "structure_5": [
+                                    {
+                                        "url": "example2.com",
+                                        "name": "テストURL2"
+                                    },
+                                    {
+                                        "url": "example3.com",
+                                        "name": "テストURL3"
+                                    }
+                                ]
+                            },
+                            "structure_6": [
+                                {
+                                    "url": "example_x.com",
+                                    "name": "テストURL_x"
+                                },
+                                {
+                                    "url": "example_y.com",
+                                    "name": "テストURL_y"
+                                }
+                            ],
+                            "structure_5": {
+                                "url": "example.com",
+                                "name": "テストURL1",
+                                "structure_5": {
+                                    "url": "example4.com",
+                                    "name": "テストURL4"
+                                }
+                            }
+                        }
+                    ]
+                }
+            ]
+        }
+        insert_result = self.testdb['structure_emb'].insert_one(data)
+
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            files_obj = self.make_txt_files(tmp_dir, name='emb_test', qty=2)
+            expected = []
+            for file_path in files_obj:
+                with file_path.open() as f:
+                    expected.append(f.read())
+
+            collection = 'structure_emb'
+            oid = insert_result.inserted_id
+            query = ['structure_2', '1']
+
+            files_obj2 = tuple([(i, True) for i in files_obj])
+            # メソッド実行
+            insert_file_emb_result = self.file.upload(
+                collection, oid, files_obj2, 'emb', query)
+
+            # ドキュメントをfindして出す
+            result = self.testdb[collection].find_one({'_id': oid})
+
+            # gridfsからデータ取得
+            out_data = []
+            self.fs = gridfs.GridFS(self.testdb)
+            for oid in result['structure_2'][1][self.config.file]:
+                data = self.fs.get(oid)
+                f_data = data.read()
+                if hasattr(data, 'compress') and data.compress == 'gzip':
+                    f_data = gzip.decompress(f_data)
+
+                out_data.append(f_data.decode())
+
+            # DBデータとファイルのデータに差異はないか
+            self.assertListEqual(sorted(expected), sorted(out_data))
+
+            # メソッド成功時のフラグ
+            self.assertTrue(insert_file_emb_result)
+
+    def test_grid_in(self):
+        if not self.db_server_connect:
+            return
+
+        # 正常系
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            sample_files = self.make_txt_files(tmp_dir, name='grid_in_test',
+                                               qty=2)
+            compress_settings = [True, False]
+            td = tuple(
+                [(p, b) for (p, b) in zip(sample_files, compress_settings)])
+
+            self.fs = gridfs.GridFS(self.testdb)
+            actual = []
+            for oid in self.file.grid_in(td):
+                data = self.fs.get(oid)
+                if data.compress == 'gzip':
+                    f_data = gzip.decompress(data.read()).decode()
+                    b_data = True
+                else:
+                    f_data = data.read().decode()
+                    b_data = False
+                actual.append([data.filename, f_data, b_data])
+
+            expected = []
+            for file_path, compress in zip(sample_files, compress_settings):
+                with file_path.open() as f:
+                    expected.append([file_path.name, f.read(), compress])
+
+            self.assertListEqual(sorted(actual), sorted(expected))
```

### Comparing `edman-2023.4.5/tests/test_multiuser.py` & `edman-2023.5.8/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/tests/test_search.py` & `edman-2023.5.8/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.4.5/tests/test_utils.py` & `edman-2023.5.8/tests/test_utils.py`

 * *Files identical despite different names*

