# Comparing `tmp/kilter_protocol-0.3.0.tar.gz` & `tmp/kilter_protocol-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilter_protocol-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "kilter_protocol-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kilter_protocol-0.3.0.tar` & `kilter_protocol-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    16726 2023-07-13 19:10:45.307281 kilter_protocol-0.3.0/LICENCE.txt
--rw-r--r--   0        0        0     4096 2023-07-20 00:12:58.721981 kilter_protocol-0.3.0/README.md
--rw-r--r--   0        0        0      673 2023-07-19 23:56:33.555128 kilter_protocol-0.3.0/kilter/protocol/__init__.py
--rw-r--r--   0        0        0     5161 2023-07-13 19:10:45.315281 kilter_protocol-0.3.0/kilter/protocol/buffer.py
--rw-r--r--   0        0        0     9225 2023-07-19 23:56:33.555128 kilter_protocol-0.3.0/kilter/protocol/core.py
--rw-r--r--   0        0        0     1932 2023-07-19 23:56:33.559128 kilter_protocol-0.3.0/kilter/protocol/exceptions.py
--rw-r--r--   0        0        0    22146 2023-07-19 23:56:33.559128 kilter_protocol-0.3.0/kilter/protocol/messages.py
--rw-r--r--   0        0        0        0 2023-07-13 19:10:45.315281 kilter_protocol-0.3.0/kilter/protocol/py.typed
--rw-r--r--   0        0        0     2617 2023-07-13 22:40:33.359295 kilter_protocol-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 kilter_protocol-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    16726 2023-07-13 22:46:35.258757 kilter_protocol-0.4.0/LICENCE.txt
+-rw-r--r--   0        0        0     4096 2023-07-20 00:11:32.412260 kilter_protocol-0.4.0/README.md
+-rw-r--r--   0        0        0      673 2023-07-30 11:01:43.475151 kilter_protocol-0.4.0/kilter/protocol/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-13 22:46:35.258757 kilter_protocol-0.4.0/kilter/protocol/buffer.py
+-rw-r--r--   0        0        0     9753 2023-07-30 11:01:43.475151 kilter_protocol-0.4.0/kilter/protocol/core.py
+-rw-r--r--   0        0        0     1932 2023-07-19 23:48:56.268122 kilter_protocol-0.4.0/kilter/protocol/exceptions.py
+-rw-r--r--   0        0        0    21723 2023-07-30 11:01:43.479151 kilter_protocol-0.4.0/kilter/protocol/messages.py
+-rw-r--r--   0        0        0        0 2023-07-13 22:46:35.258757 kilter_protocol-0.4.0/kilter/protocol/py.typed
+-rw-r--r--   0        0        0     2639 2023-07-30 11:01:43.479151 kilter_protocol-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 kilter_protocol-0.4.0/PKG-INFO
```

### Comparing `kilter_protocol-0.3.0/LICENCE.txt` & `kilter_protocol-0.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.3.0/README.md` & `kilter_protocol-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.3.0/kilter/protocol/__init__.py` & `kilter_protocol-0.4.0/kilter/protocol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from .core import ResponseMessage as ResponseMessage
 from .exceptions import *
 from .messages import *
 
 if TYPE_CHECKING:
 	from .buffer import FixedSizeBuffer as FixedSizeBuffer
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
```

### Comparing `kilter_protocol-0.3.0/kilter/protocol/buffer.py` & `kilter_protocol-0.4.0/kilter/protocol/buffer.py`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.3.0/kilter/protocol/core.py` & `kilter_protocol-0.4.0/kilter/protocol/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,20 +208,35 @@
 
 	Low-level filter implementors should use this class to process messages to and from
 	buffers.  The class checks the correctness of responses sent back to the MTA.
 	"""
 
 	def __init__(self, *, abort_on_unknown: bool = False) -> None:
 		self.abort_on_unknown = abort_on_unknown
-		self.nr = set[bytes]()
-		self.actions = set[bytes]([messages.Progress.ident])
-		self.state: tuple[messages.Message, set[bytes]]|None = None
+		self.skip = False
+		self.nr = set[int]()
+		self.actions = set[int]([messages.Progress.ident])
+		self.state: tuple[messages.Message, set[int]]|None = None
 		self._optflags = ProtocolFlags(0)
 		self._actflags = ActionFlags(0)
 
+	def needs_response(self, message: MTAMessage) -> bool:
+		"""
+		Return whether the message from an MTA requires a response
+
+		There answer to whether a response is required will rely in part on the options
+		negotiated with the MTA.
+		"""
+		match message:
+			case Negotiate():
+				return True
+			case Macro()|Abort()|Close():
+				return False
+		return message.ident not in self.nr
+
 	def read_from(
 		self,
 		buf: FixedSizeBuffer,
 	) -> Iterator[MTAMessage]:
 		"""
 		Return an iterator yielding each complete message from a buffer
 
@@ -263,22 +278,21 @@
 			self._store_mta_flags(message)
 		if self.state is not None:
 			raise UnexpectedMessage(message)
 		try:
 			responses = MTA_EVENT_RESPONSES[message.ident]
 		except KeyError:
 			raise InvalidMessage(message)
-		else:
-			assert isinstance(
-				message,
-				(
-					Negotiate, Macro, Connect, Helo, EnvelopeFrom, EnvelopeRecipient, Data,
-					Unknown, Header, EndOfHeaders, Body, EndOfMessage, Abort, Close,
-				),
-			)
+		assert isinstance(
+			message,
+			(
+				Negotiate, Macro, Connect, Helo, EnvelopeFrom, EnvelopeRecipient, Data,
+				Unknown, Header, EndOfHeaders, Body, EndOfMessage, Abort, Close,
+			),
+		)
 		if responses is not None and message.ident not in self.nr:
 			self.state = message, responses
 		return message
 
 	def _check_send(self, message: messages.Message) -> None:
 		if self.state is None:
 			raise UnexpectedMessage(message)
@@ -288,14 +302,16 @@
 		if isinstance(event, messages.EndOfMessage):
 			if message.ident in self.actions:
 				return
 			if message.ident in UPDATE_FLAG_MAP:
 				raise UnexpectedMessage(message)
 		if message.ident not in responses:
 			raise InvalidMessage(message, event)
+		if message.ident == Skip.ident and not self.skip:
+			raise UnexpectedMessage(message)
 		self.state = None
 
 	def _store_mta_flags(self, message: messages.Negotiate) -> None:
 		"""
 		Store the option flags offered by an MTA for later checking
 		"""
 		self._optflags = message.protocol_flags
@@ -316,9 +332,10 @@
 			if ActionFlags.SETSYMLIST not in self._actflags:
 				raise ValueError("requesting symbols (macros) is not offered by the MTA")
 
 		if (pflags := message.protocol_flags & ~self._optflags):
 			raise ValueError(f"requested options not offered by the MTA: {pflags!r}")
 		if (aflags := message.action_flags & ~self._actflags):
 			raise ValueError(f"requested actions not offered by the MTA: {aflags!r}")
+		self.skip = ProtocolFlags.SKIP in message.protocol_flags
 		self.nr.update(ident for ident, flag in NR_FLAG_MAP.items() if flag in message.protocol_flags)
 		self.actions.update(ident for ident, flag in UPDATE_FLAG_MAP.items() if flag in message.action_flags)
```

### Comparing `kilter_protocol-0.3.0/kilter/protocol/exceptions.py` & `kilter_protocol-0.4.0/kilter/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.3.0/kilter/protocol/messages.py` & `kilter_protocol-0.4.0/kilter/protocol/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 if TYPE_CHECKING:
 	from .buffer import FixedSizeBuffer
 
 LONG = Struct("!L")
 
 __all__ = [
-	"Family", "Stage", "BitField", "ActionFlags", "ProtocolFlags",
+	"Family", "Stage", "ActionFlags", "ProtocolFlags",
 	"Message", "Negotiate", "Macro", "Connect", "Helo", "EnvelopeFrom",
 	"EnvelopeRecipient", "Data", "Unknown", "Header", "EndOfHeaders", "Body",
 	"EndOfMessage", "Abort", "Close", "Continue", "Reject", "Discard", "Accept",
 	"TemporaryFailure", "Skip", "ReplyCode", "ChangeHeader", "Quarantine",
 	"AddHeader", "InsertHeader", "ChangeSender", "AddRecipient", "AddRecipientPar",
 	"RemoveRecipient", "ReplaceBody", "Progress",
 ]
@@ -111,56 +111,37 @@
 	ENVELOPE_FROM = 2
 	ENVELOPE_RECIPIENT = 3
 	DATA = 4
 	END_MESSAGE = 5
 	END_HEADERS = 6
 
 
-BFSelf = TypeVar("BFSelf", bound="BitField")
-
-
-class BitField(IntFlag):
-	"""
-	Base class for bit-field enums like ActionFlags and ProtocolFlags
-	"""
-
-	@classmethod
-	def pack(cls: type[BFSelf], flags: Iterable[BFSelf]) -> int:
-		rflag = 0
-		for flag in flags:
-			rflag |= flag
-		return rflag
-
-	@classmethod
-	def unpack(cls: type[BFSelf], bitfield: int) -> set[BFSelf]:
-		return {flag for flag in cls if flag & bitfield}
-
-
-class ActionFlags(BitField):
+class ActionFlags(IntFlag):
 	"""
 	Bit-field values for the `Negotiate.action_flags` field of the `Negotiate` message
 
 	The values correspond to the `SPFIF_*` codes as described in
 	https://pythonhosted.org/pymilter/milter_api/smfi_register.html#flags
 	"""
 
 	NONE = 0x0
+	ALL = 0x1ff
 
 	ADD_HEADERS = ADDHDRS = 0x1
 	CHANGE_HEADERS = CHGHDRS = 0x10
 	CHANGE_BODY = CHGBODY = 0x2
 	ADD_RECIPIENT = ADDRCPT = 0x4
 	ADD_RECIPIENT_PAR = ADDRCPT_PAR = 0x80
 	DELETE_RECIPIENT = DELRCPT = 0x8
 	QUARANTINE = 0x20
 	CHANGE_FROM = CHGFROM = 0x40
 	SETSYMLIST = 0x100
 
 
-class ProtocolFlags(BitField):
+class ProtocolFlags(IntFlag):
 	"""
 	Bit-field values for the `Negotiate.protocol_flags` field of the `Negotiate` message
 
 	The values correspond to the `SMFIP_*` codes described in
 	https://pythonhosted.org/pymilter/milter_api/xxfi_negotiate.html
 	"""
 
@@ -234,38 +215,38 @@
 	Traceback (most recent call last):
 		...
 	BufferError: Existing exports of data: object cannot be re-sized
 	>>> message.release()
 	>>> del buf[:10]
 	"""
 
-	ident: ClassVar[bytes]
+	ident: ClassVar[int]
 
-	_message_classes = dict[bytes, "type[Message]"]()
-	_hdr_struct = Struct("!lc")
+	_message_classes = dict[int, "type[Message]"]()
+	_hdr_struct = Struct("!LB")
 
 	@classmethod
 	def __init_subclass__(cls, /, ident: bytes = b""):
 		super().__init_subclass__()
 		if ident:  # pragma: no-branch
 			assert len(ident) == 1
-			Message._message_classes[ident] = cls
-			cls.ident = ident
+			cls.ident = ident[0]
+			Message._message_classes[cls.ident] = cls
 
 	@classmethod
 	def unpack(cls, buf: FixedSizeBuffer) -> tuple[Message, int]:
 		"""
 		Unpack a message in buff and return a subclass instance and the number of bytes read
 		"""
 		hdr_size = cls._hdr_struct.size
 		if buf.filled < hdr_size:
 			raise NeedsMore
 		size, ident = cls._hdr_struct.unpack_from(buf[:])
 		assert isinstance(size, int)
-		assert isinstance(ident, bytes)
+		assert isinstance(ident, int)
 		end = hdr_size + size - 1
 		if buf.filled < end:
 			raise NeedsMore
 		try:
 			msg_class = cls._message_classes[ident]
 		except KeyError:
 			raise UnknownMessage(buf[:end].tobytes())
@@ -419,18 +400,18 @@
 
 @dataclass
 class Macro(Message, ident=b"D"):
 	"""
 	A message type for transferring symbol mappings prior to a stage event
 	"""
 
-	stage: bytes
+	stage: int
 	macros: Mapping[str, str]
 
-	_struct = Struct("!c")
+	_struct = Struct("!B")
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		stage, *_ = cls._struct.unpack_from(buf)
 		macros = {}
 		with buf[1:] as buf:
 			while len(buf) > 0:
```

### Comparing `kilter_protocol-0.3.0/pyproject.toml` & `kilter_protocol-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 flake8-docstrings = ["-D10*"]
 
 [tool.flakeheaven.exceptions."doc/*"]
 flake8-docstrings = ["-*"]
 
 
 [tool.mypy]
+python_version = 3.10
 strict = true
 warn_unused_configs = true
 warn_unreachable = true
 namespace_packages = true
 explicit_package_bases = true
 allow_redefinition = true
```

### Comparing `kilter_protocol-0.3.0/PKG-INFO` & `kilter_protocol-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilter.protocol
-Version: 0.3.0
+Version: 0.4.0
 Summary: Parsers and state machines for the Sendmail milter communications protocol
 Author-email: Dom Sekotill <dom.sekotill@kodo.org.uk>
 Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

