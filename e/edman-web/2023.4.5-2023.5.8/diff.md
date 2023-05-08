# Comparing `tmp/edman_web-2023.4.5.tar.gz` & `tmp/edman_web-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2023.4.5.tar", last modified: Wed Apr  5 05:26:27 2023, max compression
+gzip compressed data, was "edman_web-2023.5.8.tar", last modified: Mon May  8 04:41:52 2023, max compression
```

## Comparing `edman_web-2023.4.5.tar` & `edman_web-2023.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.4.5/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2023-03-29 09:20:48.000000 edman_web-2023.4.5/MANIFEST.in
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-04-05 05:26:27.278967 edman_web-2023.4.5/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.4.5/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.4.5/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5632 2023-04-04 05:55:42.000000 edman_web-2023.4.5/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.4.5/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      349 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       61 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       10 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      713 2023-04-05 05:26:27.278967 edman_web-2023.4.5/setup.cfg
--rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2023-03-29 09:20:48.000000 edman_web-2023.4.5/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12368 2023-04-04 05:55:42.000000 edman_web-2023.4.5/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.4.5/tests/test_search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2023-03-29 09:20:48.000000 edman_web-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-05-08 04:41:52.696269 edman_web-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.5.8/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6477 2023-05-08 04:40:18.000000 edman_web-2023.5.8/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.5.8/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      349 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       61 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       10 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      713 2023-05-08 04:41:52.696269 edman_web-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2023-03-29 09:20:48.000000 edman_web-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13863 2023-04-25 08:38:11.000000 edman_web-2023.5.8/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.5.8/tests/test_search_manager.py
```

### Comparing `edman_web-2023.4.5/LICENSE.txt` & `edman_web-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.5/PKG-INFO` & `edman_web-2023.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2023.4.5
+Version: 2023.5.8
 Summary: sub-package of edman for web applications.
 Home-page: https://github.com/ryde/edman_web
 Author: Masaki Ohno
 Author-email: masakio@post.kek.jp
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
```

### Comparing `edman_web-2023.4.5/README.rst` & `edman_web-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.5/edman_web/file_manager.py` & `edman_web-2023.5.8/edman_web/file_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,93 @@
 import os
 import base64
-from typing import Union, List, Tuple
+import gzip
+from typing import Union, List, Tuple, Any
 from io import BytesIO
 from werkzeug.datastructures import FileStorage
 from bson import ObjectId
 from PIL import Image as PILImage
 from gridfs.errors import GridFSError
 from edman import File, Config
 from edman.utils import Utils
 from edman.exceptions import EdmanDbProcessError, EdmanInternalError
 
 
 class FileManager(File):
     def __init__(self, db=None):
         super().__init__(db)
 
-    def upload(self, up_file: FileStorage, collection: str,
-               oid: Union[str, ObjectId]) -> None:
+    def web_upload(self, collection: str, oid: Union[str, ObjectId],
+                   up_file: FileStorage, compress=False) -> None:
         """
         ファイルアップロード処理
 
-        :param FileStorage up_file:
         :param str collection:
         :param str or ObjectId oid:
+        :param FileStorage up_file:
+        :param bool compress:
         :return:
         """
         oid = Utils.conv_objectid(oid)
 
         # ドキュメント存在確認&対象ドキュメント取得
         if (doc := self.db[collection].find_one({'_id': oid})) is None:
             raise EdmanDbProcessError('対象のドキュメントが存在しません')
 
-        # gridfsにファイルを入れる
-        metadata = {'filename': up_file.filename}
         try:
-            st = BytesIO(up_file.stream.read())
-            file_oid = self.fs.put(st, **metadata)
-        except GridFSError:
+            # gridfsにファイルを入れる
+            inserted_file_oids = self.web_grid_in(up_file, compress)
+        except EdmanDbProcessError as e:
+            raise e
+        else:  # ドキュメントの更新
+            try:
+                new_doc = self.file_list_attachment(doc, inserted_file_oids)
+                replace_result = self.db[collection].replace_one({'_id': oid},
+                                                                 new_doc)
+                if replace_result.modified_count != 1:
+                    # ドキュメントが更新されていない場合はgridfsからデータを削除する
+                    self.fs_delete(inserted_file_oids)
+                    raise EdmanDbProcessError('ドキュメントの更新ができませんでした.')
+            except Exception as e:
+                # 途中で例外が起きた場合、gridfsからデータを削除する
+                self.fs_delete(inserted_file_oids)
+                raise EdmanDbProcessError(str(e))
+
+    def web_grid_in(self, file: FileStorage, compress: bool) -> list[Any]:
+        """
+        Gridfsへデータをアップロードし
+        compressに圧縮指定があればgzipで圧縮する
+
+        :param FileStorage file:
+        :param bool compress:
+        :return: inserted
+        :rtype: list
+        """
+        inserted = []
+
+        try:
+            f = file.stream.read()
+            if compress:
+                f = gzip.compress(f, compresslevel=self.comp_level)
+                compress_type = 'gzip'
+            else:
+                compress_type = None
+
+            metadata = {'filename': file.filename, 'compress': compress_type}
+
+        except OSError:
             raise EdmanDbProcessError('DBにファイルをアップロード出来ませんでした')
         except Exception:
             raise
 
-        # ドキュメントの更新
         try:
-            new_doc = self.file_list_attachment(doc, [file_oid])
-            replace_result = self.db[collection].replace_one({'_id': oid},
-                                                             new_doc)
-            if replace_result.modified_count != 1:
-                # ドキュメントが更新されていない場合はgridfsからデータを削除する
-                self.fs_delete([file_oid])
-                raise EdmanDbProcessError(
-                    'ドキュメントの更新ができませんでした.ファイルは削除されています')
-        except Exception:
-            # 途中で例外が起きた場合、gridfsからデータを削除する
-            self.fs_delete([file_oid])
-            raise EdmanDbProcessError('ドキュメントの更新ができませんでした.ファイルは削除されています')
+            inserted.append(self.fs.put(f, **metadata))
+        except GridFSError as e:
+            raise EdmanDbProcessError(e)
+        return inserted
 
     def file_delete(self, collection: str, oid: Union[str, ObjectId],
                     delete_list: List[str]):
         """
         edmanからファイルを削除する
 
         :param str collection:
```

### Comparing `edman_web-2023.4.5/edman_web/search_manager.py` & `edman_web-2023.5.8/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.5/edman_web.egg-info/PKG-INFO` & `edman_web-2023.5.8/edman_web.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman-web
-Version: 2023.4.5
+Version: 2023.5.8
 Summary: sub-package of edman for web applications.
 Home-page: https://github.com/ryde/edman_web
 Author: Masaki Ohno
 Author-email: masakio@post.kek.jp
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
```

### Comparing `edman_web-2023.4.5/setup.cfg` & `edman_web-2023.5.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edman_web
-version = 2023.4.5
+version = 2023.5.8
 author = Masaki Ohno
 author_email = masakio@post.kek.jp
 license = MIT License
 description = sub-package of edman for web applications.
 url = https://github.com/ryde/edman_web
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -16,16 +16,16 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.11
 install_requires = 
 	pymongo>=4.3.3
-	edman>=2023.4.5
-	Werkzeug>=2.2.3
+	edman>=2023.5.8
+	Werkzeug>=2.3.3
 	Pillow>=9.5.0
 
 [options.packages.find]
 exclude = 
 	tests
 
 [egg_info]
```

### Comparing `edman_web-2023.4.5/tests/test_file_manager.py` & `edman_web-2023.5.8/tests/test_file_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import configparser
 from pathlib import Path
 import tempfile
 import base64
 import os
+import gzip
 from io import BytesIO
 from unittest import TestCase
 from PIL import Image
 from pymongo import errors as py_errors, MongoClient
 from bson import ObjectId, DBRef
 import gridfs
 from werkzeug.datastructures import FileStorage
@@ -264,21 +265,21 @@
 
             expected = [files_oid.pop(0)]
             self.file_manager.file_delete(doc_col, doc_id, files_oid)
             target_doc = self.testdb[doc_col].find_one({'_id': doc_id})
             actual = target_doc[Config.file]
             self.assertListEqual(expected, actual)
 
-    def test_upload(self):
+    def test_web_upload(self):
         if not self.db_server_connect:
             return
 
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
             p = Path(tmp_dl_dir)
-            for filename in  self.make_txt_files(p, 'file_dl_list'):
+            for filename in self.make_txt_files(p, 'file_dl_list'):
                 with filename.open('rb') as f:
                     content = f.read()
                     content_name = os.path.basename(f.name)
 
             # ドキュメントのインサート
             parent_id = ObjectId()
             doc_id = ObjectId()
@@ -316,19 +317,55 @@
                 _ = self.testdb[i['col']].insert_one(i['doc'])
 
             st = FileStorage(stream=BytesIO(content), filename=content_name)
             # t = st.stream.read()
             # self.assertEquals(t, content)
 
             # 実行
-            self.file_manager.upload(st, doc_col, doc_id)
+            self.file_manager.web_upload(doc_col, doc_id, st)
 
             # アップロードしたデータを取得する
-            d = self.testdb[doc_col].find_one({'_id':doc_id})
+            d = self.testdb[doc_col].find_one({'_id': doc_id})
             upload_file_oid = d[Config.file]
             fs = gridfs.GridFS(self.testdb)
             a = fs.get(upload_file_oid[0])
 
             # テスト
             actual = a.read()
             expected = content
-            self.assertEquals(expected, actual)
+            self.assertEqual(expected, actual)
+
+    def test_web_grid_in(self):
+
+        if not self.db_server_connect:
+            return
+
+        # 正常系
+        with tempfile.TemporaryDirectory() as tmp_dl_dir:
+            files = self.make_txt_files(tmp_dl_dir, 'web_grid_in', qty=2)
+
+            # ファイルが同一か否か
+            with files[0].open('rb') as f:
+                content = f.read()
+                st = FileStorage(stream=BytesIO(content),
+                                 filename=f.name)
+            self.fs = gridfs.GridFS(self.testdb)
+            inserted = self.file_manager.web_grid_in(st, compress=False)
+            a = self.fs.get(inserted[0])
+            actual = a.read().decode()
+            expected = content.decode()
+            self.assertEqual(expected, actual)
+
+            # 圧縮が効いているか否か
+            with files[1].open('rb') as f:
+                content = f.read()
+                st = FileStorage(stream=BytesIO(content),
+                                 filename=f.name)
+            inserted = self.file_manager.web_grid_in(st, compress=True)
+            b = self.fs.get(inserted[0])
+            if b.compress == 'gzip':
+                actual = gzip.decompress(b.read()).decode()
+            else:  # 現状compress指定は"gzip"かNoneのみ
+                actual = None
+            self.assertIsNotNone(b.compress)
+            expected = content.decode()
+            self.assertEqual(expected, actual)
```

### Comparing `edman_web-2023.4.5/tests/test_search_manager.py` & `edman_web-2023.5.8/tests/test_search_manager.py`

 * *Files identical despite different names*

