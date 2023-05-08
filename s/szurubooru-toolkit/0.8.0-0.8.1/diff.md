# Comparing `tmp/szurubooru_toolkit-0.8.0.tar.gz` & `tmp/szurubooru_toolkit-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szurubooru_toolkit-0.8.0.tar", max compression
+gzip compressed data, was "szurubooru_toolkit-0.8.1.tar", max compression
```

## Comparing `szurubooru_toolkit-0.8.0.tar` & `szurubooru_toolkit-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/LICENSE
--rw-r--r--   0        0        0    22797 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/README.md
--rw-r--r--   0        0        0     2466 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1363 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/__init__.py
--rw-r--r--   0        0        0     8773 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/config.py
--rw-r--r--   0        0        0     3870 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/danbooru.py
--rw-r--r--   0        0        0     3716 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/deepbooru.py
--rw-r--r--   0        0        0     1604 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/gelbooru.py
--rw-r--r--   0        0        0     9364 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/saucenao.py
--rw-r--r--   0        0        0      405 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/__init__.py
--rw-r--r--   0        0        0    12349 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/auto_tagger.py
--rw-r--r--   0        0        0     3459 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/create_tags.py
--rw-r--r--   0        0        0     2841 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/delete_posts.py
--rw-r--r--   0        0        0     6461 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_booru.py
--rw-r--r--   0        0        0     4044 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_twitter.py
--rw-r--r--   0        0        0     6013 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_url.py
--rw-r--r--   0        0        0     3314 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/reset_posts.py
--rw-r--r--   0        0        0     4713 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/tag_posts.py
--rw-r--r--   0        0        0    10615 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/upload_media.py
--rw-r--r--   0        0        0    10195 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/szurubooru.py
--rw-r--r--   0        0        0     7036 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/twitter.py
--rw-r--r--   0        0        0    13441 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/utils.py
--rw-r--r--   0        0        0    24381 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 20:16:35.829065 szurubooru_toolkit-0.8.1/LICENSE
+-rw-r--r--   0        0        0    23244 2023-05-08 20:16:35.829065 szurubooru_toolkit-0.8.1/README.md
+-rw-r--r--   0        0        0     2466 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1430 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/__init__.py
+-rw-r--r--   0        0        0     8809 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/config.py
+-rw-r--r--   0        0        0     5146 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/danbooru.py
+-rw-r--r--   0        0        0     3716 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/deepbooru.py
+-rw-r--r--   0        0        0     1604 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/gelbooru.py
+-rw-r--r--   0        0        0    10520 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/saucenao.py
+-rw-r--r--   0        0        0      405 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/__init__.py
+-rw-r--r--   0        0        0    12349 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/auto_tagger.py
+-rw-r--r--   0        0        0     3544 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/create_tags.py
+-rw-r--r--   0        0        0     2841 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/delete_posts.py
+-rw-r--r--   0        0        0     6461 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_booru.py
+-rw-r--r--   0        0        0     4044 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_twitter.py
+-rw-r--r--   0        0        0     6013 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_url.py
+-rw-r--r--   0        0        0     3314 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/reset_posts.py
+-rw-r--r--   0        0        0     4713 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/tag_posts.py
+-rw-r--r--   0        0        0    10615 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/upload_media.py
+-rw-r--r--   0        0        0    10195 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/szurubooru.py
+-rw-r--r--   0        0        0     7036 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/twitter.py
+-rw-r--r--   0        0        0    13441 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/utils.py
+-rw-r--r--   0        0        0    24828 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.8.1/PKG-INFO
```

### Comparing `szurubooru_toolkit-0.8.0/LICENSE` & `szurubooru_toolkit-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/README.md` & `szurubooru_toolkit-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
    the commands you would like to run regularly. An example command is provided
    in `crontab_sample`.
 1. Make sure to set the `src_path` option in `config.toml` to use
    `/szurubooru-toolkit/upload_src`. If you're using a different directory than
    `upload_src`, you may need to update the `docker-compose.yml` binding to be
    something like `./uploads:/szurubooru-toolkit/uploads`, and set
    `/szurubooru-toolkit/uploads` as the `src_path` option instead.
+1. Create the folder `tmp` in the same location.
 1. If you would like to use deepbooru or tag files, create `misc/deepbooru`
    and/or `misc/tags` in the same location and follow the instructions linked
    below
 1. Run `touch szurubooru_toolkit.log` in the same location to create a file for
    the log. You may need to set the log location to
    `/szurubooru-toolkit/szurubooru_toolkit.log` in `config.toml`
 1. Use `docker-compose up` or `docker-compose up -d` to start the container, or
@@ -75,22 +76,25 @@
 | `auto_tagger` | `saucenao_enabled` | Set this to `false` and `deepbooru_enabled` to `true` if you only want to tag with Deepbooru | `true` |
 | `auto_tagger` | `deepbooru_enabled` | If enabled, tag the post with Deepbooru if no tags with SauceNAO were found | `false` |
 | `auto_tagger` | `deepbooru_model` | Path to the Deepbooru model | `"./misc/deepbooru/model-resnet_custom_v3.h5"` |
 | `auto_tagger` | `deepbooru_threshold` | Define how accurate the matched tag from Deepbooru has to be | `"0.7"` |
 | `auto_tagger` | `deepbooru_forced` | Always tag with SauceNAO and Deepbooru | `false` |
 | `auto_tagger` | `deepbooru_set_tag` | Tag Deepbooru post with tag `deepbooru` | `true` |
 | `auto_tagger` | `hide_progress` | Set this to true to hide the progress bar | `false` |
+| `auto_tagger` | `use_pixiv_artist` | If the artist could only be found on pixiv, create and use the pixiv artist. Category has to be 'artist'. | `false` |
 | `danbooru` | `user` | Danbooru user | `"None"` |
 | `danbooru` | `api_key` | Danbooru api key | `"None"` |
 | `gelbooru` | `user` | Gelbooru user | `"None"` |
 | `gelbooru` | `api_key` | Gelbooru api key | `"None"` |
 | `konachan` | `user` | Konachan user | `"None"` |
 | `konachan` | `password` | Konachan password | `"None"` |
 | `yandere` | `user` | Yandere user | `"None"` |
 | `yandere` | `password` | Yandere password | `"None"` |
+| `sankaku` | `user` | Sankaku user | `"None"` |
+| `sankaku` | `password` | Sankaku password | `"None"` |
 | `pixiv` | `user` | Pixiv user. Currently not being used. | `"None"` |
 | `pixiv` | `password` | Pixiv password. Currently not being used. | `"None"` |
 | `pixiv` | `token` | Pixiv token. Currently not being used. | `"None"` |
 | `twitter` | `user_id` | The user id which should be queried. | `"None"` |
 | `twitter` | `consumer_key` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `twitter` | `consumer_secret` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `twitter` | `access_token` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
@@ -270,14 +274,15 @@
 
 ```
 
 __Examples__
 * `import-from-url "https://danbooru.donmai.us/posts?tags=foo"`
 * `import-from-url "https://chan.sankakucomplex.com/?tags=foo"`
 * `import-from-url "https://beta.sankakucomplex.com/post/show/<id>"`
+* `import-from-url --input-file urls.txt "https://danbooru.donmai.us/posts?tags=foo" "https://beta.sankakucomplex.com/post/show/<id>"`
 
 ### :dove: import-from-twitter
 This script fetches media files from your Twitter likes, uploads and optionally tags them.
 
 :warning: __OAuth 1.0a credentials are required to read the likes from a user. See https://developer.twitter.com/en/docs/authentication/oauth-1-0a on how to generate them.__
 
 The `user_id` can be converted on sites like https://tweeterid.com/. If you configured above credentials, you can also get your own ID from the `access_token`, which is in following format: `<user_id>-<random_string>`
```

### Comparing `szurubooru_toolkit-0.8.0/pyproject.toml` & `szurubooru_toolkit-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 
 
 [tool.poetry]
 name = "szurubooru-toolkit"
-version = "0.8.0"
+version = "0.8.1"
 description = "Python package and script collection to manage szurubooru."
 authors = ["reluce <reluce@fkosquad.moe>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/reluce/szurubooru-toolkit"
 documentation = "https://github.com/reluce/szurubooru-toolkit"
 keywords = ["szurubooru", "szuru", "booru", "saucenao", "deepbooru"]
```

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/__init__.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 
 from loguru import logger
 
 from .config import Config
 from .danbooru import Danbooru  # noqa F401
 from .gelbooru import Gelbooru  # noqa F401
-from .saucenao import SauceNao  # noqa F401
 from .szurubooru import Post  # noqa F401
 from .szurubooru import Szurubooru
 from .twitter import Twitter  # noqa F401
 from .utils import audit_rating  # noqa F401
 from .utils import collect_sources  # noqa F401
 from .utils import convert_rating  # noqa F401
 from .utils import download_media  # noqa F401
@@ -38,7 +37,9 @@
 config = Config()
 if config.auto_tagger['deepbooru_enabled']:
     from .deepbooru import Deepbooru  # noqa F401
 
 setup_logger(config)
 
 szuru = Szurubooru(config.szurubooru['url'], config.szurubooru['username'], config.szurubooru['api_token'])
+# SauceNao imports the szuru object, so we have to include it here
+from .saucenao import SauceNao  # noqa F401
```

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/config.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 'saucenao_enabled',
                 'deepbooru_enabled',
                 'deepbooru_model',
                 'deepbooru_threshold',
                 'deepbooru_forced',
                 'deepbooru_set_tag',
                 'hide_progress',
+                'use_pixiv_artist',
             ],
             'upload_media': [
                 'src_path',
                 'hide_progress',
                 'cleanup',
                 'tags',
                 'max_similarity',
```

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/danbooru.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/danbooru.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         if not danbooru_user == 'None' and not danbooru_api_key == 'None':
             self.client = Danbooru_Module('danbooru', username=danbooru_user, api_key=danbooru_api_key)
             logger.debug(f'Using Danbooru user {danbooru_user} with API key')
         else:
             self.client = Danbooru_Module('danbooru')
             logger.debug('Using Danbooru without user and API key')
 
+        self.session = requests.Session()
+        headers = {'User-Agent': 'Danbooru dummy agent'}
+        self.session.headers.update(headers)
+
     def get_by_md5(self, md5sum):
         for _ in range(1, 12):
             try:
                 logger.debug(f'Trying to fetch result by md5sum {md5sum}')
                 result = self.client.post_list(md5=md5sum)
                 logger.debug(f'Returning result: {result}')
 
@@ -58,16 +62,50 @@
 
     def get_rating(self, result):
         result_rating = result['rating']
         logger.debug(f'Returning rating: {result_rating}')
 
         return result_rating
 
-    @staticmethod
-    def download_tags(query: str = '*', min_post_count: int = 10, limit: int = 100) -> list:
+    def search_artist(self, artist) -> str:
+        """Search main artist name on Danbooru and return it
+
+        Args:
+            artist (str): The artist name. Can be an alias as well.
+        """
+
+        for _ in range(1, 12):
+            try:
+                result = self.client.artist_list(artist.lower())
+                if result:
+                    artist = result[0]['name']
+                else:
+                    artist = self.session.get(
+                        f'https://danbooru.donmai.us/artists.json?search[any_other_name_like]={artist.lower()}',
+                    ).json()[0]['name']
+                    self.session.close()
+
+                logger.debug(f'Returning artist: {artist}')
+
+                break
+            except (IndexError, KeyError):
+                logger.debug(f'Could not find artist "{artist.lower()}"')
+                artist = None
+
+                break
+            except (TimeoutError, PybooruError, PybooruHTTPError, PybooruAPIError):
+                logger.debug('Could not establish connection to Danbooru, trying again in 5s...')
+                sleep(5)
+        else:
+            logger.debug('Could not establish connection to Danbooru. Skip this artist...')
+            artist = None
+
+        return artist
+
+    def download_tags(self, query: str = '*', min_post_count: int = 10, limit: int = 100) -> list:
         """Download and return tags from Danbooru.
 
         Args:
             query (str, optional): Search for specific tag, accepts wildcard (*).
                 If not specified, download all tags. Defaults to '*'.
             min_post_count (int, optional): The minimum amount of posts the tag should have been used in.
                 Defaults to 10.
@@ -76,18 +114,14 @@
 
         Returns:
             list: A list with found tags.
         """
 
         tag_base_url = 'https://danbooru.donmai.us/tags.json'
 
-        session = requests.Session()
-        headers = {'User-Agent': 'Danbooru dummy agent'}
-        session.headers.update(headers)
-
         if limit > 1000:
             pages = limit // 1000
         else:
             pages = 1
 
         for page in range(1, pages + 1):
             tag_url = (
@@ -100,12 +134,12 @@
                 + str(limit)
                 + '&page='
                 + str(page)
             )
 
             try:
                 logger.info(f'Fetching tags from URL {tag_url}...')
-                yield session.get(tag_url, timeout=30).json()
+                yield self.session.get(tag_url, timeout=30).json()
             except Exception as e:
                 logger.critical(f'Could not fetch tags: {e}')
 
-        session.close()
+        self.session.close()
```

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/deepbooru.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/deepbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/gelbooru.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/gelbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/saucenao.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/saucenao.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pybooru.moebooru import Moebooru
 from pysaucenao import SauceNao as PySauceNao
 from syncer import sync
 
 from szurubooru_toolkit import Config
 from szurubooru_toolkit import Danbooru
 from szurubooru_toolkit import Gelbooru
+from szurubooru_toolkit import szuru
 from szurubooru_toolkit.utils import audit_rating
 from szurubooru_toolkit.utils import collect_sources
 from szurubooru_toolkit.utils import convert_rating
 from szurubooru_toolkit.utils import scrape_sankaku
 
 
 class SauceNao:
@@ -42,14 +43,15 @@
         if not config.auto_tagger['saucenao_api_token'] == 'None':
             logger.debug('Using SauceNAO API token')
 
         self.danbooru = Danbooru(config.danbooru['user'], config.danbooru['api_key'])
         self.gelbooru = Gelbooru(config.gelbooru['user'], config.gelbooru['api_key'])
         self.konachan = Moebooru('konachan', config.konachan['user'], config.konachan['password'])
         self.yandere = Moebooru('yandere', config.yandere['user'], config.yandere['password'])
+        self.use_pixiv_artist = config.auto_tagger['use_pixiv_artist']
 
     @sync
     async def get_metadata(self, content_url: str, image: bytes = None) -> tuple:
         """Retrieve results from SauceNAO and aggregate all metadata.
 
         Args:
             content_url (str): Image URL where SauceNAO should retrieve the image from.
@@ -63,27 +65,31 @@
         # Should not affect scraped data
         metadata = dict(tags=[], source='', rating='')
         metadata_dan = metadata.copy()
         metadata_gel = metadata.copy()
         metadata_san = metadata.copy()
         metadata_yan = metadata.copy()
         metadata_kona = metadata.copy()
+        metadata_pix = metadata.copy()
 
         limit_short = 1
         limit_long = 10
 
         response = await self.get_result(content_url, image)
 
         # Sometimes multiple results from the same Booru are found.
         # Results are sorted by their similiarity (highest first).
         # As soon as the highest similarity result is processed, skip other results from the same booru.
         danbooru_found = False
         gelbooru_found = False
         yandere_found = False
         konachan_found = False
+        sankaku_found = False
+
+        pixiv_artist = None
 
         if response and not response == 'Limit reached':
             for result in response:
                 if result.url is not None and 'danbooru' in result.url and not danbooru_found:
                     result_dan = self.danbooru.get_result(result.danbooru_id)
 
                     if not result_dan:
@@ -123,41 +129,60 @@
                         continue
 
                     metadata_kona['tags'] = result_kona['tags'].split()
                     metadata_kona['rating'] = convert_rating(result_kona['rating'])
                     metadata_kona['source'] = result.url
 
                     konachan_found = True
-                elif result.url is not None and 'sankaku' in result.url:
+                elif result.url is not None and 'sankaku' in result.url and not sankaku_found:
                     metadata_san['tags'], metadata_san['rating'] = scrape_sankaku(result.url)
                     metadata_san['source'] = result.url
 
+                    sankaku_found = True
+                elif result.url is not None and 'pixiv' in result.url:
+                    pixiv_artist = result.author_name
+
+                    metadata_pix['source'] = result.url
+
+            if pixiv_artist and not any([danbooru_found, gelbooru_found, konachan_found, yandere_found, sankaku_found]):
+                artist = self.danbooru.search_artist(pixiv_artist)
+
+                # Use the pixiv artist as a fallback if configured
+                if not artist and self.use_pixiv_artist:
+                    artist = pixiv_artist
+                    artist = artist.lower().replace(' ', '_')
+                    szuru.create_tag(artist, category='artist', overwrite=True)
+
+                metadata_pix['tags'] = [artist]
+
             limit_short = response.short_remaining
             logger.debug(f'Limit short: {limit_short}')
             limit_long = response.long_remaining
             logger.debug(f'Limit long: {limit_long}')
 
         # Collect scraped tags
         tags = list(
             set().union(
                 metadata_gel['tags'],
                 metadata_san['tags'],
                 metadata_dan['tags'],
                 metadata_yan['tags'],
                 metadata_kona['tags'],
+                metadata_pix['tags'],
             ),
         )
 
         # Collect scraped sources. Remove empty strings/sources in the process.
         source = collect_sources(
             metadata_gel['source'],
             metadata_san['source'],
             metadata_dan['source'],
             metadata_yan['source'],
             metadata_kona['source'],
+            metadata_pix['source'],
         )
         source_debug = source.replace('\n', '\\n')  # Don't display line breaks in logs
 
         # Get highest rating
         rating = audit_rating(
             metadata_gel['rating'],
             metadata_san['rating'],
@@ -166,23 +191,25 @@
             metadata_kona['rating'],
         )
 
         if response == 'Limit reached':
             limit_long = 0
 
         if metadata_dan['tags']:
-            logger.debug('Found result in Danbooru')
+            logger.debug('Found result on Danbooru')
         if metadata_gel['tags']:
-            logger.debug('Found result in Gelbooru')
+            logger.debug('Found result on Gelbooru')
         if metadata_san['tags']:
-            logger.debug('Found result in Sankaku')
+            logger.debug('Found result on Sankaku')
         if metadata_yan['tags']:
-            logger.debug('Found result in Yande.re')
+            logger.debug('Found result on Yande.re')
         if metadata_kona['tags']:
-            logger.debug('Found result in Konachan')
+            logger.debug('Found result on Konachan')
+        if metadata_pix['tags']:
+            logger.debug('Found result on pixiv')
 
         logger.debug(f'Returning tags: {tags}')
         logger.debug(f'Returning sources: {source_debug}')
         logger.debug(f'Returning rating: {rating}')
 
         return tags, source, rating, limit_short, limit_long
```

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/auto_tagger.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/auto_tagger.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/create_tags.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/create_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,15 +91,16 @@
 
                     try:
                         szuru.create_tag(tag_name, tag_category)
                     except TagExistsError as e:  # noqa F841
                         # logger.warning(e)  # Could result in lots of output with larger tag files
                         pass
         else:
-            results = Danbooru.download_tags(query, min_post_count, limit)
+            danbooru = Danbooru(config.danbooru['user'], config.danbooru['api_key'])
+            results = danbooru.download_tags(query, min_post_count, limit)
 
             for result in results:
                 for tag in result:
                     try:
                         szuru.create_tag(tag['name'], convert_tag_category(tag['category']), overwrite)
                     except TagExistsError as e:  # noqa F841
                         pass
```

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/delete_posts.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/delete_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_booru.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_booru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_twitter.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_url.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_url.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/reset_posts.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/reset_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/tag_posts.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/tag_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/upload_media.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/upload_media.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/szurubooru.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/szurubooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/twitter.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/utils.py` & `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.0/PKG-INFO` & `szurubooru_toolkit-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szurubooru-toolkit
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python package and script collection to manage szurubooru.
 Home-page: https://github.com/reluce/szurubooru-toolkit
 License: GPL-3.0-only
 Keywords: szurubooru,szuru,booru,saucenao,deepbooru
 Author: reluce
 Author-email: reluce@fkosquad.moe
 Requires-Python: >=3.8,<3.11
@@ -71,14 +71,15 @@
    the commands you would like to run regularly. An example command is provided
    in `crontab_sample`.
 1. Make sure to set the `src_path` option in `config.toml` to use
    `/szurubooru-toolkit/upload_src`. If you're using a different directory than
    `upload_src`, you may need to update the `docker-compose.yml` binding to be
    something like `./uploads:/szurubooru-toolkit/uploads`, and set
    `/szurubooru-toolkit/uploads` as the `src_path` option instead.
+1. Create the folder `tmp` in the same location.
 1. If you would like to use deepbooru or tag files, create `misc/deepbooru`
    and/or `misc/tags` in the same location and follow the instructions linked
    below
 1. Run `touch szurubooru_toolkit.log` in the same location to create a file for
    the log. You may need to set the log location to
    `/szurubooru-toolkit/szurubooru_toolkit.log` in `config.toml`
 1. Use `docker-compose up` or `docker-compose up -d` to start the container, or
@@ -113,22 +114,25 @@
 | `auto_tagger` | `saucenao_enabled` | Set this to `false` and `deepbooru_enabled` to `true` if you only want to tag with Deepbooru | `true` |
 | `auto_tagger` | `deepbooru_enabled` | If enabled, tag the post with Deepbooru if no tags with SauceNAO were found | `false` |
 | `auto_tagger` | `deepbooru_model` | Path to the Deepbooru model | `"./misc/deepbooru/model-resnet_custom_v3.h5"` |
 | `auto_tagger` | `deepbooru_threshold` | Define how accurate the matched tag from Deepbooru has to be | `"0.7"` |
 | `auto_tagger` | `deepbooru_forced` | Always tag with SauceNAO and Deepbooru | `false` |
 | `auto_tagger` | `deepbooru_set_tag` | Tag Deepbooru post with tag `deepbooru` | `true` |
 | `auto_tagger` | `hide_progress` | Set this to true to hide the progress bar | `false` |
+| `auto_tagger` | `use_pixiv_artist` | If the artist could only be found on pixiv, create and use the pixiv artist. Category has to be 'artist'. | `false` |
 | `danbooru` | `user` | Danbooru user | `"None"` |
 | `danbooru` | `api_key` | Danbooru api key | `"None"` |
 | `gelbooru` | `user` | Gelbooru user | `"None"` |
 | `gelbooru` | `api_key` | Gelbooru api key | `"None"` |
 | `konachan` | `user` | Konachan user | `"None"` |
 | `konachan` | `password` | Konachan password | `"None"` |
 | `yandere` | `user` | Yandere user | `"None"` |
 | `yandere` | `password` | Yandere password | `"None"` |
+| `sankaku` | `user` | Sankaku user | `"None"` |
+| `sankaku` | `password` | Sankaku password | `"None"` |
 | `pixiv` | `user` | Pixiv user. Currently not being used. | `"None"` |
 | `pixiv` | `password` | Pixiv password. Currently not being used. | `"None"` |
 | `pixiv` | `token` | Pixiv token. Currently not being used. | `"None"` |
 | `twitter` | `user_id` | The user id which should be queried. | `"None"` |
 | `twitter` | `consumer_key` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `twitter` | `consumer_secret` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `twitter` | `access_token` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
@@ -308,14 +312,15 @@
 
 ```
 
 __Examples__
 * `import-from-url "https://danbooru.donmai.us/posts?tags=foo"`
 * `import-from-url "https://chan.sankakucomplex.com/?tags=foo"`
 * `import-from-url "https://beta.sankakucomplex.com/post/show/<id>"`
+* `import-from-url --input-file urls.txt "https://danbooru.donmai.us/posts?tags=foo" "https://beta.sankakucomplex.com/post/show/<id>"`
 
 ### :dove: import-from-twitter
 This script fetches media files from your Twitter likes, uploads and optionally tags them.
 
 :warning: __OAuth 1.0a credentials are required to read the likes from a user. See https://developer.twitter.com/en/docs/authentication/oauth-1-0a on how to generate them.__
 
 The `user_id` can be converted on sites like https://tweeterid.com/. If you configured above credentials, you can also get your own ID from the `access_token`, which is in following format: `<user_id>-<random_string>`
```

