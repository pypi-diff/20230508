# Comparing `tmp/diffcord-0.0.7.tar.gz` & `tmp/diffcord-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffcord-0.0.7.tar", last modified: Mon Mar 20 22:52:38 2023, max compression
+gzip compressed data, was "diffcord-0.0.8.tar", last modified: Mon May  8 20:25:47 2023, max compression
```

## Comparing `diffcord-0.0.7.tar` & `diffcord-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 22:52:38.621718 diffcord-0.0.7/
--rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2576 2023-03-20 22:52:38.620721 diffcord-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2167 2023-03-20 17:31:15.000000 diffcord-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 22:52:38.569420 diffcord-0.0.7/diffcord/
--rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-0.0.7/diffcord/__init__.py
--rw-rw-rw-   0        0        0     2110 2023-03-20 17:25:00.000000 diffcord-0.0.7/diffcord/api.py
--rw-rw-rw-   0        0        0     6747 2023-03-20 17:34:03.000000 diffcord-0.0.7/diffcord/client.py
--rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-0.0.7/diffcord/error.py
--rw-rw-rw-   0        0        0     3043 2023-03-20 22:50:09.000000 diffcord-0.0.7/diffcord/vote.py
-drwxrwxrwx   0        0        0        0 2023-03-20 22:52:38.579417 diffcord-0.0.7/diffcord.egg-info/
--rw-rw-rw-   0        0        0     2576 2023-03-20 22:52:38.000000 diffcord-0.0.7/diffcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-03-20 22:52:38.000000 diffcord-0.0.7/diffcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 22:52:38.000000 diffcord-0.0.7/diffcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 17:40:35.000000 diffcord-0.0.7/diffcord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-03-20 22:52:38.000000 diffcord-0.0.7/diffcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 22:52:38.000000 diffcord-0.0.7/diffcord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 22:52:38.621718 diffcord-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-03-20 22:51:06.000000 diffcord-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 22:52:38.618719 diffcord-0.0.7/tests/
--rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-0.0.7/tests/test_client.py
--rw-rw-rw-   0        0        0     4232 2023-03-20 16:20:58.000000 diffcord-0.0.7/tests/test_webhook_listener.py
--rw-rw-rw-   0        0        0     1992 2023-03-20 22:22:40.000000 diffcord-0.0.7/tests/testing_main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.143549 diffcord-0.0.8/
+-rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2611 2023-05-08 20:25:47.142547 diffcord-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2202 2023-03-20 23:26:24.000000 diffcord-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.112556 diffcord-0.0.8/diffcord/
+-rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-0.0.8/diffcord/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-0.0.8/diffcord/api.py
+-rw-rw-rw-   0        0        0     6747 2023-05-08 03:04:14.000000 diffcord-0.0.8/diffcord/client.py
+-rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-0.0.8/diffcord/error.py
+-rw-rw-rw-   0        0        0     3333 2023-05-07 19:38:24.000000 diffcord-0.0.8/diffcord/vote.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.122574 diffcord-0.0.8/diffcord.egg-info/
+-rw-rw-rw-   0        0        0     2611 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 17:40:35.000000 diffcord-0.0.8/diffcord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 20:25:47.143549 diffcord-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-05-08 20:25:14.000000 diffcord-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.140577 diffcord-0.0.8/tests/
+-rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-0.0.8/tests/test_client.py
+-rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-0.0.8/tests/test_webhook_listener.py
+-rw-rw-rw-   0        0        0     2103 2023-05-08 19:58:25.000000 diffcord-0.0.8/tests/testing_main.py
```

### Comparing `diffcord-0.0.7/LICENSE` & `diffcord-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.7/PKG-INFO` & `diffcord-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,14 +57,15 @@
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=8080, handle_vote=on_vote, verify_code="WEBHOOK_AUTH_CODE_HERE")
 
 diff_client = Client(bot, "YOUR_DIFFCORD_API_TOKEN", diff_webhook_listener,
                      send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
 
+bot.diffcord_client = diff_client
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener & start send stats
     await diff_client.start()  # required
```

### Comparing `diffcord-0.0.7/README.md` & `diffcord-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=8080, handle_vote=on_vote, verify_code="WEBHOOK_AUTH_CODE_HERE")
 
 diff_client = Client(bot, "YOUR_DIFFCORD_API_TOKEN", diff_webhook_listener,
                      send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
 
+bot.diffcord_client = diff_client
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener & start send stats
     await diff_client.start()  # required
```

### Comparing `diffcord-0.0.7/diffcord/api.py` & `diffcord-0.0.8/diffcord/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         """ API Token """
 
         self.base_url: str = base_url
         """ Base URL of the API in which the requests will be made to """
 
         self.__headers = {
             "x-api-key": self.token,
+            "Authorization": self.token,
             "Content-Type": "application/json",
             "User-Agent": f"Diffcord-Python-SDK",
         }
 
     async def make_request(self, method: str, path: str, **kwargs: Any) -> Any:
         """ Make a request to the Diffcord API.
         :param: method: The method of the request
@@ -27,14 +28,17 @@
         :param: kwargs: The kwargs of the request
         :return: The response from the Diffcord API
         """
         async with httpx.AsyncClient() as client:
 
             response = await client.request(method, self.base_url + path, **kwargs, headers=self.__headers)
 
+            if response.status_code == 204:
+                return None
+
             json_data = response.json()
 
             if response.status_code == 401:
                 if json_data["error"]["code"] == "ERR_INVALID_API_KEY":
                     raise InvalidTokenException(json_data["error"], response)
 
                 raise HTTPException(response.status_code, json_data["error"]["message"], json_data["error"]["code"])
```

### Comparing `diffcord-0.0.7/diffcord/client.py` & `diffcord-0.0.8/diffcord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """ Represents a client connection to the Diffcord API.
     """
     __SEND_STATS_SLEEP_DURATION = datetime.timedelta(hours=1)
 
     def __init__(self, bot: Any, token: str, vote_listener: VoteWebhookListener, send_stats: bool = True,
                  send_stats_success: Callable[[], Awaitable[None]] = None,
                  send_stats_failure: Callable[[Exception], Awaitable[None]] = None, base_url: str = None) -> None:
-        super().__init__(token, "https://api.diffcord.com" if base_url is None else base_url)
+        super().__init__(token, "https://diffcord.com/api" if base_url is None else base_url)
 
         self.bot: Any = bot
         """ The bot object. """
 
         self.token: str = token
         """ The Diffcord API token. """
```

### Comparing `diffcord-0.0.7/diffcord/error.py` & `diffcord-0.0.8/diffcord/error.py`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.7/diffcord/vote.py` & `diffcord-0.0.8/diffcord/vote.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,34 +45,40 @@
         return self.__repr__()
 
 
 class UserVoteInformation:
     """ Represents a user vote information.
     """
 
-    def __init__(self, user_id: str, bot_id: str, monthly_votes: int, since_last_vote: int, until_next_vote: int):
+    def __init__(self, user_id: str, bot_id: str, monthly_votes: int, since_last_vote: int | None, until_next_vote: int):
         self.user_id: str = user_id
         """ The id of the target user. """
 
         self.bot_id: str = bot_id
         """ The id of the bot which the user has voted for. """
 
         self.monthly_votes: int = monthly_votes
         """ The number of votes this user has for the given bot this month. """
 
-        self.since_last_vote: datetime.timedelta = datetime.timedelta(seconds=since_last_vote)
+        self.since_last_vote: datetime.timedelta = datetime.timedelta(seconds=since_last_vote) if since_last_vote is not None else None
         """ Time in seconds since the last vote. """
 
         self.until_next_vote: datetime.timedelta = datetime.timedelta(seconds=until_next_vote)
         """ Time in seconds till the next vote. """
 
-        self.last_vote: datetime.datetime = datetime.datetime.now() - self.since_last_vote
+        self.last_vote: datetime.datetime = datetime.datetime.now() - self.since_last_vote if self.since_last_vote is not None else None
         """ The last time the user voted. """
 
         self.next_vote: datetime.datetime = datetime.datetime.now() + self.until_next_vote
         """ The next time the user can vote. """
 
+    @property
+    def can_vote(self) -> bool:
+        """ Whether the user can vote or not.
+        """
+        return not self.until_next_vote or self.until_next_vote.total_seconds() <= 0
+
     def __repr__(self):
         return f"<UserVoteInformation user_id={self.user_id} bot_id={self.bot_id} votes_this_month={self.monthly_votes} since_last_vote={self.since_last_vote} until_next_vote={self.until_next_vote}>"
 
     def __str__(self):
         return self.__repr__()
```

### Comparing `diffcord-0.0.7/diffcord.egg-info/PKG-INFO` & `diffcord-0.0.8/diffcord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,14 +57,15 @@
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=8080, handle_vote=on_vote, verify_code="WEBHOOK_AUTH_CODE_HERE")
 
 diff_client = Client(bot, "YOUR_DIFFCORD_API_TOKEN", diff_webhook_listener,
                      send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
 
+bot.diffcord_client = diff_client
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener & start send stats
     await diff_client.start()  # required
```

### Comparing `diffcord-0.0.7/setup.py` & `diffcord-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='diffcord',
-    version='0.0.7',
+    version='0.0.8',
     description="A Python wrapper for the Diffcord API written in Python.",
     packages=find_packages(),
     author='jadelasmar4@gmail.com',
     zip_safe=False,
     install_requires=requirements,
     python_requires='>=3.7.0',
     long_description_content_type="text/markdown",
```

### Comparing `diffcord-0.0.7/tests/test_webhook_listener.py` & `diffcord-0.0.8/tests/test_webhook_listener.py`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.7/tests/testing_main.py` & `diffcord-0.0.8/tests/testing_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,33 +19,34 @@
     print("Stats failed to send:", e)
 
 
 async def on_vote(vote: UserBotVote) -> None:
     """ Handle the vote.
     """
     # LOGIC HERE... (give rewards, etc.)
-
     user = await bot.fetch_user(vote.user_id)  # Get the discord user object from the user id
     await user.send("Thanks for voting!")  # Send a DM to the user who voted
 
 
 # create Diffcord client & webhook listener
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=6969, handle_vote=on_vote, verify_code="diffcord-basketbot")
 
-diff_client = Client(bot, "2c0a7f4354f74a199bca20d5f0dd0ba7", diff_webhook_listener,
-                     send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
+diff_client = Client(bot, "f993dbf85d94e8159f9cd1e6d131e61ec4bf5642ac41253e2967003c93ce4004", diff_webhook_listener,
+                     send_stats_success=send_stats_success, send_stats_failure=send_stats_failure,
+                     base_url="https://diffcord-v2.vercel.app/api")
 
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener
     await diff_client.start()
+    pass
 
 
 # on bot close even
 
 
 @bot.slash_command(name="test")
 async def test_command(ctx):
@@ -56,8 +57,8 @@
     bot_votes_this_month: int = await diff_client.bot_votes_this_month()
 
     # respond
     message = f"You have voted {user_vote_info.monthly_votes} times this month! This bot has {bot_votes_this_month} votes this month!"
     await ctx.respond(message)
 
 
-bot.run("MTA1MzE1ODc4MDk1MjY0NTY2Mg.GMKTP-.iW4SSYBjLDjKTGyRyUXWOlWEkpUvEJGSJGkUM4")
+bot.run("MTA1MzE1ODc4MDk1MjY0NTY2Mg.GMKTP-.iW4SSYBjLDjKTGyRyUXWOlWEkpUvEJGSJGkUM4")
```

