# Comparing `tmp/fasttq-1.0.7.tar.gz` & `tmp/fasttq-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttq-1.0.7.tar", last modified: Sat Jun 10 05:51:38 2023, max compression
+gzip compressed data, was "fasttq-1.0.8.tar", last modified: Sun Jul 30 01:06:17 2023, max compression
```

## Comparing `fasttq-1.0.7.tar` & `fasttq-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 05:51:38.532118 fasttq-1.0.7/
--rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1848 2023-06-10 05:51:38.531587 fasttq-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 05:51:38.515607 fasttq-1.0.7/fasttq/
--rw-rw-rw-   0        0        0      133 2023-06-10 05:50:00.000000 fasttq-1.0.7/fasttq/__init__.py
--rw-rw-rw-   0        0        0     6025 2023-06-06 13:39:37.000000 fasttq-1.0.7/fasttq/client.py
--rw-rw-rw-   0        0        0     9709 2023-06-10 05:21:59.000000 fasttq-1.0.7/fasttq/queue.py
--rw-rw-rw-   0        0        0     6034 2023-06-06 14:47:22.000000 fasttq-1.0.7/fasttq/worker.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:51:38.530589 fasttq-1.0.7/fasttq.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.7/fasttq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 05:51:38.000000 fasttq-1.0.7/fasttq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 05:51:38.532118 fasttq-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:06:17.223296 fasttq-1.0.8/
+-rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1848 2023-07-30 01:06:17.222300 fasttq-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 01:06:17.200377 fasttq-1.0.8/fasttq/
+-rw-rw-rw-   0        0        0      133 2023-07-30 01:03:30.000000 fasttq-1.0.8/fasttq/__init__.py
+-rw-rw-rw-   0        0        0     6106 2023-07-30 00:41:07.000000 fasttq-1.0.8/fasttq/client.py
+-rw-rw-rw-   0        0        0     9782 2023-07-30 00:59:19.000000 fasttq-1.0.8/fasttq/queue.py
+-rw-rw-rw-   0        0        0     6034 2023-07-29 16:42:02.000000 fasttq-1.0.8/fasttq/worker.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:06:17.221303 fasttq-1.0.8/fasttq.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-07-30 01:06:16.000000 fasttq-1.0.8/fasttq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-30 01:06:16.000000 fasttq-1.0.8/fasttq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:06:16.000000 fasttq-1.0.8/fasttq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.8/fasttq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-07-30 01:06:16.000000 fasttq-1.0.8/fasttq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 01:06:16.000000 fasttq-1.0.8/fasttq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 01:06:17.223296 fasttq-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.8/setup.py
```

### Comparing `fasttq-1.0.7/LICENSE` & `fasttq-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.7/PKG-INFO` & `fasttq-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.7
+Version: 1.0.8
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.7/README.md` & `fasttq-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.7/fasttq/client.py` & `fasttq-1.0.8/fasttq/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     
     m, _, f = s.rpartition(".")
     module = importlib.import_module(m)
     return getattr(module, f)
 
 def serialize(data:Any, retrys:int = 1, retry_delay:float = 0.01):
     d = dict(
-        data=data if isinstance(data, str) else data.__dict__,
+        data=data if isinstance(data, str) else json.dumps(data),
         retrys=retrys,
         retry_delay=retry_delay
     )
     return json.dumps(d)
 
 def unserialize(data:str):
     s = str(data, encoding="utf8")
-    return json.loads(s) if s.startswith("{") else s
+    return json.loads(s) if s[0] in "{[" else s
 
 class Client(ABC):
 
     default_topics_header = "fasttq:topics"
     default_workers_header = "fasttq:workers"
     default_handlers_header = "fasttq:handlers"
     default_jobs_header = "fasttq:jobs:%s"
@@ -64,15 +64,15 @@
         pass
 
     @abstractmethod
     def push_topic(self, topic:str, jobs:List[str]):
         pass
 
     @abstractmethod
-    def push_topics(self, jobs:Dict[str, str]):
+    def push_topics(self, jobs:Dict[str, str], retrys:int = 1, retry_delay:float = 1.0):
         pass
 
     @abstractmethod
     def insert_topic(self, topic:str, jobs:List[str]):
         pass
 
     @abstractmethod
@@ -125,15 +125,15 @@
 
     # 推入某个topic的任务
     def push_topic(self, topic:str, jobs:List[str]):
         with self.connect() as conn:
             return conn.lpush(self.default_jobs_header % topic, *jobs)
 
     # 推入多个topic的任务
-    def push_topics(self, jobs:Dict[str, str]):
+    def push_topics(self, jobs:Dict[str, List], retrys:int = 1, retry_delay:float = 1.0):
         with self.connect() as conn:
             return {topic:conn.lpush(self.default_jobs_header % topic, *_jobs) for topic,_jobs in jobs.items()}
 
     # 优先插入某个topic的任务
     def insert_topic(self, topic:str, jobs:List[str]):
         with self.connect() as conn:
             return conn.rpush(self.default_jobs_header % topic, *jobs)
```

### Comparing `fasttq-1.0.7/fasttq/queue.py` & `fasttq-1.0.8/fasttq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def items2chunk(items:list, chunksize:int = 100):
     return (items[i*chunksize:(i+1)*chunksize] for i in range(len(items)//chunksize+1))
 
 def items2dict(items:list):
     return {k:v for k,v in items}
 
 def dict2chunk(d:dict, chunksize:int = 100):
-    return [items2dict(items) for items in items2chunk(d.items(), chunksize)]
+    return [items2dict(items) for items in items2chunk(list(d.items()), chunksize)]
 
 def start_worker(client_str:str, conn_url:str, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 0, retrys:int = 10, retry_delay:int = 1):
     worker = Worker(client_str, conn_url, assignor, chunksize, retrys, retry_delay)
     worker.work()
 
 def start_pusher(client_str:str, conn_url:str, topic:str = None, jobs:Union[List, Dict] = None):
     pusher = Pusher(client_str, conn_url)
@@ -68,17 +68,18 @@
             return self.getJobs
         return decorator        
 
     def pending(self, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100, **kwargs):
         for getJob in self.getJobs:
             topic = getJob.args[0]
             if topic is None:
-                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob(**kwargs).items()}
                 for chunk in dict2chunk(jobs, chunksize):
-                    self.client.push_topics(chunk)
+                    for topic, data in chunk.items():
+                        jobs = [serialize(d, retrys, retry_delay) for d in data]
+                        self.client.push_topic(topic, jobs)
             else:
                 jobs = [serialize(data, retrys, retry_delay) for data in getJob(**kwargs)]
                 for chunk in items2chunk(jobs, chunksize):
                     self.client.push_topic(topic, chunk)
 
     #########################################################################################
     # 方案3.0，替换成Pool模式
@@ -148,17 +149,18 @@
             jobs = [serialize(data, retrys, retry_delay) for data in func()]
             for chunk in items2chunk(jobs, chunksize):
                 self.client.push_topic(topic, chunk)
         return decorator
 
     def topics(self, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100):
         def decorator(func:Callable):
-            jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in func().items()}
-            for chunk in dict2chunk(jobs, chunksize):
-                self.client.push_topics(chunk)
+            for chunk in dict2chunk(func(), chunksize):
+                for topic, data in chunk.items():
+                    jobs = [serialize(d, retrys, retry_delay) for d in data]
+                    self.client.push_topic(topic, jobs)
         return decorator
 
     def clear_worker(self):
         # 收集死进程
         _tobekill = []
         for pid, process in self._workers.items():
             if not process.is_alive():
@@ -195,14 +197,14 @@
             workers = self.clear_worker()
         # for pid, process in self._workers.items():
         #     process.close()
         #     process.join()
 
     def start(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1, **kwargs):
         client_str = func2str(self.client)
-        self.pending(*args, retrys, retry_delay, **kwargs)
+        self.pending(retrys, retry_delay, **kwargs)
         self.start_workers(client_str, self.client.conn_url, workers, assignor, chunksize, retrys, retry_delay)
         
     def start_mp(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1, **kwargs):
         client_str = func2str(self.client)
         self.pending_mp(client_str, self.client.conn_url, retrys, retry_delay, chunksize, **kwargs)
         self.start_workers(client_str, self.client.conn_url, workers, assignor, chunksize, retrys, retry_delay)
```

### Comparing `fasttq-1.0.7/fasttq/worker.py` & `fasttq-1.0.8/fasttq/worker.py`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.7/fasttq.egg-info/PKG-INFO` & `fasttq-1.0.8/fasttq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.7
+Version: 1.0.8
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.7/setup.py` & `fasttq-1.0.8/setup.py`

 * *Files identical despite different names*

