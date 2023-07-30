# Comparing `tmp/tcafe attending bot-0.1.2.tar.gz` & `tmp/tcafe_attending_bot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcafe attending bot-0.1.2.tar", last modified: Sun Sep  5 11:34:47 2021, max compression
+gzip compressed data, was "tcafe_attending_bot-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcafe attending bot-0.1.2.tar` & `tcafe_attending_bot-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-05 11:34:47.843536 tcafe attending bot-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-09-05 11:34:40.000000 tcafe attending bot-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-09-05 11:34:47.843536 tcafe attending bot-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-09-05 11:34:40.000000 tcafe attending bot-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-05 11:34:47.843536 tcafe attending bot-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-09-05 11:34:40.000000 tcafe attending bot-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-05 11:34:47.843536 tcafe attending bot-0.1.2/tcafe_attending_bot/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-05 11:34:40.000000 tcafe attending bot-0.1.2/tcafe_attending_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-09-05 11:34:40.000000 tcafe attending bot-0.1.2/tcafe_attending_bot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-05 11:34:47.843536 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-05 11:34:47.000000 tcafe attending bot-0.1.2/tcafe_attending_bot.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-05 11:34:47.843536 tcafe attending bot-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-09-05 11:34:40.000000 tcafe attending bot-0.1.2/test/test_api.py
+-rw-r--r--   0        0        0     1075 2023-07-30 08:31:33.630666 tcafe_attending_bot-1.0.0/LICENSE
+-rw-r--r--   0        0        0      645 2023-07-30 08:31:33.630666 tcafe_attending_bot-1.0.0/README.md
+-rw-r--r--   0        0        0     1352 2023-07-30 08:31:33.630666 tcafe_attending_bot-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3196 2023-07-30 08:31:33.630666 tcafe_attending_bot-1.0.0/tcafe_attending_bot/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-30 08:31:33.634666 tcafe_attending_bot-1.0.0/tcafe_attending_bot/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:31:33.634666 tcafe_attending_bot-1.0.0/tcafe_attending_bot/py.typed
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 tcafe_attending_bot-1.0.0/PKG-INFO
```

### Comparing `tcafe attending bot-0.1.2/LICENSE` & `tcafe_attending_bot-1.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Byeonghoon Yoo
+Copyright (c) 2019-2023 Byeonghoon Yoo
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tcafe attending bot-0.1.2/README.md` & `tcafe_attending_bot-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tcafe attending bot-0.1.2/tcafe_attending_bot/__main__.py` & `tcafe_attending_bot-1.0.0/tcafe_attending_bot/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,101 @@
-#!/usr/bin/env python
-# coding: UTF-8
+"""Auto attending bot for TCafe."""
+
+from __future__ import annotations
 
 import asyncio
 import json
 import logging
-from pathlib import Path
-from typing import Generator, List, Tuple
+import pathlib
+from collections.abc import Iterable, Generator
+from itertools import chain
+from typing import Final
 
 import aiohttp
-from bs4 import BeautifulSoup
-from xdg import BaseDirectory
+import bs4
+import xdg_base_dirs
 
-_BASE_URL = 'http://tcafe2a.com'
-_APP_NAME = 'tcafe'
-_ID_KEY = 'id'
-_PW_KEY = 'password'
+__version__ = '1.0.0'
 
-logger = logging.getLogger(__name__)
+_log: Final[logging.Logger] = logging.getLogger(__name__)
+_BASE_URL: Final[str] = 'https://tcafe2a.com'
+_APP_NAME: Final[str] = 'tcafe'
 
 
 async def attend(identifier: str, password: str) -> None:
-    logger.info(f'Processing {identifier}...')
+    _log.info(f'Processing {identifier}...')
 
     try:
-        async with aiohttp.ClientSession() as session:
+        async with aiohttp.ClientSession(base_url=_BASE_URL) as session:
             data = dict(mb_id=identifier, mb_password=password)
 
             # login
-            async with session.post(_BASE_URL + '/bbs/login_check.php', data=data):
-                pass
+            async with session.post('/bbs/login_check.php', data=data) as res:
+                if not res.ok:
+                    raise ValueError('Failed to log in')
+
+                result_page = bs4.BeautifulSoup(await res.text(), features='html.parser')
+                title = result_page.select_one('title')
+                if '오류' in title.text:
+                    raise ValueError('Failed to log in')
 
             # get hidden values
-            async with session.get(_BASE_URL + '/attendance/selfattend2.php') as res:
-                attend_page = BeautifulSoup(await res.text(), features='html.parser')
+            async with session.get('/community/attendance') as res:
+                if not res.ok:
+                    raise ValueError('Failed to get attendance page')
+
+                attend_page = bs4.BeautifulSoup(await res.text(), features='html.parser')
                 # language=JQuery-CSS
-                hidden_values: List[BeautifulSoup] = attend_page.select('form[name=frm1] input[type=hidden]')
+                hidden_values: Iterable[bs4.Tag] = attend_page.select('form[name=frm1] input[type=hidden]')
 
                 data = {v.attrs['name']: v.attrs['value'] for v in hidden_values}
+                _log.info(data)
 
             # attend
-            async with session.post(_BASE_URL + '/attendance/selfattend2_p.php', data=data):
-                pass
+            async with session.post('/attendance/selfattend2_p.php', data=data):
+                if not res.ok:
+                    raise ValueError('Failed to attend')
     except IOError:
-        logger.exception(f'Fail to attend {identifier}')
+        _log.exception(f'Fail to attend {identifier}')
     else:
-        logger.info(f'{identifier} is attended!')
+        _log.info(f'{identifier} is attended!')
 
 
-def _get_accounts() -> Generator[Tuple[str, str], None, None]:
-    for directory in BaseDirectory.xdg_data_dirs:
-        config_path = Path(directory) / _APP_NAME / 'accounts.json'
+def _get_accounts() -> Generator[tuple[str, str], None, None]:
+    for directory in chain(xdg_base_dirs.xdg_data_dirs(), (xdg_base_dirs.xdg_data_home(),)):
+        config_path = pathlib.Path(directory) / _APP_NAME / 'accounts.json'
 
         if not config_path.is_file():
             continue
 
         try:
             with config_path.open() as fp:
                 config = json.load(fp)
         except IOError:
-            logger.exception(f'Fail to read account info from {config_path}')
+            _log.exception(f'Fail to read account info from {config_path}')
             continue
 
         if not isinstance(config, list):
             continue
 
         for account in config:
-            if not isinstance(account, dict) or \
-                    not isinstance(account.get(_ID_KEY), str) or not isinstance(account.get(_PW_KEY), str):
+            if (
+                not isinstance(account, dict)
+                or not isinstance(account.get('id'), str)
+                or not isinstance(account.get('password'), str)
+            ):
                 continue
 
-            yield account[_ID_KEY], account[_PW_KEY]
-
-    yield from ()
-
-
-async def main() -> None:
-    accounts = tuple(_get_accounts())
+            yield account['id'], account['password']
 
-    if len(accounts) != 0:
-        await asyncio.gather(*(attend(_id, _pw) for _id, _pw in _get_accounts()))
 
+async def run() -> None:
+    _log.addHandler(logging.StreamHandler())
+    _log.setLevel(logging.INFO)
 
-def console_entry() -> None:
-    asyncio.run(main())
+    results = await asyncio.gather(*(attend(_id, _pw) for _id, _pw in _get_accounts()))
+    if len(results) == 0:
+        raise ValueError('Empty accounts')
 
 
-if __name__ == '__main__':
-    asyncio.run(main())
+def main() -> None:
+    asyncio.run(run())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

