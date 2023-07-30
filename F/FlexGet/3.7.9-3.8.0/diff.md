# Comparing `tmp/FlexGet-3.7.9.tar.gz` & `tmp/FlexGet-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-exxe270e/FlexGet-3.7.9.tar", last modified: Tue Jul 11 15:14:55 2023, max compression
+gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-c9yz_u5z/FlexGet-3.8.0.tar", last modified: Sun Jul 30 15:11:30 2023, max compression
```

## Comparing `FlexGet-3.7.9.tar` & `FlexGet-3.8.0.tar`

### file list

```diff
@@ -1,982 +1,982 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-11 15:14:30.000000 FlexGet-3.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 15:14:30.000000 FlexGet-3.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-11 15:14:55.000000 FlexGet-3.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-11 15:14:30.000000 FlexGet-3.7.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-11 15:14:30.000000 FlexGet-3.7.9/dev-requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-11 15:14:30.000000 FlexGet-3.7.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-11 15:14:43.000000 FlexGet-3.7.9/flexget/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/templates/api_response.html
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/templates/swagger-ui.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/archives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/backlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/backlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/bittorrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/convert_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/magnet_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/private_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_scrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/emby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83806 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/api_emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/from_emby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/estimate_release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimate_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_movies_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_released_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_series_tvmaze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/failed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/retry_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/ftp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/ftp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23176 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/sftp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/imdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/from_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/irc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/couchpotato_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/entry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/imdb_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/movie_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/pending_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/plex_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/radarr_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/sonarr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/subtitle_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/thetvdb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/yaml_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notification_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/cronitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/gotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/ifttt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/microsoftteams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/notifymyandroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/ntfysh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/prowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushalot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushsafer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/rapidpush.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/sms_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/parser_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/parser_guessit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/parser_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/plugin_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/pending_approval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/pending_approval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/rejected/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/remember_rejected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/scheduler/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/seen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/seen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/seen_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/seen_movies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/all_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    47041 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/configure_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    57516 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/gen_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/internal_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/metainfo_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/next_series_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/next_series_seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    53392 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series_begin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series_premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/sites/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/allyoulike.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/alpharatio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/animeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/anirena.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/archetorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/argenteam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/awesomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/bakabt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/btn.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/cinemageddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/cpasbien.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/deadfrog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/descargas2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/ettv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/eztv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/filelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/filelist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/frenchtorrentdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/fuzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/google_cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/hebits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/hliang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/horriblesubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/koreus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/limetorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/lostfilm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/magnetdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/morethantv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/ncore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/newtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/newznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/nnmclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/passthepopcorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/ptn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rarbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rlsbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rmz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/serienjunkies.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/shortened.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/site_1337x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/site_rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/solidtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrentday.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrentz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/wordpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/yts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/urlrewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/urlrewrite_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/urlrewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/thetvdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/api_tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/thetvdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/tmdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/api_tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/tmdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/api_trakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/next_trakt_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/trakt_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/trakt_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/trakt_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/tvmaze/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/api_tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/tvmaze_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/variables/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/variables/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/db_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/explain_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/perf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/try_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/wiki_qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/win32_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/pyload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40357 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/daemon/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/abort_if_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/accept_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/best_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/content_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/crossmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/exists_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/exists_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/if_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/limit_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/magnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/only_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/proper_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/require_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/thetvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/cron_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/db_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/db_vacuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/log_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/input/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/anidb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/apple_trailers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/betaseries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/filmweb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/from_piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/from_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/from_telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/input_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/kitsu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/letterboxd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/medusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/my_anime_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/myepisodes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/next_sonarr_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/npo_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/plex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/pogcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/regexp_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/rlslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/rottentomatoes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/sceper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/sickbeard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/torznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/twitterfeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/api_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/api_rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/change_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/metainfo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/assume_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/bluray_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/media_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/metainfo_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/nfo_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/nzb_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/rottentomatoes_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/subtitles_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/modify/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/path_by_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/path_by_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/plugin_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/reorder_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/set_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/sort_by_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/operate/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/abort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/cfscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/debug_db_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/debug_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/disable_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/domain_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/entry_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/formlogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/free_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/max_reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/spy_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/verbose_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/verify_ssl_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/output/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/download_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/dump_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/mock_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/rtorrent_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/subtitles_periscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/subtitles_subliminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/utorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/kodi_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/myepisodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/pogcal_acquired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/resources/flexget.png
--rw-r--r--   0 runner    (1001) docker     (123)    28388 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/templates/entry/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/entry/default.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/templates/task/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/task/default.template
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/task/html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/task/rss.template
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/app.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.eot
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/splash.js
--rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/vendor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/splash.css
--rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/vendor.css
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/build.js
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/inject.js
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/lint.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/scripts.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/server.js
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/test.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/watch.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/load.failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/specs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.scss
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/images/header.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/_error-dialog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/_login.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/components.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.route.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/_database.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/_sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/user/user.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/construction.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/directives.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/palette-background/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/layout.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.route.js
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.scss
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/plugins.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-field/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.js
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/_loading-bar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/flexget.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/services/schema.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/execute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/history.js
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/movie_list.js
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/registerPlugin.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/schedules.js
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/seen.js
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/series.js
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/states.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
--rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
--rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
--rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
--rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
--rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
--rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
--rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
--rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
--rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
--rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
--rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
--rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/bittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/cached_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/lazy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/utils/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/simple_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/soup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 15:14:30.000000 FlexGet-3.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/requirements-docker.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-11 15:14:30.000000 FlexGet-3.7.9/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-11 15:14:30.000000 FlexGet-3.7.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:14:55.000000 FlexGet-3.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 15:11:30.000000 FlexGet-3.8.0/FlexGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-30 15:11:08.000000 FlexGet-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-30 15:11:08.000000 FlexGet-3.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-30 15:11:30.000000 FlexGet-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-30 15:11:08.000000 FlexGet-3.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-30 15:11:08.000000 FlexGet-3.8.0/dev-requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-30 15:11:08.000000 FlexGet-3.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 15:11:20.000000 FlexGet-3.8.0/flexget/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/templates/api_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/api/templates/swagger-ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archive/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archives/archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archives/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/backlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/backlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/backlog/backlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/backlog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/backlog/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/bittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/convert_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/magnet_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/private_torrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/torrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/torrent_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/torrent_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/torrent_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/torrent_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/torrent_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/bittorrent/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/emby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83806 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/api_emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/emby_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/emby_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/emby_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/emby_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/emby/from_emby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/estimate_release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/estimate_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/estimate_release/estimate_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/estimate_release/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/estimate_release/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/estimate_release/estimators/est_movies_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/estimate_release/estimators/est_released_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/estimate_release/estimators/est_series_tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/failed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/failed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/failed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/failed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/failed/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/failed/retry_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/ftp/ftp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/ftp/ftp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/ftp/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/ftp/sftp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/history/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/history/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/history/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/imdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/from_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/imdb_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/imdb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/imdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/irc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/irc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/irc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/irc/irc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/managed_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/list_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/list_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/list_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/list_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/couchpotato_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/entry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/imdb_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/movie_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/pending_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/plex_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/radarr_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/sonarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/subtitle_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/thetvdb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/managed_lists/lists/yaml_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notification_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/cronitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/ifttt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/microsoftteams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/notifymyandroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/ntfysh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/pushalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/pushsafer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/rapidpush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/sms_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notifiers/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/parsing/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/parsing/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/parsing/parsers/parser_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/parsing/parsers/parser_guessit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/parsing/parsers/parser_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/parsing/plugin_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/pending_approval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/pending_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/pending_approval/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/pending_approval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/pending_approval/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/pending_approval/pending_approval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/rejected/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/rejected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/rejected/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/rejected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/rejected/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/rejected/remember_rejected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/scheduler/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/seen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/seen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/seen_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/seen/seen_movies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/all_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47001 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/configure_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57484 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/gen_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/internal_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/metainfo_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/next_series_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/next_series_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53425 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/series_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/series_premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/series_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/sites/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/allyoulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/alpharatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/animeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/anirena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/archetorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/argenteam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/awesomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/bakabt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/cinemageddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/cpasbien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/deadfrog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/descargas2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/ettv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/eztv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/filelist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/frenchtorrentdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/fuzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/google_cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/hebits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/hliang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/horriblesubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/koreus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/limetorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/lostfilm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/magnetdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/morethantv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/ncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/newtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/nnmclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/passthepopcorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/ptn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/rarbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/rlsbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/rmz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/serienjunkies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/shortened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/site_1337x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/site_rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/solidtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/torrent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/torrentday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/torrentz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/wordpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/sites/yts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/urlrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/urlrewrite_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/urlrewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/sites/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/status/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/status/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/status/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/thetvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/thetvdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/thetvdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/thetvdb/api_tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/thetvdb/thetvdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tmdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tmdb/api_tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tmdb/tmdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/api_trakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/next_trakt_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/trakt_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/trakt_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/trakt/trakt_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/tvmaze/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tvmaze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tvmaze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26641 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tvmaze/api_tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/tvmaze/tvmaze_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/components/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/variables/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/components/variables/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42625 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/explain_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/perf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/try_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/wiki_qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/cli/win32_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31599 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/pyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40341 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/clients/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/daemon/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/abort_if_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/accept_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/best_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/content_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/crossmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/exists_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/exists_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/if_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/limit_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/magnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/only_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/proper_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/require_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/thetvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/filter/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/cron_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/db_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/db_vacuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/log_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/generic/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/anidb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/apple_trailers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/betaseries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/filmweb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/from_piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/from_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/from_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/input_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/kitsu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/letterboxd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/medusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/my_anime_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/myepisodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/next_sonarr_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/npo_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/plex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/pogcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/regexp_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/rlslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/rottentomatoes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/sceper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/sickbeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/torznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/input/twitterfeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/internal/api_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/internal/api_rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/internal/change_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/metainfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/assume_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/bluray_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/media_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/metainfo_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/nfo_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/nzb_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/rottentomatoes_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/subtitles_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/metainfo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/modify/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/path_by_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/path_by_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/plugin_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/reorder_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/set_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/modify/sort_by_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/abort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/cfscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/debug_db_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/debug_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/disable_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/domain_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/entry_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/formlogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/free_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/max_reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/spy_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/verbose_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/verify_ssl_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/operate/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22421 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/download_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/dump_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/mock_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/rtorrent_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/subtitles_periscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/subtitles_subliminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/output/utorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/services/kodi_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/services/myepisodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/plugins/services/pogcal_acquired.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/resources/flexget.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28331 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/templates/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/templates/entry/default.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/templates/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/templates/task/default.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/templates/task/html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/templates/task/rss.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/app.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/app/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/app/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/app/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/scripts/splash.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/scripts/vendor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/styles/splash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-07-30 15:11:21.000000 FlexGet-3.8.0/flexget/ui/v1/app/styles/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/build.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/inject.js
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/lint.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulp/watch.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/load.failure.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/specs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/app.loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/app.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/app.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/assets/images/header.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/_error-dialog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/exception/exception.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/exception/exception.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/pagination.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/pagination.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/router/router-helper.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/router/router-helper.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/_login.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.config.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/components.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.route.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/_database.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/_sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/components/user/user.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/construction.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/directives/directives.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/directives/palette-background/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/layout.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/plugins.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-field/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/server.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/server.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/server.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/scss/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/scss/_loading-bar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/scss/flexget.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/src/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/src/services/schema.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/execute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/movie_list.js
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/registerPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/schedules.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/seen.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/series.js
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/states.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
+-rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
+-rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-30 15:11:22.000000 FlexGet-3.8.0/flexget/ui/v2/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/ui/v2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/bittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/cached_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:11:30.000000 FlexGet-3.8.0/flexget/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/parsers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/parsers/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28476 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/parsers/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/simple_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/soup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-30 15:11:08.000000 FlexGet-3.8.0/flexget/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-30 15:11:08.000000 FlexGet-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-07-30 15:11:08.000000 FlexGet-3.8.0/requirements-docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-30 15:11:08.000000 FlexGet-3.8.0/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-30 15:11:08.000000 FlexGet-3.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:11:30.000000 FlexGet-3.8.0/setup.cfg
```

### Comparing `FlexGet-3.7.9/FlexGet.egg-info/PKG-INFO` & `FlexGet-3.8.0/FlexGet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.7.9
+Version: 3.8.0
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.7.9/FlexGet.egg-info/SOURCES.txt` & `FlexGet-3.8.0/FlexGet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/FlexGet.egg-info/requires.txt` & `FlexGet-3.8.0/FlexGet.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 [:python_version >= "3.7" and python_version < "3.10"]
-importlib-metadata==6.1.0
+importlib-metadata==6.7.0
 zipp==3.11.0
 
 [:python_version >= "3.7" and python_version < "3.9"]
 backports-zoneinfo==0.2.1
 importlib-resources==5.10.1
 pkgutil-resolve-name==1.3.10
 
@@ -54,35 +54,35 @@
 pynzb==0.1.0
 pyparsing==3.0.9
 pyrsistent==0.19.2
 pyrss2gen==1.1
 python-dateutil==2.8.2
 pytz-deprecation-shim==0.1.0.post0
 pytz==2022.6
-pyyaml==6.0
+pyyaml==6.0.1
 rebulk==3.1.0
 requests==2.31.0
 rich==12.6.0
 rpyc==5.3.1
 setuptools==65.6.3
 sgmllib3k==1.0.0
 six==1.16.0
 soupsieve==2.3.2.post1
 sqlalchemy==2.0.15
 tempora==5.1.0
-typing-extensions==4.4.0
+typing-extensions==4.7.1
 tzdata==2022.7
 tzlocal==4.2
 urllib3==1.26.13
 webencodings==0.5.1
 werkzeug==2.2.3
 zc-lockfile==2.0
 zxcvbn==4.4.28
 
-[:python_version >= "3.7" and python_version < "4.0" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")]
+[:python_version >= "3.7" and python_version < "4.0" and (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64")]
 greenlet==2.0.1
 
 [:python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"]
 win32-setctime==1.1.0
 
 [:sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"]
 pywin32==305
```

### Comparing `FlexGet-3.7.9/LICENSE` & `FlexGet-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/PKG-INFO` & `FlexGet-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.7.9
+Version: 3.8.0
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.7.9/README.rst` & `FlexGet-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/dev-requirements-extras.txt` & `FlexGet-3.8.0/dev-requirements-extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
 cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.7" and python_version < "4.0"
 dogpile-cache==1.1.8 ; python_version >= "3.7" and python_version < "4.0"
 enzyme==0.4.1 ; python_version >= "3.7" and python_version < "4.0"
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.8"
+importlib-metadata==6.7.0 ; python_version >= "3.7" and python_version < "3.8"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 jmespath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
 paramiko==2.12.0 ; python_version >= "3.7" and python_version < "4.0"
 pbr==5.11.0 ; python_version >= "3.7" and python_version < "4.0"
 plexapi==4.13.1 ; python_version >= "3.7" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0"
 pynacl==1.5.0 ; python_version >= "3.7" and python_version < "4.0"
@@ -32,10 +32,10 @@
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 s3transfer==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
 stevedore==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
 subliminal==2.1.0 ; python_version >= "3.7" and python_version < "4.0"
-typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "3.8"
+typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "3.8"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.9"
```

### Comparing `FlexGet-3.7.9/dev-requirements.txt` & `FlexGet-3.8.0/dev-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and (sys_platform == "win32" or platform_system == "Windows")
 coverage==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 coverage[toml]==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 distlib==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
 docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
 exceptiongroup==1.0.4 ; python_version >= "3.7" and python_version < "3.11"
 execnet==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
-filelock==3.8.2 ; python_version >= "3.7" and python_version < "4.0"
+filelock==3.12.2 ; python_version >= "3.7" and python_version < "4.0"
 gitdb==4.0.10 ; python_version >= "3.7" and python_version < "4.0"
 gitpython==3.1.29 ; python_version >= "3.7" and python_version < "4.0"
 identify==2.5.9 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
 imagesize==1.4.1 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
+importlib-metadata==6.7.0 ; python_version >= "3.7" and python_version < "3.10"
 iniconfig==1.1.1 ; python_version >= "3.7" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 multidict==6.0.3 ; python_version >= "3.7" and python_version < "4.0"
 mypy-extensions==0.4.3 ; python_version >= "3.7" and python_version < "4.0"
 mypy==0.991 ; python_version >= "3.7" and python_version < "4.0"
 nodeenv==1.7.0 ; python_version >= "3.7" and python_version < "4.0"
 packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
 pathspec==0.10.3 ; python_version >= "3.7" and python_version < "4.0"
-platformdirs==2.6.0 ; python_version >= "3.7" and python_version < "4.0"
+platformdirs==3.9.1 ; python_version >= "3.7" and python_version < "4.0"
 pluggy==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pre-commit==2.20.0 ; python_version >= "3.7" and python_version < "4.0"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-cov==4.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-runner==6.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-xdist==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest==7.2.0 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
-pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
+pyyaml==6.0.1 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 ruff==0.0.261 ; python_version >= "3.7" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 smmap==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
 snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinx==5.3.0 ; python_version >= "3.7" and python_version < "4.0"
@@ -53,14 +53,14 @@
 sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.7" and python_version < "4.0"
 sqlalchemy-stubs==0.4 ; python_version >= "3.7" and python_version < "4.0"
 toml==0.10.2 ; python_version >= "3.7" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.7" and python_full_version < "3.11.0a7"
 typed-ast==1.5.4 ; python_version < "3.8" and python_version >= "3.7"
-typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
+typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "4.0"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 vcrpy==4.2.1 ; python_version >= "3.7" and python_version < "4.0"
-virtualenv==20.17.1 ; python_version >= "3.7" and python_version < "4.0"
+virtualenv==20.24.0 ; python_version >= "3.7" and python_version < "4.0"
 wrapt==1.14.1 ; python_version >= "3.7" and python_version < "4.0"
 yarl==1.8.2 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
```

### Comparing `FlexGet-3.7.9/flexget/__init__.py` & `FlexGet-3.8.0/flexget/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/app.py` & `FlexGet-3.8.0/flexget/api/app.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/authentication.py` & `FlexGet-3.8.0/flexget/api/core/authentication.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/cached.py` & `FlexGet-3.8.0/flexget/api/core/cached.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/database.py` & `FlexGet-3.8.0/flexget/api/core/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/format_checker.py` & `FlexGet-3.8.0/flexget/api/core/format_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/plugins.py` & `FlexGet-3.8.0/flexget/api/core/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/schema.py` & `FlexGet-3.8.0/flexget/api/core/schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/server.py` & `FlexGet-3.8.0/flexget/api/core/server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/tasks.py` & `FlexGet-3.8.0/flexget/api/core/tasks.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/core/user.py` & `FlexGet-3.8.0/flexget/api/core/user.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/templates/api_response.html` & `FlexGet-3.8.0/flexget/api/templates/api_response.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/api/templates/swagger-ui.html` & `FlexGet-3.8.0/flexget/api/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/archive/archive.py` & `FlexGet-3.8.0/flexget/components/archive/archive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/archive/cli.py` & `FlexGet-3.8.0/flexget/components/archive/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/archive/db.py` & `FlexGet-3.8.0/flexget/components/archive/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/archives/archives.py` & `FlexGet-3.8.0/flexget/components/archives/archives.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/archives/decompress.py` & `FlexGet-3.8.0/flexget/components/archives/decompress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/archives/utils.py` & `FlexGet-3.8.0/flexget/components/archives/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/backlog/backlog.py` & `FlexGet-3.8.0/flexget/components/backlog/backlog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/backlog/cli.py` & `FlexGet-3.8.0/flexget/components/backlog/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/backlog/db.py` & `FlexGet-3.8.0/flexget/components/backlog/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/convert_magnet.py` & `FlexGet-3.8.0/flexget/components/bittorrent/convert_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/magnet_info_hash.py` & `FlexGet-3.8.0/flexget/components/bittorrent/magnet_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/private_torrents.py` & `FlexGet-3.8.0/flexget/components/bittorrent/private_torrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/torrent.py` & `FlexGet-3.8.0/flexget/components/bittorrent/torrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/torrent_alive.py` & `FlexGet-3.8.0/flexget/components/bittorrent/torrent_alive.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,16 +150,16 @@
         return 0
     except OSError as e:
         logger.warning('Server error: {}', e)
         return 0
     if not data:
         logger.debug('No data received from tracker scrape.')
         return 0
-    logger.debug('get_http_seeds is returning: {}', list(data.values())[0]['complete'])
-    return list(data.values())[0]['complete']
+    logger.debug('get_http_seeds is returning: {}', next(iter(data.values()))['complete'])
+    return next(iter(data.values()))['complete']
 
 
 def get_tracker_seeds(url, info_hash):
     if url.startswith('udp'):
         return get_udp_seeds(url, info_hash)
     elif url.startswith('http'):
         return get_http_seeds(url, info_hash)
```

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/torrent_files.py` & `FlexGet-3.8.0/flexget/components/bittorrent/torrent_files.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/torrent_match.py` & `FlexGet-3.8.0/flexget/components/bittorrent/torrent_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/torrent_scrub.py` & `FlexGet-3.8.0/flexget/components/bittorrent/torrent_scrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/bittorrent/trackers.py` & `FlexGet-3.8.0/flexget/components/bittorrent/trackers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/emby/api_emby.py` & `FlexGet-3.8.0/flexget/components/emby/api_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/emby/emby_list.py` & `FlexGet-3.8.0/flexget/components/emby/emby_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/emby/emby_lookup.py` & `FlexGet-3.8.0/flexget/components/emby/emby_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/emby/emby_refresh.py` & `FlexGet-3.8.0/flexget/components/emby/emby_refresh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/emby/emby_util.py` & `FlexGet-3.8.0/flexget/components/emby/emby_util.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/emby/from_emby.py` & `FlexGet-3.8.0/flexget/components/emby/from_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/estimate_release/estimate_release.py` & `FlexGet-3.8.0/flexget/components/estimate_release/estimate_release.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_movies_bluray.py` & `FlexGet-3.8.0/flexget/components/estimate_release/estimators/est_movies_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_released_movies.py` & `FlexGet-3.8.0/flexget/components/estimate_release/estimators/est_released_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_series_tvmaze.py` & `FlexGet-3.8.0/flexget/components/estimate_release/estimators/est_series_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/failed/api.py` & `FlexGet-3.8.0/flexget/components/failed/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/failed/cli.py` & `FlexGet-3.8.0/flexget/components/failed/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/failed/db.py` & `FlexGet-3.8.0/flexget/components/failed/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/failed/retry_failed.py` & `FlexGet-3.8.0/flexget/components/failed/retry_failed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/ftp/ftp_download.py` & `FlexGet-3.8.0/flexget/components/ftp/ftp_download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/ftp/ftp_list.py` & `FlexGet-3.8.0/flexget/components/ftp/ftp_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,15 @@
         entry = Entry()
 
         title = self.FTP.path.basename(path)
         location = self.FTP.path.abspath(path)
 
         entry['title'] = title
         entry['location'] = location
-        entry['url'] = 'ftp://{}:{}@{}:{}/{}'.format(
-            self.username, self.password, self.host, self.port, location
-        )
+        entry['url'] = f'ftp://{self.username}:{self.password}@{self.host}:{self.port}/{location}'
         entry['filename'] = title
 
         logger.debug('adding entry {}', entry)
         if entry.isvalid():
             return entry
         else:
             logger.warning('tried to return an illegal entry: {}', entry)
```

### Comparing `FlexGet-3.7.9/flexget/components/ftp/sftp.py` & `FlexGet-3.8.0/flexget/components/ftp/sftp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/ftp/sftp_client.py` & `FlexGet-3.8.0/flexget/components/ftp/sftp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         self.username: str = username
         self.password: Optional[str] = password
         self.private_key: Optional[str] = private_key
         self.private_key_pass: Optional[str] = private_key_pass
         self.host_key: Optional[HostKey] = host_key
 
         self.prefix: str = self._get_prefix()
-        self._sftp: 'pysftp.Connection' = self._connect(connection_tries)
+        self._sftp: pysftp.Connection = self._connect(connection_tries)
         self._handler_builder: HandlerBuilder = HandlerBuilder(
             self._sftp, self.prefix, self.private_key, self.private_key_pass, self.host_key
         )
 
     def list_directories(
         self,
         directories: List[str],
@@ -308,15 +308,15 @@
 
     def _connect(self, connection_tries: int) -> 'pysftp.Connection':
         tries: int = connection_tries
         retry_interval: int = RETRY_INTERVAL_SEC
 
         logger.debug('Connecting to {}', self.host)
 
-        sftp: Optional['pysftp.Connection'] = None
+        sftp: Optional[pysftp.Connection] = None
 
         while not sftp:
             try:
                 pysftp.Connection._set_authentication = _set_authentication_patch
                 sftp = pysftp.Connection(
                     host=self.host,
                     username=self.username,
```

### Comparing `FlexGet-3.7.9/flexget/components/history/api.py` & `FlexGet-3.8.0/flexget/components/history/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/history/cli.py` & `FlexGet-3.8.0/flexget/components/history/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/history/db.py` & `FlexGet-3.8.0/flexget/components/history/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/history/history.py` & `FlexGet-3.8.0/flexget/components/history/history.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/api.py` & `FlexGet-3.8.0/flexget/components/imdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/db.py` & `FlexGet-3.8.0/flexget/components/imdb/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/from_imdb.py` & `FlexGet-3.8.0/flexget/components/imdb/from_imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/imdb.py` & `FlexGet-3.8.0/flexget/components/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/imdb_lookup.py` & `FlexGet-3.8.0/flexget/components/imdb/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/imdb_url.py` & `FlexGet-3.8.0/flexget/components/imdb/imdb_url.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/imdb_watchlist.py` & `FlexGet-3.8.0/flexget/components/imdb/imdb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/imdb/utils.py` & `FlexGet-3.8.0/flexget/components/imdb/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/irc/api.py` & `FlexGet-3.8.0/flexget/components/irc/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/irc/cli.py` & `FlexGet-3.8.0/flexget/components/irc/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/irc/irc.py` & `FlexGet-3.8.0/flexget/components/irc/irc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/list_add.py` & `FlexGet-3.8.0/flexget/components/managed_lists/list_add.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/list_clear.py` & `FlexGet-3.8.0/flexget/components/managed_lists/list_clear.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/list_match.py` & `FlexGet-3.8.0/flexget/components/managed_lists/list_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/list_remove.py` & `FlexGet-3.8.0/flexget/components/managed_lists/list_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/couchpotato_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/couchpotato_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/api.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/cli.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,24 +121,20 @@
         db_entry = db.get_entry_by_title(list_id=entry_list.id, title=title, session=session)
         if db_entry:
             console(
                 "Entry with the title `{}` already exist with list `{}`. Will replace identifiers if given".format(
                     title, entry_list.name
                 )
             )
-            output = 'Successfully updated entry `{}` to entry list `{}` '.format(
-                title, entry_list.name
-            )
+            output = f'Successfully updated entry `{title}` to entry list `{entry_list.name}` '
         else:
             console(f"Adding entry with title `{title}` to list `{entry_list.name}`")
             db_entry = db.EntryListEntry(entry=entry, entry_list_id=entry_list.id)
             session.add(db_entry)
-            output = 'Successfully added entry `{}` to entry list `{}` '.format(
-                title, entry_list.name
-            )
+            output = f'Successfully added entry `{title}` to entry list `{entry_list.name}` '
         if options.attributes:
             console(f'Adding attributes to entry `{title}`')
             for identifier in options.attributes:
                 for k, v in identifier.items():
                     entry[k] = v
             db_entry.entry = entry
         console(output)
```

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/db.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/entry_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/entry_list/entry_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/imdb_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/imdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/api.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             db.get_list_by_id(list_id=list_id, session=session)
         except NoResultFound:
             raise NotFoundError('list_id %d does not exist' % list_id)
         data = request.json
         movie_identifiers = data.get('movie_identifiers', [])
         # Validates ID type based on allowed ID
         for id_name in movie_identifiers:
-            if list(id_name)[0] not in MovieListBase().supported_ids:
+            if next(iter(id_name)) not in MovieListBase().supported_ids:
                 raise BadRequest('movie identifier %s is not allowed' % id_name)
         title, year = data['movie_name'], data.get('movie_year')
         movie = db.get_movie_by_title_and_year(
             list_id=list_id, title=title, year=year, session=session
         )
         if movie:
             raise Conflict('movie with name "%s" already exist in list %d' % (title, list_id))
@@ -321,15 +321,15 @@
             movie = db.get_movie_by_id(list_id=list_id, movie_id=movie_id, session=session)
         except NoResultFound:
             raise NotFoundError('could not find movie with id %d in list %d' % (movie_id, list_id))
         data = request.json
 
         # Validates ID type based on allowed ID
         for id_name in data:
-            if list(id_name)[0] not in MovieListBase().supported_ids:
+            if next(iter(id_name)) not in MovieListBase().supported_ids:
                 raise BadRequest('movie identifier %s is not allowed' % id_name)
         movie.ids[:] = db.get_db_movie_identifiers(
             identifier_list=data, movie_id=movie_id, session=session
         )
         session.commit()
         return jsonify(movie.to_dict())
```

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/cli.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,30 +172,24 @@
 
         try:
             movie_exist = db.get_movie_by_id(
                 list_id=movie_list.id, movie_id=int(options.movie), session=session
             )
         except NoResultFound:
             console(
-                'Could not find movie with ID {} in list `{}`'.format(
-                    int(options.movie), options.list_name
-                )
+                f'Could not find movie with ID {int(options.movie)} in list `{options.list_name}`'
             )
             return
         except ValueError:
             title, year = split_title_year(options.movie)
             movie_exist = db.get_movie_by_title_and_year(
                 list_id=movie_list.id, title=title, year=year, session=session
             )
         if not movie_exist:
-            console(
-                'Could not find movie with title {} in list {}'.format(
-                    options.movie, options.list_name
-                )
-            )
+            console(f'Could not find movie with title {options.movie} in list {options.list_name}')
             return
         else:
             console(f'Removing movie {movie_exist.title} from list {options.list_name}')
             session.delete(movie_exist)
 
 
 def movie_list_purge(options):
```

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/db.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/movie_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/movie_list/movie_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/api.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/cli.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,19 +135,15 @@
             operation = 'added'
         if options.attributes:
             console(f'Adding attributes to entry `{title}`')
             for identifier in options.attributes:
                 for k, v in identifier.items():
                     entry[k] = v
             db_entry.entry = entry
-        console(
-            'Successfully {} entry `{}` to pending list `{}` '.format(
-                operation, title, pending_list.name
-            )
-        )
+        console(f'Successfully {operation} entry `{title}` to pending list `{pending_list.name}` ')
 
 
 def pending_list_approve(options, approve=None):
     with Session() as session:
         try:
             entry_list = db.get_list_by_exact_name(options.list_name)
         except NoResultFound:
```

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/db.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/pending_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/pending_list/pending_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/plex_watchlist.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/plex_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/radarr_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/radarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/cli.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,17 +56,15 @@
             regexp_list = db.create_list(options.list_name, session=session)
 
         regexp = db.get_regexp(list_id=regexp_list.id, regexp=options.regexp, session=session)
         if not regexp:
             console(f"Adding regexp {options.regexp} to list {regexp_list.name}")
             db.add_to_list_by_name(regexp_list.name, options.regexp, session=session)
             console(
-                'Successfully added regexp {} to regexp list {} '.format(
-                    options.regexp, regexp_list.name
-                )
+                f'Successfully added regexp {options.regexp} to regexp list {regexp_list.name} '
             )
         else:
             console(f"Regexp {options.regexp} already exists in list {regexp_list.name}")
 
 
 def action_del(options):
     with Session() as session:
@@ -75,19 +73,15 @@
             console(f'Could not find regexp list with name {options.list_name}')
             return
         regexp = db.get_regexp(list_id=regexp_list.id, regexp=options.regexp, session=session)
         if regexp:
             console(f'Removing regexp {options.regexp} from list {options.list_name}')
             session.delete(regexp)
         else:
-            console(
-                'Could not find regexp {} in list {}'.format(
-                    options.movie_title, options.list_name
-                )
-            )
+            console(f'Could not find regexp {options.movie_title} in list {options.list_name}')
             return
 
 
 def action_purge(options):
     with Session() as session:
         regexp_list = db.get_list_by_exact_name(options.list_name)
         if not regexp_list:
```

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/db.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/regexp_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/regexp_list/regexp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/sonarr_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/sonarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/subtitle_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/subtitle_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/thetvdb_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/thetvdb_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,15 @@
                 else:
                     series_name = series.name
                     if self.config.get('strip_dates'):
                         # Remove year from end of series name if present
                         series_name, _ = split_title_year(series_name)
                     entry = Entry()
                     entry['title'] = entry['series_name'] = series_name
-                    entry['url'] = 'http://thetvdb.com/index.php?tab=series&id={}'.format(
-                        str(series.id)
-                    )
+                    entry['url'] = f'http://thetvdb.com/index.php?tab=series&id={series.id!s}'
                     entry['tvdb_id'] = str(series.id)
                     self._items.append(entry)
         return self._items
 
     def invalidate_cache(self):
         self._items = None
```

### Comparing `FlexGet-3.7.9/flexget/components/managed_lists/lists/yaml_list.py` & `FlexGet-3.8.0/flexget/components/managed_lists/lists/yaml_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notification_framework.py` & `FlexGet-3.8.0/flexget/components/notify/notification_framework.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/bark.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/bark.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/cronitor.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/cronitor.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/discord.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/email.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/gotify.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/gotify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/ifttt.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/ifttt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/join.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/join.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/matrix.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/matrix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/microsoftteams.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/microsoftteams.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/mqtt.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/mqtt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/notifymyandroid.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/notifymyandroid.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/ntfysh.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/ntfysh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/prowl.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/prowl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/pushalot.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/pushalot.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/pushbullet.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/pushbullet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/pushover.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/pushover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/pushsafer.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/pushsafer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/rapidpush.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/rapidpush.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/slack.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/sms_ru.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/sms_ru.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/telegram.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/toast.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/toast.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notifiers/xmpp.py` & `FlexGet-3.8.0/flexget/components/notify/notifiers/xmpp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/notify/notify.py` & `FlexGet-3.8.0/flexget/components/notify/notify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/parsing/parsers/parser_common.py` & `FlexGet-3.8.0/flexget/components/parsing/parsers/parser_common.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/parsing/parsers/parser_guessit.py` & `FlexGet-3.8.0/flexget/components/parsing/parsers/parser_guessit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/parsing/parsers/parser_internal.py` & `FlexGet-3.8.0/flexget/components/parsing/parsers/parser_internal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/parsing/plugin_parsing.py` & `FlexGet-3.8.0/flexget/components/parsing/plugin_parsing.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/pending_approval/api.py` & `FlexGet-3.8.0/flexget/components/pending_approval/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/pending_approval/cli.py` & `FlexGet-3.8.0/flexget/components/pending_approval/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/pending_approval/db.py` & `FlexGet-3.8.0/flexget/components/pending_approval/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/pending_approval/pending_approval.py` & `FlexGet-3.8.0/flexget/components/pending_approval/pending_approval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/rejected/api.py` & `FlexGet-3.8.0/flexget/components/rejected/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/rejected/cli.py` & `FlexGet-3.8.0/flexget/components/rejected/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/rejected/db.py` & `FlexGet-3.8.0/flexget/components/rejected/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/rejected/remember_rejected.py` & `FlexGet-3.8.0/flexget/components/rejected/remember_rejected.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/scheduler/api.py` & `FlexGet-3.8.0/flexget/components/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/scheduler/scheduler.py` & `FlexGet-3.8.0/flexget/components/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/seen/api.py` & `FlexGet-3.8.0/flexget/components/seen/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/seen/cli.py` & `FlexGet-3.8.0/flexget/components/seen/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/seen/db.py` & `FlexGet-3.8.0/flexget/components/seen/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/seen/seen.py` & `FlexGet-3.8.0/flexget/components/seen/seen.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/seen/seen_info_hash.py` & `FlexGet-3.8.0/flexget/components/seen/seen_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/seen/seen_movies.py` & `FlexGet-3.8.0/flexget/components/seen/seen_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/all_series.py` & `FlexGet-3.8.0/flexget/components/series/all_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/api.py` & `FlexGet-3.8.0/flexget/components/series/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -842,17 +842,15 @@
                 release_items.append(release)
 
         for release in release_items:
             if args.get('forget'):
                 fire_event('forget', release.title)
             db.delete_season_release_by_id(release.id)
         return success_response(
-            'successfully deleted all releases for season {} from show {}'.format(
-                season_id, show_id
-            )
+            f'successfully deleted all releases for season {season_id} from show {show_id}'
         )
 
     @api.response(
         200, 'Successfully reset all downloaded releases for season', model=base_message_schema
     )
     @api.doc(
         description='Resets all of the downloaded releases of an season, clearing the quality to be downloaded '
```

### Comparing `FlexGet-3.7.9/flexget/components/series/cli.py` & `FlexGet-3.8.0/flexget/components/series/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,19 +147,15 @@
                 _, entity_type = db.set_series_begin(series, ep_id)
             except ValueError as e:
                 console(e)
             else:
                 if entity_type == 'season':
                     console('`%s` was identified as a season.' % ep_id)
                     ep_id += 'E01'
-                console(
-                    'Releases for `{}` will be accepted starting with `{}`.'.format(
-                        series.name, ep_id
-                    )
-                )
+                console(f'Releases for `{series.name}` will be accepted starting with `{ep_id}`.')
                 session.commit()
             manager.config_changed()
 
 
 def remove(manager, options, forget=False):
     name = options.series_name
     if options.episode_id:
@@ -272,17 +268,15 @@
         else:
             footer += '\n `{}` uses `{}` mode to identify episode numbering.'.format(
                 series.name,
                 series.identified_by,
             )
         begin_text = 'option'
         if series.begin:
-            footer += ' \n Begin for `{}` is set to `{}`.'.format(
-                series.name, series.begin.identifier
-            )
+            footer += f' \n Begin for `{series.name}` is set to `{series.begin.identifier}`.'
             begin_text = 'and `begin` options'
         footer += ' \n See `identified_by` %s for more information.' % begin_text
     table = TerminalTable(*header, table_type=options.table_type, title=table_title)
     for row in table_data:
         table.add_row(*row)
     console(table)
     if not options.table_type == 'porcelain':
```

### Comparing `FlexGet-3.7.9/flexget/components/series/configure_series.py` & `FlexGet-3.8.0/flexget/components/series/configure_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/db.py` & `FlexGet-3.8.0/flexget/components/series/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,17 +547,15 @@
     def name_normalized(self):
         return self._alt_name_normalized
 
     def __init__(self, name):
         self.alt_name = name
 
     def __str__(self):
-        return '<SeriesAlternateName(series_id={}, alt_name={})>'.format(
-            self.series_id, self.alt_name
-        )
+        return f'<SeriesAlternateName(series_id={self.series_id}, alt_name={self.alt_name})>'
 
     def __repr__(self):
         return str(self).encode('ascii', 'replace')
 
 
 class SeriesTask(Base):
     __tablename__ = 'series_tasks'
```

### Comparing `FlexGet-3.7.9/flexget/components/series/gen_series.py` & `FlexGet-3.8.0/flexget/components/series/gen_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/internal_estimator.py` & `FlexGet-3.8.0/flexget/components/series/internal_estimator.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/metainfo_series.py` & `FlexGet-3.8.0/flexget/components/series/metainfo_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/next_series_episodes.py` & `FlexGet-3.8.0/flexget/components/series/next_series_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/next_series_seasons.py` & `FlexGet-3.8.0/flexget/components/series/next_series_seasons.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/series.py` & `FlexGet-3.8.0/flexget/components/series/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
                     # If group name is not a valid quality requirement string, do nothing.
                     pass
             group_settings = config['settings'].get(group_name, {})
             for series in config[group_name]:
                 # convert into dict-form if necessary
                 series_settings = {}
                 if isinstance(series, dict):
-                    series, series_settings = list(series.items())[0]
+                    series, series_settings = next(iter(series.items()))
                 # Make sure this isn't a series with no name
                 if not series:
                     logger.warning('Series config contains a series with no name!')
                     continue
                 # make sure series name is a string to accommodate for "24"
                 if not isinstance(series, str):
                     series = str(series)
@@ -295,15 +295,15 @@
         """Combines the series from multiple lists, making sure there are no doubles.
 
         If keyword argument log_once is set to True, an error message will be printed if a series
         is listed more than once, otherwise log_once will be used."""
         unique_series = {}
         for series_list in series_lists:
             for series in series_list:
-                series, series_settings = list(series.items())[0]
+                series, series_settings = next(iter(series.items()))
                 if series not in unique_series:
                     unique_series[series] = series_settings
                 else:
                     if kwargs.get('log_once'):
                         log_once(
                             'Series `%s` is already configured in series plugin' % series, logger
                         )
@@ -366,15 +366,15 @@
 
     def auto_exact(self, config):
         """Automatically enable exact naming option for series that look like a problem"""
 
         # generate list of all series in one dict
         all_series = {}
         for series_item in config:
-            series_name, series_config = list(series_item.items())[0]
+            series_name, series_config = next(iter(series_item.items()))
             all_series[series_name] = series_config
 
         # scan for problematic names, enable exact mode for them
         for series_name, series_config in all_series.items():
             for name in list(all_series.keys()):
                 if (name.lower().startswith(series_name.lower())) and (
                     name.lower() != series_name.lower()
@@ -410,34 +410,34 @@
                     entries_map[word[:1].lower()].append(entry)
 
         with Session() as session:
             # Preload series
             # str() added to make sure number shows (e.g. 24) are turned into strings
 
             # First add all series config names (normalized)
-            series_names = [str(normalize_series_name(list(s.keys())[0])) for s in config]
+            series_names = [str(normalize_series_name(next(iter(s.keys())))) for s in config]
             # Add series names from the config without normalization to capture configs
             #  that use slightly different series names. See https://github.com/Flexget/Flexget/issues/2057
             series_names.extend(
-                str(list(s.keys())[0])
+                str(next(iter(s.keys())))
                 for s in config
-                if str(list(s.keys())[0]) not in series_names
+                if str(next(iter(s.keys()))) not in series_names
             )
 
             existing_db_series = []
 
             for chunk in chunked(series_names):
                 existing_db_series.extend(
                     session.query(db.Series).filter(db.Series.name.in_(chunk))
                 )
 
             existing_db_series = {s.name_normalized: s for s in existing_db_series}
 
             for series_item in config:
-                series_name, series_config = list(series_item.items())[0]
+                series_name, series_config = next(iter(series_item.items()))
                 alt_names = get_config_as_array(series_config, 'alternate_name')
                 db_series = existing_db_series.get(normalize_series_name(series_name))
                 db_identified_by = db_series.identified_by if db_series else None
                 letters = set(
                     [series_name[:1].lower()]
                     + [normalize_series_name(series_name)[:1].lower()]
                     + [alt[:1].lower() for alt in alt_names]
@@ -463,29 +463,29 @@
                 and entry.get('series_parser')
             ):
                 found_series.setdefault(entry['series_name'], []).append(entry)
 
         # Prefetch series
         with Session() as session:
             # str() added to make sure number shows (e.g. 24) are turned into strings
-            series_names = [str(list(s.keys())[0]) for s in config]
+            series_names = [str(next(iter(s.keys()))) for s in config]
             existing_series = (
                 session.query(db.Series)
                 .filter(db.Series.name.in_(series_names))
                 .options(joinedload(db.Series.alternate_names))
                 .all()
             )
             existing_series_map = {s.name_normalized: s for s in existing_series}
             # Expunge so we can work on de-attached while processing the series to minimize db locks
             session.expunge_all()
 
         start_time = preferred_clock()
         for series_item in config:
             with Session() as session:
-                series_name, series_config = list(series_item.items())[0]
+                series_name, series_config = next(iter(series_item.items()))
 
                 if series_config.get('parse_only'):
                     logger.debug(
                         'Skipping filtering of series `{}` because of parse_only', series_name
                     )
                     continue
 
@@ -1114,25 +1114,25 @@
 
             session.query(db.SeriesTask).filter(db.SeriesTask.name == task.name).delete()
             if not task.config.get('series'):
                 return
             config = self.prepare_config(task.config['series'])
 
             # Prefetch series
-            names = [str(list(series.keys())[0]) for series in config]
+            names = [str(next(iter(series.keys()))) for series in config]
             existing_series = (
                 session.query(db.Series)
                 .filter(db.Series.name.in_(names))
                 .options(joinedload(db.Series.alternate_names))
                 .all()
             )
             existing_series_map = {s.name_normalized: s for s in existing_series}
 
             for series_item in config:
-                series_name, series_config = list(series_item.items())[0]
+                series_name, series_config = next(iter(series_item.items()))
                 # Make sure number shows (e.g. 24) are turned into strings
                 series_name = str(series_name)
                 db_series = existing_series_map.get(normalize_series_name(series_name))
                 alts = series_config.get('alternate_name', [])
                 if not isinstance(alts, list):
                     alts = [alts]
                 if db_series:
```

### Comparing `FlexGet-3.7.9/flexget/components/series/series_begin.py` & `FlexGet-3.8.0/flexget/components/series/series_begin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/series_premiere.py` & `FlexGet-3.8.0/flexget/components/series/series_premiere.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/series/series_remove.py` & `FlexGet-3.8.0/flexget/components/series/series_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/allyoulike.py` & `FlexGet-3.8.0/flexget/components/sites/sites/allyoulike.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/alpharatio.py` & `FlexGet-3.8.0/flexget/components/sites/sites/alpharatio.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/animeindex.py` & `FlexGet-3.8.0/flexget/components/sites/sites/animeindex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/anirena.py` & `FlexGet-3.8.0/flexget/components/sites/sites/anirena.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/archetorrent.py` & `FlexGet-3.8.0/flexget/components/sites/sites/archetorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/argenteam.py` & `FlexGet-3.8.0/flexget/components/sites/sites/argenteam.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/awesomehd.py` & `FlexGet-3.8.0/flexget/components/sites/sites/awesomehd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/bakabt.py` & `FlexGet-3.8.0/flexget/components/sites/sites/bakabt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/btn.py` & `FlexGet-3.8.0/flexget/components/sites/sites/btn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/cinemageddon.py` & `FlexGet-3.8.0/flexget/components/sites/sites/cinemageddon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/cpasbien.py` & `FlexGet-3.8.0/flexget/components/sites/sites/cpasbien.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/deadfrog.py` & `FlexGet-3.8.0/flexget/components/sites/sites/deadfrog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/descargas2020.py` & `FlexGet-3.8.0/flexget/components/sites/sites/descargas2020.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/ettv.py` & `FlexGet-3.8.0/flexget/components/sites/sites/ettv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/eztv.py` & `FlexGet-3.8.0/flexget/components/sites/sites/eztv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/filelist.py` & `FlexGet-3.8.0/flexget/components/sites/sites/filelist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/filelist_api.py` & `FlexGet-3.8.0/flexget/components/sites/sites/filelist_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             for result in results:
                 entry = Entry()
 
                 entry['title'] = result['name']
                 entry['url'] = result['download_link']
                 entry['imdb'] = result['imdb']
                 # size is returned in bytes but expected in MiB
-                entry['content_size'] = result['size'] / 2**20
+                entry['content_size'] = result['size']
                 entry['torrent_snatches'] = result['times_completed']
                 entry['torrent_seeds'] = result['seeders']
                 entry['torrent_leeches'] = result['leechers']
                 entry['torrent_internal'] = bool(result['internal'])
                 entry['torrent_moderated'] = bool(result['moderated'])
                 entry['torrent_freeleech'] = bool(result['freeleech'])
                 entry['torrent_genres'] = [
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/frenchtorrentdb.py` & `FlexGet-3.8.0/flexget/components/sites/sites/frenchtorrentdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/fuzer.py` & `FlexGet-3.8.0/flexget/components/sites/sites/fuzer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/google_cse.py` & `FlexGet-3.8.0/flexget/components/sites/sites/google_cse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/hebits.py` & `FlexGet-3.8.0/flexget/components/sites/sites/hebits.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                 continue
 
             search_results = search_results_response['response']['results']
             for result in search_results:
                 torrent_id = result['torrents'][0]['torrentId']
                 seeders = result['torrents'][0]['seeders']
                 leechers = result['torrents'][0]['leechers']
-                size = result['torrents'][0]['size'] / 2**20
+                size = result['torrents'][0]['size']
                 title = result['torrents'][0]['release']
 
                 entry = Entry(
                     torrent_seeds=seeders,
                     torrent_leeches=leechers,
                     torrent_availability=torrent_availability(seeders, leechers),
                     content_size=size,
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/hliang.py` & `FlexGet-3.8.0/flexget/components/sites/sites/hliang.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/horriblesubs.py` & `FlexGet-3.8.0/flexget/components/sites/sites/horriblesubs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/iptorrents.py` & `FlexGet-3.8.0/flexget/components/sites/sites/iptorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/koreus.py` & `FlexGet-3.8.0/flexget/components/sites/sites/koreus.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/limetorrents.py` & `FlexGet-3.8.0/flexget/components/sites/sites/limetorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/lostfilm.py` & `FlexGet-3.8.0/flexget/components/sites/sites/lostfilm.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,15 @@
         for s_item in cfg_list:
             if isinstance(s_item, str):
                 names_list.add(LostFilm._simplify_name(s_item))
             elif isinstance(s_item, int) or isinstance(s_item, float):
                 # The name is something like '365' or '36.6'
                 names_list.add(LostFilm._simplify_name(str(s_item)))
             elif isinstance(s_item, dict):
-                s_name, s_cfg = list(s_item.items())[0]
+                s_name, s_cfg = next(iter(s_item.items()))
                 names_list.add(LostFilm._simplify_name(s_name))
                 if s_cfg.get('alternate_name'):
                     if isinstance(s_cfg['alternate_name'], str):
                         names_list.add(LostFilm._simplify_name(s_cfg['alternate_name']))
                     elif isinstance(s_cfg['alternate_name'], list):
                         # A list of alternate names
                         for a_name in s_cfg['alternate_name']:
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/magnetdl.py` & `FlexGet-3.8.0/flexget/components/sites/sites/magnetdl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/morethantv.py` & `FlexGet-3.8.0/flexget/components/sites/sites/morethantv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/ncore.py` & `FlexGet-3.8.0/flexget/components/sites/sites/ncore.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,17 @@
                     e['title'] = a.text
                     e['url'] = URL + f'/torrents.php?action=download&id={id}&' + PASSKEY
 
                     parent = a.parent.parent.parent.parent
 
                     e['torrent_seeds'] = parent.find('div', class_='box_s2').string
                     e['torrent_leeches'] = parent.find('div', class_='box_l2').string
-                    e['content_size'] = parent.find('div', class_='box_meret2').string
+                    e['content_size'] = (
+                        float(parent.find('div', class_='box_meret2').string) * 1024**2
+                    )
                     e['torrent_availability'] = torrent_availability(
                         e['torrent_seeds'], e['torrent_leeches']
                     )
 
                     yield e
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/newtorrents.py` & `FlexGet-3.8.0/flexget/components/sites/sites/newtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/newznab.py` & `FlexGet-3.8.0/flexget/components/sites/sites/newznab.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 new_entry = Entry()
 
                 for key in list(rss_entry.keys()):
                     new_entry[key] = rss_entry[key]
                 new_entry['url'] = new_entry['link']
                 if rss_entry.enclosures:
                     size = int(rss_entry.enclosures[0]['length'])  # B
-                    new_entry['content_size'] = size / (2**20)  # MB
+                    new_entry['content_size'] = size  # B
                 entries.append(new_entry)
 
         return entries
 
     def search(self, task, entry, config=None):
         url, params = self.get_url_and_params(config)
         if config['category'] == 'movie':
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/nnmclub.py` & `FlexGet-3.8.0/flexget/components/sites/sites/nnmclub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/nyaa.py` & `FlexGet-3.8.0/flexget/components/sites/sites/nyaa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/passthepopcorn.py` & `FlexGet-3.8.0/flexget/components/sites/sites/passthepopcorn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/piratebay.py` & `FlexGet-3.8.0/flexget/components/sites/sites/piratebay.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,17 +180,15 @@
         entry['title'] = json_result['name']
         entry['torrent_seeds'] = int(json_result['seeders'])
         entry['torrent_leeches'] = int(json_result['leechers'])
         entry['torrent_timestamp'] = int(json_result['added'])  # custom field for sorting by date
         entry['torrent_availability'] = torrent_availability(
             entry['torrent_seeds'], entry['torrent_leeches']
         )
-        entry['content_size'] = int(
-            round(int(json_result['size']) / (1024 * 1024))
-        )  # content_size is in MiB
+        entry['content_size'] = int(json_result['size'])  # content_size is in bytes
         entry['torrent_info_hash'] = json_result['info_hash']
         entry['url'] = self.info_hash_to_magnet(json_result['info_hash'], json_result['name'])
         return entry
 
 
 @event('plugin.register')
 def register_plugin():
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/ptn.py` & `FlexGet-3.8.0/flexget/components/sites/sites/ptn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/rarbg.py` & `FlexGet-3.8.0/flexget/components/sites/sites/rarbg.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 for result in response.get('torrent_results'):
                     e = Entry()
 
                     e['title'] = result.get('title')
                     e['url'] = result.get('download')
                     e['torrent_seeds'] = int(result.get('seeders'))
                     e['torrent_leeches'] = int(result.get('leechers'))
-                    e['content_size'] = int(result.get('size')) / 1024 / 1024
+                    e['content_size'] = int(result.get('size'))
                     episode_info = result.get('episode_info')
                     if episode_info:
                         e['imdb_id'] = episode_info.get('imdb')
                         e['tvdb_id'] = episode_info.get('tvdb')
                         e['tvrage_id'] = episode_info.get('tvrage')
 
                     entries.add(e)
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/redirect.py` & `FlexGet-3.8.0/flexget/components/sites/sites/redirect.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/rlsbb.py` & `FlexGet-3.8.0/flexget/components/sites/sites/rlsbb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/rmz.py` & `FlexGet-3.8.0/flexget/components/sites/sites/rmz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/rss.py` & `FlexGet-3.8.0/flexget/components/sites/sites/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/rutracker.py` & `FlexGet-3.8.0/flexget/components/sites/sites/rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/serienjunkies.py` & `FlexGet-3.8.0/flexget/components/sites/sites/serienjunkies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/shortened.py` & `FlexGet-3.8.0/flexget/components/sites/sites/shortened.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/site_1337x.py` & `FlexGet-3.8.0/flexget/components/sites/sites/site_1337x.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/site_rutracker.py` & `FlexGet-3.8.0/flexget/components/sites/sites/site_rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/solidtorrents.py` & `FlexGet-3.8.0/flexget/components/sites/sites/solidtorrents.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,15 @@
             time.mktime(
                 datetime.strptime(json_result['imported'], '%Y-%m-%dT%H:%M:%S.%fZ').timetuple()
             )
         )
         entry['torrent_availability'] = torrent_availability(
             entry['torrent_seeds'], entry['torrent_leeches']
         )
-        entry['content_size'] = int(
-            round(int(json_result['size']) / (1024 * 1024))
-        )  # content_size is in MiB
+        entry['content_size'] = int(json_result['size'])  # content_size is in bytes
         entry['torrent_info_hash'] = json_result['infohash']
         entry['url'] = json_result['magnet']
         return entry
 
 
 @event('plugin.register')
 def register_plugin():
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/torrent_cache.py` & `FlexGet-3.8.0/flexget/components/sites/sites/torrent_cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/torrentday.py` & `FlexGet-3.8.0/flexget/components/sites/sites/torrentday.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/torrentleech.py` & `FlexGet-3.8.0/flexget/components/sites/sites/torrentleech.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/torrentz.py` & `FlexGet-3.8.0/flexget/components/sites/sites/torrentz.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 if not m:
                     logger.debug('regexp did not find seeds / peer data')
                     continue
 
                 entry = Entry()
                 entry['title'] = item.title
                 entry['url'] = item.link
-                entry['content_size'] = int(m.group(1))
+                entry['content_size'] = int(m.group(1)) * 1024**2
                 entry['torrent_seeds'] = int(m.group(2).replace(',', ''))
                 entry['torrent_leeches'] = int(m.group(3).replace(',', ''))
                 entry['torrent_info_hash'] = m.group(4).upper()
                 entry['torrent_availability'] = torrent_availability(
                     entry['torrent_seeds'], entry['torrent_leeches']
                 )
                 entries.add(entry)
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/wordpress.py` & `FlexGet-3.8.0/flexget/components/sites/sites/wordpress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/sites/yts.py` & `FlexGet-3.8.0/flexget/components/sites/sites/yts.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/urlrewrite.py` & `FlexGet-3.8.0/flexget/components/sites/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/urlrewrite_search.py` & `FlexGet-3.8.0/flexget/components/sites/urlrewrite_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # search accepted
         for entry in task.accepted:
             # loop through configured searches
             for name in config:
                 search_config = None
                 if isinstance(name, dict):
                     # the name is the first/only key in the dict.
-                    name, search_config = list(name.items())[0]
+                    name, search_config = next(iter(name.items()))
                 logger.verbose('Searching `{}` from {}', entry['title'], name)
                 try:
                     try:
                         results = plugins[name].search(
                             task=task, entry=entry, config=search_config
                         )
                     except TypeError:
```

### Comparing `FlexGet-3.7.9/flexget/components/sites/urlrewriting.py` & `FlexGet-3.8.0/flexget/components/sites/urlrewriting.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/sites/utils.py` & `FlexGet-3.8.0/flexget/components/sites/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/status/api.py` & `FlexGet-3.8.0/flexget/components/status/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/status/cli.py` & `FlexGet-3.8.0/flexget/components/status/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/status/db.py` & `FlexGet-3.8.0/flexget/components/status/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/status/status.py` & `FlexGet-3.8.0/flexget/components/status/status.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/thetvdb/api.py` & `FlexGet-3.8.0/flexget/components/thetvdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/thetvdb/api_tvdb.py` & `FlexGet-3.8.0/flexget/components/thetvdb/api_tvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/thetvdb/thetvdb_lookup.py` & `FlexGet-3.8.0/flexget/components/thetvdb/thetvdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/tmdb/api.py` & `FlexGet-3.8.0/flexget/components/tmdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/tmdb/api_tmdb.py` & `FlexGet-3.8.0/flexget/components/tmdb/api_tmdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,17 +318,15 @@
         if smart_match and not (title or tmdb_id or imdb_id):
             # If smart_match was specified, parse it into a title and year
             title_parser = plugin.get('parsing', 'api_tmdb').parse_movie(smart_match)
             title = title_parser.name
             year = title_parser.year
         if not (title or tmdb_id or imdb_id):
             raise LookupError('No criteria specified for TMDb lookup')
-        id_str = '<title={}, year={}, tmdb_id={}, imdb_id={}>'.format(
-            title, year, tmdb_id, imdb_id
-        )
+        id_str = f'<title={title}, year={year}, tmdb_id={tmdb_id}, imdb_id={imdb_id}>'
 
         logger.debug('Looking up TMDb information for {}', id_str)
         movie = None
         if imdb_id or tmdb_id:
             ors = []
             if tmdb_id:
                 ors.append(TMDBMovie.id == tmdb_id)
```

### Comparing `FlexGet-3.7.9/flexget/components/tmdb/tmdb_lookup.py` & `FlexGet-3.8.0/flexget/components/tmdb/tmdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/api.py` & `FlexGet-3.8.0/flexget/components/trakt/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/api_trakt.py` & `FlexGet-3.8.0/flexget/components/trakt/api_trakt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/cli.py` & `FlexGet-3.8.0/flexget/components/trakt/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/db.py` & `FlexGet-3.8.0/flexget/components/trakt/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/next_trakt_episodes.py` & `FlexGet-3.8.0/flexget/components/trakt/next_trakt_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/trakt_calendar.py` & `FlexGet-3.8.0/flexget/components/trakt/trakt_calendar.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/trakt_list.py` & `FlexGet-3.8.0/flexget/components/trakt/trakt_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/trakt/trakt_lookup.py` & `FlexGet-3.8.0/flexget/components/trakt/trakt_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/tvmaze/api.py` & `FlexGet-3.8.0/flexget/components/tvmaze/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/tvmaze/api_tvmaze.py` & `FlexGet-3.8.0/flexget/components/tvmaze/api_tvmaze.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,15 @@
         self.search_name = search_name.lower()
         if series_id:
             self.series_id = series_id
         if series:
             self.series = series
 
     def __repr__(self):
-        return '<TVMazeLookup(search_name={},series_id={})'.format(
-            self.search_name, self.series_id
-        )
+        return f'<TVMazeLookup(search_name={self.search_name},series_id={self.series_id})'
 
 
 class TVMazeSeries(Base):
     __tablename__ = 'tvmaze_series'
 
     tvmaze_id = Column(Integer, primary_key=True)
     status = Column(Unicode)
```

### Comparing `FlexGet-3.7.9/flexget/components/tvmaze/tvmaze_lookup.py` & `FlexGet-3.8.0/flexget/components/tvmaze/tvmaze_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/variables/api.py` & `FlexGet-3.8.0/flexget/components/variables/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/components/variables/variables.py` & `FlexGet-3.8.0/flexget/components/variables/variables.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/config_schema.py` & `FlexGet-3.8.0/flexget/config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import jsonschema
 from jsonschema import ValidationError
 from loguru import logger
 
 from flexget.event import fire_event
 from flexget.utils import qualities, template
 from flexget.utils.template import get_template
-from flexget.utils.tools import parse_episode_identifier, parse_timedelta
+from flexget.utils.tools import parse_episode_identifier, parse_filesize, parse_timedelta
 
 logger = logger.bind(name='config_schema')
 
 BASE_SCHEMA_NAME = 'draft4'
 BASE_SCHEMA_URI = 'http://json-schema.org/draft-04/schema#'
 BaseValidator = jsonschema.Draft4Validator
 # Type hint for json schemas. (If we upgrade to a newer json schema version, the type might allow more than dicts.)
@@ -179,26 +179,21 @@
     percent_input = percent_input.rstrip('%')
     try:
         return float(percent_input)
     except ValueError:
         raise ValueError("should be in format '0-x%'")
 
 
-def parse_size(size_input: str) -> int:
+def parse_size(size_input: str, si: bool = False) -> int:
     """Takes a size string from the config and turns it into int(bytes)."""
-    prefixes = [None, 'K', 'M', 'G', 'T', 'P']
     try:
         # Bytes
         return int(size_input)
     except ValueError:
-        size_input = size_input.upper().rstrip('IB')
-        value, unit = float(size_input[:-1]), size_input[-1:]
-        if unit not in prefixes:
-            raise ValueError("should be in format '0-x (KiB, MiB, GiB, TiB, PiB)'")
-        return int(1024 ** prefixes.index(unit) * value)
+        return parse_filesize(size_input, si=si)
 
 
 # Public API end here, the rest should not be used outside this module
 
 
 class RefResolver(jsonschema.RefResolver):
     def __init__(self, *args, **kwargs):
@@ -412,15 +407,15 @@
         if not no_type_errors:
             # If all of the branches had a 'type' error, create our own virtual type error with all possible types
             for e in validator.descend(error.instance, {'type': valid_types}):
                 yield e
         elif len(no_type_errors) == 1:
             # If one of the possible schemas did not have a 'type' error, assume that is the intended one and issue
             # all errors from that subschema
-            for e in list(no_type_errors.values())[0]:
+            for e in next(iter(no_type_errors.values())):
                 e.schema_path.extendleft(reversed(error.schema_path))
                 e.path.extendleft(reversed(error.path))
                 yield e
         else:
             yield error
```

### Comparing `FlexGet-3.7.9/flexget/db_schema.py` & `FlexGet-3.8.0/flexget/db_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/entry.py` & `FlexGet-3.8.0/flexget/entry.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/event.py` & `FlexGet-3.8.0/flexget/event.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ipc.py` & `FlexGet-3.8.0/flexget/ipc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/log.py` & `FlexGet-3.8.0/flexget/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/manager.py` & `FlexGet-3.8.0/flexget/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         self.lockfile: str = ''
         self.database_uri: str = ''
         self.db_upgraded = False
         self._has_lock = False
         self.is_daemon = False
         self.ipc_server: IPCServer
         self.task_queue: TaskQueue
-        self.persist: 'SimplePersistence'
+        self.persist: SimplePersistence
         self.initialized = False
 
         self.config: Dict = {}
 
         self.options = self.parse_initial_options(args)
         self._init_config(create=False)
         # When we are in test mode, we use a different lock file and db
```

### Comparing `FlexGet-3.7.9/flexget/options.py` & `FlexGet-3.8.0/flexget/options.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugin.py` & `FlexGet-3.8.0/flexget/plugin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/check.py` & `FlexGet-3.8.0/flexget/plugins/cli/check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/cli_config.py` & `FlexGet-3.8.0/flexget/plugins/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/database.py` & `FlexGet-3.8.0/flexget/plugins/cli/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/debug_info.py` & `FlexGet-3.8.0/flexget/plugins/cli/debug_info.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/doc.py` & `FlexGet-3.8.0/flexget/plugins/cli/doc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/explain_sql.py` & `FlexGet-3.8.0/flexget/plugins/cli/explain_sql.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/filters.py` & `FlexGet-3.8.0/flexget/plugins/cli/filters.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/inject.py` & `FlexGet-3.8.0/flexget/plugins/cli/inject.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/perf_tests.py` & `FlexGet-3.8.0/flexget/plugins/cli/perf_tests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/performance.py` & `FlexGet-3.8.0/flexget/plugins/cli/performance.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/plugins.py` & `FlexGet-3.8.0/flexget/plugins/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/templates.py` & `FlexGet-3.8.0/flexget/plugins/cli/templates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/try_regexp.py` & `FlexGet-3.8.0/flexget/plugins/cli/try_regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/web.py` & `FlexGet-3.8.0/flexget/plugins/cli/web.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/wiki_qualities.py` & `FlexGet-3.8.0/flexget/plugins/cli/wiki_qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/cli/win32_service.py` & `FlexGet-3.8.0/flexget/plugins/cli/win32_service.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/aria2.py` & `FlexGet-3.8.0/flexget/plugins/clients/aria2.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/deluge.py` & `FlexGet-3.8.0/flexget/plugins/clients/deluge.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     # Fields we provide outside of the deluge_ prefixed namespace
     settings_map = {
         'name': 'title',
         'hash': 'torrent_info_hash',
         'num_peers': 'torrent_peers',
         'num_seeds': 'torrent_seeds',
-        'total_size': ('content_size', lambda size: size / 1024 / 1024),
+        'total_size': 'content_size',
         'files': ('content_files', lambda file_dicts: [f['path'] for f in file_dicts]),
     }
 
     schema = {
         'anyOf': [
             {'type': 'boolean'},
             {
```

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/nzbget.py` & `FlexGet-3.8.0/flexget/plugins/clients/nzbget.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/pyload.py` & `FlexGet-3.8.0/flexget/plugins/clients/pyload.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/qbittorrent.py` & `FlexGet-3.8.0/flexget/plugins/clients/qbittorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
                     logger.debug("filtered `%s` by not completed" % torrent['name'])
                     continue
 
             yield Entry(
                 title=torrent['name'],
                 url=torrent['magnet_uri'],
                 content_files=[f['name'] for f in torrent.files],
-                content_size=torrent['size'] // 1024 // 1024,
+                content_size=torrent['size'],
                 torrent_info_hash=torrent['infohash_v1'],
                 torrent_info_hash_v2=torrent['infohash_v2'],
                 torrent_seeds=torrent['num_seeds'],
                 torrent_peers=torrent['num_leechs'],
                 qbittorrent_ratio=torrent['ratio'],
                 qbittorrent_category=torrent['category'],
                 qbittorrent_state=torrent['state'],
```

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/rtorrent.py` & `FlexGet-3.8.0/flexget/plugins/clients/rtorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/clients/transmission.py` & `FlexGet-3.8.0/flexget/plugins/clients/transmission.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                 seed_ratio_ok and idle_limit_ok and torrent.progress == 100
             ):
                 continue
             entry = Entry(
                 title=torrent.name,
                 url='',
                 torrent_info_hash=torrent.hashString,
-                content_size=torrent.total_size / (1024 * 1024),
+                content_size=torrent.total_size,
             )
             # Location of torrent is only valid if transmission is on same machine as flexget
             if config['host'] in ('localhost', '127.0.0.1'):
                 entry['location'] = torrent.torrent_file
                 entry['url'] = pathlib.Path(torrent.torrent_file).as_uri()
             for attr, field in {
                 'id': 'id',
```

### Comparing `FlexGet-3.7.9/flexget/plugins/daemon/web_server.py` & `FlexGet-3.8.0/flexget/plugins/daemon/web_server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/abort_if_exists.py` & `FlexGet-3.8.0/flexget/plugins/filter/abort_if_exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/accept_all.py` & `FlexGet-3.8.0/flexget/plugins/filter/accept_all.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/age.py` & `FlexGet-3.8.0/flexget/plugins/filter/age.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/best_quality.py` & `FlexGet-3.8.0/flexget/plugins/filter/best_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/content_filter.py` & `FlexGet-3.8.0/flexget/plugins/filter/content_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/content_size.py` & `FlexGet-3.8.0/flexget/plugins/filter/content_size.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,67 @@
 from sys import maxsize
+from typing import Tuple
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.event import event
 from flexget.utils.log import log_once
+from flexget.utils.tools import format_filesize, parse_filesize
 
 logger = logger.bind(name='content_size')
 
 
 class FilterContentSize:
     schema = {
         'type': 'object',
         'properties': {
-            'min': {'type': 'number'},
-            'max': {'type': 'number'},
+            'min': {'type': ['number', 'string'], 'format': 'size'},
+            'max': {'type': ['number', 'string'], 'format': 'size'},
             'strict': {'type': 'boolean', 'default': True},
         },
         'additionalProperties': False,
     }
 
+    @staticmethod
+    def process_config(config: dict) -> Tuple[int, int]:
+        min_size = config.get('min', 0)
+        if isinstance(min_size, (int, float)):
+            min_size = min_size * 1024**2
+        else:
+            min_size = parse_filesize(min_size)
+        max_size = maxsize
+        if config.get('max'):
+            max_size = config['max']
+            if isinstance(max_size, (int, float)):
+                max_size = max_size * 1024**2
+            else:
+                max_size = parse_filesize(max_size)
+        return min_size, max_size
+
     def process_entry(self, task, entry, config, remember=True):
         """Rejects this entry if it does not pass content_size requirements. Returns true if the entry was rejected."""
         if 'content_size' in entry:
+            min_size, max_size = self.process_config(config)
             size = entry['content_size']
-            logger.debug('{} size {} MB', entry['title'], size)
+            logger.debug('{} size {}', entry['title'], format_filesize(size))
             # Avoid confusion by printing a reject message to info log, as
             # download plugin has already printed a downloading message.
-            if size < config.get('min', 0):
+            if size < min_size:
                 log_once('Entry `%s` too small, rejecting' % entry['title'], logger)
                 entry.reject(
-                    'minimum size {} MB, got {} MB'.format(config['min'], size), remember=remember
+                    f'minimum size {format_filesize(min_size)}, got {format_filesize(size)}',
+                    remember=remember,
                 )
                 return True
-            if size > config.get('max', maxsize):
+            if size > max_size:
                 log_once('Entry `%s` too big, rejecting' % entry['title'], logger)
                 entry.reject(
-                    'maximum size {} MB, got {} MB'.format(config['max'], size), remember=remember
+                    f'maximum size {format_filesize(max_size)}, got {format_filesize(size)}',
+                    remember=remember,
                 )
                 return True
 
     @plugin.priority(130)
     def on_task_filter(self, task, config):
         # Do processing on filter phase in case input plugin provided the size
         for entry in task.entries:
```

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/crossmatch.py` & `FlexGet-3.8.0/flexget/plugins/filter/crossmatch.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/delay.py` & `FlexGet-3.8.0/flexget/plugins/filter/delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/duplicates.py` & `FlexGet-3.8.0/flexget/plugins/filter/duplicates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/exists.py` & `FlexGet-3.8.0/flexget/plugins/filter/exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/exists_movie.py` & `FlexGet-3.8.0/flexget/plugins/filter/exists_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/exists_series.py` & `FlexGet-3.8.0/flexget/plugins/filter/exists_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/if_condition.py` & `FlexGet-3.8.0/flexget/plugins/filter/if_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 break
         else:
             raise AttributeError(item)
 
         def handle_phase(task, config):
             entry_actions = {'accept': Entry.accept, 'reject': Entry.reject, 'fail': Entry.fail}
             for item in config:
-                requirement, action = list(item.items())[0]
+                requirement, action = next(iter(item.items()))
                 passed_entries = (e for e in task.entries if self.check_condition(requirement, e))
                 if isinstance(action, str):
                     if not phase == 'filter':
                         continue
                     # Simple entry action (accept, reject or fail) was specified as a string
                     for entry in passed_entries:
                         entry_actions[action](entry, 'Matched requirement: %s' % requirement)
```

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/limit_new.py` & `FlexGet-3.8.0/flexget/plugins/filter/limit_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/magnets.py` & `FlexGet-3.8.0/flexget/plugins/filter/magnets.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/only_new.py` & `FlexGet-3.8.0/flexget/plugins/filter/only_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/proper_movies.py` & `FlexGet-3.8.0/flexget/plugins/filter/proper_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/quality.py` & `FlexGet-3.8.0/flexget/plugins/filter/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/regexp.py` & `FlexGet-3.8.0/flexget/plugins/filter/regexp.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         for operation, regexps in config.items():
             if operation in ['rest', 'from']:
                 continue
             for regexp_item in regexps:
                 if not isinstance(regexp_item, dict):
                     regexp = regexp_item
                     regexp_item = {regexp: {}}
-                regexp, opts = list(regexp_item.items())[0]
+                regexp, opts = next(iter(regexp_item.items()))
                 # Parse custom settings for this regexp
                 if not isinstance(opts, dict):
                     opts = {'path': opts}
                 else:
                     # We don't want to modify original config
                     opts = opts.copy()
                 # advanced configuration
@@ -205,15 +205,15 @@
         """
         matched = set()
         method = Entry.accept if 'accept' in operation else Entry.reject
         match_mode = 'excluding' not in operation
         for entry in entries:
             logger.trace('testing {} regexps to {}', len(regexps), entry['title'])
             for regexp_opts in regexps:
-                regexp, opts = list(regexp_opts.items())[0]
+                regexp, opts = next(iter(regexp_opts.items()))
 
                 # check if entry matches given regexp configuration
                 field = self.matches(entry, regexp, opts.get('from'), opts.get('not'))
 
                 # Run if we are in match mode and have a hit, or are in non-match mode and don't have a hit
                 if match_mode == bool(field):
                     # Creates the string with the reason for the hit
```

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/require_field.py` & `FlexGet-3.8.0/flexget/plugins/filter/require_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/rottentomatoes.py` & `FlexGet-3.8.0/flexget/plugins/filter/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/thetvdb.py` & `FlexGet-3.8.0/flexget/plugins/filter/thetvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/timeframe.py` & `FlexGet-3.8.0/flexget/plugins/filter/timeframe.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/unique.py` & `FlexGet-3.8.0/flexget/plugins/filter/unique.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/filter/upgrade.py` & `FlexGet-3.8.0/flexget/plugins/filter/upgrade.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/generic/cron_env.py` & `FlexGet-3.8.0/flexget/plugins/generic/cron_env.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/generic/db_vacuum.py` & `FlexGet-3.8.0/flexget/plugins/generic/db_vacuum.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/generic/log_start.py` & `FlexGet-3.8.0/flexget/plugins/generic/log_start.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/generic/urlfix.py` & `FlexGet-3.8.0/flexget/plugins/generic/urlfix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/generic/welcome.py` & `FlexGet-3.8.0/flexget/plugins/generic/welcome.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/anidb_list.py` & `FlexGet-3.8.0/flexget/plugins/input/anidb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/anilist.py` & `FlexGet-3.8.0/flexget/plugins/input/anilist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/apple_trailers.py` & `FlexGet-3.8.0/flexget/plugins/input/apple_trailers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/betaseries_list.py` & `FlexGet-3.8.0/flexget/plugins/input/betaseries_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/discover.py` & `FlexGet-3.8.0/flexget/plugins/input/discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,15 @@
 
     def __init__(self, title, task):
         self.title = title
         self.task = task
         self.last_execution = None
 
     def __str__(self):
-        return '<DiscoverEntry(title={},task={},added={})>'.format(
-            self.title,
-            self.task,
-            self.last_execution,
-        )
+        return f'<DiscoverEntry(title={self.title},task={self.task},added={self.last_execution})>'
 
 
 Index('ix_discover_entry_title_task', DiscoverEntry.title, DiscoverEntry.task)
 
 
 @event('manager.db_cleanup')
 def db_cleanup(manager, session):
@@ -114,15 +110,15 @@
         """
 
         result = []
         for index, entry in enumerate(entries):
             entry_results = []
             for item in config['from']:
                 if isinstance(item, dict):
-                    plugin_name, plugin_config = list(item.items())[0]
+                    plugin_name, plugin_config = next(iter(item.items()))
                 else:
                     plugin_name, plugin_config = item, None
                 search = plugin.get(plugin_name, self)
                 if not callable(search.search):
                     logger.critical(
                         'Search plugin {} does not implement search method', plugin_name
                     )
```

### Comparing `FlexGet-3.7.9/flexget/plugins/input/filesystem.py` & `FlexGet-3.8.0/flexget/plugins/input/filesystem.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/filmweb_watchlist.py` & `FlexGet-3.8.0/flexget/plugins/input/filmweb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/from_piratebay.py` & `FlexGet-3.8.0/flexget/plugins/input/from_piratebay.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         entry['title'] = json_result['name']
         entry['torrent_seeds'] = int(json_result['seeders'])
         entry['torrent_leeches'] = int(json_result['leechers'])
         entry['torrent_timestamp'] = int(json_result['added'])  # custom field for sorting by date
         entry['torrent_availability'] = torrent_availability(
             entry['torrent_seeds'], entry['torrent_leeches']
         )
-        entry['content_size'] = int(round(int(json_result['size']) / (1024 * 1024)))
+        entry['content_size'] = int(json_result['size'])
         entry['torrent_info_hash'] = json_result['info_hash']
         entry['url'] = self.info_hash_to_magnet(json_result['info_hash'], json_result['name'])
         return entry
 
 
 @event('plugin.register')
 def register_plugin():
```

### Comparing `FlexGet-3.7.9/flexget/plugins/input/from_task.py` & `FlexGet-3.8.0/flexget/plugins/input/from_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/from_telegram.py` & `FlexGet-3.8.0/flexget/plugins/input/from_telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/gazelle.py` & `FlexGet-3.8.0/flexget/plugins/input/gazelle.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/generate.py` & `FlexGet-3.8.0/flexget/plugins/input/generate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/html.py` & `FlexGet-3.8.0/flexget/plugins/input/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/input_csv.py` & `FlexGet-3.8.0/flexget/plugins/input/input_csv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/inputs.py` & `FlexGet-3.8.0/flexget/plugins/input/inputs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/json.py` & `FlexGet-3.8.0/flexget/plugins/input/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/kitsu.py` & `FlexGet-3.8.0/flexget/plugins/input/kitsu.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,17 +49,15 @@
         'oneOf': [{'required': ['username']}, {'required': ['user_id']}],
         'additionalProperties': False,
     }
 
     @cached('kitsu', persist='2 hours')
     def on_task_input(self, task, config):
         user_id = self._resolve_user_id(task, config)
-        next_url = 'https://kitsu.io/api/edge/users/{user_id}/library-entries'.format(
-            user_id=user_id
-        )
+        next_url = f'https://kitsu.io/api/edge/users/{user_id}/library-entries'
 
         payload = {
             'filter[status]': ','.join(config['lists']),
             'filter[kind]': 'anime',
             'include': 'anime',
             'fields[anime]': 'canonicalTitle,titles,endDate,subtype',
             'fields[libraryEntries]': 'anime',
@@ -123,17 +121,15 @@
                     yield entry
 
             next_url = json_data['links'].get('next')
             if next_url:
                 try:
                     response = task.requests.get(next_url)
                 except RequestException as e:
-                    error_message = 'Error getting list from next page url: {url}'.format(
-                        url=e.request.url
-                    )
+                    error_message = f'Error getting list from next page url: {e.request.url}'
                     if hasattr(e, 'response'):
                         error_message += f' status: {e.response.status_code}'
                     logger.opt(exception=True).debug(error_message)
                     raise plugin.PluginError(error_message)
                 json_data = response.json()
             else:
                 break
```

### Comparing `FlexGet-3.7.9/flexget/plugins/input/letterboxd.py` & `FlexGet-3.8.0/flexget/plugins/input/letterboxd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/limit.py` & `FlexGet-3.8.0/flexget/plugins/input/limit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/medusa.py` & `FlexGet-3.8.0/flexget/plugins/input/medusa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/mock.py` & `FlexGet-3.8.0/flexget/plugins/input/mock.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/my_anime_list.py` & `FlexGet-3.8.0/flexget/plugins/input/my_anime_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/myepisodes_list.py` & `FlexGet-3.8.0/flexget/plugins/input/myepisodes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/next_sonarr_episodes.py` & `FlexGet-3.8.0/flexget/plugins/input/next_sonarr_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/npo_watchlist.py` & `FlexGet-3.8.0/flexget/plugins/input/npo_watchlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,16 @@
 
         headers = {
             'Origin': 'https://www.npostart.nl',
             'X-XSRF-TOKEN': requests.cookies['XSRF-TOKEN'],
             'X-Requested-With': 'XMLHttpRequest',
         }
         if page > 1:
-            headers['Referer'] = episode_tiles_url.format(mediaId) + '?page={}'.format(
-                page - 1
+            headers['Referer'] = (
+                episode_tiles_url.format(mediaId) + f'?page={page - 1}'
             )  # referer from prev page
 
         logger.debug(
             'Retrieving episodes page {} for {} ({})', page, series_info['npo_name'], mediaId
         )
         try:
             episodes = requests.get(
```

### Comparing `FlexGet-3.7.9/flexget/plugins/input/parameterize.py` & `FlexGet-3.8.0/flexget/plugins/input/parameterize.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/plex.py` & `FlexGet-3.8.0/flexget/plugins/input/plex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/pogcal.py` & `FlexGet-3.8.0/flexget/plugins/input/pogcal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/regexp_parse.py` & `FlexGet-3.8.0/flexget/plugins/input/regexp_parse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/rlslog.py` & `FlexGet-3.8.0/flexget/plugins/input/rlslog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/rottentomatoes_list.py` & `FlexGet-3.8.0/flexget/plugins/input/rottentomatoes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/rss.py` & `FlexGet-3.8.0/flexget/plugins/input/rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         config['title'] = fp_field_name(config['title'])
         if config.get('other_fields'):
             other_fields = []
             for item in config['other_fields']:
                 if isinstance(item, str):
                     key, val = item, item
                 else:
-                    key, val = list(item.items())[0]
+                    key, val = next(iter(item.items()))
                 other_fields.append({fp_field_name(key): val.lower()})
             config['other_fields'] = other_fields
         # set default value for group_links as deactivated
         config.setdefault('group_links', False)
         # set default for all_entries
         config.setdefault('all_entries', True)
         return config
```

### Comparing `FlexGet-3.7.9/flexget/plugins/input/sceper.py` & `FlexGet-3.8.0/flexget/plugins/input/sceper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/sickbeard.py` & `FlexGet-3.8.0/flexget/plugins/input/sickbeard.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/tail.py` & `FlexGet-3.8.0/flexget/plugins/input/tail.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/text.py` & `FlexGet-3.8.0/flexget/plugins/input/text.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/input/torznab.py` & `FlexGet-3.8.0/flexget/plugins/input/torznab.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                 logger.warning(
                     "Item '{}' does not contain a bittorent enclosure.", item.title.string
                 )
                 continue
             else:
                 entry['url'] = enclosure.attrib['url']
                 try:
-                    entry['content_size'] = int(enclosure.attrib['length']) // (2**20)
+                    entry['content_size'] = int(enclosure.attrib['length'])
                 except ValueError:
                     entry['content_size'] = 0
                 entry['type'] = enclosure.attrib['type']
 
             ns = {'torznab': 'http://torznab.com/schemas/2015/feed'}
             self._parse_torznab_attrs(entry, item.findall('torznab:attr', ns))
 
@@ -237,15 +237,15 @@
         if 'peers' in misc.keys():
             if 'torrent_leeches' not in entry.keys() and 'torrent_seeds' in entry.keys():
                 entry['torrent_leeches'] = misc['peers'] - entry['torrent_seeds']
             if 'torrent_leeches' in entry.keys() and 'torrent_seeds' not in entry.keys():
                 entry['torrent_seeds'] = misc['peers'] - entry['torrent_leeches']
 
         if 'content_size' not in entry.keys() and 'size' in misc.keys():
-            entry['content_size'] = misc['size'] // (2**20)
+            entry['content_size'] = misc['size']
 
         if 'torrent_seeds' in entry.keys() and 'torrent_leeches' in entry.keys():
             entry['torrent_availability'] = torrent_availability(
                 entry['torrent_seeds'], entry['torrent_leeches']
             )
 
     def _convert_query_parameters(self, entry, fields):
```

### Comparing `FlexGet-3.7.9/flexget/plugins/input/twitterfeed.py` & `FlexGet-3.8.0/flexget/plugins/input/twitterfeed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/internal/api_bluray.py` & `FlexGet-3.8.0/flexget/plugins/internal/api_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/internal/api_rottentomatoes.py` & `FlexGet-3.8.0/flexget/plugins/internal/api_rottentomatoes.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,17 +152,15 @@
         if self.year:
             age = datetime.now().year - self.year
             refresh_interval += age * 5
             logger.debug('movie `{}` age {} expires in {} days', self.title, age, refresh_interval)
         return self.updated < datetime.now() - timedelta(days=refresh_interval)
 
     def __repr__(self) -> str:
-        return '<RottenTomatoesMovie(title={},id={},year={})>'.format(
-            self.title, self.id, self.year
-        )
+        return f'<RottenTomatoesMovie(title={self.title},id={self.id},year={self.year})>'
 
 
 class RottenTomatoesGenre(Base):
     __tablename__ = 'rottentomatoes_genres'
 
     id = Column(Integer, primary_key=True)
     name = Column(String)
```

### Comparing `FlexGet-3.7.9/flexget/plugins/internal/change_warn.py` & `FlexGet-3.8.0/flexget/plugins/internal/change_warn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/assume_quality.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/assume_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/bluray_lookup.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/bluray_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/content_size.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/content_size.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import math
 import os.path
 import re
 from pathlib import Path
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.event import event
+from flexget.utils.tools import format_filesize, parse_filesize
 
 logger = logger.bind(name='metanfo_csize')
 
-SIZE_RE = re.compile(r'Size[^\d]{0,7}(\d*\.?\d+).{0,5}(MB|GB)', re.IGNORECASE)
+SIZE_RE = re.compile(r'Size[^\d]{0,7}(\d*\.?\d+).{0,5}(MB|GB)', re.IGNORECASE | re.UNICODE)
 
 
 class MetainfoContentSize:
     """
     Utility:
 
     Check if content size is mentioned in description and set content_size attribute for entries if it is.
@@ -34,46 +34,33 @@
                 # Don't override if already set
                 logger.trace(
                     'skipping content size check because it is already set for {!r}',
                     entry['title'],
                 )
                 continue
             # Try to parse size from description
-            match = False
             description = entry.get('description', '')
             if isinstance(description, str):
-                match = SIZE_RE.search(description)
-            if match:
                 try:
-                    amount = float(match.group(1).replace(',', '.'))
-                except Exception:
-                    logger.error(
-                        'BUG: Unable to convert {} into float ({})', match.group(1), entry['title']
-                    )
+                    entry['content_size'] = parse_filesize(description, si=False, match_re=SIZE_RE)
                     continue
-                unit = match.group(2).lower()
-                count += 1
-                if unit == 'gb':
-                    amount = math.ceil(amount * 1024)
-                logger.trace('setting content size to {}', amount)
-                entry['content_size'] = int(amount)
-                continue
+                except ValueError:
+                    pass
             # If this entry has a local file, (it was added by filesystem plugin) grab the size.
-            elif entry.get('location'):
+            if entry.get('location'):
                 # If it is a .torrent or .nzb, don't bother getting the size as it will not be the content's size
                 location = entry['location']
                 if isinstance(location, str):
                     location = Path(location)
                 if location.suffix in ('.nzb', '.torrent'):
                     continue
                 try:
                     if location.is_file():
                         amount = os.path.getsize(entry['location'])
-                        amount = int(amount / (1024 * 1024))
-                        logger.trace('setting content size to {}', amount)
+                        logger.trace('setting content size to {}', format_filesize(amount))
                         entry['content_size'] = amount
                         continue
                 except OSError:
                     # is_file can throw OSError for invalid paths (at least on windows)
                     continue
 
         if count:
```

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/media_id.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/media_id.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/metainfo_movie.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/metainfo_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/nfo_lookup.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/nfo_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/nzb_size.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/nzb_size.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import mimetypes
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.event import event
+from flexget.utils.tools import format_filesize
 
 logger = logger.bind(name='nzb_size')
 
 # a bit hacky, add nzb as a known mimetype
 mimetypes.add_type('application/x-nzb', '.nzb')
 
 
@@ -52,17 +53,16 @@
                     continue
 
                 size = 0
                 for nzbfile in nzbfiles:
                     for segment in nzbfile.segments:
                         size += segment.bytes
 
-                size_mb = size / 1024 / 1024
-                logger.debug('{} content size: {} MB', entry['title'], size_mb)
-                entry['content_size'] = size_mb
+                logger.debug('{} content size: {}', entry['title'], format_filesize(size))
+                entry['content_size'] = size
             else:
                 logger.trace('{} does not seem to be nzb', entry['title'])
 
 
 @event('plugin.register')
 def register_plugin():
     plugin.register(NzbSize, 'nzb_size', api_ver=2, builtin=True)
```

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/quality.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/rottentomatoes_lookup.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/rottentomatoes_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/subtitles_check.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/subtitles_check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/metainfo/task.py` & `FlexGet-3.8.0/flexget/plugins/metainfo/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/extension.py` & `FlexGet-3.8.0/flexget/plugins/modify/extension.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/headers.py` & `FlexGet-3.8.0/flexget/plugins/modify/headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/manipulate.py` & `FlexGet-3.8.0/flexget/plugins/modify/manipulate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/path_by_ext.py` & `FlexGet-3.8.0/flexget/plugins/modify/path_by_ext.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/path_by_space.py` & `FlexGet-3.8.0/flexget/plugins/modify/path_by_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/plugin_priority.py` & `FlexGet-3.8.0/flexget/plugins/modify/plugin_priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/regex_extract.py` & `FlexGet-3.8.0/flexget/plugins/modify/regex_extract.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/reorder_quality.py` & `FlexGet-3.8.0/flexget/plugins/modify/reorder_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def __init__(self):
         self.quality_priorities = {}
 
     def on_task_start(self, task, config):
         self.quality_priorities = {}
         for quality, _config in config.items():
-            action, other_quality = list(_config.items())[0]
+            action, other_quality = next(iter(_config.items()))
 
             if quality not in qualities._registry:
                 raise plugin.PluginError('%s is not a valid quality' % quality)
 
             quality_component = qualities._registry[quality]
             other_quality_component = qualities._registry[other_quality]
```

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/set_field.py` & `FlexGet-3.8.0/flexget/plugins/modify/set_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/sort_by.py` & `FlexGet-3.8.0/flexget/plugins/modify/sort_by.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/modify/sort_by_weight.py` & `FlexGet-3.8.0/flexget/plugins/modify/sort_by_weight.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,20 +261,15 @@
         for arg in args:
             if isinstance(arg, timedelta):
                 short_args.append(arg.days)
             elif isinstance(arg, datetime):
                 date = arg.date()
                 short_args.append(f'{date.year}-{date.month}-{date.day}')
             elif isinstance(arg, Quality):
-                quality_string = '[ {} ]-{}-{}, [ {} ]'.format(
-                    arg.resolution,
-                    arg.source,
-                    arg.codec,
-                    arg.audio,
-                )
+                quality_string = f'[ {arg.resolution} ]-{arg.source}-{arg.codec}, [ {arg.audio} ]'
                 if quality_string not in short_args:
                     short_args.append(quality_string)
             else:
                 short_args.append(arg)
         entry['weights'][key] = f'{weight} = {short_args}'
```

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/cfscraper.py` & `FlexGet-3.8.0/flexget/plugins/operate/cfscraper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/cookies.py` & `FlexGet-3.8.0/flexget/plugins/operate/cookies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/debug_db_sessions.py` & `FlexGet-3.8.0/flexget/plugins/operate/debug_db_sessions.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,19 +79,15 @@
 def after_end(session, transaction):
     caller_info = find_caller(inspect.stack()[1:])
     with open_transactions_lock:
         if transaction not in open_transactions:
             # Transaction was created but a connection was never opened for it
             return
         open_time = time.time() - open_transactions[transaction][0]
-        msg = 'Transaction 0x{:08X} closed {} (open time {})'.format(
-            id(transaction),
-            caller_info,
-            open_time,
-        )
+        msg = f'Transaction 0x{id(transaction):08X} closed {caller_info} (open time {open_time})'
         if open_time > 2:
             logger.warning(msg)
         else:
             logger.debug(msg)
         del open_transactions[transaction]
```

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/debug_warnings.py` & `FlexGet-3.8.0/flexget/plugins/operate/debug_warnings.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/digest.py` & `FlexGet-3.8.0/flexget/plugins/operate/digest.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/disable.py` & `FlexGet-3.8.0/flexget/plugins/operate/disable.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/disable_phases.py` & `FlexGet-3.8.0/flexget/plugins/operate/disable_phases.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/domain_delay.py` & `FlexGet-3.8.0/flexget/plugins/operate/domain_delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/entry_trace.py` & `FlexGet-3.8.0/flexget/plugins/operate/entry_trace.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/formlogin.py` & `FlexGet-3.8.0/flexget/plugins/operate/formlogin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/free_space.py` & `FlexGet-3.8.0/flexget/plugins/operate/free_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/include.py` & `FlexGet-3.8.0/flexget/plugins/operate/include.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/interval.py` & `FlexGet-3.8.0/flexget/plugins/operate/interval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/log_filter.py` & `FlexGet-3.8.0/flexget/plugins/operate/log_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/manual.py` & `FlexGet-3.8.0/flexget/plugins/operate/manual.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/max_reruns.py` & `FlexGet-3.8.0/flexget/plugins/operate/max_reruns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/pathscrub.py` & `FlexGet-3.8.0/flexget/plugins/operate/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/priority.py` & `FlexGet-3.8.0/flexget/plugins/operate/priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/proxy.py` & `FlexGet-3.8.0/flexget/plugins/operate/proxy.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/rerun.py` & `FlexGet-3.8.0/flexget/plugins/operate/rerun.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/run_task.py` & `FlexGet-3.8.0/flexget/plugins/operate/run_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/sequence.py` & `FlexGet-3.8.0/flexget/plugins/operate/sequence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/sleep.py` & `FlexGet-3.8.0/flexget/plugins/operate/sleep.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/spy_headers.py` & `FlexGet-3.8.0/flexget/plugins/operate/spy_headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/template.py` & `FlexGet-3.8.0/flexget/plugins/operate/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/verbose.py` & `FlexGet-3.8.0/flexget/plugins/operate/verbose.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/verbose_details.py` & `FlexGet-3.8.0/flexget/plugins/operate/verbose_details.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/verify_ssl_certificates.py` & `FlexGet-3.8.0/flexget/plugins/operate/verify_ssl_certificates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/operate/version_checker.py` & `FlexGet-3.8.0/flexget/plugins/operate/version_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/download.py` & `FlexGet-3.8.0/flexget/plugins/output/download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/download_auth.py` & `FlexGet-3.8.0/flexget/plugins/output/download_auth.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/dump.py` & `FlexGet-3.8.0/flexget/plugins/output/dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from rich.highlighter import ReprHighlighter
 from rich.markup import escape
 from rich.pretty import Pretty, is_expandable
 
 from flexget import options, plugin
 from flexget.event import event
 from flexget.terminal import TerminalTable, console
+from flexget.utils.tools import format_filesize
 
 logger = logger.bind(name='dump')
 
 
 def dump(entries, debug=False, eval_lazy=False, trace=False, title_only=False):
     """
     Dump *entries* to stdout
@@ -61,14 +62,16 @@
                     value = entry[field]
                 except KeyError:
                     renderable = '[italic]<LazyField - lazy lookup failed>[/italic]'
                 else:
                     if field.rsplit('_', maxsplit=1)[-1] == 'url':
                         url = quote(value, safe=":/")
                         renderable = f'[link={url}][repr.url]{escape(value)}[/repr.url][/link]'
+                    elif field == 'content_size':
+                        renderable = highlighter(str(value)) + f' ({format_filesize(value)})'
                     elif isinstance(value, str):
                         renderable = escape(value.replace('\r', '').replace('\n', ''))
                     elif is_expandable(value):
                         renderable = Pretty(value)
                     else:
                         try:
                             renderable = highlighter(str(value))
```

### Comparing `FlexGet-3.7.9/flexget/plugins/output/dump_config.py` & `FlexGet-3.8.0/flexget/plugins/output/dump_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/exec.py` & `FlexGet-3.8.0/flexget/plugins/output/exec.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/file_operations.py` & `FlexGet-3.8.0/flexget/plugins/output/file_operations.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/html.py` & `FlexGet-3.8.0/flexget/plugins/output/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/memusage.py` & `FlexGet-3.8.0/flexget/plugins/output/memusage.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/mock_output.py` & `FlexGet-3.8.0/flexget/plugins/output/mock_output.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/rss.py` & `FlexGet-3.8.0/flexget/plugins/output/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/rtorrent_magnet.py` & `FlexGet-3.8.0/flexget/plugins/output/rtorrent_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/sabnzbd.py` & `FlexGet-3.8.0/flexget/plugins/output/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/sns.py` & `FlexGet-3.8.0/flexget/plugins/output/sns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/subtitles.py` & `FlexGet-3.8.0/flexget/plugins/output/subtitles.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/subtitles_periscope.py` & `FlexGet-3.8.0/flexget/plugins/output/subtitles_periscope.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/subtitles_subliminal.py` & `FlexGet-3.8.0/flexget/plugins/output/subtitles_subliminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/symlink.py` & `FlexGet-3.8.0/flexget/plugins/output/symlink.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/output/utorrent.py` & `FlexGet-3.8.0/flexget/plugins/output/utorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/services/kodi_library.py` & `FlexGet-3.8.0/flexget/plugins/services/kodi_library.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/services/myepisodes.py` & `FlexGet-3.8.0/flexget/plugins/services/myepisodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/plugins/services/pogcal_acquired.py` & `FlexGet-3.8.0/flexget/plugins/services/pogcal_acquired.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/resources/flexget.png` & `FlexGet-3.8.0/flexget/resources/flexget.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/task.py` & `FlexGet-3.8.0/flexget/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,18 +567,15 @@
             )
             logger.critical(msg)
             self.abort(msg)
         except PluginError as err:
             err.logger.critical(err.value)
             self.abort(err.value)
         except DependencyError as e:
-            msg = 'Plugin `{}` cannot be used because dependency `{}` is missing.'.format(
-                keyword,
-                e.missing,
-            )
+            msg = f'Plugin `{keyword}` cannot be used because dependency `{e.missing}` is missing.'
             logger.critical(e.message)
             self.abort(msg)
         except Warning as e:
             # If warnings have been elevated to errors
             msg = f'Warning during plugin {keyword}: {e}'
             logger.exception(msg)
             self.abort(msg)
```

### Comparing `FlexGet-3.7.9/flexget/task_queue.py` & `FlexGet-3.8.0/flexget/task_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class TaskQueue:
     """Task processing thread.
 
     Only executes one task at a time, if more are requested they are queued up and run in turn.
     """
 
     def __init__(self) -> None:
-        self.run_queue: 'queue.PriorityQueue[Task]' = queue.PriorityQueue()
+        self.run_queue: queue.PriorityQueue[Task] = queue.PriorityQueue()
         self._shutdown_now = False
         self._shutdown_when_finished = False
 
         self.current_task: Optional[Task] = None
         self._thread = None
 
     def start(self) -> None:
```

### Comparing `FlexGet-3.7.9/flexget/templates/task/default.template` & `FlexGet-3.8.0/flexget/templates/task/default.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/templates/task/html.template` & `FlexGet-3.8.0/flexget/templates/task/html.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/templates/task/rss.template` & `FlexGet-3.8.0/flexget/templates/task/rss.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/terminal.py` & `FlexGet-3.8.0/flexget/terminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/tray_icon.py` & `FlexGet-3.8.0/flexget/tray_icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 class TrayIcon:
     def __init__(self, path_to_image: Path = image_path):
         # Silence PIL noisy logging
         logging.getLogger('PIL.PngImagePlugin').setLevel(logging.INFO)
         logging.getLogger('PIL.Image').setLevel(logging.INFO)
 
         self.path_to_image: Path = path_to_image
-        self.icon: Optional['Icon'] = None
-        self._menu: Optional['Menu'] = None
-        self.menu_items: List['MenuItem'] = []
+        self.icon: Optional[Icon] = None
+        self._menu: Optional[Menu] = None
+        self.menu_items: List[MenuItem] = []
 
         self.active: bool = _import_success
         self.running: bool = False
 
         self.add_core_menu_items()
 
     @check_if_tray_is_active
```

### Comparing `FlexGet-3.7.9/flexget/ui/v1/__init__.py` & `FlexGet-3.8.0/flexget/ui/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/app.html` & `FlexGet-3.8.0/flexget/ui/v1/app/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/assets/images/header.png` & `FlexGet-3.8.0/flexget/ui/v1/app/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/favicon.ico` & `FlexGet-3.8.0/flexget/ui/v1/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/FontAwesome.otf` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.eot` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.svg` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.eot` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.svg` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.ttf` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.woff` & `FlexGet-3.8.0/flexget/ui/v1/app/fonts/ui-grid.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/scripts/app.js` & `FlexGet-3.8.0/flexget/ui/v1/app/scripts/app.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/scripts/splash.js` & `FlexGet-3.8.0/flexget/ui/v1/app/scripts/splash.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/scripts/vendor.js` & `FlexGet-3.8.0/flexget/ui/v1/app/scripts/vendor.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/styles/app.css` & `FlexGet-3.8.0/flexget/ui/v1/app/styles/app.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/styles/splash.css` & `FlexGet-3.8.0/flexget/ui/v1/app/styles/splash.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/app/styles/vendor.css` & `FlexGet-3.8.0/flexget/ui/v1/app/styles/vendor.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/bower.json` & `FlexGet-3.8.0/flexget/ui/v1/bower.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/build.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/build.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/inject.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/inject.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/lint.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/lint.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/proxy.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/proxy.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/server.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/server.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/styles.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/styles.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/test.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/test.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/gulp/watch.js` & `FlexGet-3.8.0/flexget/ui/v1/gulp/watch.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/karma.conf.js` & `FlexGet-3.8.0/flexget/ui/v1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/package.json` & `FlexGet-3.8.0/flexget/ui/v1/package.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/specs.html` & `FlexGet-3.8.0/flexget/ui/v1/specs.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/app.html` & `FlexGet-3.8.0/flexget/ui/v1/src/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/app.module.js` & `FlexGet-3.8.0/flexget/ui/v1/src/app.module.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/app.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/app.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/assets/images/header.png` & `FlexGet-3.8.0/flexget/ui/v1/src/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/error/error.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/exception/exception.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/exception/exception.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/_pagination.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/pagination.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.provider.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/router/router-helper.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/components/404/404.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.config.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/auth.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/components/auth/login.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.config.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.provider.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/core/core.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.config.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/components/database/database.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/components/home/home.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/_sidenav.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/_sidenav.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.semver.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.semver.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.provider.js` & `FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/construction.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/construction.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js` & `FlexGet-3.8.0/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/favicon.ico` & `FlexGet-3.8.0/flexget/ui/v1/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/config/config.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.filter.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/execute/execute.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/history/history.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/log/log.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/pending/pending.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/seen/seen.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.spec.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/series/series.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/loading-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.config.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/server.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/server/server.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.component.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.route.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.tmpl.html` & `FlexGet-3.8.0/flexget/ui/v1/src/plugins/status/status.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/scss/_header.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/scss/flexget.scss` & `FlexGet-3.8.0/flexget/ui/v1/src/scss/flexget.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/src/services/schema.service.js` & `FlexGet-3.8.0/flexget/ui/v1/src/services/schema.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/config.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/execute.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/execute.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/history.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/history.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/movie_list.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/movie_list.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/seen.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/seen.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/series.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/series.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/states.js` & `FlexGet-3.8.0/flexget/ui/v1/tests-mock-data/states.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/__init__.py` & `FlexGet-3.8.0/flexget/ui/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map` & `FlexGet-3.8.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/ui/v2/dist/index.html` & `FlexGet-3.8.0/flexget/ui/v2/dist/index.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/bittorrent.py` & `FlexGet-3.8.0/flexget/utils/bittorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/cache.py` & `FlexGet-3.8.0/flexget/utils/cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/cached_input.py` & `FlexGet-3.8.0/flexget/utils/cached_input.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/database.py` & `FlexGet-3.8.0/flexget/utils/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/json.py` & `FlexGet-3.8.0/flexget/utils/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/lazy_dict.py` & `FlexGet-3.8.0/flexget/utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/log.py` & `FlexGet-3.8.0/flexget/utils/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/parsers/generic.py` & `FlexGet-3.8.0/flexget/utils/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/parsers/movie.py` & `FlexGet-3.8.0/flexget/utils/parsers/movie.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,15 @@
         self.name = None
         self.year = None
         self.year_pos = None
         self.quality = qualities.Quality()
         self.proper_count = 0
 
     def __str__(self):
-        return "<MovieParser(name={},year={},quality={})>".format(
-            self.name, self.year, self.quality
-        )
+        return f"<MovieParser(name={self.name},year={self.year},quality={self.quality})>"
 
     def parse(self, data=None):
         """Parse movie name. Populates name, year, quality and proper_count attributes"""
 
         # Reset before parsing, so the parser can be reused.
         self.reset()
```

### Comparing `FlexGet-3.7.9/flexget/utils/parsers/parser.py` & `FlexGet-3.8.0/flexget/utils/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/parsers/series.py` & `FlexGet-3.8.0/flexget/utils/parsers/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,15 @@
     date_regexps = ReList(
         [
             TitleParser.re_not_in_word(regexp)
             for regexp in [
                 fr'(\d{{2,4}}){separators}(\d{{1,2}}){separators}(\d{{1,2}})',
                 fr'(\d{{1,2}}){separators}(\d{{1,2}}){separators}(\d{{2,4}})',
                 r'(\d{4})x(\d{1,2})%s(\d{1,2})' % separators,
-                r'(\d{{1,2}})(?:st|nd|rd|th)?{}([a-z]{{3,10}}){}(\d{{4}})'.format(
-                    separators, separators
-                ),
+                fr'(\d{{1,2}})(?:st|nd|rd|th)?{separators}([a-z]{{3,10}}){separators}(\d{{4}})',
             ]
         ]
     )
     sequence_regexps = ReList(
         [
             TitleParser.re_not_in_word(regexp)
             for regexp in [
```

### Comparing `FlexGet-3.7.9/flexget/utils/pathscrub.py` & `FlexGet-3.8.0/flexget/utils/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/qualities.py` & `FlexGet-3.8.0/flexget/utils/qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/requests.py` & `FlexGet-3.8.0/flexget/utils/requests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/serialization.py` & `FlexGet-3.8.0/flexget/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/simple_persistence.py` & `FlexGet-3.8.0/flexget/utils/simple_persistence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/sqlalchemy_utils.py` & `FlexGet-3.8.0/flexget/utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/flexget/utils/template.py` & `FlexGet-3.8.0/flexget/utils/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 )
 from jinja2.nativetypes import NativeTemplate
 from loguru import logger
 
 from flexget.event import event
 from flexget.utils.lazy_dict import LazyDict
 from flexget.utils.pathscrub import pathscrub
-from flexget.utils.tools import split_title_year
+from flexget.utils.tools import parse_filesize, split_title_year
 
 if TYPE_CHECKING:
     from flexget.entry import Entry
     from flexget.manager import Manager
     from flexget.task import Task
 
 logger = logger.bind(name='utils.template')
@@ -183,49 +183,23 @@
     return split_title_year(name).title
 
 
 def filter_get_year(name: str) -> str:
     return split_title_year(name).year
 
 
-def filter_parse_size(
-    val: str, match_re: Optional[str] = None, si: bool = False, case: bool = True
-) -> int:
+def filter_parse_size(val: str, si: bool = False, match_re: Optional[str] = None) -> int:
     """Parse human-readable file size to bytes"""
     if not isinstance(val, str):
         return val
 
-    base = 1000 if si else 1024
-    size_map = {
-        'B': 1,
-        'KB': base,
-        'MB': base**2,
-        'GB': base**3,
-        'TB': base**4,
-        'PB': base**5,
-        'EB': base**6,
-        'KiB': 1024,
-        'MiB': 1024**2,
-        'GiB': 1024**3,
-        'TiB': 1024**4,
-        'PiB': 1024**5,
-        'EiB': 1024**6,
-    }
-    size_map = {k.casefold(): v for k, v in size_map.items()}
-
-    match_re = match_re or r'(?P<digit>\d+(?:\.\d+)?)\s*(?P<unit>[KMGTPE]?i?B)'
-    matched_size = re.search(match_re, val, flags=0 if case else re.IGNORECASE)
-
-    if matched_size:
-        unit = matched_size['unit'].casefold()
-        unit_base = size_map.get(unit)
-        if unit_base is not None:
-            size = float(matched_size['digit'])
-            return int(size * unit_base)
-    return 0
+    try:
+        return parse_filesize(val, si=si, match_re=match_re)
+    except ValueError:
+        return 0
 
 
 def is_fs_file(pathname: Union[str, os.PathLike]) -> bool:
     """Test whether item is existing file in filesystem"""
     return os.path.isfile(pathname)
```

### Comparing `FlexGet-3.7.9/flexget/utils/tools.py` & `FlexGet-3.8.0/flexget/utils/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import hashlib
 import locale
 import operator
 import queue
 import re
 import sys
 import weakref
-from collections import OrderedDict, defaultdict
+from collections import defaultdict
 from collections.abc import MutableMapping
 from datetime import datetime, timedelta
 from html.entities import name2codepoint
 from pprint import pformat
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -48,32 +48,14 @@
 def str_to_int(string: str) -> Optional[int]:
     try:
         return int(string.replace(',', ''))
     except ValueError:
         return None
 
 
-def convert_bytes(bytes_num: Union[int, float]) -> str:
-    """Returns given bytes as prettified string."""
-
-    bytes_num = float(bytes_num)
-    units_prefixes = OrderedDict(
-        {
-            'T': 1099511627776,  # 1024 ** 4
-            'G': 1073741824,  # 1024 ** 3
-            'M': 1048576,  # 1024 ** 2
-            'K': 1024,
-        }
-    )
-    for unit, threshold in units_prefixes.items():
-        if bytes_num > threshold:
-            return f'{bytes_num/threshold:.2f}{unit}'
-    return f'{bytes_num:.2f}b'
-
-
 class MergeException(Exception):
     def __init__(self, value: str):
         self.value = value
 
     def __str__(self) -> str:
         return repr(self.value)
 
@@ -361,29 +343,32 @@
         return None
 
 
 def get_current_flexget_version() -> str:
     return flexget.__version__
 
 
-def parse_filesize(text_size: str, si: bool = True) -> float:
+def parse_filesize(
+    text_size: str, si: bool = True, match_re: Optional[Union[str, Pattern[str]]] = None
+) -> int:
     """
-    Parses a data size and returns its value in mebibytes
+    Parses a data size and returns its value in bytes
 
     :param string text_size: string containing the data size to parse i.e. "5 GB"
     :param bool si: If True, possibly ambiguous units like KB, MB, GB will be assumed to be base 10 units,
-    rather than the default base 2. i.e. if si then 50 GB = 47684 else 50GB = 51200
+      rather than base 2. i.e. if si then 1 KB = 1000 B else 1 KB = 1024 B
+    :param match_re: A custom regex can be defined to match the size. The first capture group should match
+      the number, and the second should match the unit.
 
-    :returns: an float with the data size in mebibytes
+    :returns: an int with the data size in bytes
     """
     prefix_order = {'': 0, 'k': 1, 'm': 2, 'g': 3, 't': 4, 'p': 5}
 
-    parsed_size = re.match(
-        r'(\d+(?:[.,\s]\d+)*)(?:\s*)((?:[ptgmk]i?)?b)', text_size.strip().lower(), flags=re.UNICODE
-    )
+    match_re = match_re or r'\b(\d+(?:[.,\s]\d+)*)\s*((?:[ptgmk]i?)?b)\b'
+    parsed_size = re.search(match_re, text_size.lower())
     if not parsed_size:
         raise ValueError('%s does not look like a file size' % text_size)
     amount_str = parsed_size.group(1)
     unit = parsed_size.group(2)
     if not unit.endswith('b'):
         raise ValueError('%s does not look like a file size' % text_size)
     unit = unit.rstrip('b')
@@ -391,15 +376,38 @@
         si = False
         unit = unit.rstrip('i')
     if unit not in prefix_order:
         raise ValueError('%s does not look like a file size' % text_size)
     order = prefix_order[unit]
     amount = float(amount_str.replace(',', '').replace(' ', ''))
     base = 1000 if si else 1024
-    return (amount * (base**order)) / 1024**2
+    return int(amount * (base**order))
+
+
+def format_filesize(num_bytes: Union[int, float], si: bool = False) -> str:
+    """Returns given bytes as prettified string."""
+
+    base = 1000 if si else 1024
+    amount = float(num_bytes)
+    prefix = ''
+    unit_prefixes = [
+        # For some reason the convention is to use lowercase k for si kilobytes
+        'k' if si else 'K',
+        'M',
+        'G',
+        'T',
+        'P',
+    ]
+    for unit in unit_prefixes:
+        if amount >= base:
+            amount /= base
+            prefix = f'{unit}{"" if si else "i"}'
+        else:
+            break
+    return f'{round(amount, 2)} {prefix}B'
 
 
 def get_config_hash(config: Any) -> str:
     """
     :param dict config: Configuration
     :return: MD5 hash for *config*
     """
```

### Comparing `FlexGet-3.7.9/flexget/webserver.py` & `FlexGet-3.8.0/flexget/webserver.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/pyproject.toml` & `FlexGet-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.9/requirements-docker.txt` & `FlexGet-3.8.0/requirements-docker.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
 flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
 flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
 flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
-greenlet==2.0.1 ; python_version >= "3.7" and python_version < "4.0" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")
+greenlet==2.0.1 ; python_version >= "3.7" and python_version < "4.0" and (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64")
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
+importlib-metadata==6.7.0 ; python_version >= "3.7" and python_version < "3.10"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-functools==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
@@ -56,30 +56,30 @@
 pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
 pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 python-telegram-bot==12.8 ; python_version >= "3.7" and python_version < "4.0"
 pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
-pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
+pyyaml==6.0.1 ; python_version >= "3.7" and python_version < "4.0"
 qbittorrent-api==2023.3.44 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
 sqlalchemy==2.0.15 ; python_version >= "3.7" and python_version < "4.0"
 tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
 tornado==6.2 ; python_version >= "3.7" and python_version < "4.0"
 transmission-rpc==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
-typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
+typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "4.0"
 tzdata==2022.7 ; python_version >= "3.7" and python_version < "4.0"
 tzlocal==4.2 ; python_version >= "3.7" and python_version < "4.0"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
 win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.7.9/requirements-release.txt` & `FlexGet-3.8.0/requirements-release.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and (os_name == "nt" or platform_system == "Windows")
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
 cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "4.0"
+importlib-metadata==6.7.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jeepney==0.8.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 keyring==23.11.0 ; python_version >= "3.7" and python_version < "4.0"
 more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
 packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
 pep517==0.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pkginfo==1.9.2 ; python_version >= "3.7" and python_version < "4.0"
@@ -25,11 +25,11 @@
 requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 rfc3986==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 secretstorage==3.3.3 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.7" and python_version < "3.11"
 twine==4.0.2 ; python_version >= "3.7" and python_version < "4.0"
-typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "3.9"
+typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "3.9"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.7.9/requirements.txt` & `FlexGet-3.8.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
 flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
 flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
 flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
-greenlet==2.0.1 ; python_version >= "3.7" and python_version < "4.0" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")
+greenlet==2.0.1 ; python_version >= "3.7" and python_version < "4.0" and (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64")
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
+importlib-metadata==6.7.0 ; python_version >= "3.7" and python_version < "3.10"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-functools==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
@@ -49,26 +49,26 @@
 pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
 pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
 pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
-pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
+pyyaml==6.0.1 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
 sqlalchemy==2.0.15 ; python_version >= "3.7" and python_version < "4.0"
 tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
-typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
+typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "4.0"
 tzdata==2022.7 ; python_version >= "3.7" and python_version < "4.0"
 tzlocal==4.2 ; python_version >= "3.7" and python_version < "4.0"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
 win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
```

