# Comparing `tmp/nsdotpy-1.1.1.tar.gz` & `tmp/nsdotpy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.1.1.tar", max compression
+gzip compressed data, was "nsdotpy-1.1.3.tar", max compression
```

## Comparing `nsdotpy-1.1.1.tar` & `nsdotpy-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.1.1/LICENSE.md
--rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.1.1/nsdotpy/__init__.py
--rw-r--r--   0        0        0    32154 2023-05-06 07:46:35.968122 nsdotpy-1.1.1/nsdotpy/session.py
--rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.1.1/nsdotpy/valid_tags.py
--rw-r--r--   0        0        0      665 2023-05-06 07:45:43.726513 nsdotpy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      738 2023-05-06 07:51:44.902801 nsdotpy-1.1.1/README.md
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 nsdotpy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.1.3/LICENSE.md
+-rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.1.3/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    36937 2023-05-08 03:40:29.548242 nsdotpy-1.1.3/nsdotpy/session.py
+-rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.1.3/nsdotpy/valid_tags.py
+-rw-r--r--   0        0        0      667 2023-05-08 03:44:44.215911 nsdotpy-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2454 2023-05-08 03:53:02.121422 nsdotpy-1.1.3/README.md
+-rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 nsdotpy-1.1.3/PKG-INFO
```

### Comparing `nsdotpy-1.1.1/LICENSE.md` & `nsdotpy-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.1/nsdotpy/__init__.py` & `nsdotpy-1.1.3/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.1/nsdotpy/session.py` & `nsdotpy-1.1.3/nsdotpy/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,20 +10,26 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with NSDotPy. If not, see <https://www.gnu.org/licenses/>.
 
+# standard library imports
 import time  # for ratelimiting and userclick
 import logging  # for logging
+import mimetypes  # for flag and banner uploading
+
+# external library imports
 import keyboard  # for the required user input
 import requests  # for http stuff
 from tendo.singleton import SingleInstance  # so it can only be run once at a time
 from bs4 import BeautifulSoup  # for parsing html and xml
+
+# local imports
 from . import valid_tags  # for valid region tags
 
 
 def canonicalize(string: str) -> str:
     """Converts a string to its canonical form used by the nationstates api.
 
     Args:
@@ -55,15 +61,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.1.1"
+        self.VERSION = "1.1.3"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -84,15 +90,20 @@
         self.pin: str = ""
         self.nation: str = ""
         self.region: str = ""
         self.keybind = keybind
         self.logger.info(f"Initialized. Keybind to continue is {self.keybind}.")
 
     def _set_user_agent(
-        self, script_name, script_version, script_author, script_user, link_to_src
+        self,
+        script_name: str,
+        script_version: str,
+        script_author: str,
+        script_user: str,
+        link_to_src: str,
     ):
         self.user_agent = (
             f"{script_name}/{script_version} (by:{script_author}; usedBy:{script_user})"
         )
         if link_to_src:
             self.user_agent = f"{self.user_agent}; src:{link_to_src}"
         self.user_agent = f"{self.user_agent}; Written with NSDotPy/{self.VERSION} (by:Sweeze; src:github.com/sw33ze/NSDotPy)"
@@ -174,15 +185,15 @@
             if len(value) > max_lengths[key]:
                 raise ValueError(f"{key} is too long, max length is {max_lengths[key]}")
             if len(value) < 2 and key != "slogan":
                 raise ValueError(f"{key} should have a minimum length of 2 characters.")
             # check if pretitle contains any non-alphanumeric characters (except spaces)
             if key == "pretitle" and not value.replace(" ", "").isalnum():
                 raise ValueError(
-                    "Pretitle should only contain alphanumeric characters or space."
+                    "Pretitle should only contain alphanumeric characters or spaces."
                 )
 
     def _html_request(
         self, url, data={}, files=None, allow_redirects=False, auth=None
     ) -> requests.Response:
         data |= {"chk": self.chk, "localid": self.localid}
         userclick = self._wait_for_input(self.keybind)
@@ -342,15 +353,15 @@
         data = {
             "nationname": self.nation,
         }
         files = {
             "file": (
                 flag_filename,
                 open(flag_filename, "rb"),
-                f"image/{flag_filename.lower().split('.')[-1]}",
+                mimetypes.guess_type(flag_filename)[0],
             )
         }
 
         response = self.request(url, data=data, files=files)
 
         if "page=settings" in response.headers["location"]:
             self._refresh_auth_values()
@@ -653,15 +664,15 @@
             "region": self.region,
             "expect": "json",
         }
         files = {
             f"file_upload_r{type}": (
                 filename,
                 open(filename, "rb"),
-                f"image/{filename.lower().split('.')[-1]}",
+                mimetypes.guess_type(filename)[0],
             )
         }
         response = self.request(url, data, files=files)
 
         return response.json()["id"]
 
     def set_flag_and_banner(
@@ -725,14 +736,15 @@
 
         Args:
             target (str): The region to request the embassy with.
 
         Returns:
             bool: Whether the request was successfully sent or not
         """
+        self.logger.info(f"Requesting embassy with {target}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
             "requestembassyregion": target,
             "requestembassy": "1",  # it's silly that requesting needs this but not closing, aborting, or cancelling
         }
         response = self.request(url, data)
         return "Your proposal for the construction of embassies with" in response.text
@@ -742,42 +754,45 @@
 
         Args:
             target (str): The region with which to close the embassy.
 
         Returns:
             bool: Whether the embassy was successfully closed or not
         """
+        self.logger.info(f"Closing embassy with {target}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {"cancelembassyregion": target}
         response = self.request(url, data)
         return " has been scheduled for demolition." in response.text
 
     def abort_embasy(self, target: str) -> bool:
         """Aborts an embassy with a region.
 
         Args:
             target (str): The region with which to abort the embassy.
 
         Returns:
             bool: Whether the embassy was successfully aborted or not
         """
+        self.logger.info(f"Aborting embassy with {target}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {"abortembassyregion": target}
         response = self.request(url, data)
         return " aborted." in response.text
 
     def cancel_embassy(self, target: str) -> bool:
         """Cancels an embassy with a region.
 
         Args:
             target (str): The region with which to cancel the embassy.
 
         Returns:
             bool: Whether the embassy was successfully cancelled or not
         """
+        self.logger.info(f"Cancelling embassy with {target}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {"cancelembassyclosureregion": target}
         response = self.request(url, data)
         return "Embassy closure order cancelled." in response.text
 
     # end methods for embassies
 
@@ -794,20 +809,129 @@
         Returns:
             bool: Whether the tag was successfully added or removed
         """
         if action not in ["add", "remove"]:
             raise ValueError("action must be 'add' or 'remove'")
         if canonicalize(tag) not in valid_tags.tags:
             raise ValueError(f"{tag} is not a valid tag")
+        self.logger.info(f"{action.capitalize()}ing tag {tag} for {self.region}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
             f"{action}_tag": canonicalize(tag),
             "updatetagsbutton": "1",
         }
         response = self.request(url, data)
         return "Region Tags updated!" in response.text
 
     # end methods for region control
 
+    def junk_card(self, id: str, season: str) -> bool:
+        """Junks a card from the current nation's deck.
+
+        Args:
+            id (str): ID of the card to junk
+            season (str): Season of the card to junk
+
+        Returns:
+            bool: Whether the card was successfully junked or not
+        """
+        self.logger.info(f"Junking card {id} from season {season}")
+        url = "https://www.nationstates.net/template-overall=none/page=deck"
+
+        data = {"page": "ajax3", "a": "junkcard", "card": id, "season": season}
+        response = self.request(url, data)
+
+        return "Your Deck" in response.text
+
+    #    def open_pack(self) -> bool:
+    #        """Opens a card pack.
+    #
+    #        Returns:
+    #            bool: Whether the pack was successfully opened or not
+    #        """
+    #        cards = []
+    #        self.logger.info(f"Opening pack {each} of {count}")
+    #        url = "https://www.nationstates.net/template-overall=none/page=deck"
+    #
+    #        data = {"open_loot_box": "1"}
+    #        response = self.request(url, data)
+    #        return "Tap cards to reveal..." in response.text
+    #
+    #    def ask(self, price: str, card_id: str, season: str) -> bool:
+    #        """Asks a price on a card in a season
+    #
+    #        Args:
+    #            price (str): Price to ask
+    #            card_id (str): ID of the card
+    #            season (str): Season of the card
+    #
+    #        Returns:
+    #            bool: Whether theask was successfully lodged or not
+    #        """
+    #        self.logger.info(f"Asking for {price} on {card_id} season {season}")
+    #        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+    #
+    #        data = {"auction_ask": price, "auction_submit": ask}
+    #        response = self.request(url, data)
+    #        return f"Your ask of {price} has been lodged." in response.text
+    #
+    #    def bid(self, price: str, card_id: str, season: str) -> bool:
+    #        """Places a bid on a card in a season
+    #
+    #        Args:
+    #            price (str): Amount of bank to bid
+    #            card_id (str): ID of the card
+    #            season (str): Season of the card
+    #
+    #        Returns:
+    #            bool: Whether the bid was successfully lodged or not
+    #        """
+    #        self.logger.info(f"Putting a bid for {price} on {card_id} season {season}")
+    #        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+    #
+    #        data = {"auction_bid": price, "auction_submit": bid}
+    #        response = self.request(url, data)
+    #
+    #        return f"Your bid of {price} has been lodged." in response.text
+
+    def remove_ask(self, price: str, card_id: str, season: str) -> bool:
+        """Removes an ask on card_id in season at price
+
+        Args:
+            price (str): Price of the ask to remove
+            card_id (str): ID of the card
+            season (str): Season of the card
+
+        Returns:
+            bool: Whether the ask was successfully removed or not
+        """
+
+        self.logger.info(f"removing an ask for {price} on {card_id} season {season}")
+        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+
+        data = {"new_price": price, "remove_ask_price": price}
+        response = self.request(url, data)
+        return f"Removed your ask for {price}" in response.text
+
+    def remove_bid(self, price: str, card_id: str, season: str) -> bool:
+        """Removes a big on a card
+
+        Args:
+            price (str): Price of the bid to remove
+            card_id (str): ID of the card
+            season (str): Season of the card
+
+        Returns:
+            bool: Whether the bid was successfully removed or not
+        """
+
+        self.logger.info(f"Removing a bid for {price} on {card_id} season {season}")
+        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+
+        data = {"new_price": price, "remove_bid_price": price}
+        response = self.request(url, data)
+
+        return f"Removed your bid for {price}" in response.text
+
 
 if __name__ == "__main__":
     print("this is a module/library, not a script")
```

### Comparing `nsdotpy-1.1.1/nsdotpy/valid_tags.py` & `nsdotpy-1.1.3/nsdotpy/valid_tags.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.1/pyproject.toml` & `nsdotpy-1.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.1.1"
+version = "1.1.3"
 description = "A wrapper around requests that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
@@ -16,8 +16,8 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pdoc = "^13.1.1"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

