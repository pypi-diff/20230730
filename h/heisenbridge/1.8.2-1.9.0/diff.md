# Comparing `tmp/heisenbridge-1.8.2.tar.gz` & `tmp/heisenbridge-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heisenbridge-1.8.2.tar", last modified: Fri Dec 24 19:30:27 2021, max compression
+gzip compressed data, was "heisenbridge-1.9.0.tar", last modified: Wed Dec 29 19:14:17 2021, max compression
```

## Comparing `heisenbridge-1.8.2.tar` & `heisenbridge-1.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 19:30:27.352747 heisenbridge-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11558 2021-12-24 19:30:27.352747 heisenbridge-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11185 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 19:30:27.352747 heisenbridge-1.8.2/heisenbridge/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25064 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/appservice.py
--rw-r--r--   0 runner    (1001) docker     (121)    21859 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/channel_room.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/command_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    22028 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/control_room.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/event_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/identd.py
--rw-r--r--   0 runner    (1001) docker     (121)     9224 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/irc.py
--rw-r--r--   0 runner    (1001) docker     (121)    64009 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/network_room.py
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    14658 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/plumbed_room.py
--rw-r--r--   0 runner    (1001) docker     (121)    22535 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/private_room.py
--rw-r--r--   0 runner    (1001) docker     (121)    15032 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/room.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/heisenbridge/version.py
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 19:30:27.352747 heisenbridge-1.8.2/heisenbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11558 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      853 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-24 19:30:27.000000 heisenbridge-1.8.2/heisenbridge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 19:30:27.352747 heisenbridge-1.8.2/logo/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/logo/heisenbridge-dark-transparent.png
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/logo/heisenbridge-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/logo/heisenbridge-light-transparent.png
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/logo/heisenbridge-light.png
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/logo/heisenbridge.svg
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-12-24 19:30:27.356747 heisenbridge-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-12-24 19:30:23.000000 heisenbridge-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 19:14:17.950409 heisenbridge-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11633 2021-12-29 19:14:17.950409 heisenbridge-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11260 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 19:14:17.950409 heisenbridge-1.9.0/heisenbridge/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28074 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1581 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/appservice.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22284 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/channel_room.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/command_parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22028 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/control_room.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3393 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/event_queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/identd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9680 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/irc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67591 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/network_room.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4847 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14658 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/plumbed_room.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23439 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/private_room.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15565 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/room.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5504 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/space_room.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/heisenbridge/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 19:14:17.950409 heisenbridge-1.9.0/heisenbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11633 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-29 19:14:17.000000 heisenbridge-1.9.0/heisenbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 19:14:17.950409 heisenbridge-1.9.0/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/logo/heisenbridge-dark-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/logo/heisenbridge-dark.png
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/logo/heisenbridge-light-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/logo/heisenbridge-light.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4457 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/logo/heisenbridge.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2021-12-29 19:14:17.954409 heisenbridge-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-12-29 19:14:15.000000 heisenbridge-1.9.0/setup.py
```

### Comparing `heisenbridge-1.8.2/LICENSE` & `heisenbridge-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/PKG-INFO` & `heisenbridge-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heisenbridge
-Version: 1.8.2
+Version: 1.9.0
 Summary: a bouncer-style Matrix IRC bridge
 Home-page: https://github.com/hifi/heisenbridge
 Author: Toni Spets (hifi)
 Author-email: toni.spets@iki.fi
 License: MIT license
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -49,14 +49,15 @@
 * smart message formatting from Matrix to IRC using IRC conventions
 * smart message edits from Matrix to IRC by sending only corrections
 * automatic identify/auth with server password or automatic command on connect
 * SASL plain authentication
 * CertFP authentication
 * CTCP support
 * SOCKS proxy configuration per server
+* bridge managed spaces to organize your channels and PMs within a network
 
 Comparison
 ----------
 
 To help understand where Heisenbridge is a good fit here's a feature matrix of some of the key differences between other popular solutions:
 
 |                         | Matrix |  IRC | Appservice | Ratelimit | Self-host | Permissions  |
```

### Comparing `heisenbridge-1.8.2/README.md` & `heisenbridge-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 * smart message formatting from Matrix to IRC using IRC conventions
 * smart message edits from Matrix to IRC by sending only corrections
 * automatic identify/auth with server password or automatic command on connect
 * SASL plain authentication
 * CertFP authentication
 * CTCP support
 * SOCKS proxy configuration per server
+* bridge managed spaces to organize your channels and PMs within a network
 
 Comparison
 ----------
 
 To help understand where Heisenbridge is a good fit here's a feature matrix of some of the key differences between other popular solutions:
 
 |                         | Matrix |  IRC | Appservice | Ratelimit | Self-host | Permissions  |
```

### Comparing `heisenbridge-1.8.2/heisenbridge/__main__.py` & `heisenbridge-1.9.0/heisenbridge/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 from mautrix.api import Path
 from mautrix.api import SynapseAdminPath
 from mautrix.appservice import AppService as MauService
 from mautrix.appservice.state_store import ASStateStore
 from mautrix.client.state_store.memory import MemoryStateStore
 from mautrix.errors import MatrixRequestError
 from mautrix.errors import MForbidden
+from mautrix.errors import MUserInUse
 from mautrix.types import Membership
 from mautrix.util.config import yaml
 
 from heisenbridge import __version__
 from heisenbridge.appservice import AppService
 from heisenbridge.channel_room import ChannelRoom
 from heisenbridge.control_room import ControlRoom
 from heisenbridge.identd import Identd
 from heisenbridge.network_room import NetworkRoom
 from heisenbridge.plumbed_room import PlumbedRoom
 from heisenbridge.private_room import PrivateRoom
 from heisenbridge.room import Room
 from heisenbridge.room import RoomInvalidError
+from heisenbridge.space_room import SpaceRoom
 
 
 class MemoryBridgeStateStore(ASStateStore, MemoryStateStore):
     def __init__(self) -> None:
         ASStateStore.__init__(self)
         MemoryStateStore.__init__(self)
 
@@ -96,24 +98,48 @@
     def strip_nick(self, nick: str) -> Tuple[str, str]:
         m = re.match(r"^([~&@%\+]?)(.+)$", nick)
         if m:
             return (m.group(2), (m.group(1) if len(m.group(1)) > 0 else None))
         else:
             raise TypeError(f"Input nick is not valid: '{nick}'")
 
+    def split_irc_user_id(self, user_id):
+        (name, server) = user_id.split(":")
+
+        network = None
+        nick = None
+
+        if server != self.server_name:
+            return None, None
+
+        print(name, self.puppet_prefix)
+
+        if not name.startswith("@" + self.puppet_prefix):
+            return None, None
+
+        network_nick = name[len(self.puppet_prefix) + 1 :]
+
+        m = re.match(r"([^" + self.puppet_separator + r"]+).(.+)$", network_nick)
+
+        if m:
+            network = re.sub(r"=([0-9a-z]{2})", lambda m: bytes.fromhex(m.group(1)).decode("utf-8"), m.group(1)).lower()
+            nick = re.sub(r"=([0-9a-z]{2})", lambda m: bytes.fromhex(m.group(1)).decode("utf-8"), m.group(2)).lower()
+
+        return network, nick
+
     def nick_from_irc_user_id(self, network, user_id):
         (name, server) = user_id.split(":")
 
         if server != self.server_name:
             return None
 
         prefix = "@" + re.sub(
             r"[^0-9a-z\-\.=\_/]",
             lambda m: "=" + m.group(0).encode("utf-8").hex(),
-            f"{self.puppet_prefix}{network}_".lower(),
+            f"{self.puppet_prefix}{network}{self.puppet_separator}".lower(),
         )
 
         if not name.startswith(prefix):
             return None
 
         nick = name[len(prefix) :]
         nick = re.sub(r"=([0-9a-z]{2})", lambda m: bytes.fromhex(m.group(1)).decode("utf-8"), nick)
@@ -181,50 +207,61 @@
             except Exception:
                 logging.exception("Ignoring exception from room handler. This should be fixed.")
         elif (
             str(event.type) == "m.room.member"
             and event.sender != self.user_id
             and event.content.membership == Membership.INVITE
         ):
+            if not self.is_user(event.sender):
+                logging.info(f"Non-whitelisted user {event.sender} tried to invite us, ignoring.")
+                return
+            else:
+                logging.info(f"Got an invite from {event.sender}")
+
             if not event.content.is_direct:
                 logging.debug("Got an invite to non-direct room, ignoring")
                 return
 
-            logging.info(f"Got an invite from {event.sender}")
-
-            # only respond to an invite
+            # only respond to invites unknown new rooms
             if event.room_id in self._rooms:
-                logging.debug("Control room already open, uhh")
+                logging.debug("Got an invite to room we're already in, ignoring")
                 return
 
             # handle invites against puppets
             if event.state_key != self.user_id:
                 logging.info(f"Whitelisted user {event.sender} invited {event.state_key}, going to reject.")
 
                 try:
                     await self.az.intent.user(event.state_key).kick_user(
                         event.room_id,
                         event.state_key,
-                        "Inviting puppets is not supported",
+                        "Will invite YOU instead",
                     )
                 except Exception:
                     logging.exception("Failed to reject invitation.")
 
+                (network, nick) = self.split_irc_user_id(event.state_key)
+
+                if network is not None and nick is not None:
+                    for room in self.find_rooms(NetworkRoom, event.sender):
+                        if room.name.lower() == network.lower():
+                            logging.debug(
+                                "Found matching network room ({network}) for {event.sender}, emulating query command for {nick}"
+                            )
+                            await room.cmd_query(argparse.Namespace(nick=nick, message=[]))
+                            break
+
                 return
 
             # set owner if we have none and the user is from the same HS
             if self.config.get("owner", None) is None and event.sender.endswith(":" + self.server_name):
                 logging.info(f"We have an owner now, let us rejoice, {event.sender}!")
                 self.config["owner"] = event.sender
                 await self.save()
 
-            if not self.is_user(event.sender):
-                logging.info(f"Non-whitelisted user {event.sender} tried to invite us, ignoring.")
-                return
-
             logging.info(f"Whitelisted user {event.sender} invited us, going to accept.")
 
             # accept invite sequence
             try:
                 room = ControlRoom(id=event.room_id, user_id=event.sender, serv=self, members=[event.sender], bans=[])
                 await room.save()
                 self.register_room(room)
@@ -382,16 +419,34 @@
         self.puppet_separator = m.group(2)
         self.puppet_prefix = m.group(1) + self.puppet_separator
 
         print(f"Heisenbridge v{__version__}", flush=True)
         if safe_mode:
             print("Safe mode is enabled.", flush=True)
 
-        # mautrix migration requires us to call whoami manually at this point
         self.api = HTTPAPI(base_url=homeserver_url, token=self.registration["as_token"])
+
+        # conduit requires that the appservice user is registered before whoami
+        try:
+            await self.api.request(
+                Method.POST,
+                Path.register,
+                {
+                    "type": "m.login.application_service",
+                    "username": self.registration["sender_localpart"],
+                },
+            )
+            logging.debug("Appservice user registration succeeded.")
+        except MUserInUse:
+            logging.debug("Appservice user is already registered.")
+        except Exception:
+            logging.exception("Unexpected failure when registering appservice user.")
+            return
+
+        # mautrix migration requires us to call whoami manually at this point
         whoami = await self.api.request(Method.GET, Path.account.whoami)
 
         logging.info("We are " + whoami["user_id"])
 
         self.user_id = whoami["user_id"]
         self.server_name = self.user_id.split(":")[1]
 
@@ -423,14 +478,15 @@
         self.config = {
             "networks": {},
             "owner": None,
             "allow": {},
             "idents": {},
             "member_sync": "half",
             "media_url": None,
+            "namespace": self.puppet_prefix,
         }
         logging.debug(f"Default config: {self.config}")
         self.synapse_admin = False
 
         try:
             is_admin = await self.api.request(Method.GET, SynapseAdminPath.v1.users[self.user_id].admin)
             self.synapse_admin = is_admin["admin"]
@@ -463,31 +519,40 @@
 
             if len(new_servers) > 0:
                 logging.debug("Migrating servers from old to new config format")
                 network["servers"] = new_servers
 
         logging.debug(f"Merged configuration from HS: {self.config}")
 
+        # prevent starting bridge with changed namespace
+        if self.config["namespace"] != self.puppet_prefix:
+            logging.error(
+                f"Previously used namespace '{self.config['namespace']}' does not match current '{self.puppet_prefix}'."
+            )
+            sys.exit(1)
+
         # honor command line owner
         if owner is not None and self.config["owner"] != owner:
             logging.info(f"Overriding loaded owner with '{owner}'")
             self.config["owner"] = owner
-            await self.save()
+
+        # always ensure our merged and migrated configuration is up-to-date
+        await self.save()
 
         print("Fetching joined rooms...", flush=True)
 
         joined_rooms = await self.az.intent.get_joined_rooms()
         logging.debug(f"Appservice rooms: {joined_rooms}")
 
         print(f"Bridge is in {len(joined_rooms)} rooms, initializing them...", flush=True)
 
         Room.init_class(self.az)
 
         # room types and their init order, network must be before chat and group
-        room_types = [ControlRoom, NetworkRoom, PrivateRoom, ChannelRoom, PlumbedRoom]
+        room_types = [ControlRoom, NetworkRoom, PrivateRoom, ChannelRoom, PlumbedRoom, SpaceRoom]
 
         room_type_map = {}
         for room_type in room_types:
             room_type_map[room_type.__name__] = room_type
 
         # import all rooms
         for room_id in joined_rooms:
@@ -535,17 +600,30 @@
                 if safe_mode:
                     print("Safe mode enabled, not leaving room.", flush=True)
                 else:
                     await self.leave_room(room_id, joined.keys())
 
         print("All valid rooms initialized, connecting network rooms...", flush=True)
 
-        # connect network rooms one by one, this may take a while
         wait = 1
-        for room in self._rooms.values():
+        for room in list(self._rooms.values()):
+            await room.post_init()
+
+            # check again if we're still valid
+            if not room.is_valid():
+                logging.debug(f"Room {room.id} failed validation after post init, leaving.")
+
+                self.unregister_room(room.id)
+
+                if not safe_mode:
+                    await self.leave_room(room.id, room.members)
+
+                continue
+
+            # connect network rooms one by one, this may take a while
             if type(room) == NetworkRoom and room.connected:
 
                 def sync_connect(room):
                     asyncio.ensure_future(room.connect())
 
                 asyncio.get_event_loop().call_later(wait, sync_connect, room)
                 wait += 1
```

### Comparing `heisenbridge-1.8.2/heisenbridge/appservice.py` & `heisenbridge-1.9.0/heisenbridge/appservice.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/channel_room.py` & `heisenbridge-1.9.0/heisenbridge/channel_room.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,21 @@
 
         if "member_sync" in config:
             self.member_sync = config["member_sync"]
 
         if "autocmd" in config:
             self.autocmd = config["autocmd"]
 
+        # initialize lazy members dict if sync is not off
+        if self.member_sync != "off":
+            if self.lazy_members is None:
+                self.lazy_members = {}
+        else:
+            self.lazy_members = None
+
     def to_config(self) -> dict:
         return {**(super().to_config()), "key": self.key, "member_sync": self.member_sync, "autocmd": self.autocmd}
 
     @staticmethod
     def create(network: NetworkRoom, name: str) -> "ChannelRoom":
         logging.debug(f"ChannelRoom.create(network='{network.name}', name='{name}'")
 
@@ -192,14 +199,18 @@
             [self.network.user_id],
         )
         self.serv.register_room(self)
         await self.save()
         # start event queue now that we have an id
         self._queue.start()
 
+        # attach to network space
+        if self.network.space:
+            await self.network.space.attach(self.id)
+
     def is_valid(self) -> bool:
         if not self.in_room(self.user_id):
             return False
 
         return super().is_valid()
 
     def cleanup(self) -> None:
@@ -235,15 +246,15 @@
             await self.save()
         elif args.full:
             self.member_sync = "full"
             await self.save()
         elif args.off:
             self.member_sync = "off"
             # prevent anyone already in lazy list to be invited
-            self.lazy_members = {}
+            self.lazy_members = None
             await self.save()
 
         self.send_notice(f"Member sync is set to {self.member_sync}", forward=args._forward)
 
     async def cmd_mode(self, args) -> None:
         self.network.conn.mode(self.name, " ".join(args.args))
 
@@ -313,14 +324,17 @@
         to_add = []
         names = list(self.names_buffer)
         self.names_buffer = []
         modes: Dict[str, List[str]] = {}
         others = []
         on_channel = []
 
+        # always reset lazy list because it can be toggled on-the-fly
+        self.lazy_members = {} if self.member_sync != "off" else None
+
         # build to_remove list from our own puppets
         for member in self.members:
             (name, server) = member.split(":")
 
             if name.startswith("@" + self.serv.puppet_prefix) and server == self.serv.server_name:
                 to_remove.append(member)
 
@@ -354,14 +368,18 @@
                 to_remove.remove(irc_user_id)
                 continue
 
             # if this user is not in room, add to invite list
             if not self.in_room(irc_user_id):
                 to_add.append((irc_user_id, nick))
 
+            # always put everyone in the room to lazy list if we have any member sync
+            if self.lazy_members is not None:
+                self.lazy_members[irc_user_id] = nick
+
         # never remove us or appservice
         if self.serv.user_id in to_remove:
             to_remove.remove(self.serv.user_id)
         if self.user_id in to_remove:
             to_remove.remove(self.user_id)
 
         self.send_notice(
@@ -393,25 +411,19 @@
             self.send_notice(f"Users with '{mode}': {', '.join(nicks)}")
 
         # show everyone else
         if len(others) > 0:
             others = sorted(others, key=str.casefold)
             self.send_notice(f"Users: {', '.join(others)}")
 
-        # always reset lazy list because it can be toggled on-the-fly
-        self.lazy_members = {}
-
         if self.member_sync == "full":
             for (irc_user_id, nick) in to_add:
                 self._add_puppet(nick)
         else:
             self.send_notice(f"Member sync is set to {self.member_sync}, skipping invites.")
-            if self.member_sync != "off":
-                for (irc_user_id, nick) in to_add:
-                    self.lazy_members[irc_user_id] = nick
 
         for irc_user_id in to_remove:
             self._remove_puppet(irc_user_id)
 
         # trust the names reply is always up-to-date
         self.on_channel = on_channel
```

### Comparing `heisenbridge-1.8.2/heisenbridge/command_parse.py` & `heisenbridge-1.9.0/heisenbridge/command_parse.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/control_room.py` & `heisenbridge-1.9.0/heisenbridge/control_room.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/event_queue.py` & `heisenbridge-1.9.0/heisenbridge/event_queue.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/identd.py` & `heisenbridge-1.9.0/heisenbridge/identd.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/irc.py` & `heisenbridge-1.9.0/heisenbridge/irc.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         server,
         port,
         nickname,
         password=None,
         username=None,
         ircname=None,
         connect_factory=AioFactory(),
+        sasl_mechanism=None,
         sasl_username=None,
         sasl_password=None,
     ):
         if self.connected:
             self.disconnect("Changing servers")
 
         self.buffer = self.buffer_class()
@@ -154,14 +155,15 @@
         self.server = server
         self.port = port
         self.server_address = (server, port)
         self.nickname = nickname
         self.username = username or nickname
         self.ircname = ircname or nickname
         self.password = password
+        self.sasl_mechanism = sasl_mechanism
         self.sasl_username = sasl_username
         self.sasl_password = sasl_password
         self.connect_factory = connect_factory
 
         protocol_instance = self.protocol_class(self, self.reactor.loop)
         connection = self.connect_factory(protocol_instance, self.server_address)
         transport, protocol = await connection
@@ -172,30 +174,37 @@
         self.connected = True
         self._task = asyncio.ensure_future(self._run())
         self.reactor._on_connect(self.protocol, self.transport)
         return self
 
     async def register(self):
         # SASL stuff
-        if self.sasl_username is not None and self.sasl_password is not None:
+        sasl_creds = self.sasl_username is not None and self.sasl_password is not None
+        if (self.sasl_mechanism == "plain" and sasl_creds) or self.sasl_mechanism == "external":
             self.cap("REQ", "sasl")
 
             try:
                 (connection, event) = await self.expect("cap")
                 if not event.arguments or event.arguments[0] != "ACK":
                     raise ServerConnectionError("SASL requested but not supported by server.")
 
-                self.send_items("AUTHENTICATE PLAIN")
+                if self.sasl_mechanism == "plain":
+                    self.send_items("AUTHENTICATE PLAIN")
+                else:
+                    self.send_items("AUTHENTICATE EXTERNAL")
 
                 (connection, event) = await self.expect("authenticate")
                 if event.target != "+":
                     raise ServerConnectionError("SASL AUTHENTICATE was rejected.")
 
-                sasl = f"{self.sasl_username}\0{self.sasl_username}\0{self.sasl_password}"
-                self.send_items("AUTHENTICATE", base64.b64encode(sasl.encode("utf8")).decode("utf8"))
+                if self.sasl_mechanism == "plain":
+                    sasl = f"{self.sasl_username}\0{self.sasl_username}\0{self.sasl_password}"
+                    self.send_items("AUTHENTICATE", base64.b64encode(sasl.encode("utf8")).decode("utf8"))
+                else:
+                    self.send_items("AUTHENTICATE", "+")
                 (connection, event) = await self.expect(["903", "904", "908"])
                 if event.type != "903":
                     raise ServerConnectionError(event.arguments[0])
 
             except asyncio.TimeoutError:
                 raise ServerConnectionError("SASL authentication timed out.")
```

### Comparing `heisenbridge-1.8.2/heisenbridge/network_room.py` & `heisenbridge-1.9.0/heisenbridge/network_room.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from heisenbridge.irc import HeisenReactor
 from heisenbridge.parser import IRCMatrixParser
 from heisenbridge.plumbed_room import PlumbedRoom
 from heisenbridge.private_room import parse_irc_formatting
 from heisenbridge.private_room import PrivateRoom
 from heisenbridge.private_room import unix_to_local
 from heisenbridge.room import Room
+from heisenbridge.space_room import SpaceRoom
 
 
 def connected(f):
     def wrapper(*args, **kwargs):
         self = args[0]
 
         if not self.conn or not self.conn.connected:
@@ -82,14 +83,15 @@
     # configuration stuff
     name: str
     connected: bool
     nick: str
     username: str
     ircname: str
     password: str
+    sasl_mechanism: str
     sasl_username: str
     sasl_password: str
     autocmd: str
     pills_length: int
     pills_ignore: list
     autoquery: bool
     tls_cert: str
@@ -104,22 +106,25 @@
     real_host: str
     real_user: str
     pending_kickbans: Dict[str, List[Tuple[str, str]]]
     backoff: int
     backoff_task: Any
     next_server: int
     connected_at: int
+    space: SpaceRoom
+    post_init_done: bool
 
     def init(self):
         self.name = None
         self.connected = False
         self.nick = None
         self.username = None
         self.ircname = None
         self.password = None
+        self.sasl_mechanism = None
         self.sasl_username = None
         self.sasl_password = None
         self.autocmd = None
         self.pills_length = 2
         self.pills_ignore = []
         self.autoquery = True
         self.allow_ctcp = False
@@ -138,14 +143,16 @@
         self.disconnect = True
         self.real_host = "?" * 63  # worst case default
         self.real_user = "?" * 8  # worst case default
         self.keys = {}  # temp dict of join channel keys
         self.keepnick_task = None  # async task
         self.whois_data = defaultdict(dict)  # buffer for keeping partial whois replies
         self.pending_kickbans = defaultdict(list)
+        self.space = None
+        self.post_init_done = False
 
         cmd = CommandParser(
             prog="NICK",
             description="set/change nickname",
             epilog=(
                 "You can always see your current nickname on the network without arguments.\n"
                 "If connected new nickname will be sent to the server immediately. It may be rejected and an underscore appended"
@@ -196,27 +203,32 @@
             description="set SASL PLAIN credentials",
             epilog=(
                 "If the network supports SASL authentication you can configure them with this command.\n"
                 "\n"
                 "Note: Bridge administrators can trivially see the stored password if they want to.\n"
             ),
         )
+        cmd.add_argument(
+            "--mechanism", choices=["auto", "none", "plain", "external"], help="SASL authentication mechanism"
+        )
         cmd.add_argument("--username", help="SASL username")
         cmd.add_argument("--password", help="SASL password")
         cmd.add_argument("--remove", action="store_true", help="remove stored credentials")
         self.commands.register(cmd, self.cmd_sasl)
 
         cmd = CommandParser(
             prog="CERTFP",
             description="configure CertFP authentication for this network",
             epilog=(
                 "Using the set command requires you to paste a bundled PEM certificate (cert + key) on the next line"
                 " after the command within the same message. The certificate needs to include both the certificate and"
                 " the private key for it to be accepted.\n"
                 "\n"
+                "Some networks (OFTC) may require you to disable the SASL mechanism, see 'SASL -h' how to change it manually.\n"
+                "\n"
                 "OpenSSL generation example (from Libera.Chat guides):\n"
                 "$ openssl req -x509 -new -newkey rsa:4096 -sha256 -days 1096 -nodes -out libera.pem -keyout libera.pem"
             ),
         )
         cmd.add_argument("--set", action="store_true", help="set X509 certificate bundle (PEM)")
         cmd.add_argument("--remove", action="store_true", help="remove stored certificate")
         self.commands.register(cmd, self.cmd_certfp)
@@ -433,14 +445,17 @@
         cmd.add_argument("--disable-kick", dest="kick", action="store_false", help="Disable rejoin on kick")
         cmd.set_defaults(invite=None, kick=None)
         self.commands.register(cmd, self.cmd_rejoin)
 
         cmd = CommandParser(prog="STATUS", description="show current network status")
         self.commands.register(cmd, self.cmd_status)
 
+        cmd = CommandParser(prog="SPACE", description="create a managed Matrix space for this network")
+        self.commands.register(cmd, self.cmd_space)
+
         self.mx_register("m.room.message", self.on_mx_message)
 
     @staticmethod
     async def create(serv, network, user_id, name):
         room_id = await serv.create_room(name, "Network room for {}".format(network), [user_id])
         room = NetworkRoom(room_id, user_id, serv, [serv.user_id, user_id], bans=[])
         room.from_config({"name": network})
@@ -466,14 +481,17 @@
 
         if "ircname" in config:
             self.ircname = config["ircname"]
 
         if "password" in config:
             self.password = config["password"]
 
+        if "sasl_mechanism" in config:
+            self.sasl_mechanism = config["sasl_mechanism"]
+
         if "sasl_username" in config:
             self.sasl_username = config["sasl_username"]
 
         if "sasl_password" in config:
             self.sasl_password = config["sasl_password"]
 
         if "autocmd" in config:
@@ -504,14 +522,15 @@
         return {
             "name": self.name,
             "connected": self.connected,
             "nick": self.nick,
             "username": self.username,
             "ircname": self.ircname,
             "password": self.password,
+            "sasl_mechanism": self.sasl_mechanism,
             "sasl_username": self.sasl_username,
             "sasl_password": self.sasl_password,
             "autocmd": self.autocmd,
             "allow_ctcp": self.allow_ctcp,
             "tls_cert": self.tls_cert,
             "pills_length": self.pills_length,
             "pills_ignore": self.pills_ignore,
@@ -519,20 +538,51 @@
             "rejoin_kick": self.rejoin_kick,
         }
 
     def is_valid(self) -> bool:
         if self.name is None:
             return False
 
-        # if user leaves network room and it's not connected we can clean it up
-        if not self.in_room(self.user_id) and not self.connected:
-            return False
+        # we require user to be in network room or be connected with channels or PMs
+        if not self.in_room(self.user_id):
+
+            # if not connected (or trying to) we can clean up
+            if not self.connected:
+                return False
+
+            # only if post_init has been done and we're connected with no rooms clean up
+            if self.post_init_done and self.connected and len(self.rooms) == 0:
+                return False
 
         return True
 
+    def cleanup(self) -> None:
+        logging.debug(f"Network {self.id} cleaning up")
+
+        # prevent reconnecting ever again
+        self.connected = False
+        self.disconnect = True
+
+        if self.backoff_task:
+            self.backoff_task.cancel()
+            self.backoff_task = None
+            logging.debug("... cancelled backoff task")
+
+        if self.conn:
+            self.conn.disconnect()
+            logging.debug("... disconnected from IRC network")
+
+        if self.space:
+            self.serv.unregister_room(self.space.id)
+            self.space.cleanup()
+            asyncio.ensure_future(self.serv.leave_room(self.space.id, self.space.members))
+            logging.debug("... cleaned up space")
+
+        super().cleanup()
+
     async def show_help(self):
         self.send_notice_html(f"Welcome to the network room for <b>{html.escape(self.name)}</b>!")
 
         try:
             return await self.commands.trigger("HELP")
         except CommandParserError as e:
             return self.send_notice(str(e))
@@ -799,19 +849,23 @@
         if args.remove:
             self.sasl_username = None
             self.sasl_password = None
             await self.save()
             self.send_notice("SASL credentials removed.")
             return
 
-        if args.username is None and args.password is None:
+        if args.mechanism is None and args.username is None and args.password is None:
+            self.send_notice(f"SASL mechanism: {self.sasl_mechanism if self.sasl_mechanism else 'auto'}")
             self.send_notice(f"SASL username: {self.sasl_username}")
             self.send_notice(f"SASL password: {self.sasl_password}")
             return
 
+        if args.mechanism:
+            self.sasl_mechanism = args.mechanism if args.mechanism != "auto" else None
+
         if args.username:
             self.sasl_username = args.username
 
         if args.password:
             self.sasl_password = args.password
 
         await self.save()
@@ -992,36 +1046,53 @@
 
         if len(plumbs) > 0:
             self.send_notice(f"Plumbs: {', '.join(plumbs)}")
 
         if len(pms) > 0:
             self.send_notice(f"PMs: {', '.join(pms)}")
 
+    async def cmd_space(self, args) -> None:
+        if self.space is None:
+            # sync create to prevent race conditions
+            self.space = SpaceRoom.create(
+                self, [room.id for room in self.rooms.values() if type(room) is not PlumbedRoom]
+            )
+
+            # calls the api and attaches rooms
+            self.send_notice("Creating space and inviting you to it.")
+            await self.space.create_finalize()
+        else:
+            self.send_notice(f"Space already exists ({self.space.id}).")
+
     def kickban(self, channel: str, nick: str, reason: str) -> None:
         self.pending_kickbans[nick].append((channel, reason))
         self.conn.whois(f"{nick}")
 
     def _do_kickban(self, channel: str, user_data: Dict[str, str], reason: str) -> None:
         self.conn.mode(channel, f"+b *!*@{user_data['host']}")
         self.conn.kick(channel, user_data["nick"], reason)
 
     async def connect(self) -> None:
+        if not self.is_valid():
+            logging.warning("Trying to connect an invalid network {self.id}, this is likely a dangling network.")
+            return
+
         if self.connlock.locked():
             self.send_notice("Already connecting.")
             return
 
         async with self.connlock:
             if self.conn and self.conn.connected:
                 self.send_notice("Already connected.")
                 return
 
             self.disconnect = False
             await self._connect()
 
-    async def _connect(self) -> None:
+    async def post_init(self) -> None:
         # attach loose sub-rooms to us
         for type in [PrivateRoom, ChannelRoom, PlumbedRoom]:
             for room in self.serv.find_rooms(type, self.user_id):
                 if room.name not in self.rooms and (
                     room.network_id == self.id or (room.network_id is None and room.network_name == self.name)
                 ):
                     room.network = self
@@ -1030,14 +1101,17 @@
                         logging.debug(f"{self.id} attaching and migrating {room.id}")
                         room.network_id = self.id
                         await room.save()
                     else:
                         logging.debug(f"{self.id} attaching {room.id}")
                     self.rooms[room.name] = room
 
+        self.post_init_done = True
+
+    async def _connect(self) -> None:
         # force cleanup
         if self.conn:
             self.conn.close()
             self.conn = None
 
         network = self.serv.config["networks"][self.name]
 
@@ -1099,29 +1173,43 @@
                     with_proxy = " through a SOCKS proxy"
 
                 self.send_notice(f"Connecting to {server['address']}:{server['port']}{with_tls}{with_proxy}...")
 
                 if proxy:
                     sock = await proxy.connect(dest_host=server["address"], dest_port=server["port"])
 
+                sasl_mechanism = None
                 if self.sasl_username and self.sasl_password:
                     self.send_notice(f"Using SASL credentials for username {self.sasl_username}")
+                    sasl_mechanism = "plain"
+                elif self.tls_cert:
+                    sasl_mechanism = "external"
+
+                if sasl_mechanism:
+                    # if sasl mechanism is overridden, respect that
+                    if self.sasl_mechanism == "none":
+                        sasl_mechanism = None
+                    elif self.sasl_mechanism in ["plain", "external"]:
+                        sasl_mechanism = self.sasl_mechanism
+
+                    self.send_notice(f"SASL mechanism set to '{sasl_mechanism if sasl_mechanism else 'none'}'")
 
                 reactor = HeisenReactor(loop=asyncio.get_event_loop())
                 irc_server = reactor.server()
                 irc_server.buffer_class = buffer.LenientDecodingLineBuffer
                 factory = irc.connection.AioFactory(ssl=ssl_ctx, sock=sock, server_hostname=server_hostname)
                 self.conn = await irc_server.connect(
                     address,
                     port,
                     self.get_nick(),
                     self.password,
                     username=self.get_ident() if self.username is None else self.username,
                     ircname=self.ircname,
                     connect_factory=factory,
+                    sasl_mechanism=sasl_mechanism,
                     sasl_username=self.sasl_username,
                     sasl_password=self.sasl_password,
                 )
 
                 self.conn.add_global_handler("disconnect", self.on_disconnect)
 
                 self.conn.add_global_handler("welcome", self.on_welcome)
@@ -1232,17 +1320,18 @@
                 break
             finally:
                 self.backoff_task = None
 
         self.send_notice("Connection aborted.")
 
     def on_disconnect(self, conn, event) -> None:
-        self.conn.disconnect()
-        self.conn.close()
-        self.conn = None
+        if self.conn:
+            self.conn.disconnect()
+            self.conn.close()
+            self.conn = None
 
         # if we were connected for a while, consider the server working
         if self.connected_at > 0 and asyncio.get_event_loop().time() - self.connected_at > 300:
             self.backoff = 0
             self.next_server = 0
             self.connected_at = 0
```

### Comparing `heisenbridge-1.8.2/heisenbridge/parser.py` & `heisenbridge-1.9.0/heisenbridge/parser.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/plumbed_room.py` & `heisenbridge-1.9.0/heisenbridge/plumbed_room.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge/private_room.py` & `heisenbridge-1.9.0/heisenbridge/private_room.py`

 * *Files 5% similar despite different names*

```diff
@@ -282,14 +282,18 @@
             )
             self.serv.register_room(self)
             await self.az.intent.user(irc_user_id).ensure_joined(self.id)
             await self.save()
             # start event queue now that we have an id
             self._queue.start()
 
+            # attach to network space
+            if self.network.space:
+                await self.network.space.attach(self.id)
+
     def is_valid(self) -> bool:
         if self.network_id is None and self.network_name is None:
             return False
 
         if self.name is None:
             return False
 
@@ -298,18 +302,32 @@
 
         if not self.in_room(self.user_id):
             return False
 
         return True
 
     def cleanup(self) -> None:
+        logging.debug(f"Cleaning up network connected room {self.id}.")
+
+        # cleanup us from network space if we have it
+        if self.network and self.network.space:
+            asyncio.ensure_future(self.network.space.detach(self.id))
+
         # cleanup us from network rooms
         if self.network and self.name in self.network.rooms:
+            logging.debug(f"... and we are attached to network {self.network.id}, detaching.")
             del self.network.rooms[self.name]
 
+            # if leaving this room invalidated the network, clean it up
+            if not self.network.is_valid():
+                logging.debug(f"... and we invalidated network {self.network.id} while cleaning up.")
+                self.network.serv.unregister_room(self.network.id)
+                self.network.cleanup()
+                asyncio.ensure_future(self.network.serv.leave_room(self.network.id, self.network.members))
+
         super().cleanup()
 
     def send_notice(
         self,
         text: str,
         user_id: Optional[str] = None,
         formatted=None,
```

### Comparing `heisenbridge-1.8.2/heisenbridge/room.py` & `heisenbridge-1.9.0/heisenbridge/room.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
 class Room(ABC):
     az: MauService
     id: str
     user_id: str
     serv: AppService
     members: List[str]
-    lazy_members: Dict[str, str]
+    lazy_members: Optional[Dict[str, str]]
     bans: List[str]
     displaynames: Dict[str, str]
 
     _mx_handlers: Dict[str, List[Callable[[dict], bool]]]
     _queue: EventQueue
 
     def __init__(self, id: str, user_id: str, serv: AppService, members: List[str], bans: List[str]):
         self.id = id
         self.user_id = user_id
         self.serv = serv
         self.members = list(members)
         self.bans = list(bans) if bans else []
-        self.lazy_members = {}
+        self.lazy_members = None
         self.displaynames = {}
         self.last_messages = defaultdict(str)
 
         self._mx_handlers = {}
         self._queue = EventQueue(self._flush_events)
 
         # start event queue
@@ -54,14 +54,17 @@
 
         self.init()
 
     @classmethod
     def init_class(cls, az: MauService):
         cls.az = az
 
+    async def post_init(self):
+        pass
+
     def from_config(self, config: dict) -> None:
         pass
 
     def init(self) -> None:
         pass
 
     def is_valid(self) -> bool:
@@ -144,28 +147,26 @@
     async def _join(self, user_id, nick=None):
         await self.az.intent.user(user_id).ensure_joined(self.id, ignore_cache=True)
 
         self.members.append(user_id)
         if nick is not None:
             self.displaynames[user_id] = nick
 
-        if user_id in self.lazy_members:
-            del self.lazy_members[user_id]
-
     async def _flush_events(self, events):
         for event in events:
             try:
                 if event["type"] == "_join":
+                    if self.lazy_members is not None:
+                        self.lazy_members[event["user_id"]] = event["nick"]
+
                     if event["user_id"] not in self.members:
-                        if event["lazy"]:
-                            self.lazy_members[event["user_id"]] = event["nick"]
-                        else:
+                        if not event["lazy"]:
                             await self._join(event["user_id"], event["nick"])
                 elif event["type"] == "_leave":
-                    if event["user_id"] in self.lazy_members:
+                    if self.lazy_members is not None and event["user_id"] in self.lazy_members:
                         del self.lazy_members[event["user_id"]]
 
                     if event["user_id"] in self.members:
                         if event["reason"] is not None:
                             await self.az.intent.user(event["user_id"]).kick_user(
                                 self.id, event["user_id"], event["reason"]
                             )
@@ -175,23 +176,31 @@
                         if event["user_id"] in self.displaynames:
                             del self.displaynames[event["user_id"]]
                 elif event["type"] == "_rename":
                     old_irc_user_id = self.serv.irc_user_id(self.network.name, event["old_nick"])
                     new_irc_user_id = self.serv.irc_user_id(self.network.name, event["new_nick"])
 
                     # if we are lazy loading and this user has never spoken, update that
-                    if old_irc_user_id in self.lazy_members:
+                    if (
+                        self.lazy_members is not None
+                        and old_irc_user_id in self.lazy_members
+                        and old_irc_user_id not in self.members
+                    ):
                         del self.lazy_members[old_irc_user_id]
                         self.lazy_members[new_irc_user_id] = event["new_nick"]
                         continue
 
                     # this event is created for all rooms, skip if irrelevant
                     if old_irc_user_id not in self.members:
                         continue
 
+                    # always ensure new irc user id is in lazy list
+                    if self.lazy_members is not None:
+                        self.lazy_members[new_irc_user_id] = event["new_nick"]
+
                     # check if we can just update the displayname
                     if old_irc_user_id != new_irc_user_id:
                         # ensure we have the new puppet
                         await self.serv.ensure_irc_user_id(self.network.name, event["new_nick"])
 
                         # old puppet away
                         await self.az.intent.user(old_irc_user_id).kick_user(
@@ -220,15 +229,19 @@
                         intent = intent.user(event["user_id"])
 
                     await intent.send_state_event(
                         self.id, EventType.find(event["type"]), state_key=event["state_key"], content=event["content"]
                     )
                 else:
                     # invite puppet *now* if we are lazy loading and it should be here
-                    if event["user_id"] in self.lazy_members and event["user_id"] not in self.members:
+                    if (
+                        self.lazy_members is not None
+                        and event["user_id"] in self.lazy_members
+                        and event["user_id"] not in self.members
+                    ):
                         await self.serv.ensure_irc_user_id(self.network.name, self.lazy_members[event["user_id"]])
                         await self._join(event["user_id"], self.lazy_members[event["user_id"]])
 
                     # if we get an event from unknown user (outside room for some reason) we may have a fallback
                     if event["user_id"] is not None and event["user_id"] not in self.members:
                         if "fallback_html" in event and event["fallback_html"] is not None:
                             fallback_html = event["fallback_html"]
```

### Comparing `heisenbridge-1.8.2/heisenbridge/version.py` & `heisenbridge-1.9.0/heisenbridge/version.py`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/heisenbridge.egg-info/PKG-INFO` & `heisenbridge-1.9.0/heisenbridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heisenbridge
-Version: 1.8.2
+Version: 1.9.0
 Summary: a bouncer-style Matrix IRC bridge
 Home-page: https://github.com/hifi/heisenbridge
 Author: Toni Spets (hifi)
 Author-email: toni.spets@iki.fi
 License: MIT license
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -49,14 +49,15 @@
 * smart message formatting from Matrix to IRC using IRC conventions
 * smart message edits from Matrix to IRC by sending only corrections
 * automatic identify/auth with server password or automatic command on connect
 * SASL plain authentication
 * CertFP authentication
 * CTCP support
 * SOCKS proxy configuration per server
+* bridge managed spaces to organize your channels and PMs within a network
 
 Comparison
 ----------
 
 To help understand where Heisenbridge is a good fit here's a feature matrix of some of the key differences between other popular solutions:
 
 |                         | Matrix |  IRC | Appservice | Ratelimit | Self-host | Permissions  |
```

### Comparing `heisenbridge-1.8.2/heisenbridge.egg-info/SOURCES.txt` & `heisenbridge-1.9.0/heisenbridge.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 heisenbridge/identd.py
 heisenbridge/irc.py
 heisenbridge/network_room.py
 heisenbridge/parser.py
 heisenbridge/plumbed_room.py
 heisenbridge/private_room.py
 heisenbridge/room.py
+heisenbridge/space_room.py
 heisenbridge/version.py
 heisenbridge/version.txt
 heisenbridge.egg-info/PKG-INFO
 heisenbridge.egg-info/SOURCES.txt
 heisenbridge.egg-info/dependency_links.txt
 heisenbridge.egg-info/entry_points.txt
 heisenbridge.egg-info/requires.txt
```

### Comparing `heisenbridge-1.8.2/logo/heisenbridge.svg` & `heisenbridge-1.9.0/logo/heisenbridge.svg`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/setup.cfg` & `heisenbridge-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `heisenbridge-1.8.2/setup.py` & `heisenbridge-1.9.0/setup.py`

 * *Files identical despite different names*

