# Comparing `tmp/bodhi_messages-7.2.0.tar.gz` & `tmp/bodhi_messages-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_messages-7.2.0.tar", max compression
+gzip compressed data, was "bodhi_messages-7.2.1.tar", max compression
```

## Comparing `bodhi_messages-7.2.0.tar` & `bodhi_messages-7.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    18018 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/COPYING
--rw-r--r--   0        0        0       97 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/README.rst
--rw-r--r--   0        0        0      906 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/bodhi/messages/__init__.py
--rw-r--r--   0        0        0      793 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/__init__.py
--rw-r--r--   0        0        0     9240 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/base.py
--rw-r--r--   0        0        0     5116 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/buildroot_override.py
--rw-r--r--   0        0        0    11249 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/compose.py
--rw-r--r--   0        0        0     3783 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/errata.py
--rw-r--r--   0        0        0    30333 2023-04-29 13:40:09.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/update.py
--rw-r--r--   0        0        0     1271 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/bodhi/messages/utils.py
--rw-r--r--   0        0        0     3618 2023-04-30 06:59:12.000000 bodhi_messages-7.2.0/pyproject.toml
--rw-r--r--   0        0        0      788 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2713 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_base.py
--rw-r--r--   0        0        0     3500 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_buildroot_override.py
--rw-r--r--   0        0        0     6651 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_compose.py
--rw-r--r--   0        0        0     5321 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_errata.py
--rw-r--r--   0        0        0    43182 2023-04-29 13:40:09.000000 bodhi_messages-7.2.0/tests/test_update.py
--rw-r--r--   0        0        0     1960 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/tests/utils.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 bodhi_messages-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0    18018 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/COPYING
+-rw-r--r--   0        0        0       97 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/README.rst
+-rw-r--r--   0        0        0      906 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/bodhi/messages/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/bodhi/messages/schemas/__init__.py
+-rw-r--r--   0        0        0     9240 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/bodhi/messages/schemas/base.py
+-rw-r--r--   0        0        0     5116 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/bodhi/messages/schemas/buildroot_override.py
+-rw-r--r--   0        0        0    11249 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/bodhi/messages/schemas/compose.py
+-rw-r--r--   0        0        0     3783 2023-05-13 08:55:56.000000 bodhi_messages-7.2.1/bodhi/messages/schemas/errata.py
+-rw-r--r--   0        0        0    34198 2023-07-30 14:37:08.000000 bodhi_messages-7.2.1/bodhi/messages/schemas/update.py
+-rw-r--r--   0        0        0     1589 2023-07-30 14:37:08.000000 bodhi_messages-7.2.1/bodhi/messages/utils.py
+-rw-r--r--   0        0        0     3666 2023-07-30 14:39:48.000000 bodhi_messages-7.2.1/pyproject.toml
+-rw-r--r--   0        0        0      788 2023-06-20 08:06:31.000000 bodhi_messages-7.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2713 2023-06-20 08:06:31.000000 bodhi_messages-7.2.1/tests/test_base.py
+-rw-r--r--   0        0        0     3500 2023-06-20 08:06:31.000000 bodhi_messages-7.2.1/tests/test_buildroot_override.py
+-rw-r--r--   0        0        0     6651 2023-06-20 08:06:31.000000 bodhi_messages-7.2.1/tests/test_compose.py
+-rw-r--r--   0        0        0     5321 2023-06-20 08:06:31.000000 bodhi_messages-7.2.1/tests/test_errata.py
+-rw-r--r--   0        0        0    44247 2023-07-30 14:37:08.000000 bodhi_messages-7.2.1/tests/test_update.py
+-rw-r--r--   0        0        0     2099 2023-07-30 14:37:08.000000 bodhi_messages-7.2.1/tests/utils.py
+-rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 bodhi_messages-7.2.1/setup.py
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 bodhi_messages-7.2.1/PKG-INFO
```

### Comparing `bodhi_messages-7.2.0/COPYING` & `bodhi_messages-7.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/__init__.py` & `bodhi_messages-7.2.1/bodhi/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/schemas/__init__.py` & `bodhi_messages-7.2.1/bodhi/messages/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/schemas/base.py` & `bodhi_messages-7.2.1/bodhi/messages/schemas/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/schemas/buildroot_override.py` & `bodhi_messages-7.2.1/bodhi/messages/schemas/buildroot_override.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/schemas/compose.py` & `bodhi_messages-7.2.1/bodhi/messages/schemas/compose.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/schemas/errata.py` & `bodhi_messages-7.2.1/bodhi/messages/schemas/errata.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/bodhi/messages/schemas/update.py` & `bodhi_messages-7.2.1/bodhi/messages/schemas/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 <https://fedora-messaging.readthedocs.io/en/stable/>`_ documentation on
 messages.
 """
 
 import copy
 import typing
 
+from fedora_messaging.message import DEBUG
+
+from ..utils import past_tense, truncate
 from .base import BodhiMessage, BuildV1, ReleaseV1, SCHEMA_URL, UpdateV1, UserV1
-from ..utils import truncate
 
 
 class UpdateMessage(BodhiMessage):
     """Base class for update messages."""
 
     @property
     def url(self) -> str:
@@ -78,14 +80,27 @@
         return self.update.packages
 
     @property
     def _update(self) -> dict:
         """Return a dictionary from the body representing an update."""
         return self.body['update']
 
+    @property
+    def _builds_summary(self):
+        """Return a truncated list of the update's builds."""
+        return truncate(' '.join([b.nvr for b in self.update.builds]))
+
+    @property
+    def _owner_qual(self):
+        """Return a string to qualify whether the update belongs to the agent."""
+        if self.agent_name == self.update.user.name:
+            return "their"
+        else:
+            return f"{self.update.user.name}'s"
+
     def __str__(self) -> str:
         """
         Return a human-readable representation of this message.
 
         This should provide a detailed representation of the message, much like the body
         of an email.
 
@@ -213,30 +228,30 @@
         This should provide a short summary of the message, much like the subject line
         of an email.
 
         Returns:
             A summary for this message.
         """
         return (
-            f"{self.update.user.name}'s {truncate(' '.join([b.nvr for b in self.update.builds]))} "
+            f"{self.update.user.name}'s {self._builds_summary} "
             f"bodhi update completed push to {self.update.status}")
 
     def __str__(self) -> str:
         """
         Return a human-readable representation of this message.
 
         This should provide a detailed representation of the message, much like the body
         of an email.
 
         Returns:
             A human readable representation of this message.
         """
         new_line = "\n"
         return (
-            f"{self.update.user.name}'s Bodhi update {self.update.alias}"
+            f"{self.update.user.name}'s Bodhi update {self.update.alias} "
             f"completed push to {self.update.status}\n"
             f"Builds:\n"
             f"{new_line.join([b.nvr for b in self.update.builds])} ")
 
 
 class UpdateCompleteTestingV1(UpdateMessage):
     """Sent when an update is available in the testing repository."""
@@ -265,30 +280,30 @@
         This should provide a short summary of the message, much like the subject line
         of an email.
 
         Returns:
             A summary for this message.
         """
         return (
-            f"{self.update.user.name}'s {truncate(' '.join([b.nvr for b in self.update.builds]))} "
+            f"{self.update.user.name}'s {self._builds_summary} "
             f"bodhi update completed push to {self.update.status}")
 
     def __str__(self) -> str:
         """
         Return a human-readable representation of this message.
 
         This should provide a detailed representation of the message, much like the body
         of an email.
 
         Returns:
             A human readable representation of this message.
         """
         new_line = "\n"
         return (
-            f"{self.update.user.name}'s Bodhi update {self.update.alias}"
+            f"{self.update.user.name}'s Bodhi update {self.update.alias} "
             f"completed push to {self.update.status}\n"
             f"Builds:\n"
             f"{new_line.join([b.nvr for b in self.update.builds])} ")
 
 
 class UpdateEditV1(UpdateMessage):
     """Sent when an update is edited."""
@@ -338,15 +353,18 @@
 
         This should provide a short summary of the message, much like the subject line
         of an email.
 
         Returns:
             A summary for this message.
         """
-        return f"{self.agent_name} edited {self.update.alias}"
+        return (
+            f"{self.agent_name} edited {self._owner_qual} update {self.update.alias} "
+            f"({self._builds_summary})"
+        )
 
     def __str__(self) -> str:
         """
         Return a human-readable representation of this message.
 
         This should provide a detailed representation of the message, much like the body
         of an email.
@@ -452,15 +470,15 @@
         This should provide a short summary of the message, much like the subject line
         of an email.
 
         Returns:
             A summary for this message.
         """
         return (
-            f"{self.update.user.name}'s {truncate(' '.join([b.nvr for b in self.update.builds]))} "
+            f"{self.update.user.name}'s {self._builds_summary} "
             f"bodhi update was ejected from the {self.repo} mash. Reason: \"{self.reason}\"")
 
 
 class UpdateKarmaThresholdV1(UpdateMessage):
     """Sent when an update reaches its karma threshold."""
 
     body_schema = {
@@ -496,15 +514,36 @@
 
         This should provide a short summary of the message, much like the subject line
         of an email.
 
         Returns:
             A summary for this message.
         """
-        return f"{self.update.alias} reached the {self.status} karma threshold"
+        return (
+            f"{self.update.user.name}'s {self._builds_summary} bodhi update "
+            f"has reached the {self.status} karma threshold"
+        )
+
+    def __str__(self) -> str:
+        """
+        Return a human-readable representation of this message.
+
+        This should provide a detailed representation of the message, much like the body
+        of an email.
+
+        Returns:
+            A human readable representation of this message.
+        """
+        new_line = "\n"
+        return (
+            f"{self.update.user.name}'s bodhi update {self.update.alias} "
+            f"has reached the {self.status} karma threshold.\n"
+            f"Builds:\n"
+            f"{new_line.join([b.nvr for b in self.update.builds])}"
+        )
 
 
 class UpdateRequestMessage(UpdateMessage):
     """Sent when an update's request is changed."""
 
     @property
     def summary(self) -> str:
@@ -515,19 +554,47 @@
         of an email.
 
         Returns:
             A summary for this message.
         """
         status = self.topic.split('.')[-1]
         if status in ('unpush', 'obsolete', 'revoke'):
-            # make our status past-tense
-            status = status + (status[-1] == 'e' and 'd' or 'ed')
-            return f"{self.agent_name} {status} {self.update.alias}"
+            return (
+                f"{self.agent_name} {past_tense(status)} {self._owner_qual} update "
+                f"{self.update.alias} ({self._builds_summary})"
+            )
+        else:
+            return (
+                f"{self.agent_name} submitted {self._owner_qual} update {self.update.alias} "
+                f"({self._builds_summary}) to {status}"
+            )
+
+    def __str__(self) -> str:
+        """
+        Return a human-readable representation of this message.
+
+        This should provide a detailed representation of the message, much like the body
+        of an email.
+
+        Returns:
+            A human readable representation of this message.
+        """
+        status = self.topic.split('.')[-1]
+        if status in ('unpush', 'obsolete', 'revoke'):
+            action = past_tense(status)
         else:
-            return f"{self.agent_name} submitted {self.update.alias} to {status}"
+            action = "submitted"
+        content = [
+            f"{self.agent_name} {action} {self._owner_qual} update {self.update.alias}"
+        ]
+        if action == "submitted":
+            content.append(f" to {status}")
+        content.append(".\nBuilds:\n")
+        content.append("\n".join([b.nvr for b in self.update.builds]))
+        return "".join(content)
 
 
 class UpdateRequestRevokeV1(UpdateRequestMessage):
     """Sent when an update is revoked."""
 
     body_schema = {
         'id': f'{SCHEMA_URL}/v1/bodhi.update.request.revoke#',
@@ -643,15 +710,15 @@
         }
     }
 
     topic = "bodhi.update.request.obsolete"
 
 
 class UpdateRequirementsMetStableV1(UpdateMessage):
-    """Sent when all the update requirements are meant for stable."""
+    """Sent when all the update requirements are met for stable."""
 
     body_schema = {
         'id': f'{SCHEMA_URL}/v1/bodhi.update.requirements_met.stable#',
         '$schema': 'http://json-schema.org/draft-04/schema#',
         'description': 'Schema for message sent when an update meets stable requirements',
         'type': 'object',
         'properties': {
@@ -672,15 +739,36 @@
 
         This should provide a short summary of the message, much like the subject line
         of an email.
 
         Returns:
             A summary for this message.
         """
-        return f'{self.update.alias} has met stable testing requirements'
+        return (
+            f"{self.update.user.name}'s {self._builds_summary} "
+            f"bodhi update has met stable testing requirements"
+        )
+
+    def __str__(self) -> str:
+        """
+        Return a human-readable representation of this message.
+
+        This should provide a detailed representation of the message, much like the body
+        of an email.
+
+        Returns:
+            A human readable representation of this message.
+        """
+        new_line = "\n"
+        return (
+            f"{self.update.user.name}'s Bodhi update {self.update.alias}"
+            f" has met stable testing requirements.\n"
+            f"Builds:\n"
+            f"{new_line.join([b.nvr for b in self.update.builds])}"
+        )
 
 
 class UpdateReadyForTestingV1(BodhiMessage):
     """
     Sent when an update is ready to be tested. Original version.
 
     Does not have 'update' property or inherit from UpdateMessage.
@@ -800,14 +888,15 @@
         're-trigger': {
             'type': 'bool',
             'description': 'This flag is True if the message is sent to re-trigger tests'
         }
     }
 
     topic = "bodhi.update.status.testing.koji-build-group.build.complete"
+    severity = DEBUG
 
     @property
     def summary(self) -> str:
         """
         Return a short, human-readable representation of this message.
 
         This should provide a short summary of the message, much like the subject line
@@ -896,7 +985,39 @@
     # one expected by UpdateV1.schema()
     body_schema['definitions']['artifactbuild'] = copy.deepcopy(body_schema['definitions']['build'])
     renamed = {'$ref': '#/definitions/artifactbuild'}
     body_schema['properties']['artifact']['properties']['builds']['items'] = renamed
     body_schema['definitions']['build'] = BuildV1.schema()
     body_schema['properties']['update'] = UpdateV1.schema()
     body_schema['required'].append('update')
+
+    @property
+    def summary(self) -> str:
+        """
+        Return a short, human-readable representation of this message.
+
+        This should provide a short summary of the message, much like the subject line
+        of an email.
+
+        Returns:
+            A summary for this message.
+        """
+        return (
+            f"{self.body['update']['user']['name']}'s "
+            f"{truncate(' '.join([b['nvr'] for b in self.body['artifact']['builds']]))} "
+            f"bodhi update is ready for testing")
+
+    def __str__(self) -> str:
+        """
+        Return a human-readable representation of this message.
+
+        This should provide a detailed representation of the message, much like the body
+        of an email.
+
+        Returns:
+            A human readable representation of this message.
+        """
+        new_line = "\n"
+        return (
+            f"{self.body['update']['user']['name']}'s Bodhi update is ready for testing\n"
+            f"Builds:\n"
+            f"{new_line.join([b['nvr'] for b in self.body['artifact']['builds']])} ")
```

### Comparing `bodhi_messages-7.2.0/bodhi/messages/utils.py` & `bodhi_messages-7.2.1/bodhi/messages/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,7 +30,19 @@
     return title
 
 
 # Keep this in sync with bodhi.server.util.MENTION_RE
 # (enhancement: create a bodhi-common package that every subpackage
 # would depend on and put it there)
 MENTION_RE = r'(?<!\S)(@\w+)'
+
+
+def past_tense(verb):
+    """Return a verb in the past tense (in English).
+
+    Args:
+        verb (str): a verb, such as "obsolete", "revoke", and "push"
+
+    Returns:
+        str: the verb in the past tense, such as "obsoleted", "revoked", and "pushed"
+    """
+    return verb + ("d" if verb[-1] == 'e' else "ed")
```

### Comparing `bodhi_messages-7.2.0/pyproject.toml` & `bodhi_messages-7.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-messages"
-version = "7.2.0"
+version = "7.2.1"
 description = "JSON schema for messages sent by Bodhi"
 readme = "README.rst"
 authors = ["Fedora Infrastructure Team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 repository = "https://github.com/fedora-infra/bodhi"
 homepage = "https://bodhi.fedoraproject.org"
 keywords = ["fedora", "fedora-messaging"]
@@ -29,14 +29,17 @@
     { include = "tests", format = "sdist" }
 ]
 include = [
     { path = "*.txt", format = "sdist" },
     { path = "COPYING", format = "sdist" }
 ]
 
+[tool.poetry.build]
+generate-setup-file = true
+
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
 fedora-messaging = ">=3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.0"
 pytest-cov = ">=2.11.1"
```

### Comparing `bodhi_messages-7.2.0/tests/__init__.py` & `bodhi_messages-7.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/tests/test_base.py` & `bodhi_messages-7.2.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/tests/test_buildroot_override.py` & `bodhi_messages-7.2.1/tests/test_buildroot_override.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/tests/test_compose.py` & `bodhi_messages-7.2.1/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/tests/test_errata.py` & `bodhi_messages-7.2.1/tests/test_errata.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.2.0/tests/test_update.py` & `bodhi_messages-7.2.1/tests/test_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """Unit tests for the update message schemas."""
 
 
 from bodhi.messages.schemas.base import BuildV1, ReleaseV1, UpdateV1, UserV1
-from bodhi.messages.schemas.update import (UpdateCommentV1,
-                                           UpdateCompleteStableV1,
-                                           UpdateCompleteTestingV1,
-                                           UpdateEditV1,
-                                           UpdateEditV2,
-                                           UpdateEjectV1,
-                                           UpdateKarmaThresholdV1,
-                                           UpdateReadyForTestingV1,
-                                           UpdateReadyForTestingV2,
-                                           UpdateRequestObsoleteV1,
-                                           UpdateRequestRevokeV1,
-                                           UpdateRequestStableV1,
-                                           UpdateRequestTestingV1,
-                                           UpdateRequestUnpushV1,
-                                           UpdateRequirementsMetStableV1)
+from bodhi.messages.schemas.update import (
+    UpdateCommentV1,
+    UpdateCompleteStableV1,
+    UpdateCompleteTestingV1,
+    UpdateEditV1,
+    UpdateEditV2,
+    UpdateEjectV1,
+    UpdateKarmaThresholdV1,
+    UpdateReadyForTestingV1,
+    UpdateReadyForTestingV2,
+    UpdateRequestObsoleteV1,
+    UpdateRequestRevokeV1,
+    UpdateRequestStableV1,
+    UpdateRequestTestingV1,
+    UpdateRequestUnpushV1,
+    UpdateRequirementsMetStableV1,
+)
 
 from .utils import check_message
 
 
 class TestUpdateMessage:
     """A set of unit tests for classes in :py:mod:`bodhi_messages.schemas.update`"""
 
@@ -95,15 +97,15 @@
         expected = {
             "topic": "bodhi.update.complete.stable",
             "summary": (
                 "eclipseo's golang-github-SAP-go-hdb-0.14.1-1.fc29 t… bodhi update "
                 "completed push to stable"
             ),
             "__str__": (
-                "eclipseo's Bodhi update FEDORA-2019-d64d0caab3completed push to stable"
+                "eclipseo's Bodhi update FEDORA-2019-d64d0caab3 completed push to stable"
                 "\nBuilds:\ngolang-github-SAP-go-hdb-0.14.1-1.fc29\ntexworks-0.6.3-1.fc29 "
             ),
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-d64d0caab3",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
@@ -139,15 +141,15 @@
         expected = {
             "topic": "bodhi.update.complete.testing",
             "summary": (
                 "eclipseo's golang-github-SAP-go-hdb-0.14.1-1.fc29 t… bodhi update "
                 "completed push to testing"
             ),
             "__str__": (
-                "eclipseo's Bodhi update FEDORA-2019-d64d0caab3completed push to testing"
+                "eclipseo's Bodhi update FEDORA-2019-d64d0caab3 completed push to testing"
                 "\nBuilds:\ngolang-github-SAP-go-hdb-0.14.1-1.fc29\ntexworks-0.6.3-1.fc29 "
             ),
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-d64d0caab3",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
@@ -242,19 +244,19 @@
         )
         check_message(msg, expected)
 
     def test_ready_for_testing_v2(self):
         expected = {
             "topic": "bodhi.update.status.testing.koji-build-group.build.complete",
             "summary": (
-                "BaseOS CI's libselinux-2.8-6.fc29.x86_64 libsepol-2.… bodhi update "
+                "plautrba's libselinux-2.8-6.fc29.x86_64 libsepol-2.… bodhi update "
                 "is ready for testing"
             ),
             "__str__": (
-                "BaseOS CI's Bodhi update is ready for testing\nBuilds:"
+                "plautrba's Bodhi update is ready for testing\nBuilds:"
                 "\nlibselinux-2.8-6.fc29.x86_64\nlibsepol-2.8-3.fc29.x86_64 "
             ),
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-d64d0caab3",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
@@ -314,16 +316,18 @@
             }
         )
         check_message(msg, expected)
 
     def test_request_testing_v1_multiple(self):
         expected = {
             "topic": "bodhi.update.request.testing",
-            "summary": "lmacken submitted FEDORA-2019-f1ca3c00e5 to testing",
-            "__str__": "lmacken submitted FEDORA-2019-f1ca3c00e5 to testing",
+            "summary": "lmacken submitted hadess's update FEDORA-2019-f1ca3c00e5 "
+                       "(gnome-settings-daemon-3.6.1-1.fc18 contr…) to testing",
+            "__str__": "lmacken submitted hadess's update FEDORA-2019-f1ca3c00e5 to testing.\n"
+                       "Builds:\ngnome-settings-daemon-3.6.1-1.fc18\ncontrol-center-3.6.1-1.fc18",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-f1ca3c00e5",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "203f6cb95b44b5d38aa21425b066dd522d3e19d8919cf4b339f29e0ea7f03e9b"
                 "?s=64&d=retro"
@@ -430,16 +434,18 @@
         )
         check_message(msg, expected)
 
     def test_request_unpush_v1(self):
         """Test a request unpush message."""
         expected = {
             "topic": "bodhi.update.request.unpush",
-            "summary": "ralph unpushed FEDORA-2019-8da6360454",
-            "__str__": "ralph unpushed FEDORA-2019-8da6360454",
+            "summary": "ralph unpushed their update FEDORA-2019-8da6360454 "
+                       "(python-operator-courier-1.2.0-1.fc28)",
+            "__str__": "ralph unpushed their update FEDORA-2019-8da6360454.\n"
+                       "Builds:\npython-operator-courier-1.2.0-1.fc28",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-8da6360454",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "9c9f7784935381befc302fe3c814f9136e7a33953d0318761669b8643f4df55c"
                 "?s=64&d=retro"
@@ -464,16 +470,18 @@
             }
         )
         check_message(msg, expected)
 
     def test_request_obsolete_v1(self):
         expected = {
             "topic": "bodhi.update.request.obsolete",
-            "summary": "lmacken obsoleted FEDORA-2019-d64d0caab3",
-            "__str__": "lmacken obsoleted FEDORA-2019-d64d0caab3",
+            "summary": "lmacken obsoleted eclipseo's update FEDORA-2019-d64d0caab3 "
+                       "(golang-github-SAP-go-hdb-0.14.1-1.fc29)",
+            "__str__": "lmacken obsoleted eclipseo's update FEDORA-2019-d64d0caab3.\n"
+                       "Builds:\ngolang-github-SAP-go-hdb-0.14.1-1.fc29",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-d64d0caab3",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "203f6cb95b44b5d38aa21425b066dd522d3e19d8919cf4b339f29e0ea7f03e9b"
                 "?s=64&d=retro"
@@ -499,16 +507,18 @@
             }
         )
         check_message(msg, expected)
 
     def test_request_stable_v1(self):
         expected = {
             "topic": "bodhi.update.request.stable",
-            "summary": "lmacken submitted FEDORA-2019-d64d0caab3 to stable",
-            "__str__": "lmacken submitted FEDORA-2019-d64d0caab3 to stable",
+            "summary": "lmacken submitted eclipseo's update FEDORA-2019-d64d0caab3 "
+                       "(golang-github-SAP-go-hdb-0.14.1-1.fc29) to stable",
+            "__str__": "lmacken submitted eclipseo's update FEDORA-2019-d64d0caab3 to stable.\n"
+                       "Builds:\ngolang-github-SAP-go-hdb-0.14.1-1.fc29",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-d64d0caab3",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "203f6cb95b44b5d38aa21425b066dd522d3e19d8919cf4b339f29e0ea7f03e9b"
                 "?s=64&d=retro"
@@ -533,16 +543,18 @@
             }
         )
         check_message(msg, expected)
 
     def test_request_revoke_v1(self):
         expected = {
             "topic": "bodhi.update.request.revoke",
-            "summary": "lmacken revoked FEDORA-2019-d64d0caab3",
-            "__str__": "lmacken revoked FEDORA-2019-d64d0caab3",
+            "summary": "lmacken revoked eclipseo's update FEDORA-2019-d64d0caab3 "
+                       "(golang-github-SAP-go-hdb-0.14.1-1.fc29)",
+            "__str__": "lmacken revoked eclipseo's update FEDORA-2019-d64d0caab3.\nBuilds:\n"
+                       "golang-github-SAP-go-hdb-0.14.1-1.fc29",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-d64d0caab3",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "203f6cb95b44b5d38aa21425b066dd522d3e19d8919cf4b339f29e0ea7f03e9b"
                 "?s=64&d=retro"
@@ -567,16 +579,19 @@
             }
         )
         check_message(msg, expected)
 
     def test_request_testing_v1(self):
         expected = {
             "topic": "bodhi.update.request.testing",
-            "summary": "eclipseo submitted FEDORA-2019-f1ca3c00e5 to testing",
-            "__str__": "eclipseo submitted FEDORA-2019-f1ca3c00e5 to testing",
+            "summary": "eclipseo submitted their update FEDORA-2019-f1ca3c00e5 "
+                       "(golang-github-Masterminds-semver-2.0.0-0…) to testing",
+            "__str__": "eclipseo submitted their update FEDORA-2019-f1ca3c00e5 to testing.\n"
+                       "Builds:\n"
+                       "golang-github-Masterminds-semver-2.0.0-0.1.20190319git3c92f33.fc29",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-f1ca3c00e5",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "899e8719059bf1b2d3aba96e3e276f72f24f18a9e1f4fbfa7a331995a628e760"
                 "?s=64&d=retro"
@@ -604,16 +619,23 @@
             }
         )
         check_message(msg, expected)
 
     def test_requirements_met_stable_v1(self):
         expected = {
             "topic": "bodhi.update.requirements_met.stable",
-            "summary": "FEDORA-2019-f1ca3c00e5 has met stable testing requirements",
-            "__str__": "FEDORA-2019-f1ca3c00e5 has met stable testing requirements",
+            "summary": (
+                "eclipseo's golang-github-Masterminds-semver-2.0.0-0… bodhi update has met "
+                "stable testing requirements"
+            ),
+            "__str__": (
+                "eclipseo's Bodhi update FEDORA-2019-f1ca3c00e5 has met stable testing "
+                "requirements.\nBuilds:\n"
+                "golang-github-Masterminds-semver-2.0.0-0.1.20190319git3c92f33.fc29"
+            ),
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-f1ca3c00e5",
             "agent_avatar": None,
             "usernames": ["eclipseo"],
             "packages": ["golang-github-Masterminds-semver"],
             'update': UpdateV1(
@@ -685,15 +707,15 @@
             }
         )
         check_message(msg, expected)
 
     def test_edit_v1(self):
         expected = {
             "topic": "bodhi.update.edit",
-            "summary": "ralph edited FEDORA-2019-7dbbb74a13",
+            "summary": "ralph edited their update FEDORA-2019-7dbbb74a13 (tzdata-2014i-1.fc19)",
             "__str__": "ralph edited FEDORA-2019-7dbbb74a13 adding 2 new bugs",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-7dbbb74a13",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
                 "9c9f7784935381befc302fe3c814f9136e7a33953d0318761669b8643f4df55c"
@@ -783,15 +805,15 @@
             }
         )
         check_message(msg, expected)
 
     def test_edit_v2(self):
         expected = {
             "topic": "bodhi.update.edit",
-            "summary": "ralph edited FEDORA-2019-7dbbb74a13",
+            "summary": "ralph edited their update FEDORA-2019-7dbbb74a13 (tzdata-2014i-1.fc19)",
             "__str__": ("ralph edited FEDORA-2019-7dbbb74a13 adding 2 new bug(s), "
                         "adding 1 build(s), and removing 1 build(s)"),
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-7dbbb74a13",
             "agent_avatar": (
                 "https://seccdn.libravatar.org/avatar/"
@@ -884,16 +906,18 @@
             }
         )
         check_message(msg, expected)
 
     def test_karma_threshold_v1(self):
         expected = {
             "topic": "bodhi.update.karma.threshold.reach",
-            "summary": "FEDORA-EPEL-2015-0238 reached the stable karma threshold",
-            "__str__": "FEDORA-EPEL-2015-0238 reached the stable karma threshold",
+            "summary": "ralph's tzdata-2014i-1.fc19 bodhi update has reached "
+                       "the stable karma threshold",
+            "__str__": "ralph's bodhi update FEDORA-EPEL-2015-0238 has reached the stable "
+                       "karma threshold.\nBuilds:\ntzdata-2014i-1.fc19",
             "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
             "app_name": "bodhi",
             "url": "https://bodhi.fedoraproject.org/updates/FEDORA-EPEL-2015-0238",
             "agent_avatar": None,
             "usernames": ['ralph'],
             "packages": ["tzdata"],
             'update': UpdateV1('FEDORA-EPEL-2015-0238', [BuildV1('tzdata-2014i-1.fc19')],
```

### Comparing `bodhi_messages-7.2.0/tests/utils.py` & `bodhi_messages-7.2.1/tests/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """Utilities to do unit testing of message schemas."""
 
 import typing
 
+
 if typing.TYPE_CHECKING:  # pragma: no cover
     from bodhi.messages.schemas.base import BodhiMessage  # noqa: 401
 
 
 def check_message(msg: 'BodhiMessage', expected: typing.Mapping[str, typing.Any]):
     """
     Assert that the given message matches the information described in the expected mapping.
@@ -32,12 +33,14 @@
             the expected dictionary's value. A special key, __str__, may be used in expected to
             index a string for how the message should be rendered by str().
     """
     # Let's make sure the message matches the expected schema.
     msg.validate()
     for prop, expected_value in expected.items():
         if prop == "__str__":
-            assert str(msg) == expected_value
+            assert str(msg) == expected_value, (
+                f"string representation does not match: msg has {str(msg)!r}, "
+                f"expected is {expected_value!r}")
         else:
             assert getattr(msg, prop) == expected_value, (
-                f"key {prop} does not match: msg has {getattr(msg, prop)}, "
-                f"expected is {expected_value}")
+                f"key {prop} does not match: msg has {getattr(msg, prop)!r}, "
+                f"expected is {expected_value!r}")
```

