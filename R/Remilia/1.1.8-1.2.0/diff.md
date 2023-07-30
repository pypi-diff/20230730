# Comparing `tmp/remilia-1.1.8.tar.gz` & `tmp/remilia-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remilia-1.1.8.tar", last modified: Wed Jun 21 05:16:52 2023, max compression
+gzip compressed data, was "remilia-1.2.0.tar", last modified: Sun Jul 30 03:02:46 2023, max compression
```

## Comparing `remilia-1.1.8.tar` & `remilia-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,26 @@
--rw-r--r--   0        0        0     1063 2023-06-21 05:16:27.809928 remilia-1.1.8/LICENSE
--rw-r--r--   0        0        0     1063 2023-06-21 05:16:27.809928 remilia-1.1.8/LICENSE
--rw-r--r--   0        0        0      795 2023-06-21 05:16:27.809928 remilia-1.1.8/README.md
--rw-r--r--   0        0        0      795 2023-06-21 05:16:27.809928 remilia-1.1.8/README.md
--rw-r--r--   0        0        0     1282 2023-06-21 05:16:52.766036 remilia-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      220 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/__init__.py
--rw-r--r--   0        0        0      128 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/base/__init__.py
--rw-r--r--   0        0        0       33 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/base/exceptions.py
--rw-r--r--   0        0        0      694 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/base/models.py
--rw-r--r--   0        0        0     1881 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/base/rtypes.py
--rw-r--r--   0        0        0     5156 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/log.py
--rw-r--r--   0        0        0     3111 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/mixin.py
--rw-r--r--   0        0        0     5085 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/mixin_decorations/__init__.py
--rw-r--r--   0        0        0     3255 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/mixin_decorations/omixin.py
--rw-r--r--   0        0        0     5280 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/res.py
--rw-r--r--   0        0        0     4868 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/structdb.py
--rw-r--r--   0        0        0      997 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/DecoratorUtils.py
--rw-r--r--   0        0        0     1851 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/SignParas.py
--rw-r--r--   0        0        0      158 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/__init__.py
--rw-r--r--   0        0        0      764 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/cli/prompts_extension/__init__.py
--rw-r--r--   0        0        0       71 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/net/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/net/pixiv.py
--rw-r--r--   0        0        0       41 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/os/__init__.py
--rw-r--r--   0        0        0       51 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/os/win/__init__.py
--rw-r--r--   0        0        0      360 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/os/win/exeutils.py
--rw-r--r--   0        0        0     4163 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/thread/Timeout.py
--rw-r--r--   0        0        0      241 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/thread/__init__.py
--rw-r--r--   0        0        0     1149 2023-06-21 05:16:27.809928 remilia-1.1.8/src/Remilia/utils/thread/terminable_thread.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 remilia-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-30 03:02:06.674510 remilia-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1063 2023-07-30 03:02:06.674510 remilia-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1009 2023-07-30 03:02:06.674510 remilia-1.2.0/README.md
+-rw-r--r--   0        0        0     1009 2023-07-30 03:02:06.674510 remilia-1.2.0/README.md
+-rw-r--r--   0        0        0     1282 2023-07-30 03:02:46.158661 remilia-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-30 03:02:46.154661 remilia-1.2.0/src/Remilia/__version__.py
+-rw-r--r--   0        0        0      102 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/exceptions.py
+-rw-r--r--   0        0        0      695 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/models.py
+-rw-r--r--   0        0        0     1920 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/rtypes.py
+-rw-r--r--   0        0        0     5161 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/log.py
+-rw-r--r--   0        0        0    13515 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/mixin.py
+-rw-r--r--   0        0        0     5280 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/res.py
+-rw-r--r--   0        0        0     5182 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/shadow.py
+-rw-r--r--   0        0        0      518 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/signs.py
+-rw-r--r--   0        0        0     5797 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/structdb.py
+-rw-r--r--   0        0        0      151 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/__init__.py
+-rw-r--r--   0        0        0      628 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/cli/prompts_extension/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/misc.py
+-rw-r--r--   0        0        0     6579 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/pixiv.py
+-rw-r--r--   0        0        0     4163 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/thread/Timeout.py
+-rw-r--r--   0        0        0      242 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/thread/__init__.py
+-rw-r--r--   0        0        0     1149 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/thread/terminable_thread.py
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 remilia-1.2.0/PKG-INFO
```

### Comparing `remilia-1.1.8/LICENSE` & `remilia-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remilia-1.1.8/README.md` & `remilia-1.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 <div align=center>
   <img width=200 src="https://raw.githubusercontent.com/H2Sxxa/Remilia/main/background.png"  alt="[BG](https://raw.githubusercontent.com/H2Sxxa/Remilia/main/background.png)"/>
-  <h1 align="center">Remilia</h1> 
+  <h1 align="center">Remilia</h1>
 </div>
+
 <div align=center>
   <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">
   <img src="https://img.shields.io/github/languages/code-size/H2Sxxa/Remilia" alt="size">
   <img src="https://img.shields.io/github/license/H2Sxxa/Remilia" alt="license">
 </div>
 
-# Install
+# What's this?
 
-```shell
-pip install Remilia
-```
+A package with many utils, in order to help build application faster.
 
-# Quick start
+use Remilia,you can print colorful log,you can use mixin to modify any class(but most build-in class not supported),you can use the res to manage your resource(based on Pathlib)
 
-## [ REWRITE NOW ]
+# Install
 
-# QA
+```shell
+pip install Remilia #Install basic package
 
-## Q: AttributeError: module 'Remilia' has no attribute '...'
+pip install Remilia[tui] #Install tui package
 
-See the pyproject.toml ,there offer some other optional dependiences
+pip install Remilia[all] #Install full package
+```
 
-# Learn more in our WIKI
+# How to use?
 
-## https://github.com/H2Sxxa/Remilia/wiki
+See our wiki -> <https://github.com/H2Sxxa/Remilia/wiki>
```

### Comparing `remilia-1.1.8/pyproject.toml` & `remilia-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ]
 dependencies = [
     "colorama",
     "pyyaml",
     "pydantic",
     "typing_extensions",
 ]
-version = "1.1.8"
+version = "1.2.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://pypi.org/project/Remilia/"
 Repository = "https://github.com/H2Sxxa/Remilia"
```

### Comparing `remilia-1.1.8/src/Remilia/base/models.py` & `remilia-1.2.0/src/Remilia/base/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing_extensions import Self
 from pydantic import BaseModel
+from typing_extensions import Self
+
 
 class Ruler(BaseModel):
     '''
     self -> Type(Log)
     '''
     level:int=5
     excolor:str="fore.LIGHTGREEN_EX+'[ '+name+' '+time+' '+location+'] '+style.RESET_ALL+text"
```

### Comparing `remilia-1.1.8/src/Remilia/base/rtypes.py` & `remilia-1.2.0/src/Remilia/base/rtypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from types import MethodType
 from typing import Generic, TypeVar
+
 from typing_extensions import Self
 
 RT=TypeVar("RT")
 T=TypeVar("T")
 NT=TypeVar("NT")
 VT=TypeVar("VT")
 class VarBuilder:
@@ -19,15 +21,18 @@
         return not attr.startswith("__")
     
     def warp(self,warpin):
         def inner(*arg,**args):
             return warpin(*arg,**args)
         return inner
     
-import json,re
+import json
+import re
+
+
 def typedet(string:str,strict=True) -> any:
     if not re.match(r"[\u4E00-\u9FA5A-Za-z]",string) and re.match(r"[0-9]",string) and not re.match(r"[`~!@#$%^&*()_\-+=<>?:\"{}|,\/;'\\[\]·~！@#￥%……&*（）——\-+={}|《》？：“”【】、；‘'，。、]",string):
         if "." in string:
             try:
                 return float(string)
             except:
                 pass
```

### Comparing `remilia-1.1.8/src/Remilia/log.py` & `remilia-1.2.0/src/Remilia/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         return self
     
     def _subwrite(self,*logs:Log) -> None:
         for sub in self.all_subs:
             mode ="a" if sub.value.exists() else "w"
             for log in logs:
                 if sub.name(log):
-                    sub.value.write(data=log.plain,mode=mode)
+                    sub.value.write(data=log.plain+"\n",mode=mode)
             
     
 class Logger:
     def __init__(self,logcat:LogCat=LogCat(),ruler_map:Optional[Dict[str,Ruler]]={},model:str="'%s[ '+name+' '+time+' '+location+'] %s'+text") -> None:
         self.ruler_map={
             "DEBUG":Ruler(level=3).exgenerate(model,Fore.CYAN,Style.RESET_ALL),
             "INFO":Ruler(level=5).exgenerate(model,Fore.LIGHTGREEN_EX,Style.RESET_ALL),
```

### Comparing `remilia-1.1.8/src/Remilia/mixin_decorations/__init__.py` & `remilia-1.2.0/src/Remilia/shadow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,162 +1,147 @@
-from typing import Callable, List
-from ..base.rtypes import Pair
-from ..utils.SignParas import ParaFilter
-from .omixin import gc_Mixin
-from . import omixin
-from abc import abstractmethod
-
-__all__=["omixin"]
-
-class DecorationBase:
-    def __call__(self,obj):
-        self.obj=obj
-        return self
-    def withObj(self,obj):
-        self.obj=obj
-        return self
-    
-    @abstractmethod
-    def warp(self,pair:Pair) -> Pair:
-        return Pair(Pair.name,Pair.value)
-
-class ParaHandleBase:
-    @abstractmethod
-    def warp_para(self,arg):pass
-
-class ParaReplacer(ParaHandleBase):
-    def __init__(self,paragen=lambda para:para,condition=lambda para:True) -> None:
-        '''
-        paragen: method(para) -> replace arg
-        condition: wont work until it return True
-        '''
-        self.paragen=paragen
-        self.condition=condition
-    
-    def warp_para(self, arg):
-        if self.condition(arg):
-            return self.paragen(arg)
-        else:
-            return arg
+from types import MethodType
+from typing import Any, Callable, Dict, List, Type, Union
+from inspect import _empty
+from uuid import uuid4
+
+from .mixin import MixinBase, MixinTools
+from .base.exceptions import ExistedObjectError, NoSuchMethodError
+from .signs import Signs
+
+SHADOW_MAP = "__shadowmethod_map__"
+
+EmptyType = _empty
+
+
+def getShadowWarpWithCls(cls):
+    return Shadow.withCls(cls)
+
+
+class Shadow(MixinBase):
+    def mixin(self) -> None:
+        for t_cls in self.configs.target:
+            if not self.mixin_hasattr(t_cls, SHADOW_MAP):
+                self.mixin_setattr(t_cls, SHADOW_MAP, dict())
+
+            shadowmap: Dict[str, Dict[MethodType, List]]
+            shadowmap = self.mixin_getattr(t_cls, SHADOW_MAP)
+            if not shadowmap.__contains__(self.method):
+                shadowmap.update({self.method: dict()})
+                if self.mixin_hasattr(t_cls, self.method):
+                    shadowmap.get(self.method).update(
+                        {
+                            self.mixin_getattr(
+                                t_cls, self.method
+                            ): Signs.getParasAsType(
+                                self.mixin_getattr(t_cls, self.method)
+                            )
+                        }
+                    )
+            while True:
+                tmpname = self.shadowName
+                if not self.mixin_hasattr(t_cls, tmpname):
+                    self.mixin_setattr(t_cls, tmpname, self.mixinmethod)
+                    shadowmap.get(self.method).update(
+                        {
+                            self.mixin_getattr(t_cls, tmpname): Signs.getParasAsType(
+                                self.mixinmethod
+                            )
+                        }
+                    )
+                    break
 
-class ParaMixin(ParaHandleBase):
-    def __init__(self,mixins:Pair[str,Callable]=[],condition=lambda para:True,gc=False) -> None:
-        '''
-        mixins: Pair(method_name,Method)
-        condition: wont work until it return True
-        '''
-        self.mixins=mixins
-        self.cd=condition
-        self.gc=gc
-    def warp_para(self, arg):
-        if not self.cd(arg):
-            return arg
-        new_arg=arg
-        for mixin in self.mixins:
-            if self.gc:
-                gc_Mixin(new_arg,mixin.value,mixin.name)
-            else:
-                setattr(new_arg,mixin.name,mixin.value)
-        return new_arg
-    
-class ParaHooker(ParaHandleBase):
-    def __init__(self,hookname="__getattribute__",bfhooker=lambda *_,**__:None,afhooker=lambda result,*_,**__:result,condition=lambda para:True,gc=False) -> None:
-        '''
-        ### via mixin inject target , wont work for some buildin method
-        hookname: hook target(default is all(maybe) )
-        bfhooker: hook before call it
-        afhooker: hook after call it
-        condition: wont work until it return True
-        '''
-        self.hn=hookname
-        self.bf=bfhooker
-        self.af=afhooker
-        self.cd=condition
-        self.gc=gc
-    def warp_para(self,arg):
-        if not self.cd(arg):
-            return arg
-        new_arg=arg
-        rawattr=getattr(arg,self.hn)
-        def rebuild(*_,**__):
-            self.bf(*_,**__)
-            result=rawattr(*_,**__)
-            return self.af(result,*_,**__)
-        if self.gc:
-            gc_Mixin(new_arg,rebuild,self.hn)
-        else:
-            setattr(new_arg,self.hn,rebuild)
-        return new_arg
-    
-class Hooker(DecorationBase):
-    def __init__(self,bfhooker=lambda *_,**__:None,afhooker=lambda obj,result,*_,**__:result,parahandle:List[Pair]=[]) -> None:
-        '''
-        parahandle : [Pair(the index of para,parahandlebase's subclass instance),...]
-        bfhooker: hook before call it
-        afhooker: hook after call it
-        '''
-        self.bf=bfhooker
-        self.af=afhooker
-        self.ph=parahandle
-    def warp(self,pair) -> Pair:
-        return Pair(pair.name,self.warpper)
-    
     @property
-    def warpper(self):
-        filter=ParaFilter(self.obj)
-        filter.load_default()
-        filter.fill_none()
-        for pair in self.ph:
-            filter.index_put(pair.name,pair.value)
-        def tmp(*args,**kwargs):
-            self.bf(self.obj,*args,**kwargs)
-            for arg,index in zip(args,range(0,len(args))):
-                default=filter.kwargs[filter.get_index(index).name]
-                if isinstance(default,ParaHandleBase):
-                    filter.index_put(index,default.warp_para(arg))
-                else:
-                    filter.index_put(index,arg)
-            for k,v in kwargs.items():
-                default=filter.get_name(k)
-                if isinstance(default,ParaHandleBase):
-                    filter.kwargs.update({k:default.warp_para(arg)})
-                else:
-                    filter.kwargs.update({k:v})
-            result=self.obj(**filter.kwargs)
-            return self.af(self.obj,result,*args,**kwargs)
-        return tmp
-        
-        
-class NameTransform(DecorationBase):
-    def __init__(self,real_name) -> None:
-        '''
-        use to inject self into attr 'real_name'
-        PS:Usally in the outside of all decorations
-        
-        ---
-        examples:
-        
-        ```python
-        x=NameTransform("__nameless_var__").withObj(8)
-        
-        @NameTransform("__nameless_method__")
-        def x(self):pass
-        
-        
-        #for some special method,it may be "_cls__method"
-        #recommand to use str,instead of a concrete method
-        ```
-        '''
-        if isinstance(real_name,str):
-            self.real_name=real_name
+    def shadowName(self) -> str:
+        return self.method + "_%s" % str(uuid4()).replace("-", "")
+
+    @staticmethod
+    def withValue(
+        method: Union[str, MethodType, None] = None,
+        gc: bool = None,
+        mixintools: MixinTools = MixinTools(),
+    ):
+        return Shadow.cast(Shadow, None, method, gc, mixintools).init
+
+
+class ShadowInvoker:
+    def __init__(self, cls: Type) -> None:
+        self.cls = cls
+
+    def getShadowMap(self) -> Dict:
+        return getattr(self.cls, SHADOW_MAP)
+
+    def findAllWithType(self, paratype: List[object]) -> List[MethodType]:
+        shadowmap: Dict[str, Dict[MethodType, List]]
+        shadowmap = getattr(self.cls, SHADOW_MAP)
+        result = []
+        for nvmap in [v for _, v in shadowmap.items()]:
+            result.extend([n for n, v in nvmap.items() if v == paratype])
+        return result
+
+    def findFirstWithType(self, paratype: List[object]) -> List[MethodType]:
+        try:
+            return self.findAllWithType(paratype)[0]
+        except:
+            raise NoSuchMethodError(
+                "can't find method with %s in %s" % (paratype, self.cls)
+            )
+
+    def findAll(
+        self, method: Union[str, MethodType], paratype: List[object]
+    ) -> List[MethodType]:
+        shadowmap: Dict[str, Dict[MethodType, List]]
+        shadowmap = getattr(self.cls, SHADOW_MAP)
+        if not issubclass(method.__class__, str):
+            methodN = method.__name__
         else:
-            self.real_name=real_name.__name__
-    def __call__(self,obj):
-        self.obj=obj
-        return self
-    
-    def withObj(self,obj):
-        self.obj=obj
-        return self
-    
-    def warp(self, *_) -> Pair:
-        return Pair(self.real_name,self.obj)
+            methodN = method
+        return [
+            method for method, paras in shadowmap[methodN].items() if paras == paratype
+        ]
+
+    def findFirst(
+        self, method: Union[str, MethodType], paratype: List[object]
+    ) -> MethodType:
+        try:
+            return self.findAll(method, paratype)[0]
+        except:
+            raise NoSuchMethodError(
+                "can't find '%s' method with %s in %s" % (method, paratype, self.cls)
+            )
+
+    def invokeAll(
+        self, method: Union[str, MethodType], paratype: List[object], *args, **kwargs
+    ) -> List[Any]:
+        return [mtd(*args, **kwargs) for mtd in self.findAll(method, paratype)]
+
+    def invokeFirst(
+        self, method: Union[str, MethodType], paratype: List[object], *args, **kwargs
+    ) -> Any:
+        return self.findFirst(method, paratype)(*args, **kwargs)
+
+    def invokeAllWithType(self, paratype: List[object], *args, **kwargs) -> List[Any]:
+        return [mtd(*args, **kwargs) for mtd in self.findAllWithType(paratype)]
+
+    def invokeFirstWithType(self, paratype: List[object], *args, **kwargs) -> Any:
+        return self.findFirstWithType(paratype)(*args, **kwargs)
+
+
+class ShadowAccessor:
+    def __init__(self, cls: Type, force=False) -> None:
+        self.cls = cls
+        self.force = force
+
+    def setAccessible(self, name: str, force=None) -> None:
+        if force == None:
+            force = self.force
+        if not force:
+            if hasattr(self.cls, name):
+                raise ExistedObjectError(
+                    "%s has existed object -> %s" % (self.cls.__name__, name)
+                )
+        setattr(
+            self.cls, name, lambda _: getattr(_, "_%s%s" % (_.__class__.__name__, name))
+        )
+        setattr(self.cls, name, property(getattr(self.cls, name)))
+
+    def Accessor(self, method: Callable):
+        self.setAccessible(method.__name__)
```

### Comparing `remilia-1.1.8/src/Remilia/res.py` & `remilia-1.2.0/src/Remilia/res.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.8/src/Remilia/structdb.py` & `remilia-1.2.0/src/Remilia/structdb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-import json,yaml
+import json
+from abc import ABC, abstractmethod
 from typing import Callable, Dict, List, Union
+
+import yaml
 from typing_extensions import Self
-from abc import ABC,abstractmethod
 
-from .res import rDir, rFile, rPath,DirectoryNotFoundError
-from .base.rtypes import NT,VT
+from .base.rtypes import NT, VT
+from .res import DirectoryNotFoundError, rDir, rFile, rPath
+
 
 class DataStructBase(ABC):
     def readkv(self,file:rFile,key:NT) -> VT:
         return self.readdict(file)[str(key)]
     
     def readdict(self,file:rFile) -> Dict[NT,VT]:
         return self._todict(file.text)
@@ -16,15 +19,15 @@
     def writekv(self,file:rFile,key:NT,value:VT) -> Self:
         return self.writedict(file,{key:value})
     
     def writedict(self,file:rFile,data:Dict[NT,VT]) -> Self:
         file.write(self._tostring(self.__updatedict(self.readdict(file),data)))
         return self
     
-    def pop(self,file:rFile,key:NT) -> Self:
+    def popkv(self,file:rFile,key:NT) -> Self:
         data=self.readdict(file)
         data.pop(key)
         return self.writedict(file,data)
     
     def fastwrite(self,file:rFile,func:Callable[[Dict[NT,VT]],Dict[NT,VT]]) -> Self:
         return self.writedict(file,func(self.readdict(file)))
     
@@ -74,36 +77,38 @@
         self.root.to_dictory().makedirs()
     
     def getf(self,name:str) -> rFile:
         if self.auto_create:
             return self.cget_file(name)
         else:
             return self.get_file(name)
-        
+    
     def getc(self,name:str) -> "DataBase":
         if self.auto_create:
             return self.cget_cate(name)
         else:
             return self.get_cate(name)
     
     def get_file(self,name:str) -> rFile:
         rf=rFile(self.root,name)
         if rf.check():
             return rf
         else:
             raise FileNotFoundError("%s does't exist"%rf)
 
+    
+    
     def get_cate(self,name:str) -> "DataBase":
         rf=rDir(self.root,name)
         if rf.check():
             return DataBase(rf,self.struct,self.auto_create)
         else:
             raise DirectoryNotFoundError("%s does't exist"%rf)
 
-    def cget_file(self,name:str) -> "DataBase":
+    def cget_file(self,name:str) -> rFile:
         rf=rFile(self.root,name)
         return rf if rf.check() else self.createfile(name)
 
     def cget_cate(self,name:str) -> "DataBase":
         rf=rDir(self.root,name)
         return DataBase(rf,self.struct,self.auto_create) if rf.check() else self.createcate(name)
 
@@ -111,35 +116,66 @@
         return DataBase(rPath(self.root,name).to_dictory().makedirs(),self.struct,self.auto_create)
     
     def createfile(self,name:str) -> rFile:
         return rFile(self.root,name).write(self.struct._initdata())
 
     def get_all(self) -> List[Union["DataBase",rFile]]:
         return [rp.to_file() if rp.to_file().check() else DataBase(rp,self.struct,self.auto_create) for rp in self.root.glob("*")]
-
+    
+    def get_dbsf(self,name:str) -> "DBSubFile":
+        return DBSubFile(self.getf(name),self)
+    
     #struct
     def readkv(self,name:str,key:NT) -> VT:
         return self.struct.readkv(self.getf(name),key)
     
     def readdict(self,name:str) -> Dict[NT,VT]:
         return self.struct.readdict(self.getf(name))
     
     def writekv(self,name:str,key:NT,value:VT) -> Self:
         return self.struct.writekv(self.getf(name),key,value)
     
     def writedict(self,name:str,data:Dict[NT,VT]) -> Self:
         self.struct.writedict(self.getf(name),data)
         return self
     
-    def pop(self,name:str,key:NT) -> Self:
-        self.struct.pop(self.getf(name),key)
+    def popkv(self,name:str,key:NT) -> Self:
+        self.struct.popkv(self.getf(name),key)
         return self
     
     def fastwrite(self,name:str,func:Callable[[Dict[NT,VT]],Dict[NT,VT]]) -> Self:
         self.struct.fastwrite(self.getf(name),func)
         return self
     
+    #magic
     def __str__(self) -> str:
         return self.root.to_string()
     
     def __repr__(self) -> str:
-        return "DataBase('%s')" % self.root
+        return "DataBase('%s')" % self.root
+
+class DBSubFile:
+    def __init__(self,file:rFile,db:DataBase) -> None:
+        self.db=db
+        self.file=file
+        
+    def writekv(self,key:NT,value:VT) -> Self:
+        self.db.writekv(self.file.name,key,value)
+        return self
+    
+    def writedict(self,data:Dict[NT,VT]) -> Self:
+        self.db.writedict(self.file.name,data)
+        return self
+    
+    def popkv(self,key:NT) -> Self:
+        self.db.popkv(self.file.name,key)
+        return self
+    
+    def fastwrite(self,func:Callable[[Dict[NT,VT]],Dict[NT,VT]]) -> Self:
+        self.db.fastwrite(self.file.name,func)
+        return self
+    
+    def readkv(self,key:NT) -> VT:
+        return self.db.readkv(self.file.name,key)
+    
+    def readdict(self) -> Dict[NT,VT]:
+        return self.db.readdict(self.file.name)
```

### Comparing `remilia-1.1.8/src/Remilia/utils/net/pixiv.py` & `remilia-1.2.0/src/Remilia/utils/pixiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,22 @@
     '''
     use getAuth before it
     '''
     return buildheader(auth["access_token"])
 
 
 import asyncio
-import logging
 import json
-import socket
-from typing import List, Dict, Any
-import ssl
-import aiohttp
 import re
+import socket
+from typing import Any, Dict, List
 
-from aiohttp.abc import AbstractResolver
+import aiohttp
 from aiohttp import ClientTimeout
+from aiohttp.abc import AbstractResolver
 
 '''
 come from pixiv_async
 
 https://pypi.org/project/PixivPy-Async/
 
 LICENSE: https://github.com/Mikubill/pixivpy-async/blob/master/LICENSE UNLICENSE
```

### Comparing `remilia-1.1.8/src/Remilia/utils/thread/Timeout.py` & `remilia-1.2.0/src/Remilia/utils/thread/Timeout.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.8/src/Remilia/utils/thread/terminable_thread.py` & `remilia-1.2.0/src/Remilia/utils/thread/terminable_thread.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.8/PKG-INFO` & `remilia-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: remilia
-Version: 1.1.8
+Name: Remilia
+Version: 1.2.0
 Summary: Use python with next generation api
 Author-Email: H2Sxxa <H2Sxxa0w0@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 H2Sxxa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,34 +43,35 @@
 Requires-Dist: pixivpy_async; extra == "all"
 Provides-Extra: tui
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align=center>
   <img width=200 src="https://raw.githubusercontent.com/H2Sxxa/Remilia/main/background.png"  alt="[BG](https://raw.githubusercontent.com/H2Sxxa/Remilia/main/background.png)"/>
-  <h1 align="center">Remilia</h1> 
+  <h1 align="center">Remilia</h1>
 </div>
+
 <div align=center>
   <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">
   <img src="https://img.shields.io/github/languages/code-size/H2Sxxa/Remilia" alt="size">
   <img src="https://img.shields.io/github/license/H2Sxxa/Remilia" alt="license">
 </div>
 
-# Install
+# What's this?
 
-```shell
-pip install Remilia
-```
+A package with many utils, in order to help build application faster.
 
-# Quick start
+use Remilia,you can print colorful log,you can use mixin to modify any class(but most build-in class not supported),you can use the res to manage your resource(based on Pathlib)
 
-## [ REWRITE NOW ]
+# Install
 
-# QA
+```shell
+pip install Remilia #Install basic package
 
-## Q: AttributeError: module 'Remilia' has no attribute '...'
+pip install Remilia[tui] #Install tui package
 
-See the pyproject.toml ,there offer some other optional dependiences
+pip install Remilia[all] #Install full package
+```
 
-# Learn more in our WIKI
+# How to use?
 
-## https://github.com/H2Sxxa/Remilia/wiki
+See our wiki -> <https://github.com/H2Sxxa/Remilia/wiki>
```

