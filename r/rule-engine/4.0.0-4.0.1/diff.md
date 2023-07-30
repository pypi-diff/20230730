# Comparing `tmp/rule-engine-4.0.0.tar.gz` & `tmp/rule-engine-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule-engine-4.0.0.tar", last modified: Sat Jul 15 16:37:00 2023, max compression
+gzip compressed data, was "rule-engine-4.0.1.tar", last modified: Sun Jul 30 03:02:41 2023, max compression
```

## Comparing `rule-engine-4.0.0.tar` & `rule-engine-4.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-15 16:36:32.000000 rule-engine-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-15 16:37:00.653619 rule-engine-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-15 16:36:32.000000 rule-engine-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/lib/rule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52126 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/debug_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23588 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21819 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/lib/rule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:37:00.653619 rule-engine-4.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-07-15 16:36:32.000000 rule-engine-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.735775 rule-engine-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-30 03:02:01.000000 rule-engine-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-30 03:02:41.735775 rule-engine-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-30 03:02:01.000000 rule-engine-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.727774 rule-engine-4.0.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.731774 rule-engine-4.0.1/lib/rule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52714 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/debug_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/debug_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23588 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21819 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.735775 rule-engine-4.0.1/lib/rule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:02:41.735775 rule-engine-4.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-07-30 03:02:01.000000 rule-engine-4.0.1/setup.py
```

### Comparing `rule-engine-4.0.0/LICENSE` & `rule-engine-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/PKG-INFO` & `rule-engine-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 4.0.0
+Version: 4.0.1
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
```

### Comparing `rule-engine-4.0.0/README.rst` & `rule-engine-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/__init__.py` & `rule-engine-4.0.1/lib/rule_engine/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '4.0.0'
+__version__ = '4.0.1'
 
 from .engine import resolve_attribute
 from .engine import resolve_item
 from .engine import type_resolver_from_dict
 from .engine import Context
 from .engine import Rule
```

### Comparing `rule-engine-4.0.0/lib/rule_engine/_utils.py` & `rule-engine-4.0.1/lib/rule_engine/_utils.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/ast.py` & `rule-engine-4.0.1/lib/rule_engine/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1045,19 +1045,21 @@
 	# because there is no syntax for defining a function, they can't be reduced until symbols can be reduced
 
 	def evaluate(self, thing):
 		function = self.function.evaluate(thing)
 		if not callable(function):
 			raise errors.EvaluationError('data type mismatch (not a callable value)')
 		arguments = tuple(argument.evaluate(thing) for argument in self.arguments)
-		function_name = function.__name__ + '?'
+		function_name = '<unknown>'
 		if self.function.result_type != DataType.UNDEFINED:
 			function_type = self.function.result_type
 			function_name = function_type.value_name
 			self._validate_function(function_type, arguments)
+		elif hasattr(function, '__name__'):
+			function_name = function.__name__ + '?'
 		try:
 			result = function(*arguments)
 		except errors.FunctionCallError as error:
 			error.function_name = function_name
 			raise error
 		except Exception as error:
 			raise errors.FunctionCallError('function call failed', error=error, function_name=function_name) from None
@@ -1077,22 +1079,32 @@
 				raise errors.FunctionCallError(
 					"expected at most {} positional arguments".format(len(function_type.argument_types)),
 					function_name=function_type.value_name
 				)
 			for pos, (arg1, arg2_type) in enumerate(zip(arguments, function_type.argument_types), 1):
 				if isinstance(arg1, LiteralExpressionBase):
 					arg1_type = arg1.result_type
+				elif isinstance(arg1, SymbolExpression):
+					arg1_type = arg1.result_type
 				else:
 					arg1_type = DataType.from_value(arg1)
 				if not DataType.is_compatible(arg1_type, arg2_type):
 					raise errors.FunctionCallError(
 						"data type mismatch (argument #{})".format(pos),
 						function_name=function_type.value_name
 					)
 
+	def to_graphviz(self, digraph, *args, **kwargs):
+		super(FunctionCallExpression, self).to_graphviz(digraph, *args, **kwargs)
+		self.function.to_graphviz(digraph, *args, **kwargs)
+		digraph.edge(str(id(self)), str(id(self.function)), label='function')
+		for idx, argument in enumerate(self.arguments, 1):
+			argument.to_graphviz(digraph, *args, **kwargs)
+			digraph.edge(str(id(self)), str(id(argument)), label="argument #{}".format(idx))
+
 class Statement(ASTNodeBase):
 	"""A class representing the top level statement of the grammar text."""
 	__slots__ = ('context', 'expression', 'comment')
 	def __init__(self, context, expression, comment=None):
 		"""
 		:param context: The context to use for evaluating the statement.
 		:type context: :py:class:`~rule_engine.engine.Context`
```

### Comparing `rule-engine-4.0.0/lib/rule_engine/builtins.py` & `rule-engine-4.0.1/lib/rule_engine/builtins.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/debug_repl.py` & `rule-engine-4.0.1/lib/rule_engine/debug_repl.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/engine.py` & `rule-engine-4.0.1/lib/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/errors.py` & `rule-engine-4.0.1/lib/rule_engine/errors.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/parser.py` & `rule-engine-4.0.1/lib/rule_engine/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,33 +179,39 @@
 	t_LBRACE           = r'\{'
 	t_RBRACE           = r'\}'
 	t_FLOAT            = r'0(b[01]+|o[0-7]+|x[0-9a-fA-F]+)|[0-9]+(\.[0-9]*)?([eE][+-]?[0-9]+)?|\.[0-9]+([eE][+-]?[0-9]+)?'
 	# attributes must be valid symbol names so the right side is more specific
 	t_ATTR             = r'(?<=\S)\.(?=[a-zA-Z_][a-zA-Z0-9_]*)'
 	t_ATTR_SAFE        = r'(?<=\S)&\.(?=[a-zA-Z_][a-zA-Z0-9_]*)'
 
-	# tokens are listed from lowest to highest precedence, ones that appear
-	# later are effectively evaluated first
-	# see: https://en.wikipedia.org/wiki/Order_of_operations#Programming_languages
-	precedence = (
-		('left',     'OR'),
-		('left',     'AND'),
-		('right',    'NOT'),
-		('left',     'BWOR'),
-		('left',     'BWXOR'),
-		('left',     'BWAND'),
-		('right',    'QMARK', 'COLON'),
-		('nonassoc', 'EQ', 'NE', 'EQ_FZM', 'EQ_FZS', 'NE_FZM', 'NE_FZS', 'GE', 'GT', 'LE', 'LT', 'IN'),  # Nonassociative operators
-		('left',     'ADD', 'SUB'),
-		('left',     'BWLSH', 'BWRSH'),
-		('left',     'MUL', 'TDIV', 'FDIV', 'MOD'),
-		('left',     'POW'),
-		('right',    'UMINUS'),
-		('left',     'ATTR', 'ATTR_SAFE'),
-	)
+	# Tokens are listed from highest to lowest precedence, ones that appear
+	# later are effectively evaluated last
+	# see:
+	#   * https://en.wikipedia.org/wiki/Order_of_operations#Programming_languages
+	#   * https://docs.python.org/3/reference/expressions.html
+	precedence = tuple(
+		# reverse the order to lowest to highest for ply
+		reversed((
+			('nonassoc', 'LPAREN', 'RPAREN'),
+			('left',     'ATTR', 'ATTR_SAFE'),
+			('right',    'UMINUS'),
+			('left',     'POW'),
+			('left',     'MUL', 'TDIV', 'FDIV', 'MOD'),
+			('left',     'BWLSH', 'BWRSH'),
+			('left',     'ADD', 'SUB'),
+			('nonassoc', 'EQ', 'NE', 'EQ_FZM', 'EQ_FZS', 'NE_FZM', 'NE_FZS', 'GE', 'GT', 'LE', 'LT', 'IN'),  # Nonassociative operators
+			('right',    'QMARK', 'COLON'),
+			('left',     'BWAND'),
+			('left',     'BWXOR'),
+			('left',     'BWOR'),
+			('right',    'NOT'),
+			('left',     'AND'),
+			('left',     'OR'),
+		)
+	))
 
 	@classmethod
 	def get_token_regex(cls, token_name):
 		"""
 		Return the regex that is used by the specified token.
 
 		:param str token_name: The token for which to return the regex.
```

### Comparing `rule-engine-4.0.0/lib/rule_engine/suggestions.py` & `rule-engine-4.0.1/lib/rule_engine/suggestions.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine/types.py` & `rule-engine-4.0.1/lib/rule_engine/types.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.0/lib/rule_engine.egg-info/PKG-INFO` & `rule-engine-4.0.1/lib/rule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 4.0.0
+Version: 4.0.1
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
```

### Comparing `rule-engine-4.0.0/setup.py` & `rule-engine-4.0.1/setup.py`

 * *Files identical despite different names*

