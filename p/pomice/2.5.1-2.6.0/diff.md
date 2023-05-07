# Comparing `tmp/pomice-2.5.1.tar.gz` & `tmp/pomice-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomice-2.5.1.tar", last modified: Wed May  3 23:49:48 2023, max compression
+gzip compressed data, was "pomice-2.6.0.tar", last modified: Sun May  7 23:28:20 2023, max compression
```

## Comparing `pomice-2.5.1.tar` & `pomice-2.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.056567 pomice-2.5.1/
--rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     5445 2023-05-03 23:49:48.054563 pomice-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 23:49:47.985417 pomice-2.5.1/pomice/
--rw-rw-rw-   0        0        0      853 2023-05-03 23:48:41.000000 pomice-2.5.1/pomice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.042346 pomice-2.5.1/pomice/applemusic/
--rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.5.1/pomice/applemusic/__init__.py
--rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.5.1/pomice/applemusic/client.py
--rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/applemusic/exceptions.py
--rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.5.1/pomice/applemusic/objects.py
--rw-rw-rw-   0        0        0     8043 2023-05-03 23:47:11.000000 pomice-2.5.1/pomice/enums.py
--rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.5.1/pomice/events.py
--rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.5.1/pomice/exceptions.py
--rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.5.1/pomice/filters.py
--rw-rw-rw-   0        0        0     5302 2023-04-23 18:14:31.000000 pomice-2.5.1/pomice/objects.py
--rw-rw-rw-   0        0        0    23884 2023-05-01 11:42:50.000000 pomice-2.5.1/pomice/player.py
--rw-rw-rw-   0        0        0    35055 2023-05-03 23:47:13.000000 pomice-2.5.1/pomice/pool.py
--rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.5.1/pomice/py.typed
--rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.5.1/pomice/queue.py
--rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/routeplanner.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.052423 pomice-2.5.1/pomice/spotify/
--rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/spotify/__init__.py
--rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.5.1/pomice/spotify/client.py
--rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/spotify/exceptions.py
--rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.5.1/pomice/spotify/objects.py
--rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.5.1/pomice/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.033822 pomice-2.5.1/pomice.egg-info/
--rw-rw-rw-   0        0        0     5445 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 23:49:48.056567 pomice-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2171 2023-04-29 18:06:01.000000 pomice-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.265076 pomice-2.6.0/
+-rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0     5445 2023-05-07 23:28:20.265076 pomice-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.231722 pomice-2.6.0/pomice/
+-rw-rw-rw-   0        0        0      853 2023-05-07 23:27:35.000000 pomice-2.6.0/pomice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.260114 pomice-2.6.0/pomice/applemusic/
+-rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.6.0/pomice/applemusic/__init__.py
+-rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.6.0/pomice/applemusic/client.py
+-rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/applemusic/exceptions.py
+-rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.6.0/pomice/applemusic/objects.py
+-rw-rw-rw-   0        0        0     8043 2023-05-03 23:47:11.000000 pomice-2.6.0/pomice/enums.py
+-rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.6.0/pomice/events.py
+-rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.6.0/pomice/exceptions.py
+-rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.6.0/pomice/filters.py
+-rw-rw-rw-   0        0        0     5302 2023-04-23 18:14:31.000000 pomice-2.6.0/pomice/objects.py
+-rw-rw-rw-   0        0        0    23940 2023-05-07 18:56:40.000000 pomice-2.6.0/pomice/player.py
+-rw-rw-rw-   0        0        0    36635 2023-05-07 23:27:06.000000 pomice-2.6.0/pomice/pool.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.6.0/pomice/py.typed
+-rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.6.0/pomice/queue.py
+-rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/routeplanner.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.263568 pomice-2.6.0/pomice/spotify/
+-rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/spotify/__init__.py
+-rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.6.0/pomice/spotify/client.py
+-rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/spotify/exceptions.py
+-rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.6.0/pomice/spotify/objects.py
+-rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.6.0/pomice/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.255950 pomice-2.6.0/pomice.egg-info/
+-rw-rw-rw-   0        0        0     5445 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 23:28:20.265076 pomice-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2185 2023-05-07 23:14:36.000000 pomice-2.6.0/setup.py
```

### Comparing `pomice-2.5.1/LICENSE` & `pomice-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/PKG-INFO` & `pomice-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.5.1
+Version: 2.6.0
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.5.1/README.md` & `pomice-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/__init__.py` & `pomice-2.6.0/pomice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     raise DiscordPyOutdated(
         "You must have discord.py (v2.0 or greater) to use this library. "
         "Uninstall your current version and install discord.py 2.0 "
         "using 'pip install discord.py'",
     )
 
-__version__ = "2.5.1"
+__version__ = "2.6.0"
 __title__ = "pomice"
 __author__ = "cloudwithax"
 __license__ = "GPL-3.0"
 __copyright__ = "Copyright (c) 2023, cloudwithax"
 
 from .enums import *
 from .events import *
```

### Comparing `pomice-2.5.1/pomice/applemusic/client.py` & `pomice-2.6.0/pomice/applemusic/client.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/applemusic/objects.py` & `pomice-2.6.0/pomice/applemusic/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/enums.py` & `pomice-2.6.0/pomice/enums.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/events.py` & `pomice-2.6.0/pomice/events.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/exceptions.py` & `pomice-2.6.0/pomice/exceptions.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/filters.py` & `pomice-2.6.0/pomice/filters.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/objects.py` & `pomice-2.6.0/pomice/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/player.py` & `pomice-2.6.0/pomice/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,19 +430,20 @@
             await self.disconnect()
         except AttributeError:
             # 'NoneType' has no attribute '_get_voice_client_key' raised by self.cleanup() ->
             # assume we're already disconnected and cleaned up
             assert not self.is_connected and not self.channel
 
         self._node._players.pop(self.guild.id)
-        await self._node.send(
-            method="DELETE",
-            path=self._player_endpoint_uri,
-            guild_id=self._guild.id,
-        )
+        if self.node.is_connected:
+            await self._node.send(
+                method="DELETE",
+                path=self._player_endpoint_uri,
+                guild_id=self._guild.id,
+            )
 
         self._log.debug("Player has been destroyed.")
 
     async def play(
         self, track: Track, *, start: int = 0, end: int = 0, ignore_if_playing: bool = False
     ) -> Track:
         """Plays a track. If a Spotify track is passed in, it will be handled accordingly."""
```

### Comparing `pomice-2.5.1/pomice/pool.py` & `pomice-2.6.0/pomice/pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 from typing import Optional
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import Union
 from urllib.parse import quote
 
 import aiohttp
+import orjson as json
 from discord import Client
 from discord.ext import commands
 from discord.utils import MISSING
+from websockets import client
+from websockets import exceptions
+from websockets import typing as wstype
 
 from . import __version__
 from . import applemusic
 from . import spotify
 from .enums import *
 from .enums import LogLevel
 from .exceptions import AppleMusicNotEnabled
@@ -67,14 +71,16 @@
         "_bot_user",
         "_host",
         "_port",
         "_pool",
         "_password",
         "_identifier",
         "_heartbeat",
+        "_resume_key",
+        "_resume_timeout",
         "_secure",
         "_fallback",
         "_log_level",
         "_websocket_uri",
         "_rest_uri",
         "_session",
         "_websocket",
@@ -102,15 +108,17 @@
         pool: Type[NodePool],
         bot: commands.Bot,
         host: str,
         port: int,
         password: str,
         identifier: str,
         secure: bool = False,
-        heartbeat: int = 30,
+        heartbeat: int = 60,
+        resume_key: Optional[str] = None,
+        resume_timeout: int = 60,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         session: Optional[aiohttp.ClientSession] = None,
         spotify_client_id: Optional[str] = None,
         spotify_client_secret: Optional[str] = None,
         apple_music: bool = False,
         fallback: bool = False,
         log_level: LogLevel = LogLevel.INFO,
@@ -122,25 +130,27 @@
         self._bot: commands.Bot = bot
         self._host: str = host
         self._port: int = port
         self._pool: Type[NodePool] = pool
         self._password: str = password
         self._identifier: str = identifier
         self._heartbeat: int = heartbeat
+        self._resume_key: Optional[str] = resume_key
+        self._resume_timeout: int = resume_timeout
         self._secure: bool = secure
         self._fallback: bool = fallback
         self._log_level: LogLevel = log_level
         self._log_handler = log_handler
 
         self._websocket_uri: str = f"{'wss' if self._secure else 'ws'}://{self._host}:{self._port}"
         self._rest_uri: str = f"{'https' if self._secure else 'http'}://{self._host}:{self._port}"
 
         self._session: aiohttp.ClientSession = session  # type: ignore
         self._loop: asyncio.AbstractEventLoop = loop or asyncio.get_event_loop()
-        self._websocket: aiohttp.ClientWebSocketResponse
+        self._websocket: client.WebSocketClientProtocol
         self._task: asyncio.Task = None  # type: ignore
 
         self._session_id: Optional[str] = None
         self._available: bool = False
         self._version: LavalinkVersion = LavalinkVersion(0, 0, 0)
 
         self._route_planner = RoutePlanner(self)
@@ -201,15 +211,15 @@
     def bot(self) -> Client:
         """Property which returns the discord.py client linked to this node"""
         return self._bot
 
     @property
     def player_count(self) -> int:
         """Property which returns how many players are connected to this node"""
-        return len(self.players)
+        return len(self.players.values())
 
     @property
     def pool(self) -> Type[NodePool]:
         """Property which returns the pool this node is apart of"""
         return self._pool
 
     @property
@@ -312,55 +322,73 @@
         new_node = random.choice(nodes)
 
         for player in self.players.copy().values():
             await player._swap_node(new_node=new_node)
 
         await self.disconnect()
 
-    async def _listen(self) -> None:
-        backoff = ExponentialBackoff(base=7)
+    async def _configure_resuming(self) -> None:
+        if self._resume_key:
+            data = {"resumingKey": self._resume_key, "timeout": self._resume_timeout}
+            await self.send(
+                method="PATCH",
+                path=f"sessions/{self._session_id}",
+                include_version=True,
+                data=data,
+            )
 
+    async def _listen(self) -> None:
         while True:
-            msg = await self._websocket.receive()
-            if msg.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
+            try:
+                msg = await self._websocket.recv()
+                data = json.loads(msg)
+                self._log.debug(f"Recieved raw websocket message {msg}")
+                self._loop.create_task(self._handle_ws_msg(data=data))
+            except exceptions.ConnectionClosed:
+                if self.player_count > 0:
+                    for _player in self.players.values():
+                        self._loop.create_task(_player.destroy())
+
                 if self._fallback:
-                    await self._handle_node_switch()
+                    self._loop.create_task(self._handle_node_switch())
+
+                self._loop.create_task(self._websocket.close())
+
+                backoff = ExponentialBackoff(base=7)
                 retry = backoff.delay()
+                self._log.debug(f"Retrying connection to Node {self._identifier} in {retry} secs")
                 await asyncio.sleep(retry)
+
                 if not self.is_connected:
                     self._loop.create_task(self.connect(reconnect=True))
-            else:
-                self._loop.create_task(self._handle_payload(msg.json()))
 
-    async def _handle_payload(self, data: dict) -> None:
+    async def _handle_ws_msg(self, data: dict) -> None:
+        self._log.debug(f"Recieved raw payload from Node {self._identifier} with data {data}")
         op = data.get("op", None)
-        if not op:
-            return
 
         if op == "stats":
             self._stats = NodeStats(data)
             return
 
         if op == "ready":
             self._session_id = data["sessionId"]
+            await self._configure_resuming()
 
         if not "guildId" in data:
             return
 
-        player = self._players.get(int(data["guildId"]))
+        player: Optional[Player] = self._players.get(int(data["guildId"]))
         if not player:
             return
 
         if op == "event":
-            await player._dispatch_event(data)
-            return
+            return await player._dispatch_event(data)
 
         if op == "playerUpdate":
-            await player._update_state(data)
-            return
+            return await player._update_state(data)
 
     async def send(
         self,
         method: str,
         path: str,
         include_version: bool = True,
         guild_id: Optional[Union[int, str]] = None,
@@ -438,23 +466,25 @@
                 await self._handle_version_check(version=version)
                 await self._set_ext_client_session(session=self._session)
 
                 self._log.debug(
                     f"Version check from Node {self._identifier} successful. Returned version {version}",
                 )
 
-            self._websocket = await self._session.ws_connect(
+            self._websocket = await client.connect(
                 f"{self._websocket_uri}/v{self._version.major}/websocket",
-                headers=self._headers,
-                heartbeat=self._heartbeat,
+                extra_headers=self._headers,
+                ping_interval=self._heartbeat,
             )
 
             if reconnect:
-                for player in self.players.values():
-                    await player._refresh_endpoint_uri(self._session_id)
+                self._log.debug(f"Trying to reconnect to Node {self._identifier}...")
+                if self.player_count:
+                    for player in self.players.values():
+                        await player._refresh_endpoint_uri(self._session_id)
 
             self._log.debug(
                 f"Node {self._identifier} successfully connected to websocket using {self._websocket_uri}/v{self._version.major}/websocket",
             )
 
             if not self._task:
                 self._task = self._loop.create_task(self._listen())
@@ -462,23 +492,23 @@
             self._available = True
 
             end = time.perf_counter()
 
             self._log.info(f"Connected to node {self._identifier}. Took {end - start:.3f}s")
             return self
 
-        except (aiohttp.ClientConnectorError, ConnectionRefusedError):
+        except (aiohttp.ClientConnectorError, OSError, ConnectionRefusedError):
             raise NodeConnectionFailure(
                 f"The connection to node '{self._identifier}' failed.",
             ) from None
-        except aiohttp.WSServerHandshakeError:
+        except exceptions.InvalidHandshake:
             raise NodeConnectionFailure(
                 f"The password for node '{self._identifier}' is invalid.",
             ) from None
-        except aiohttp.InvalidURL:
+        except exceptions.InvalidURI:
             raise NodeConnectionFailure(
                 f"The URI for node '{self._identifier}' is invalid.",
             ) from None
 
     async def disconnect(self) -> None:
         """Disconnects a connected Lavalink node and removes it from the node pool.
         This also destroys any players connected to the node.
@@ -927,14 +957,16 @@
         bot: commands.Bot,
         host: str,
         port: int,
         password: str,
         identifier: str,
         secure: bool = False,
         heartbeat: int = 30,
+        resume_key: Optional[str] = None,
+        resume_timeout: int = 60,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         spotify_client_id: Optional[str] = None,
         spotify_client_secret: Optional[str] = None,
         session: Optional[aiohttp.ClientSession] = None,
         apple_music: bool = False,
         fallback: bool = False,
         log_level: LogLevel = LogLevel.INFO,
@@ -953,14 +985,16 @@
             bot=bot,
             host=host,
             port=port,
             password=password,
             identifier=identifier,
             secure=secure,
             heartbeat=heartbeat,
+            resume_key=resume_key,
+            resume_timeout=resume_timeout,
             loop=loop,
             spotify_client_id=spotify_client_id,
             session=session,
             spotify_client_secret=spotify_client_secret,
             apple_music=apple_music,
             fallback=fallback,
             log_level=log_level,
```

### Comparing `pomice-2.5.1/pomice/queue.py` & `pomice-2.6.0/pomice/queue.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/routeplanner.py` & `pomice-2.6.0/pomice/routeplanner.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/spotify/client.py` & `pomice-2.6.0/pomice/spotify/client.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/spotify/objects.py` & `pomice-2.6.0/pomice/spotify/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice/utils.py` & `pomice-2.6.0/pomice/utils.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/pomice.egg-info/PKG-INFO` & `pomice-2.6.0/pomice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.5.1
+Version: 2.6.0
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.5.1/pomice.egg-info/SOURCES.txt` & `pomice-2.6.0/pomice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pomice-2.5.1/setup.py` & `pomice-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # type: ignore
 import re
 
 import setuptools
 
 version = ""
-requirements = ["aiohttp>=3.7.4,<4", "orjson"]
+requirements = ["aiohttp>=3.7.4,<4", "orjson", "websockets"]
 with open("pomice/__init__.py") as f:
     version = re.search(
         r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
         f.read(),
         re.MULTILINE,
     ).group(1)
```

