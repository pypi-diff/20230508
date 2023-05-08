# Comparing `tmp/reddit-user-to-sqlite-0.1.0.tar.gz` & `tmp/reddit-user-to-sqlite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-user-to-sqlite-0.1.0.tar", last modified: Sat May  6 21:09:16 2023, max compression
+gzip compressed data, was "reddit-user-to-sqlite-0.2.0.tar", last modified: Mon May  8 07:05:33 2023, max compression
```

## Comparing `reddit-user-to-sqlite-0.1.0.tar` & `reddit-user-to-sqlite-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit-user-to-sqlite-0.1.0/LICENSE
--rw-r--r--   0        0        0     3020 2023-05-06 20:30:31.805602 reddit-user-to-sqlite-0.1.0/README.md
--rw-r--r--   0        0        0     1202 2023-05-06 17:38:08.606912 reddit-user-to-sqlite-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/__init__.py
--rw-r--r--   0        0        0     1026 2023-05-06 20:42:33.460776 reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/cli.py
--rw-r--r--   0        0        0      239 2023-05-05 03:42:09.817348 reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/helpers.py
--rw-r--r--   0        0        0     2467 2023-05-06 18:42:54.663856 reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/reddit_api.py
--rw-r--r--   0        0        0     3235 2023-05-06 21:03:04.253669 reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/sqlite_helpers.py
--rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 reddit-user-to-sqlite-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit-user-to-sqlite-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3797 2023-05-08 06:08:15.246487 reddit-user-to-sqlite-0.2.0/README.md
+-rw-r--r--   0        0        0     1202 2023-05-08 04:41:42.994469 reddit-user-to-sqlite-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-08 06:48:29.198734 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/cli.py
+-rw-r--r--   0        0        0      239 2023-05-05 03:42:09.817348 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/helpers.py
+-rw-r--r--   0        0        0     3141 2023-05-08 07:02:22.652956 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/reddit_api.py
+-rw-r--r--   0        0        0     4750 2023-05-08 05:36:28.464858 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/sqlite_helpers.py
+-rw-r--r--   0        0        0     4894 1970-01-01 00:00:00.000000 reddit-user-to-sqlite-0.2.0/PKG-INFO
```

### Comparing `reddit-user-to-sqlite-0.1.0/LICENSE` & `reddit-user-to-sqlite-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-user-to-sqlite-0.1.0/README.md` & `reddit-user-to-sqlite-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # reddit-user-to-sqlite
 
-Stores all the content from a specific user in a SQLite database. This includes their comments and will soon include their posts.
+Stores all the content from a specific user in a SQLite database. This includes their comments and their posts.
 
 ## Install
 
-The PyPI package is `reddit-user-to-sqlite` ([PyPI Link]()). Install it globally using [pipx](https://pypa.github.io/pipx/):
+The PyPI package is `reddit-user-to-sqlite` ([PyPI Link](https://pypi.org/project/reddit-user-to-sqlite/)). Install it globally using [pipx](https://pypa.github.io/pipx/):
 
 ```bash
 pipx install reddit-user-to-sqlite
 ```
 
 ## Usage
 
@@ -64,14 +64,25 @@
               "columns": ["text"]
             },
             "datasette-render-timestamps": {
               "columns": ["timestamp"]
             }
           }
         },
+        "posts": {
+          "sort_desc": "timestamp",
+          "plugins": {
+            "datasette-render-markdown": {
+              "columns": ["text"]
+            },
+            "datasette-render-timestamps": {
+              "columns": ["timestamp"]
+            }
+          }
+        },
         "subreddits": {
           "sort": "name"
         }
       }
     }
   }
 }
@@ -104,7 +115,18 @@
 ### Running Tests
 
 In your virtual environment, a simple `pytest` should run the unit test suite.
 
 ## Motivation
 
 I got nervous when I saw Reddit's [notification of upcoming API changes](https://old.reddit.com/r/reddit/comments/12qwagm/an_update_regarding_reddits_api/). To ensure I could always access data I created, I wanted to make sure I had a backup in place before anything changed in a big way.
+
+## FAQs
+
+### Why do some of my posts say `[removed]` even though I can see them?
+
+If a post is removed, only the mods and the user who posted it can see its text. Since this tool currently runs without any authentication, those removed posts can't be fetched via the API.
+
+This will be fixed in a future release, either by:
+
+- (planned) being able to pull data from a GDPR archive
+- (maybe) adding support for authentication, so you can see your own posts
```

### Comparing `reddit-user-to-sqlite-0.1.0/pyproject.toml` & `reddit-user-to-sqlite-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reddit-user-to-sqlite"
-version = "0.1.0"
+version = "0.2.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Create a SQLite database containing data pulled from Reddit about a single user."
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.10"
```

### Comparing `reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/cli.py` & `reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import click
 from sqlite_utils import Database
 
 from reddit_user_to_sqlite.helpers import clean_username
-from reddit_user_to_sqlite.reddit_api import load_comments_for_user
+from reddit_user_to_sqlite.reddit_api import load_comments_for_user, load_posts_for_user
 from reddit_user_to_sqlite.sqlite_helpers import (
     ensure_fts,
     insert_subreddits,
     insert_user,
     upsert_comments,
+    upsert_posts,
 )
 
 
 @click.group()
 @click.version_option()
 def cli():
     "Save data from Reddit to a SQLite database"
@@ -23,22 +24,30 @@
     "--db",
     "db_path",
     type=click.Path(file_okay=True, dir_okay=False, allow_dash=False),
     default="reddit.db",
 )
 def user(db_path, username):
     username = clean_username(username)
-    click.echo(f"loading data about /u/{username} into {db_path}")
+    click.echo(f"loading data about /u/{username} into {db_path}\n")
 
+    click.echo("fetching (up to 10 pages of) comments")
     comments = load_comments_for_user(username)
-    db = Database(db_path)
-
-    if not comments:
-        raise click.ClickException(f"no data found for username {username}")
 
-    insert_user(db, comments[0])
-
-    insert_subreddits(db, comments)
+    db = Database(db_path)
+    if comments:
+        insert_user(db, comments[0])
+        insert_subreddits(db, comments)
+        upsert_comments(db, comments)
+
+    click.echo("\nfetching (up to 10 pages of) posts")
+
+    posts = load_posts_for_user(username)
+    if posts:
+        insert_user(db, posts[0])
+        insert_subreddits(db, posts)
+        upsert_posts(db, posts)
 
-    upsert_comments(db, comments)
+    if not (comments or posts):
+        raise click.ClickException(f"no data found for username: {username}")
 
     ensure_fts(db)
```

### Comparing `reddit-user-to-sqlite-0.1.0/reddit_user_to_sqlite/reddit_api.py` & `reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/reddit_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional, TypedDict, final
+from typing import Literal, Optional, Sequence, TypedDict, final
 
 import requests
 from tqdm import tqdm
 
 USER_AGENT = "reddit-to-sqlite"
 
 
@@ -58,62 +58,94 @@
     # post ID
     link_id: str
     link_permalink: str
     # "r/consoledeals",
     subreddit_name_prefixed: str
 
 
+class Post(SubredditFragment, UserFragment):
+    # no prefix
+    id: str
+
+    title: str
+
+    # markdown content of the post; could be empty
+    selftext: str
+    # external link (or self link)
+    url: str
+    # link to reddit thread (sans domain)
+    permalink: str
+
+    upvote_ratio: float
+    score: int
+    total_awards_received: int
+
+    num_comments: int
+    over_18: bool
+
+    # timestamp
+    created: float
+
+
 @final
-class CommentWrapper(TypedDict):
+class ResourceWrapper(TypedDict):
     kind: str
-    data: Comment
+    data: Comment | Post
 
 
 @final
-class CommentBody(TypedDict):
+class ResponseBody(TypedDict):
     before: Optional[str]
     after: Optional[str]
     modhash: str
     geo_filter: str
     dist: int
-    children: list[CommentWrapper]
+    children: Sequence[ResourceWrapper]
 
 
 @final
-class CommentsResponse(TypedDict):
-    data: CommentBody
+class SuccessResponse(TypedDict):
+    data: ResponseBody
     kind: Literal["Listing"]
 
 
 @final
 class ErorrResponse(TypedDict):
     message: str
     error: int
 
 
 # max page size is 100
 PAGE_SIZE = 100
 
 
-def load_comments_for_user(username: str) -> list[Comment]:
-    comments: list[Comment] = []
+def _load_paged_resource(resource: Literal["comments", "submitted"], username: str):
+    result = []
     after = None
     # max number of pages we can fetch
     for _ in tqdm(range(10)):
-        response: CommentsResponse | ErorrResponse = requests.get(
-            f"https://www.reddit.com/user/{username}/comments.json",
+        response: SuccessResponse | ErorrResponse = requests.get(
+            f"https://www.reddit.com/user/{username}/{resource}.json",
             {"limit": PAGE_SIZE, "raw_json": 1, "after": after},
             headers={"user-agent": USER_AGENT},
         ).json()
 
         if "error" in response:
             raise ValueError(
                 f'Received API error from Reddit (code {response["error"]}): {response["message"]}'
             )
 
-        comments += [c["data"] for c in response["data"]["children"]]
+        result += [c["data"] for c in response["data"]["children"]]
         after = response["data"]["after"]
 
         if len(response["data"]["children"]) < PAGE_SIZE:
             break
 
-    return comments
+    return result
+
+
+def load_comments_for_user(username: str) -> list[Comment]:
+    return _load_paged_resource("comments", username)
+
+
+def load_posts_for_user(username: str) -> list[Post]:
+    return _load_paged_resource("submitted", username)
```

### Comparing `reddit-user-to-sqlite-0.1.0/PKG-INFO` & `reddit-user-to-sqlite-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-user-to-sqlite
-Version: 0.1.0
+Version: 0.2.0
 Summary: Create a SQLite database containing data pulled from Reddit about a single user.
 Keywords: sqlite,reddit,dogsheep
 Author-email: David Brownman <beamneocube@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
@@ -22,19 +22,19 @@
 Project-URL: Bug Tracker, https://github.com/xavdid/reddit-user-to-sqlite/issues
 Project-URL: Changelog, https://github.com/xavdid/reddit-user-to-sqlite/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://github.com/xavdid/reddit-user-to-sqlite
 Provides-Extra: test
 
 # reddit-user-to-sqlite
 
-Stores all the content from a specific user in a SQLite database. This includes their comments and will soon include their posts.
+Stores all the content from a specific user in a SQLite database. This includes their comments and their posts.
 
 ## Install
 
-The PyPI package is `reddit-user-to-sqlite` ([PyPI Link]()). Install it globally using [pipx](https://pypa.github.io/pipx/):
+The PyPI package is `reddit-user-to-sqlite` ([PyPI Link](https://pypi.org/project/reddit-user-to-sqlite/)). Install it globally using [pipx](https://pypa.github.io/pipx/):
 
 ```bash
 pipx install reddit-user-to-sqlite
 ```
 
 ## Usage
 
@@ -90,14 +90,25 @@
               "columns": ["text"]
             },
             "datasette-render-timestamps": {
               "columns": ["timestamp"]
             }
           }
         },
+        "posts": {
+          "sort_desc": "timestamp",
+          "plugins": {
+            "datasette-render-markdown": {
+              "columns": ["text"]
+            },
+            "datasette-render-timestamps": {
+              "columns": ["timestamp"]
+            }
+          }
+        },
         "subreddits": {
           "sort": "name"
         }
       }
     }
   }
 }
@@ -131,7 +142,18 @@
 
 In your virtual environment, a simple `pytest` should run the unit test suite.
 
 ## Motivation
 
 I got nervous when I saw Reddit's [notification of upcoming API changes](https://old.reddit.com/r/reddit/comments/12qwagm/an_update_regarding_reddits_api/). To ensure I could always access data I created, I wanted to make sure I had a backup in place before anything changed in a big way.
 
+## FAQs
+
+### Why do some of my posts say `[removed]` even though I can see them?
+
+If a post is removed, only the mods and the user who posted it can see its text. Since this tool currently runs without any authentication, those removed posts can't be fetched via the API.
+
+This will be fixed in a future release, either by:
+
+- (planned) being able to pull data from a GDPR archive
+- (maybe) adding support for authentication, so you can see your own posts
+
```

