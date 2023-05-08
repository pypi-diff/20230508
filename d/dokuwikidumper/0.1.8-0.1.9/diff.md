# Comparing `tmp/dokuwikidumper-0.1.8.tar.gz` & `tmp/dokuwikidumper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dokuwikidumper-0.1.8.tar", max compression
+gzip compressed data, was "dokuwikidumper-0.1.9.tar", max compression
```

## Comparing `dokuwikidumper-0.1.8.tar` & `dokuwikidumper-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-02-14 14:44:04.142863 dokuwikidumper-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     7029 2023-04-13 08:43:03.808779 dokuwikidumper-0.1.8/README.md
--rw-r--r--   0        0        0       57 2023-02-16 17:41:45.629101 dokuwikidumper-0.1.8/dokuWikiDumper/__init__.py
--rw-r--r--   0        0        0       73 2023-03-13 09:45:13.311407 dokuwikidumper-0.1.8/dokuWikiDumper/__main__.py
--rw-r--r--   0        0        0       24 2023-04-13 08:15:56.104911 dokuwikidumper-0.1.8/dokuWikiDumper/__version__.py
--rw-r--r--   0        0        0     8138 2023-04-02 14:44:11.506070 dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/__init__.py
--rw-r--r--   0        0        0     7672 2023-03-30 16:00:51.487847 dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/revisions.py
--rw-r--r--   0        0        0     2863 2023-03-18 10:37:28.215096 dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/titles.py
--rw-r--r--   0        0        0     9267 2023-04-13 08:40:42.244757 dokuwikidumper-0.1.8/dokuWikiDumper/dump/dokuDumper.py
--rw-r--r--   0        0        0       27 2023-03-21 03:34:03.164081 dokuwikidumper-0.1.8/dokuWikiDumper/dump/html/__init__.py
--rw-r--r--   0        0        0     4067 2023-03-26 15:11:17.495346 dokuwikidumper-0.1.8/dokuWikiDumper/dump/html/html.py
--rw-r--r--   0        0        0      216 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiDumper/dump/info/__init__.py
--rw-r--r--   0        0        0     3325 2023-04-13 06:47:42.540273 dokuwikidumper-0.1.8/dokuWikiDumper/dump/info/info.py
--rw-r--r--   0        0        0       38 2023-02-18 16:00:58.611751 dokuwikidumper-0.1.8/dokuWikiDumper/dump/media/__init__.py
--rw-r--r--   0        0        0     5741 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiDumper/dump/media/media.py
--rw-r--r--   0        0        0       82 2023-03-26 14:53:46.352338 dokuwikidumper-0.1.8/dokuWikiDumper/dump/pdf/__init__.py
--rw-r--r--   0        0        0     4404 2023-03-26 17:20:10.040898 dokuwikidumper-0.1.8/dokuWikiDumper/dump/pdf/pdf.py
--rw-r--r--   0        0        0     1208 2023-03-26 09:59:17.227185 dokuwikidumper-0.1.8/dokuWikiDumper/exceptions.py
--rw-r--r--   0        0        0      756 2023-04-13 06:46:25.970991 dokuwikidumper-0.1.8/dokuWikiDumper/utils/config.py
--rw-r--r--   0        0        0     4259 2023-04-13 08:08:16.985223 dokuwikidumper-0.1.8/dokuWikiDumper/utils/session.py
--rw-r--r--   0        0        0     4248 2023-04-13 07:21:43.558449 dokuwikidumper-0.1.8/dokuWikiDumper/utils/util.py
--rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiUploader/__init__.py
--rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.8/dokuWikiUploader/__main__.py
--rw-r--r--   0        0        0       26 2023-04-13 08:16:05.381066 dokuwikidumper-0.1.8/dokuWikiUploader/__version__.py
--rw-r--r--   0        0        0     7264 2023-04-13 07:00:32.369164 dokuwikidumper-0.1.8/dokuWikiUploader/uploader.py
--rw-r--r--   0        0        0      845 2023-04-13 08:16:17.337266 dokuwikidumper-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8368 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.8/setup.py
--rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-14 14:44:04.142863 dokuwikidumper-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     7029 2023-04-20 06:37:15.718888 dokuwikidumper-0.1.9/README.md
+-rw-r--r--   0        0        0       57 2023-02-16 17:41:45.629101 dokuwikidumper-0.1.9/dokuWikiDumper/__init__.py
+-rw-r--r--   0        0        0       73 2023-03-13 09:45:13.311407 dokuwikidumper-0.1.9/dokuWikiDumper/__main__.py
+-rw-r--r--   0        0        0       24 2023-04-29 08:23:37.232310 dokuwikidumper-0.1.9/dokuWikiDumper/__version__.py
+-rw-r--r--   0        0        0     8138 2023-04-15 05:27:24.559455 dokuwikidumper-0.1.9/dokuWikiDumper/dump/content/__init__.py
+-rw-r--r--   0        0        0     7672 2023-04-20 06:41:40.356189 dokuwikidumper-0.1.9/dokuWikiDumper/dump/content/revisions.py
+-rw-r--r--   0        0        0     2946 2023-04-27 16:58:30.507594 dokuwikidumper-0.1.9/dokuWikiDumper/dump/content/titles.py
+-rw-r--r--   0        0        0     9432 2023-04-20 08:20:29.262962 dokuwikidumper-0.1.9/dokuWikiDumper/dump/dokuDumper.py
+-rw-r--r--   0        0        0       27 2023-03-21 03:34:03.164081 dokuwikidumper-0.1.9/dokuWikiDumper/dump/html/__init__.py
+-rw-r--r--   0        0        0     4067 2023-03-26 15:11:17.495346 dokuwikidumper-0.1.9/dokuWikiDumper/dump/html/html.py
+-rw-r--r--   0        0        0      216 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.9/dokuWikiDumper/dump/info/__init__.py
+-rw-r--r--   0        0        0     3325 2023-04-13 06:47:42.540273 dokuwikidumper-0.1.9/dokuWikiDumper/dump/info/info.py
+-rw-r--r--   0        0        0       38 2023-02-18 16:00:58.611751 dokuwikidumper-0.1.9/dokuWikiDumper/dump/media/__init__.py
+-rw-r--r--   0        0        0     5741 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.9/dokuWikiDumper/dump/media/media.py
+-rw-r--r--   0        0        0       82 2023-03-26 14:53:46.352338 dokuwikidumper-0.1.9/dokuWikiDumper/dump/pdf/__init__.py
+-rw-r--r--   0        0        0     4404 2023-03-26 17:20:10.040898 dokuwikidumper-0.1.9/dokuWikiDumper/dump/pdf/pdf.py
+-rw-r--r--   0        0        0     1208 2023-03-26 09:59:17.227185 dokuwikidumper-0.1.9/dokuWikiDumper/exceptions.py
+-rw-r--r--   0        0        0      756 2023-04-13 06:46:25.970991 dokuwikidumper-0.1.9/dokuWikiDumper/utils/config.py
+-rw-r--r--   0        0        0     4259 2023-04-20 06:33:47.222711 dokuwikidumper-0.1.9/dokuWikiDumper/utils/session.py
+-rw-r--r--   0        0        0     4248 2023-04-13 07:21:43.558449 dokuwikidumper-0.1.9/dokuWikiDumper/utils/util.py
+-rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.9/dokuWikiUploader/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-26 02:14:22.276942 dokuwikidumper-0.1.9/dokuWikiUploader/__main__.py
+-rw-r--r--   0        0        0       26 2023-04-29 08:23:38.528358 dokuwikidumper-0.1.9/dokuWikiUploader/__version__.py
+-rw-r--r--   0        0        0     7974 2023-04-29 08:20:07.548642 dokuwikidumper-0.1.9/dokuWikiUploader/uploader.py
+-rw-r--r--   0        0        0      845 2023-04-29 08:23:40.484429 dokuwikidumper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8368 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.9/setup.py
+-rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 dokuwikidumper-0.1.9/PKG-INFO
```

### Comparing `dokuwikidumper-0.1.8/LICENSE.md` & `dokuwikidumper-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/README.md` & `dokuwikidumper-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/__init__.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/content/__init__.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/revisions.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/content/revisions.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/content/titles.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/content/titles.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         return getTitlesOld(url, ns=None, session=session)
     soup = BeautifulSoup(r.text, 'lxml')
     for a in soup.findAll('a', href=True):
         if a.has_attr('title'):
             title = a['title']
         else:
             query = urlparse.parse_qs(urlparse.urlparse(a['href']).query)
+
+            if 'idx' not in query or 'id' not in query:
+                continue
+
             title = (query['idx' if 'idx' in query else 'id'])[0]
         if 'idx_dir' in a['class']:
             titles += getTitles(url=url, ns=title, session=session)
         else:
             titles.append(title)
     # time.sleep(1.5)
     print('%sFound %d title(s) in namespace %s' %
```

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/dokuDumper.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/dokuDumper.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,25 @@
 from dokuWikiDumper.utils.config import update_config
 from dokuWikiDumper.utils.session import createSession, load_cookies, login_dokuwiki
 from dokuWikiDumper.utils.util import avoidSites, buildBaseUrl, getDokuUrl, smkdirs, standardizeUrl, uopen, url2prefix
 
 
 def getArgumentParser():
     parser = argparse.ArgumentParser(description='dokuWikiDumper Version: '+ DUMPER_VERSION)
-    parser.add_argument('url', help='URL of the dokuWiki', type=str)
-    parser.add_argument('--content', action='store_true', help='Dump content')
-    parser.add_argument('--media', action='store_true', help='Dump media')
-    parser.add_argument('--html', action='store_true', help='Dump HTML')
-    parser.add_argument('--pdf', action='store_true',
+    parser.add_argument('url', help='URL of the dokuWiki (provide the doku.php URL)', type=str)
+
+    group_download = parser.add_argument_group("Data to download", "What info download from the wiki")
+
+    group_download.add_argument('--content', action='store_true', help='Dump content')
+    group_download.add_argument('--media', action='store_true', help='Dump media')
+    group_download.add_argument('--html', action='store_true', help='Dump HTML')
+    group_download.add_argument('--pdf', action='store_true',
                         help='Dump PDF [default: false] (Only available on some wikis with the PDF export plugin)'+
                         ' (Only dumps the latest PDF revision)')
+
     parser.add_argument('--current-only', dest='current_only', action='store_true',
                         help='Dump latest revision, no history [default: false] (only for HTML at the moment)')
     parser.add_argument(
         '--skip-to', help='!DEV! Skip to title number [default: 0]', type=int, default=0)
     parser.add_argument(
         '--path', help='Specify dump directory [default: <site>-<date>]', type=str, default='')
     parser.add_argument(
```

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/html/html.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/html/html.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/info/info.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/info/info.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/media/media.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/media/media.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/dump/pdf/pdf.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/dump/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/exceptions.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/exceptions.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/utils/config.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/utils/config.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/utils/session.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/utils/session.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiDumper/utils/util.py` & `dokuwikidumper-0.1.9/dokuWikiDumper/utils/util.py`

 * *Files identical despite different names*

### Comparing `dokuwikidumper-0.1.8/dokuWikiUploader/uploader.py` & `dokuwikidumper-0.1.9/dokuWikiUploader/uploader.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 from dokuWikiDumper.utils.util import url2prefix
 from dokuWikiDumper.dump.info import get_info
 from dokuWikiDumper.dump.info import INFO_WIKI_NAME, INFO_RAW_TITLE, INFO_DOKU_URL, INFO_LANG, INFO_ICON_URL
 from dokuWikiDumper.utils.config import get_config
 
 from .__version__ import UPLOADER_VERSION
 
-collection = 'opensource'
-# collection = 'test_collection'
+DEFAULT_COLLECTION = 'opensource'
+TEST_COLLECTION = 'test_collection' # items here are expected to be automatically removed after 30 days. 
+# (see <https://archive.org/details/test_collection?tab=about>)
+
 USER_AGENT = 'dokuWikiUploader/' + UPLOADER_VERSION
 
 UPLOADED_MARK = 'uploaded_to_IA.mark'
 
 
 def file_sha1(path):
     buffer = bytearray(65536)
@@ -94,15 +96,15 @@
                     "wikidump",
                     title,
                     url2prefix(info.get(INFO_DOKU_URL)),
                 ]
     # Item metadata
     md = {
         "mediatype": "web",
-        "collection": collection,
+        "collection": args.collection,
         "title": "Wiki - " + title,
         "description": description,
         "last-updated-date": time.strftime("%Y-%m-%d"),
         "subject": "; ".join(
             keywords
         ),  # Keywords should be separated by ; but it doesn't matter much; the alternative is to set one per field with subject[0], subject[1], ...
         "originalurl": info.get(INFO_DOKU_URL),
@@ -144,14 +146,21 @@
             metadata=md,
             access_key=access_key,
             secret_key=secret_key,
             verbose=True,
             queue_derive=False,
         )
 
+        tries = 20
+        while not item.exists and tries > 0:
+            print("Waiting for item to be created...", tries)
+            tries -= 1
+            time.sleep(10)
+            item = get_item(identifier_remote)
+
         item.modify_metadata(md)  # update
         print(
             "You can find it in https://archive.org/details/%s"
             % (identifier_remote)
         )
     except Exception as e:
         raise e
@@ -177,17 +186,21 @@
 def main(params=[]):
 
     parser = argparse.ArgumentParser(
         """dokuWikiUploader"""
     )
     parser.description = "Upload a DokuWiki dump to Internet Archive." + f" (Version: {UPLOADER_VERSION})."
     parser.add_argument("-kf", "--keysfile", default="~/.doku_uploader_ia_keys",
-                        help="Path to the IA S3 keys file. (first line: access key, second line: secret key) [default: ~/.doku_uploader_ia_keys]")
+                        help="Path to the IA S3 keys file. (first line: access key, second line: secret key)"
+                             " [default: ~/.doku_uploader_ia_keys]")
     parser.add_argument("-p7z", "--path7z", default="7z",
                         help="Path to 7z binary. [default: 7z]")
+    parser.add_argument("-c", "--collection", default=DEFAULT_COLLECTION, choices=[DEFAULT_COLLECTION, TEST_COLLECTION, "wikiteam"],
+                        help="Collection to upload to. ('test_collection' for testing (auto-delete after 30 days) "
+                             "[default: opensource]")
     parser.add_argument("dump_dir", help="Path to the wiki dump directory.")
     args = parser.parse_args()
 
     if os.path.exists(os.path.join(args.dump_dir, UPLOADED_MARK)):
         print("This dump has already been uploaded.")
         print("If you want to upload it again, please remove the file '%s'." % UPLOADED_MARK)
         return 0
```

### Comparing `dokuwikidumper-0.1.8/pyproject.toml` & `dokuwikidumper-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dokuWikiDumper"
-version = "0.1.8"
+version = "0.1.9"
 description = "A tool for archiving DokuWiki"
 authors = ["yzqzss <yzqzss@yandex.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 packages = [
     { include = "dokuWikiDumper/**/*" },
```

### Comparing `dokuwikidumper-0.1.8/setup.py` & `dokuwikidumper-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 entry_points = \
 {'console_scripts': ['dokuWikiDumper = dokuWikiDumper:main',
                      'dokuWikiUploader = dokuWikiUploader:main']}
 
 setup_kwargs = {
     'name': 'dokuwikidumper',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A tool for archiving DokuWiki',
     'long_description': '# DokuWiki Dumper\n\n> A tool for archiving DokuWiki.\n\nRecommend using `dokuWikiDumper` on _modern_ filesystems, such as `ext4` or `btrfs`. `NTFS` is not recommended because of it denys many special characters in filename.\n\n## Requirements\n\n### dokuWikiDumper\n\n- Python 3.8+ (developed on py3.10)\n- beautifulsoup4\n- requests\n- lxml\n- rich\n\n### dokuWikiUploader\n\n> Upload wiki dump to [Internet Archive](https://archive.org/).\n> `dokuWikiUploader -h` for help.\n\n- internetarchive\n- 7z (`7z` command)\n\n## Install `dokuWikiDumper`\n\n> `dokuWikiUploader` is included in `dokuWikiDumper`.\n\n### Install `dokuWikiDumper` with `pip` (recommended)\n\n> <https://pypi.org/project/dokuwikidumper/>\n\n```bash\npip3 install dokuWikiDumper\n```\n\n### Install `dokuWikiDumper` with `Poetry` (for developers)\n\n- Install `Poetry`\n\n    ```bash\n    pip3 install poetry\n    ```\n\n- Install `dokuWikiDumper`\n\n    ```bash\n    git clone https://github.com/saveweb/dokuwiki-dumper\n    cd dokuwiki-dumper\n    poetry install\n    rm dist/ -rf\n    poetry build\n    pip install --force-reinstall dist/dokuWikiDumper*.whl\n    ```\n\n## Usage\n\n```bash\nusage: dokuWikiDumper [-h] [--content] [--media] [--html] [--skip-to SKIP_TO] [--path PATH] [--no-resume] [--threads THREADS]\n                      [--insecure] [--ignore-errors] [--ignore-action-disabled-edit] [--username USERNAME] [--password PASSWORD]\n                      [--cookies COOKIES] [--auto]\n                      url\n\ndokuWikiDumper\n\npositional arguments:\n  url                   URL of the dokuWiki\n\noptions:\n  -h, --help            show this help message and exit\n  --content             Dump content\n  --media               Dump media\n  --html                Dump HTML\n  --pdf                 Dump PDF [default: false] (Only available on some wikis with the PDF export plugin) (Only dumps the latest PDF revision)\n  --current-only        Dump latest revision, no history [default: false] (only for HTML at the moment)\n  --skip-to SKIP_TO     !DEV! Skip to title number [default: 0]\n  --path PATH           Specify dump directory [default: <site>-<date>]\n  --no-resume           Do not resume a previous dump [default: resume]\n  --threads THREADS     Number of sub threads to use [default: 1], not recommended to set > 5\n  --insecure            Disable SSL certificate verification\n  --ignore-errors       !DANGEROUS! ignore errors in the sub threads. This may cause incomplete dumps.\n  --ignore-action-disabled-edit\n                        Some sites disable edit action for anonymous users and some core pages. This option will ignore this error and textarea not found error.But\n                        you may only get a partial dump. (only works with --content)\n  --username USERNAME   login: username\n  --password PASSWORD   login: password\n  --cookies COOKIES     cookies file\n  --auto                dump: content+media+html, threads=5, ignore-action-disable-edit\n```\n\nFor most cases, you can use `--auto` to dump the site.\n\n```bash\ndokuWikiDumper https://example.com/wiki/ --auto\n```\n\nwhich is equivalent to\n\n```bash\ndokuWikiDumper https://example.com/wiki/ --content --media --html --threads 5 --ignore-action-disabled-edit\n```\n\n> Highly recommend using `--username` and `--password` to login (or using `--cookies`), because some sites may disable anonymous users to access some pages or check the raw wikitext.\n\n`--cookies` accepts a Netscape cookies file, you can use [cookies.txt Extension](https://addons.mozilla.org/en-US/firefox/addon/cookies-txt/) to export cookies from Firefox. It also accepts a json cookies file created by [Cookie Quick Manager](https://addons.mozilla.org/en-US/firefox/addon/cookie-quick-manager/).\n\n## Dump structure\n\n<!-- Dump structure -->\n| Directory or File       | Description                                 |\n|-----------              |-------------                                |\n| `attic/`                | old revisions of page. (wikitext)           |\n| `dumpMeta/`             | (dokuWikiDumper only) metadata of the dump. |\n| `dumpMeta/check.html`   | ?do=check page of the wiki.                 |\n| `dumpMeta/config.json`  | dump\'s configuration.                       |\n| `dumpMeta/favicon.ico`  | favicon of the site.                        |\n| `dumpMeta/files.txt`    | list of filename.                           |\n| `dumpMeta/index.html`   | homepage of the wiki.                       |\n| `dumpMeta/info.json`    | infomations of the wiki.                    |\n| `dumpMeta/titles.txt`   | list of page title.                         |\n| `html/`                 | (dokuWikiDumper only) HTML of the pages.    |\n| `media/`                | media files.                                |\n| `meta/`                 | metadata of the pages.                      |\n| `pages/`                | latest page content. (wikitext)             |\n<!-- /Dump structure -->\n\n## Available Backups/Dumps\n\nI made some backups for testing, you can check out the list: <https://github.com/orgs/saveweb/projects/4>.\n\n> Some wikidump has been uploaded to IA, you can check out the list: <https://archive.org/search?query=subject%3A"dokuWikiDumper">\n> \n> If you dumped a DokuWiki and want to share it, please feel free to open an issue, I will add it to the list.\n\n## How to import dump to DokuWiki\n\nIf you need to import Dokuwiki, please add the following configuration to `local.php`\n\n```php\n$conf[\'fnencode\'] = \'utf-8\'; // Dokuwiki default: \'safe\' (url encode)\n# \'safe\' => Non-ASCII characters will be escaped as %xx form.\n# \'utf-8\' => Non-ASCII characters will be preserved as UTF-8 characters.\n\n$conf[\'compression\'] = \'0\'; // Dokuwiki default: \'gz\'.\n# \'gz\' => attic/<id>.<rev_id>.txt.gz\n# \'bz2\' => attic/<id>.<rev_id>.txt.bz2\n# \'0\' => attic/<id>.<rev_id>.txt\n```\n\nImport `pages` dir if you only need the latest version of the page.  \nImport `meta` dir if you need the **changelog** of the page.  \nImport `attic` and `meta` dirs if you need the old revisions **content** of the page.  \nImport `media` dir if you need the media files.\n\n`dumpMeta` and `html` dirs are only used by `dokuWikiDumper`, you can ignore it.\n\n## Information\n\n### DokuWiki links\n\n- [DokuWiki](https://www.dokuwiki.org/)\n- [DokuWiki changelog](https://www.dokuwiki.org/changelog)\n- [DokuWiki source code](https://github.com/splitbrain/dokuwiki)\n\n### Other tools\n\n- [MediaWiki Scraper](https://github.com/mediawiki-client-tools/mediawiki-scraper) (aka `wikiteam3`), a tool for archiving MediaWiki, forked from [WikiTeam](https://github.com/wikiteam/wikiteam/) and has been rewritten in Python 3.\n- [WikiTeam](https://github.com/wikiteam/wikiteam/), a tool for archiving MediaWiki, written in Python 2.\n\n## License\n\nGPLv3\n\n## Contributors\n\nThis tool is based on an unmerged PR (_8 years ago!_) of [WikiTeam](https://github.com/WikiTeam/wikiteam/): [DokuWiki dump alpha](https://github.com/WikiTeam/wikiteam/pull/243) by [@PiRSquared17](https://github.com/PiRSquared17).\n\nI ([@yzqzss](https://github.com/yzqzss)) have rewritten the code in Python 3 and added some features, also fixed some bugs.\n',
     'author': 'yzqzss',
     'author_email': 'yzqzss@yandex.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dokuwikidumper-0.1.8/PKG-INFO` & `dokuwikidumper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dokuwikidumper
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for archiving DokuWiki
 License: GPL-3.0
 Author: yzqzss
 Author-email: yzqzss@yandex.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

