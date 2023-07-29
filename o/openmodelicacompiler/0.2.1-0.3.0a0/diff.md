# Comparing `tmp/openmodelicacompiler-0.2.1.tar.gz` & `tmp/openmodelicacompiler-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodelicacompiler-0.2.1.tar", max compression
+gzip compressed data, was "openmodelicacompiler-0.3.0a0.tar", max compression
```

## Comparing `openmodelicacompiler-0.2.1.tar` & `openmodelicacompiler-0.3.0a0.tar`

### file list

```diff
@@ -1,29 +1,56 @@
--rw-r--r--   0        0        0     8490 2023-02-07 11:07:27.918208 openmodelicacompiler-0.2.1/README.md
--rw-r--r--   0        0        0     1764 2023-02-09 01:05:28.305562 openmodelicacompiler-0.2.1/omc4py/__init__.py
--rw-r--r--   0        0        0    24955 2023-02-09 00:43:55.507376 openmodelicacompiler-0.2.1/omc4py/classes.py
--rw-r--r--   0        0        0     7275 2023-02-07 11:07:27.928208 openmodelicacompiler-0.2.1/omc4py/compiler.py
--rw-r--r--   0        0        0      600 2023-02-07 11:07:27.928208 openmodelicacompiler-0.2.1/omc4py/exception.py
--rw-r--r--   0        0        0     3053 2023-02-09 00:43:55.507376 openmodelicacompiler-0.2.1/omc4py/parser/__init__.py
--rw-r--r--   0        0        0     4439 2023-02-07 11:07:27.928208 openmodelicacompiler-0.2.1/omc4py/parser/syntax.py
--rw-r--r--   0        0        0     6391 2023-02-09 00:43:55.507376 openmodelicacompiler-0.2.1/omc4py/parser/visitor.py
--rw-r--r--   0        0        0     5500 2023-02-09 01:05:28.305562 openmodelicacompiler-0.2.1/omc4py/session.py
--rw-r--r--   0        0        0     1910 2023-02-07 11:07:27.928208 openmodelicacompiler-0.2.1/omc4py/string.py
--rw-r--r--   0        0        0      451 2023-02-07 11:07:27.928208 openmodelicacompiler-0.2.1/omc4py/v_1_13/__init__.py
--rw-r--r--   0        0        0   394880 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_13/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_14/__init__.py
--rw-r--r--   0        0        0   502843 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_14/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_15/__init__.py
--rw-r--r--   0        0        0   503616 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_15/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_16/__init__.py
--rw-r--r--   0        0        0   525063 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_16/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_17/__init__.py
--rw-r--r--   0        0        0   522352 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_17/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-07 11:07:27.938207 openmodelicacompiler-0.2.1/omc4py/v_1_18/__init__.py
--rw-r--r--   0        0        0   523226 2023-02-07 11:07:27.948207 openmodelicacompiler-0.2.1/omc4py/v_1_18/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-09 01:05:28.305562 openmodelicacompiler-0.2.1/omc4py/v_1_19/__init__.py
--rw-r--r--   0        0        0   536189 2023-02-09 01:05:28.305562 openmodelicacompiler-0.2.1/omc4py/v_1_19/_omc_interface.py
--rw-r--r--   0        0        0      451 2023-02-09 01:05:28.315562 openmodelicacompiler-0.2.1/omc4py/v_1_20/__init__.py
--rw-r--r--   0        0        0   534102 2023-02-09 01:05:28.315562 openmodelicacompiler-0.2.1/omc4py/v_1_20/_omc_interface.py
--rw-r--r--   0        0        0     1706 2023-02-09 01:05:28.315562 openmodelicacompiler-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9708 1970-01-01 00:00:00.000000 openmodelicacompiler-0.2.1/setup.py
--rw-r--r--   0        0        0     9801 1970-01-01 00:00:00.000000 openmodelicacompiler-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8890 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/README.md
+-rw-r--r--   0        0        0     9352 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/__init__.py
+-rw-r--r--   0        0        0      701 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/algorithm.py
+-rw-r--r--   0        0        0     6017 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/enumeration.py
+-rw-r--r--   0        0        0      608 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/exception.py
+-rw-r--r--   0        0        0     4688 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/interactive.py
+-rw-r--r--   0        0        0     2684 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/latest/__init__.py
+-rw-r--r--   0        0        0     2659 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/latest/aio.py
+-rw-r--r--   0        0        0     3678 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/modelica.py
+-rw-r--r--   0        0        0     5511 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/openmodelica.py
+-rw-r--r--   0        0        0    19698 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/parser.py
+-rw-r--r--   0        0        0     1043 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/py.typed
+-rw-r--r--   0        0        0       77 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/session/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/session/_session.py
+-rw-r--r--   0        0        0       53 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/session/aio.py
+-rw-r--r--   0        0        0      656 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/session/aio.pyi
+-rw-r--r--   0        0        0     2208 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/string.py
+-rw-r--r--   0        0        0     1417 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/v_1_13/__init__.py
+-rw-r--r--   0        0        0   206114 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/v_1_13/_interface.py
+-rw-r--r--   0        0        0     1388 2023-07-29 15:29:19.930678 openmodelicacompiler-0.3.0a0/omc4py/v_1_13/aio.py
+-rw-r--r--   0        0        0   186123 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_13/aio.pyi
+-rw-r--r--   0        0        0     2537 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_14/__init__.py
+-rw-r--r--   0        0        0   270774 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_14/_interface.py
+-rw-r--r--   0        0        0     2508 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_14/aio.py
+-rw-r--r--   0        0        0   244195 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_14/aio.pyi
+-rw-r--r--   0        0        0     2641 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_15/__init__.py
+-rw-r--r--   0        0        0   287811 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_15/_interface.py
+-rw-r--r--   0        0        0     2612 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_15/aio.py
+-rw-r--r--   0        0        0   259256 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_15/aio.pyi
+-rw-r--r--   0        0        0     2757 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_16/__init__.py
+-rw-r--r--   0        0        0   283522 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_16/_interface.py
+-rw-r--r--   0        0        0     2728 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_16/aio.py
+-rw-r--r--   0        0        0   255564 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_16/aio.pyi
+-rw-r--r--   0        0        0     2711 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_17/__init__.py
+-rw-r--r--   0        0        0   281683 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_17/_interface.py
+-rw-r--r--   0        0        0     2682 2023-07-29 15:29:19.940679 openmodelicacompiler-0.3.0a0/omc4py/v_1_17/aio.py
+-rw-r--r--   0        0        0   253927 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_17/aio.pyi
+-rw-r--r--   0        0        0     2707 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_18/__init__.py
+-rw-r--r--   0        0        0   282149 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_18/_interface.py
+-rw-r--r--   0        0        0     2678 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_18/aio.py
+-rw-r--r--   0        0        0   254443 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_18/aio.pyi
+-rw-r--r--   0        0        0     2753 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_19/__init__.py
+-rw-r--r--   0        0        0   289160 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_19/_interface.py
+-rw-r--r--   0        0        0     2724 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_19/aio.py
+-rw-r--r--   0        0        0   260483 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_19/aio.pyi
+-rw-r--r--   0        0        0     2687 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_20/__init__.py
+-rw-r--r--   0        0        0   288034 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_20/_interface.py
+-rw-r--r--   0        0        0     2658 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_20/aio.py
+-rw-r--r--   0        0        0   259479 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_20/aio.pyi
+-rw-r--r--   0        0        0     2687 2023-07-29 15:29:19.950679 openmodelicacompiler-0.3.0a0/omc4py/v_1_21/__init__.py
+-rw-r--r--   0        0        0   290461 2023-07-29 15:29:19.960679 openmodelicacompiler-0.3.0a0/omc4py/v_1_21/_interface.py
+-rw-r--r--   0        0        0     2658 2023-07-29 15:29:19.960679 openmodelicacompiler-0.3.0a0/omc4py/v_1_21/aio.py
+-rw-r--r--   0        0        0   261694 2023-07-29 15:29:19.960679 openmodelicacompiler-0.3.0a0/omc4py/v_1_21/aio.pyi
+-rw-r--r--   0        0        0     2016 2023-07-29 15:29:19.960679 openmodelicacompiler-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0    10162 1970-01-01 00:00:00.000000 openmodelicacompiler-0.3.0a0/PKG-INFO
```

### Comparing `openmodelicacompiler-0.2.1/README.md` & `openmodelicacompiler-0.3.0a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,22 +100,23 @@
 
 ### About session API
 
 All session methods are _OpenModelica.Scripting.*_ functions. The names and types of arguments and return values are the same as the original modelica function, and session internally converts between the python class and the modelica class.
 
 If you want to know more about each session method, you can display it with the `help ()` function.
 
-- [UserGuide for OpenModelica Scripting API (v1.14)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.14/scripting_api.html)
-- [UserGuide for OpenModelica Scripting API (v1.15)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.15/scripting_api.html)
-- [UserGuide for OpenModelica Scripting API (v1.16)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.16/scripting_api.html)
-- [UserGuide for OpenModelica Scripting API (v1.17)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.17/scripting_api.html)
-- [UserGuide for OpenModelica Scripting API (v1.18)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.18/scripting_api.html)
-
 - [UserGuide for OpenModelica Scripting API (latest)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/latest/scripting_api.html)
-
+- [UserGuide for OpenModelica Scripting API (v1.21)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.21/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.20)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.20/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.19)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.19/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.18)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.18/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.17)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.17/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.16)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.16/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.15)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.15/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.14)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.14/scripting_api.html)
 
 [Documentation in OpenModelica build server](https://build.openmodelica.org/Documentation/OpenModelica.Scripting.html) shows exhaustive information about _OpenModelica.Scripting_. You will find sub-packages not explained user guide.
 
 - _OpenModelica.Scripting.Internal.*_
 - _OpenModelica.Scripting.Experimental.*_
 
 They are available from absolute reference
```

### Comparing `openmodelicacompiler-0.2.1/omc4py/exception.py` & `openmodelicacompiler-0.3.0a0/omc4py/exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from __future__ import annotations
+
 __all__ = (
     "OMCError",
     "OMCException",
     "OMCRuntimeError",
     "OMCWarning",
 )
 
-import typing
 import warnings
 
 
 def warn_always(
-    warning_type: typing.Type[Warning],
-) -> typing.Type[Warning]:
+    warning_type: type[Warning],
+) -> type[Warning]:
     warnings.simplefilter("always", warning_type)
     return warning_type
 
 
 class OMCException(
     Exception,
 ):
```

### Comparing `openmodelicacompiler-0.2.1/omc4py/session.py` & `openmodelicacompiler-0.3.0a0/omc4py/openmodelica.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,207 +1,208 @@
-import abc
-import re
-import typing
-import warnings
-
-from . import compiler, exception
-from .classes import (
-    AbstractOMCInteractive,
-    AbstractOMCSession,
-    Component,
-    String,
-    TypeName,
-)
-from .parser import (
-    ComponentTuple,
-    parse_components,
-    parse_OMCExceptions,
-    parse_OMCValue,
-)
-
-
-def __select_session_type(
-    omc: AbstractOMCInteractive,
-) -> typing.Type[AbstractOMCSession]:
-    """
-    Session class selector.
-    Update this after new omc version supported!!!
-    """
-    from . import (
-        v_1_13,
-        v_1_14,
-        v_1_15,
-        v_1_16,
-        v_1_17,
-        v_1_18,
-        v_1_19,
-        v_1_20,
-    )
-
-    version = OMCSessionMinimal(omc).getVersionTuple()
-    if version[:2] <= (1, 13):
-        return v_1_13.OMCSession
-    elif version[:2] == (1, 14):
-        return v_1_14.OMCSession
-    elif version[:2] == (1, 15):
-        return v_1_15.OMCSession
-    elif version[:2] == (1, 16):
-        return v_1_16.OMCSession
-    elif version[:2] == (1, 17):
-        return v_1_17.OMCSession
-    elif version[:2] == (1, 18):
-        return v_1_18.OMCSession
-    elif version[:2] == (1, 19):
-        return v_1_19.OMCSession
-    elif version[:2] == (1, 20):
-        return v_1_20.OMCSession
-    else:
-        return v_1_20.OMCSession
-
-
-def open_session(
-    omc_command: typing.Optional[compiler.StrOrPathLike] = None,
-    *,
-    session_type: typing.Optional[typing.Type[AbstractOMCSession]] = None,
-) -> AbstractOMCSession:
-    omc = compiler.OMCInteractive.open(omc_command)
-
-    try:
-        if session_type is None:
-            session_type = __select_session_type(omc)
-        else:
-            if not issubclass(session_type, AbstractOMCSession):
-                raise TypeError(
-                    "session_type must be "
-                    f"subclass of {AbstractOMCSession}, "
-                    f"got {session_type}"
-                )
-
-        return session_type(omc)
-
-    except Exception:
-        omc.close()
-        raise
-
-
-class OMCSessionBase(
-    AbstractOMCSession,
-):
-    def getComponents(
-        self, name: TypeName
-    ) -> typing.Optional[typing.List[ComponentTuple]]:
-        result_literal = self.__omc__.evaluate(
-            f"getComponents({TypeName(name)})"
-        )
+from __future__ import annotations
 
-        # return None if result_literal == "\n"
-        if not result_literal or result_literal.isspace():
-            return None
-
-        try:
-            result_value = parse_components(result_literal)
-        except Exception:
-            excs = list(parse_OMCExceptions(result_literal))
-            if not excs:
-                raise exception.OMCRuntimeError(result_literal) from None
-            else:
-                for exc in excs:
-                    if isinstance(exc, Warning):
-                        warnings.warn(exc)
-                    else:
-                        raise exc from None
-                else:
-                    return None
-
-        return result_value
-
-
-class OMCSessionBase__v_1_13(
-    OMCSessionBase,
-):
-    @abc.abstractmethod
-    def getMessagesStringInternal(
-        self,
-        unique: bool,
-    ) -> typing.Iterable:
-        ...
-
-    def __check__(
-        self,
-    ):
-        for messageString in self.getMessagesStringInternal(unique=True):
-            message = str(messageString.message)
-            kind = messageString.kind.name
-            py_message = f"{kind!s}: {message!r}"
-            level = messageString.level.name
-
-            if level == "notification":
-                warnings.warn(exception.OMCNotification(py_message))
-            elif level == "warning":
-                warnings.warn(exception.OMCWarning(py_message))
-            elif level == "error":
-                raise exception.OMCError(py_message)
-            else:
-                raise exception.OMCRuntimeError(
-                    f"Unexpected message level, got {level}"
-                )
+__all__ = ("Component", "TypeName", "VariableName")
 
+import itertools
+from collections.abc import Callable, Iterable, Iterator
+from typing import TYPE_CHECKING, Any, List, NamedTuple, TypeVar, Union
 
-class OMCSessionMinimal(
-    OMCSessionBase,
-):
-    def __check__(
-        self,
-    ) -> None:
-        for exc in parse_OMCExceptions(self.getErrorString()):
-            if isinstance(exc, Warning):
-                warnings.warn(exc)
-            else:
-                raise exc
+from typing_extensions import Literal
 
-    def getComponents(
-        self, name: TypeName
-    ) -> typing.Optional[typing.List[ComponentTuple]]:
-        result = super().getComponents(name)
-        self.__check__()
-        return result
-
-    def getErrorString(
-        self,
-    ) -> str:
-        __result = self.__omc__.call_function(
-            funcName="getErrorString",
-            inputArguments=[],
-            outputArguments=[(Component(String), "errorString")],
-            parser=parse_OMCValue,
-        )
-        return str(__result)
+from .string import to_omc_literal
 
-    def getVersion(
-        self,
-    ) -> str:
-        __result = self.__omc__.call_function(
-            funcName="getVersion",
-            inputArguments=[],
-            outputArguments=[
-                (Component(String), "version"),
-            ],
-            parser=parse_OMCValue,
-        )
-        self.__check__()
-        return str(__result)
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+
+class Component(NamedTuple):
+    className: TypeName
+    name: VariableName
+    comment: str
+    protected: Literal["protected", "public"]
+    isFinal: bool
+    isFlow: bool
+    isStream: bool
+    isReplaceable: bool
+    variability: Literal["constant", "parameter", "discrete", "unspecified"]
+    innerOuter: Literal["inner", "outer", "none"]
+    inputOutput: Literal["input", "output", "unspecified"]
+    dimensions: List[str]
+
+
+# Type hints
+
+KT = TypeVar("KT")
+
+VariableNameLike = Union[
+    "TypeName",
+    "VariableName",
+    str,
+]
+
+TypeNameLike = VariableNameLike
 
-    def getVersionTuple(
-        self,
-    ) -> typing.Tuple[int, int, int]:
-        versionMatch = re.search(
-            r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<build>\d+)",
-            self.getVersion(),
-        )
-        if versionMatch is None:
-            raise ValueError("Can't parse version string")
 
+# $Code classes OpenModelica.$Code.{VariableName, TypeName}
+
+
+class _BaseVariableName:
+    __slots__ = ("__identifier",)
+    __identifier: str
+
+    def __new__(cls, identifier: str) -> Self:
+        self = super(_BaseVariableName, cls).__new__(cls)
+        self.__identifier = identifier
+        return self
+
+    def __eq__(self, other: Any) -> bool:
         return (
-            int(versionMatch.group("major")),
-            int(versionMatch.group("minor")),
-            int(versionMatch.group("build")),
+            isinstance(other, _BaseVariableName)
+            and self.__identifier == other.__identifier
+        )
+
+    def __hash__(self) -> int:
+        return hash(self.__identifier)
+
+    def __str__(self) -> str:
+        return self.__identifier
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.__identifier!r})"
+
+    __to_omc_literal__ = __str__
+
+
+class VariableName(_BaseVariableName):
+    def __new__(cls, obj: VariableNameLike) -> Self:
+        from .parser import is_variablename
+
+        if isinstance(obj, cls):
+            return obj
+
+        if isinstance(obj, str):
+            identifier = obj
+        elif isinstance(obj, TypeName):
+            identifier = to_omc_literal(obj)
+        else:
+            raise TypeError(
+                "obj must be TypeName, VariableName or str, "
+                f"got {obj!r}: {type(obj)}"
+            )
+
+        if not is_variablename(identifier):
+            raise ValueError(
+                f"Invalid modelica identifier, got {identifier!r}"
+            )
+
+        return _BaseVariableName.__new__(cls, identifier)
+
+
+class _BaseTypeName:
+    __slots__ = ("parts",)
+
+    parts: tuple[str, ...]
+
+    def __new__(cls, parts: tuple[str, ...]) -> Self:
+        self = super(_BaseTypeName, cls).__new__(cls)
+        self.parts = parts
+        return self
+
+    @property
+    def is_absolute(self) -> bool:
+        return bool(self.parts) and self.parts[0] == "."
+
+    def as_absolute(self) -> Self:
+        if self.is_absolute:
+            return self
+        else:
+            return _BaseTypeName.__new__(type(self), (".", *self.parts))
+
+    @property
+    def last_identifier(self) -> VariableName:
+        return VariableName(self.parts[-1])
+
+    @property
+    def parents(self) -> Iterator[Self]:
+        for end in reversed(range(1, len(self.parts))):
+            yield _BaseTypeName.__new__(
+                type(self),
+                self.parts[:end],
+            )
+
+    @property
+    def parent(self) -> Self:
+        for parent in self.parents:
+            return parent
+        else:
+            return self
+
+    def __hash__(self) -> int:
+        return hash(self.parts)
+
+    def __eq__(self, other: Any) -> bool:
+        return isinstance(other, _BaseTypeName) and self.parts == other.parts
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.parts})"
+
+    def __str__(self) -> str:
+        if self.is_absolute:
+            return self.parts[0] + ".".join(self.parts[1:])
+        else:
+            return ".".join(self.parts)
+
+    __to_omc_literal__ = __str__
+
+
+class TypeName(_BaseTypeName):
+    def __new__(cls, part: TypeNameLike, *parts: TypeNameLike) -> Self:
+        if isinstance(part, cls) and not parts:
+            return part
+
+        return _BaseTypeName.__new__(
+            cls, tuple(TypeName.__split_parts((part, *parts)))
         )
+
+    @staticmethod
+    def __split_parts(parts: Iterable[TypeNameLike]) -> Iterator[str]:
+        for i, part in enumerate(
+            itertools.chain(*map(TypeName.__split_part, parts))
+        ):
+            if part == "." and not i == 0:
+                raise ValueError(f"parts[{i}] is invalid, got {part!r}")
+            yield part
+
+    @staticmethod
+    def __split_part(part: TypeNameLike) -> Iterator[str]:
+        from .parser import split_typename_parts
+
+        if isinstance(part, TypeName):
+            yield from part.parts
+        elif isinstance(part, VariableName):
+            yield str(part)
+        elif isinstance(part, str):
+            if part == ".":
+                yield part
+            else:
+                yield from split_typename_parts(part)
+        else:
+            raise TypeError(f"Unexpected part, got {part}: {type(part)}")
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({str(self)!r})"
+
+    def __truediv__(self, other: TypeNameLike) -> Self:
+        return type(self)(self, other)
+
+
+def split_dict(
+    dictionary: dict[KT, Any],
+    condition: Callable[[Any], bool],
+) -> tuple[dict[KT, Any], dict[KT, Any]]:
+    yes, no = {}, {}
+    for k, v in dictionary.items():
+        if condition(v):
+            yes[k] = v
+        else:
+            no[k] = v
+    return yes, no
```

### Comparing `openmodelicacompiler-0.2.1/pyproject.toml` & `openmodelicacompiler-0.3.0a0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenModelicaCompiler"
-version = "0.2.1"
+version = "0.3.0a0"
 description = "OpenModelica compiler (omc) interface for Python"
 repository = "https://github.com/ijknabla/OpenModelicaCompilerForPython"
 authors = ["ijknabla <ijknabla@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0, OSMC-PL 1.2 (user's choice)"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -14,54 +14,72 @@
     "Topic :: Software Development :: User Interfaces",
 ]
 packages = [
     { include = "omc4py"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 Arpeggio = ">=1.6"
-numpy = ">=1.7.0"
+exceptiongroup = ">=1.0"
 pyzmq = ">=17.0.0"
-typing-extensions = ">=3.7.2"
+typing-extensions = ">=3.7.4.2"
 modelicalang = "^0.1.0a0"
 
-[tool.poetry.group.dev.dependencies]
-inquirer = "^2.8.0"
-lxml = "^4.9.2"
+[tool.poetry.group.bootstrap.dependencies]
+click = "^8.1.3"
+pyyaml = "^6.0"
 tqdm = "^4.62.3"
+
+[tool.poetry.group.dev.dependencies]
 isort = "^5.8"
-black = ">=20.8.b1"
+black = ">=23"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "^0.971"
+mypy = "^1"
 pyproject-flake8 = "^0.0.1-alpha.2"
 types-arpeggio = {git = "https://github.com/ijknabla/types-arpeggio.git", rev = "main"}
+types-pyyaml = "^6.0.12.10"
 types-setuptools = "^65.7.0.3"
+types-tqdm = "^4.65.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^6.2.5"
+pytest-asyncio = "^0.20"
+pytest-cov = "^4.0.0"
 pytest-dependency = "^0.5.1"
+typing-extensions = ">=4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
+[tool.coverage.report]
+exclude_lines = [
+    "^\\s*class \\w+\\(Protocol",
+    "^\\s*@overload$",
+    "^\\s*if TYPE_CHECKING",
+    "^\\s*raise NotImplementedError",
+    "#\\s*pragma\\s*:\\s*no\\s*cover",
+]
+
 [tool.flake8]
 exclude = ".venv"
 
 # Allow too-long line in auto-generated modules
-per-file-ignores = "omc4py/*/_omc_interface.py:E501"
-
-# The current omc4py metaclass is inevitably complicated
-# to express the behavior of the Modelica class.
-max-complexity = 20
-
-# Ignore whitespace before colon
-extend-ignore = "E203,"
+per-file-ignores = """
+    omc4py/enumeration.py:E501,
+    omc4py/v_*_*/*.py:E501,
+"""
 
 [tool.isort]
 profile = "black"
 line_length = 79
+
+[[tool.mypy.overrides]]
+module = [
+    "numpy",
+]
+ignore_missing_imports = true
```

### Comparing `openmodelicacompiler-0.2.1/setup.py` & `openmodelicacompiler-0.3.0a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,292 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openmodelicacompiler
+Version: 0.3.0a0
+Summary: OpenModelica compiler (omc) interface for Python
+Home-page: https://github.com/ijknabla/OpenModelicaCompilerForPython
+License: GPL-3.0, OSMC-PL 1.2 (user's choice)
+Author: ijknabla
+Author-email: ijknabla@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: User Interfaces
+Requires-Dist: Arpeggio (>=1.6)
+Requires-Dist: exceptiongroup (>=1.0)
+Requires-Dist: modelicalang (>=0.1.0a0,<0.2.0)
+Requires-Dist: pyzmq (>=17.0.0)
+Requires-Dist: typing-extensions (>=3.7.4.2)
+Project-URL: Repository, https://github.com/ijknabla/OpenModelicaCompilerForPython
+Description-Content-Type: text/markdown
 
-packages = \
-['omc4py',
- 'omc4py.parser',
- 'omc4py.v_1_13',
- 'omc4py.v_1_14',
- 'omc4py.v_1_15',
- 'omc4py.v_1_16',
- 'omc4py.v_1_17',
- 'omc4py.v_1_18',
- 'omc4py.v_1_19',
- 'omc4py.v_1_20']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Arpeggio>=1.6',
- 'modelicalang>=0.1.0a0,<0.2.0',
- 'numpy>=1.7.0',
- 'pyzmq>=17.0.0',
- 'typing-extensions>=3.7.2']
-
-setup_kwargs = {
-    'name': 'openmodelicacompiler',
-    'version': '0.2.1',
-    'description': 'OpenModelica compiler (omc) interface for Python',
-    'long_description': '\n# OpenModelicaCompilerForPython [![License: OSMC-PL](https://img.shields.io/badge/license-OSMC--PL-lightgrey.svg)](./COPYING) [![lint.yml](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/lint.yml/badge.svg)](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/lint.yml) [![Pytest](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/test.yml/badge.svg)](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/test.yml)\n\nOpenModelica compiler (omc) interface for Python\n\n## Change log\n\n[See CHANGELOG.md](./CHANGELOG.md)\n\n## Quick tour\n\n### Setup\n\nMake sure that OpenModelica is installed on your system.\n\n```bash\n$ omc --version\n```\n\nOpenModelica official page [https://openmodelica.org/](https://openmodelica.org/)\n\nInstall OpenModelicaCompiler with pip.\n\n```bash\n$ python3 -m pip install OpenModelicaCompiler\n```\n\n`omc4py` is acutual package name. `omc4py.open_session()` will return session object which interfaces to omc.\n\n```python3\n#!/usr/bin/env python3\nimport omc4py\n\nwith omc4py.open_session() as session:\n    print(session.getVersion())\n```\n\n### More usage about `open_session(...)`\n\nIf `omc4py.open_session` cannot find omc, such as if you have not added OpenModelica to your _PATH_ environment variable, you can specify a valid omc command name or omc executable path by `str`.\n\n```python3\nimport omc4py\n\nwith omc4py.open_session(\n    "C:/OpenModelica1.13.0-64bit/bin/omc.exe"\n) as session:\n    print(session.getVersion())\n```\n\nIt is also possible to open multiple sessions with different versions of omc at the same time by explicitly specifying omc.\n\n```python3\nimport omc4py\n\nwith \\\n    omc4py.open_session(\n        "C:/OpenModelica1.13.0-64bit/bin/omc.exe"\n    ) as session_13, \\\n    omc4py.open_session(\n        "C:/Program Files/OpenModelica1.14.0-64bit/bin/omc.exe"\n    ) as session_14:\n\n    print("v1.13.0:", session_13.getVersion())\n    print("v1.14.0:", session_14.getVersion())\n```\n\nAs shown above, __it is recommended to ensure that session is closed by calling `omc4py.open_session()` via with-statement__.\n\nHowever, sometimes you want to use session interactively, like OMShell. `omc4py` closes all unclosed sessions when exiting the python interpreter.\n\n```python3\n>>> from omc4py import *\n>>> session = open_session()\n>>> session.loadString("""\n... package A\n...     package B\n...             package C\n...             end C;\n...     end B;\n... end A;\n... """)\nTrue\n>>> list(session.getClassNames("A", recursive=True))\n[TypeName(\'A\'), TypeName(\'A.B\'), TypeName(\'A.B.C\')]\n>>>\n>>>\n>>> exit()  # session will be closed internally\n```\n\nBesides, session object has `__close__` method to explicitly close session.\n\n```python3\n>>> from omc4py import *\n>>> session = open_session()\n>>> session.__close__()\n>>>\n>>> exit()\n```\n\n### About session API\n\nAll session methods are _OpenModelica.Scripting.*_ functions. The names and types of arguments and return values are the same as the original modelica function, and session internally converts between the python class and the modelica class.\n\nIf you want to know more about each session method, you can display it with the `help ()` function.\n\n- [UserGuide for OpenModelica Scripting API (v1.14)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.14/scripting_api.html)\n- [UserGuide for OpenModelica Scripting API (v1.15)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.15/scripting_api.html)\n- [UserGuide for OpenModelica Scripting API (v1.16)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.16/scripting_api.html)\n- [UserGuide for OpenModelica Scripting API (v1.17)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.17/scripting_api.html)\n- [UserGuide for OpenModelica Scripting API (v1.18)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.18/scripting_api.html)\n\n- [UserGuide for OpenModelica Scripting API (latest)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/latest/scripting_api.html)\n\n\n[Documentation in OpenModelica build server](https://build.openmodelica.org/Documentation/OpenModelica.Scripting.html) shows exhaustive information about _OpenModelica.Scripting_. You will find sub-packages not explained user guide.\n\n- _OpenModelica.Scripting.Internal.*_\n- _OpenModelica.Scripting.Experimental.*_\n\nThey are available from absolute reference\n\n```python3\n# Example for "timerTick" and "timerTock"\n# in "OpenModelica.Scripting.Internal.Time"\nfrom omc4py import open_session\nfrom time import sleep\n\ntimer_index: int = 1\n\nwith open_session() as session:\n    session.OpenModelica.Scripting.Internal.Time.timerTick(timer_index)\n\n    sleep(0.1)\n\n    # show elapsed time from last timerTick\n    print(session.OpenModelica.Scripting.Internal.Time.timerTock(timer_index))\n```\n\n- - -\n\nLet me introduce typical API functions!\n\n#### `loadModel`\n\nLoad library and returns True if success. You can specify versions by second argument\n\n```python3\nimport omc4py\n\nwith omc4py.open_session() as session:\n    assert(session.loadModel("Modelica"))  # load MSL\n```\n\n```python3\nimport omc4py\n\nwith omc4py.open_session() as session:\n    assert(session.loadModel("Modelica", ["3.2.3"]))  # load MSL 3.2.3\n```\n\n#### `getClassNames`\n\nReturns array of class names in the given class\n\n```python3\nimport omc4py\n\nwith omc4py.open_session() as session:\n    assert(session.loadModel("Modelica"))\n    for className in session.getClassNames("Modelica"):\n        print(className)\n```\n\nBy default, `getClassNames()` only returns "sub" classes. If you want to know all classes belongs to the class set `recursive=True`.\n\n```python3\nimport omc4py\n\nwith omc4py.open_session() as session:\n    assert(session.loadModel("Modelica"))\n    for className in session.getClassNames("Modelica", recursive=True):\n        print(className)  # many class names will be printed\n```\n\n#### `getComponents`\n\nReturns array of component (variable, parameter, constant, ...etc) profiles\n\n```python3\nimport omc4py\n\nwith omc4py.open_session() as session:\n    assert(session.loadModel("Modelica", ["3.2.3"]))\n    for component in session.getComponents("Modelica.Constants"):\n        print(\n            f"{component.className.last_identifier!s:<20}"\n            f"{component.name!s:<15}"\n            f"{component.comment!r}"\n        )\n```\n\n- - -\n\n#### Exception handling\n\n<!--\n@startuml\nnamespace omc4py.exception {\n    OMCException <-- OMCNotification\n    OMCException <-- OMCWarning\n    OMCException <-- OMCError\n    OMCException <-- OMCRuntimeError\n}\n\nException <-- omc4py.exception.OMCException\n\nException <-ri- Warning\nWarning <-- omc4py.exception.OMCNotification\nWarning <-- omc4py.exception.OMCWarning\n\nException <-ri- RuntimeError\nRuntimeError <-- omc4py.exception.OMCRuntimeError\n@enduml\n-->\n![class diagram of omc4py.exception](http://www.plantuml.com/plantuml/svg/SoWkIImgAStDuSfBp4qjBaXCJbN8pqqsAQZKIwr8JYqeoSpFKwZcKW02VrzdLxYGZQukIC0lloGpBJCv4II6Kr5uOb5UPbuwJddNegBy8fooGQLv9PcvgH15jLnSA0emtAg7R0Igug9CNGMOKw0qTYFG_4LGCLGUqpOKfoDpS1g5eiCXDIy563C0)\n\n- `OMCNotification`, `OMCWarning`, `OMCError` are raised from _omc_\n- `OMCRuntimeError` is raised from `omc4py` python implementation (not from _omc_)\n\nWe are not sure about whole OpenModelica\'s exception handling policy.\nThrough `omc4py` project, We found that there are 4 situation for expection caused by function calls.\n\nomc behavior\n\n1. Function returns "\\n" instead of valid value (no exception info)\n1. Function returns formatted error messages (contains sourceInfo, level, kind, message) instead of valid value\n1. Function returns unformatted error message (typically, startswith "* Error") instead of valid value\n1. Function returns valid value and set exception messages internally\n\n`omc4py` behavior\n\n1) function returns `None` instead of valid result (no exception will be sent)\n1) function send `OMCNotification` or `OMCWarning`, or raise `OMCError`\n1) function raise `OMCRuntimeError` with the message returned by the omc\n1) function returns valid value. You can check exceptions explicitly by `session.__check__()`\n\nNormally, 4th case seems to be _notification_ or _warning_. If you want to be sure to check for exceptions, call `session.__check__()` before exit doubtful context.\n\n```python3\nfrom omc4py import open_session\n\ndef doubtful_task(session):\n    # session.doubtful_API1(...)\n    # session.doubtful_API2(...)\n    # session.doubtful_API3(...)\n    session.__check__()\n\nwith open_session() as session:\n    doubtful_task(session)\n```\n',
-    'author': 'ijknabla',
-    'author_email': 'ijknabla@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ijknabla/OpenModelicaCompilerForPython',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+
+# OpenModelicaCompilerForPython [![License: OSMC-PL](https://img.shields.io/badge/license-OSMC--PL-lightgrey.svg)](./COPYING) [![lint.yml](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/lint.yml/badge.svg)](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/lint.yml) [![Pytest](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/test.yml/badge.svg)](https://github.com/ijknabla/OpenModelicaCompilerForPython/actions/workflows/test.yml)
+
+OpenModelica compiler (omc) interface for Python
+
+## Change log
+
+[See CHANGELOG.md](./CHANGELOG.md)
+
+## Quick tour
+
+### Setup
+
+Make sure that OpenModelica is installed on your system.
+
+```bash
+$ omc --version
+```
+
+OpenModelica official page [https://openmodelica.org/](https://openmodelica.org/)
+
+Install OpenModelicaCompiler with pip.
+
+```bash
+$ python3 -m pip install OpenModelicaCompiler
+```
+
+`omc4py` is acutual package name. `omc4py.open_session()` will return session object which interfaces to omc.
+
+```python3
+#!/usr/bin/env python3
+import omc4py
+
+with omc4py.open_session() as session:
+    print(session.getVersion())
+```
+
+### More usage about `open_session(...)`
+
+If `omc4py.open_session` cannot find omc, such as if you have not added OpenModelica to your _PATH_ environment variable, you can specify a valid omc command name or omc executable path by `str`.
+
+```python3
+import omc4py
+
+with omc4py.open_session(
+    "C:/OpenModelica1.13.0-64bit/bin/omc.exe"
+) as session:
+    print(session.getVersion())
+```
+
+It is also possible to open multiple sessions with different versions of omc at the same time by explicitly specifying omc.
+
+```python3
+import omc4py
+
+with \
+    omc4py.open_session(
+        "C:/OpenModelica1.13.0-64bit/bin/omc.exe"
+    ) as session_13, \
+    omc4py.open_session(
+        "C:/Program Files/OpenModelica1.14.0-64bit/bin/omc.exe"
+    ) as session_14:
+
+    print("v1.13.0:", session_13.getVersion())
+    print("v1.14.0:", session_14.getVersion())
+```
+
+As shown above, __it is recommended to ensure that session is closed by calling `omc4py.open_session()` via with-statement__.
+
+However, sometimes you want to use session interactively, like OMShell. `omc4py` closes all unclosed sessions when exiting the python interpreter.
+
+```python3
+>>> from omc4py import *
+>>> session = open_session()
+>>> session.loadString("""
+... package A
+...     package B
+...             package C
+...             end C;
+...     end B;
+... end A;
+... """)
+True
+>>> list(session.getClassNames("A", recursive=True))
+[TypeName('A'), TypeName('A.B'), TypeName('A.B.C')]
+>>>
+>>>
+>>> exit()  # session will be closed internally
+```
+
+Besides, session object has `__close__` method to explicitly close session.
+
+```python3
+>>> from omc4py import *
+>>> session = open_session()
+>>> session.__close__()
+>>>
+>>> exit()
+```
+
+### About session API
+
+All session methods are _OpenModelica.Scripting.*_ functions. The names and types of arguments and return values are the same as the original modelica function, and session internally converts between the python class and the modelica class.
+
+If you want to know more about each session method, you can display it with the `help ()` function.
+
+- [UserGuide for OpenModelica Scripting API (latest)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/latest/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.21)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.21/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.20)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.20/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.19)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.19/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.18)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.18/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.17)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.17/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.16)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.16/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.15)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.15/scripting_api.html)
+- [UserGuide for OpenModelica Scripting API (v1.14)](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/1.14/scripting_api.html)
+
+[Documentation in OpenModelica build server](https://build.openmodelica.org/Documentation/OpenModelica.Scripting.html) shows exhaustive information about _OpenModelica.Scripting_. You will find sub-packages not explained user guide.
+
+- _OpenModelica.Scripting.Internal.*_
+- _OpenModelica.Scripting.Experimental.*_
+
+They are available from absolute reference
+
+```python3
+# Example for "timerTick" and "timerTock"
+# in "OpenModelica.Scripting.Internal.Time"
+from omc4py import open_session
+from time import sleep
+
+timer_index: int = 1
+
+with open_session() as session:
+    session.OpenModelica.Scripting.Internal.Time.timerTick(timer_index)
+
+    sleep(0.1)
+
+    # show elapsed time from last timerTick
+    print(session.OpenModelica.Scripting.Internal.Time.timerTock(timer_index))
+```
+
+- - -
+
+Let me introduce typical API functions!
+
+#### `loadModel`
+
+Load library and returns True if success. You can specify versions by second argument
+
+```python3
+import omc4py
+
+with omc4py.open_session() as session:
+    assert(session.loadModel("Modelica"))  # load MSL
+```
+
+```python3
+import omc4py
+
+with omc4py.open_session() as session:
+    assert(session.loadModel("Modelica", ["3.2.3"]))  # load MSL 3.2.3
+```
+
+#### `getClassNames`
+
+Returns array of class names in the given class
+
+```python3
+import omc4py
+
+with omc4py.open_session() as session:
+    assert(session.loadModel("Modelica"))
+    for className in session.getClassNames("Modelica"):
+        print(className)
+```
+
+By default, `getClassNames()` only returns "sub" classes. If you want to know all classes belongs to the class set `recursive=True`.
+
+```python3
+import omc4py
+
+with omc4py.open_session() as session:
+    assert(session.loadModel("Modelica"))
+    for className in session.getClassNames("Modelica", recursive=True):
+        print(className)  # many class names will be printed
+```
+
+#### `getComponents`
+
+Returns array of component (variable, parameter, constant, ...etc) profiles
+
+```python3
+import omc4py
+
+with omc4py.open_session() as session:
+    assert(session.loadModel("Modelica", ["3.2.3"]))
+    for component in session.getComponents("Modelica.Constants"):
+        print(
+            f"{component.className.last_identifier!s:<20}"
+            f"{component.name!s:<15}"
+            f"{component.comment!r}"
+        )
+```
+
+- - -
+
+#### Exception handling
+
+<!--
+@startuml
+namespace omc4py.exception {
+    OMCException <-- OMCNotification
+    OMCException <-- OMCWarning
+    OMCException <-- OMCError
+    OMCException <-- OMCRuntimeError
 }
 
+Exception <-- omc4py.exception.OMCException
+
+Exception <-ri- Warning
+Warning <-- omc4py.exception.OMCNotification
+Warning <-- omc4py.exception.OMCWarning
+
+Exception <-ri- RuntimeError
+RuntimeError <-- omc4py.exception.OMCRuntimeError
+@enduml
+-->
+![class diagram of omc4py.exception](http://www.plantuml.com/plantuml/svg/SoWkIImgAStDuSfBp4qjBaXCJbN8pqqsAQZKIwr8JYqeoSpFKwZcKW02VrzdLxYGZQukIC0lloGpBJCv4II6Kr5uOb5UPbuwJddNegBy8fooGQLv9PcvgH15jLnSA0emtAg7R0Igug9CNGMOKw0qTYFG_4LGCLGUqpOKfoDpS1g5eiCXDIy563C0)
+
+- `OMCNotification`, `OMCWarning`, `OMCError` are raised from _omc_
+- `OMCRuntimeError` is raised from `omc4py` python implementation (not from _omc_)
+
+We are not sure about whole OpenModelica's exception handling policy.
+Through `omc4py` project, We found that there are 4 situation for expection caused by function calls.
+
+omc behavior
+
+1. Function returns "\n" instead of valid value (no exception info)
+1. Function returns formatted error messages (contains sourceInfo, level, kind, message) instead of valid value
+1. Function returns unformatted error message (typically, startswith "* Error") instead of valid value
+1. Function returns valid value and set exception messages internally
+
+`omc4py` behavior
+
+1) function returns `None` instead of valid result (no exception will be sent)
+1) function send `OMCNotification` or `OMCWarning`, or raise `OMCError`
+1) function raise `OMCRuntimeError` with the message returned by the omc
+1) function returns valid value. You can check exceptions explicitly by `session.__check__()`
+
+Normally, 4th case seems to be _notification_ or _warning_. If you want to be sure to check for exceptions, call `session.__check__()` before exit doubtful context.
+
+```python3
+from omc4py import open_session
+
+def doubtful_task(session):
+    # session.doubtful_API1(...)
+    # session.doubtful_API2(...)
+    # session.doubtful_API3(...)
+    session.__check__()
+
+with open_session() as session:
+    doubtful_task(session)
+```
 
-setup(**setup_kwargs)
```

