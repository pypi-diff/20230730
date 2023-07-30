# Comparing `tmp/feeluown-3.8.8.tar.gz` & `tmp/feeluown-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/feeluown-3.8.8.tar", last modified: Tue Aug  9 12:31:40 2022, max compression
+gzip compressed data, was "feeluown-3.8.9.tar", last modified: Sun Dec 18 02:05:11 2022, max compression
```

## Comparing `feeluown-3.8.8.tar` & `feeluown-3.8.9.tar`

### file list

```diff
@@ -1,255 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-08-09 12:31:40.000000 feeluown-3.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    49557 2022-08-09 12:31:37.000000 feeluown-3.8.8/mpv_old.py
--rw-r--r--   0 runner    (1001) docker     (121)    79466 2022-08-09 12:31:37.000000 feeluown-3.8.8/mpv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-08-09 12:31:40.000000 feeluown-3.8.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/nowplaying/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/nowplaying/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/nowplaying/linux/
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/nowplaying/linux/introspect.xml
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/nowplaying/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8578 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/nowplaying/linux/mpris2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5027 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/nowplaying/global_hotkey_mac.py
--rw-r--r--   0 runner    (1001) docker     (121)     9192 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6203 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/player/
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (121)     6381 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/base_player.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/radio.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10317 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/mpvplayer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/lyric.py
--rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/fm.py
--rw-r--r--   0 runner    (1001) docker     (121)    20572 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/player/playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     7495 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/media.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/uimodels/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/uimodels/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/uimodels/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/uimodels/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/models/
--rw-r--r--   0 runner    (1001) docker     (121)    15468 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9562 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/models/uri.py
--rw-r--r--   0 runner    (1001) docker     (121)    10592 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/models/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/fuoexec/
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/fuoexec/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4943 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/fuoexec/signal_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/fuoexec/fuoexec.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/fuoexec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/entry_points/
--rw-r--r--   0 runner    (1001) docker     (121)     5514 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/entry_points/run_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/entry_points/run_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/entry_points/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/library/
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/model_protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/provider_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    12835 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/excs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4885 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/model_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/provider_protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)    28122 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/library.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/library/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/argparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/server/
--rw-r--r--   0 runner    (1001) docker     (121)     6299 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/dslv2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9176 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/server/dslv1/
--rw-r--r--   0 runner    (1001) docker     (121)     7315 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/dslv1/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/dslv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/dslv1/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/dslv1/lexer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/show.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/set_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/exec_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/search.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/excs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/handle.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/help.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/player.py
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/handlers/sub.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/excs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/server/pubsub/
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/pubsub/publishers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/pubsub/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/pubsub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/server/rpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/server/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/cli/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4135 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/app/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     8635 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/server_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/gui_app.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/once_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/mixed_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/app/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/json_.py
--rw-r--r--   0 runner    (1001) docker     (121)     8157 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/plain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/_plain_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/model_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/serializers/objs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/tips.py
--rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/tray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)     8731 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/comment_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/mpv_old.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/mpv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     5251 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/video.py
--rw-r--r--   0 runner    (1001) docker     (121)     4275 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/magicbox.py
--rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/cover_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     7314 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/tabbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/volume_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/table_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/video_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/separator.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/size_grip.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/artist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/album.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/widgets/statusline_items/
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/statusline_items/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/statusline_items/notify.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/statusline_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/labels.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/my_music.py
--rw-r--r--   0 runner    (1001) docker     (121)     9683 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/imglist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/progress_slider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/textlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     6620 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/lyric.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/frameless.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/playlist_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     3267 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/weblogin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/playlists.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/textbtn.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/messageline.py
--rw-r--r--   0 runner    (1001) docker     (121)    26018 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/songs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/statusline.py
--rw-r--r--   0 runner    (1001) docker     (121)     7556 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/widgets/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     3953 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (121)     9782 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/pages/song_explore.py
--rw-r--r--   0 runner    (1001) docker     (121)     4374 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/pages/player_playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/pages/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/pages/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/pages/coll_mixed.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/uimodels/
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimodels/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimodels/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimodels/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/page_containers/
--rw-r--r--   0 runner    (1001) docker     (121)    19826 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/page_containers/table.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/page_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3444 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/uimain/
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimain/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5477 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimain/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12277 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimain/page_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    19379 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/uimain/player_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/watch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5150 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/theme.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/mimedata.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7001 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/last.png
--rwxr-xr-x   0 runner    (1001) docker     (121)   303153 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/feeluown.icns
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/pause.png
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/cur_playlist_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/like.png
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/download_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/play.png
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/volume.png
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/already_download.png
--rw-r--r--   0 runner    (1001) docker     (121)     7730 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/tray-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/last_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    35773 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/feeluown.png
--rw-r--r--   0 runner    (1001) docker     (121)   112526 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/feeluown.ico
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/next.png
--rw-r--r--   0 runner    (1001) docker     (121)     7712 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/tray-light.png
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/like_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/like_checked_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/like_checked.png
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/play_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/next_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/volume_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/pause_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/cur_playlist.png
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/icons/already_downloaded_dark.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/gui/assets/themes/
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/themes/common.qss
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/themes/light.qss
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/themes/macos_dark.colors
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/assets/themes/dark.qss
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/hotkey.py
--rw-r--r--   0 runner    (1001) docker     (121)    11034 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/gui/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      158 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/typing_.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/aio.py
--rw-r--r--   0 runner    (1001) docker     (121)    11022 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4585 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/router.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/janus.py
--rw-r--r--   0 runner    (1001) docker     (121)    13634 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-08-09 12:31:37.000000 feeluown-3.8.8/feeluown/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-09 12:31:40.000000 feeluown-3.8.8/feeluown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-08-09 12:31:37.000000 feeluown-3.8.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-08-09 12:31:37.000000 feeluown-3.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.857154 feeluown-3.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2022-12-18 02:05:11.000000 feeluown-3.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2022-12-18 02:05:11.857154 feeluown-3.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2022-12-18 02:05:11.000000 feeluown-3.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.833153 feeluown-3.8.9/feeluown/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.837153 feeluown-3.8.9/feeluown/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/gui_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/mixed_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/once_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/app/server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.837153 feeluown-3.8.9/feeluown/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/cli/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4135 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.837153 feeluown-3.8.9/feeluown/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/entry_points/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/entry_points/run_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/entry_points/run_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.837153 feeluown-3.8.9/feeluown/fuoexec/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/fuoexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/fuoexec/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/fuoexec/fuoexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/fuoexec/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.837153 feeluown-3.8.9/feeluown/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.829153 feeluown-3.8.9/feeluown/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.841153 feeluown-3.8.9/feeluown/gui/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/already_download.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/already_downloaded_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/cur_playlist.png
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/cur_playlist_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/download_dark.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   303153 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/feeluown.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   112526 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/feeluown.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    35773 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/feeluown.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/last.png
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/last_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/like.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/like_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/like_checked_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/like_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/next_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/pause.png
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/pause_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/play_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/tray-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/tray-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/volume.png
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/icons/volume_dark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.841153 feeluown-3.8.9/feeluown/gui/assets/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/themes/common.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/themes/dark.qss
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/themes/light.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/assets/themes/macos_dark.colors
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/hotkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/mimedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.841153 feeluown-3.8.9/feeluown/gui/page_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/page_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/page_containers/scroll_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19905 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/page_containers/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.841153 feeluown-3.8.9/feeluown/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/pages/coll_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/pages/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/pages/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/pages/song_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/tray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.845153 feeluown-3.8.9/feeluown/gui/uimain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimain/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimain/player_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimain/playlist_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimain/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimain/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.845153 feeluown-3.8.9/feeluown/gui/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimodels/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/uimodels/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/accordion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/comment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/cover_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/frameless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/imglist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/magicbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/messageline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/mpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/playlist_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/progress_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/size_grip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/song_minicard_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25591 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/statusline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/gui/widgets/statusline_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/statusline_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/statusline_items/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/statusline_items/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/tabbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/table_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/textbtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/textlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/video_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/volume_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/gui/widgets/weblogin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29209 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/model_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/provider_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/library/provider_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/local/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/local/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/local/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/local/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/models/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/nowplaying/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/nowplaying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/nowplaying/global_hotkey_mac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.849154 feeluown-3.8.9/feeluown/nowplaying/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/nowplaying/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/nowplaying/linux/introspect.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/nowplaying/linux/mpris2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.853154 feeluown-3.8.9/feeluown/player/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/base_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/fm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/mpvplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/player/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.853154 feeluown-3.8.9/feeluown/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/_plain_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/json_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/model_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/serializers/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.853154 feeluown-3.8.9/feeluown/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/data_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.853154 feeluown-3.8.9/feeluown/server/dslv1/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/dslv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/dslv1/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/dslv1/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/dslv1/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/dslv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.857154 feeluown-3.8.9/feeluown/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/exec_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/set_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/handlers/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.857154 feeluown-3.8.9/feeluown/server/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/pubsub/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/pubsub/publishers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.857154 feeluown-3.8.9/feeluown/server/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.857154 feeluown-3.8.9/feeluown/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/uimodels/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/uimodels/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.857154 feeluown-3.8.9/feeluown/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/typing_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 02:05:11.833153 feeluown-3.8.9/feeluown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-18 02:05:11.000000 feeluown-3.8.9/feeluown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    79466 2022-12-18 02:05:11.000000 feeluown-3.8.9/mpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-18 02:05:11.857154 feeluown-3.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2022-12-18 02:05:11.000000 feeluown-3.8.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `feeluown-3.8.8/setup.cfg` & `feeluown-3.8.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
-description-file = README.md
+description_file = README.md
 
 [pep8]
 ignore = E402
 
 [flake8]
 max-line-length = 89
 
@@ -24,17 +24,14 @@
 	--ignore=examples/
 	--ignore=research/
 	--benchmark-skip
 	--cov-report=
 	--cov=feeluown
 	--doctest-modules
 
-[mypy-mpv_old]
-ignore_errors = True
-
 [mypy-mpv]
 ignore_errors = True
 
 [mypy-feeluown.models.*]
 ignore_errors = True
 
 [egg_info]
```

### Comparing `feeluown-3.8.8/mpv_old.py` & `feeluown-3.8.9/mpv.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 #
 # You should have received a copy of the GNU Affero General Public License along with this program.  If not, see
 # <http://www.gnu.org/licenses/>.
 #
 #
 # ------------------------------------------------
 #
-# based on v0.3.9, changes in feeluown:
+# based on v0.5.2, changes in feeluown:
 #
 # 1. read MPV_DYLIB_PATH from environ
 #    https://github.com/feeluown/FeelUOwn/pull/325
 #
-# 2. https://github.com/jaseg/python-mpv/issues/84
-#
+# 2. use API mpv_destroy since mpv_detach_destroy is deprecated since libmpv 1.29
+#    https://github.com/jaseg/python-mpv/pull/195
 
 from ctypes import *
 import ctypes.util
 import threading
 import os
 import sys
 from warnings import warn
 from functools import partial, wraps
+from contextlib import contextmanager
 import collections
 import re
 import traceback
 
 _env_name = "MPV_DYLIB_PATH"
 _nt_err_msg = ('Cannot find mpv-1.dll in your system %PATH%. One way to deal with this is to ship mpv-1.dll '
                'with your script and put the directory your script is in into %PATH% before "import mpv": '
@@ -68,17 +69,23 @@
 else:
     _dll = ctypes.util.find_library(_default_mpv_dylib)
     if _dll is None:
         raise OSError(_err_msg)
     backend = CDLL(_dll)
 
 
+class ShutdownError(SystemError):
+    pass
+
 class MpvHandle(c_void_p):
     pass
 
+class MpvRenderCtxHandle(c_void_p):
+    pass
+
 class MpvOpenGLCbContext(c_void_p):
     pass
 
 
 class PropertyUnavailableError(AttributeError):
     pass
 
@@ -93,14 +100,22 @@
     OPTION_FORMAT           = -6
     OPTION_ERROR            = -7
     PROPERTY_NOT_FOUND      = -8
     PROPERTY_FORMAT         = -9
     PROPERTY_UNAVAILABLE    = -10
     PROPERTY_ERROR          = -11
     COMMAND                 = -12
+    LOADING_FAILED          = -13
+    AO_INIT_FAILED          = -14
+    VO_INIT_FAILED          = -15
+    NOTHING_TO_PLAY         = -16
+    UNKNOWN_FORMAT          = -17
+    UNSUPPORTED             = -18
+    NOT_IMPLEMENTED         = -19
+    GENERIC                 = -20
 
     EXCEPTION_DICT = {
              0:     None,
             -1:     lambda *a: MemoryError('mpv event queue full', *a),
             -2:     lambda *a: MemoryError('mpv cannot allocate memory', *a),
             -3:     lambda *a: ValueError('Uninitialized mpv handle used', *a),
             -4:     lambda *a: ValueError('Invalid value for mpv parameter', *a),
@@ -109,27 +124,137 @@
             -7:     lambda *a: ValueError('Invalid value for mpv option', *a),
             -8:     lambda *a: AttributeError('mpv property does not exist', *a),
             # Currently (mpv 0.18.1) there is a bug causing a PROPERTY_FORMAT error to be returned instead of
             # INVALID_PARAMETER when setting a property-mapped option to an invalid value.
             -9:     lambda *a: TypeError('Tried to get/set mpv property using wrong format, or passed invalid value', *a),
             -10:    lambda *a: PropertyUnavailableError('mpv property is not available', *a),
             -11:    lambda *a: RuntimeError('Generic error getting or setting mpv property', *a),
-            -12:    lambda *a: SystemError('Error running mpv command', *a) }
+            -12:    lambda *a: SystemError('Error running mpv command', *a),
+            -14:    lambda *a: RuntimeError('Initializing the audio output failed', *a),
+            -15:    lambda *a: RuntimeError('Initializing the video output failed'),
+            -16:    lambda *a: RuntimeError('There was no audio or video data to play. This also happens if the file '
+                                            'was recognized, but did not contain any audio or video streams, or no '
+                                            'streams were selected.'),
+            -17:    lambda *a: RuntimeError('When trying to load the file, the file format could not be determined, '
+                                            'or the file was too broken to open it'),
+            -18:    lambda *a: ValueError('Generic error for signaling that certain system requirements are not fulfilled'),
+            -19:    lambda *a: NotImplementedError('The API function which was called is a stub only'),
+            -20:    lambda *a: RuntimeError('Unspecified error') }
 
     @staticmethod
     def default_error_handler(ec, *args):
         return ValueError(_mpv_error_string(ec).decode('utf-8'), ec, *args)
 
     @classmethod
     def raise_for_ec(kls, ec, func, *args):
         ec = 0 if ec > 0 else ec
         ex = kls.EXCEPTION_DICT.get(ec , kls.default_error_handler)
         if ex:
             raise ex(ec, *args)
 
+MpvGlGetProcAddressFn = CFUNCTYPE(c_void_p, c_void_p, c_char_p)
+class MpvOpenGLInitParams(Structure):
+    _fields_ = [('get_proc_address', MpvGlGetProcAddressFn),
+            ('get_proc_address_ctx', c_void_p),
+            ('extra_exts', c_void_p)]
+
+    def __init__(self, get_proc_address):
+        self.get_proc_address = get_proc_address
+        self.get_proc_address_ctx = None
+        self.extra_exts = None
+
+class MpvOpenGLFBO(Structure):
+    _fields_ = [('fbo', c_int),
+            ('w', c_int),
+            ('h', c_int),
+            ('internal_format', c_int)]
+
+    def __init__(self, w, h, fbo=0, internal_format=0):
+        self.w, self.h = w, h
+        self.fbo = fbo
+        self.internal_format = internal_format
+
+class MpvRenderFrameInfo(Structure):
+    _fields_ = [('flags', c_int64),
+            ('target_time', c_int64)]
+
+    def as_dict(self):
+        return {'flags': self.flags,
+                'target_time': self.target_time}
+
+class MpvOpenGLDRMParams(Structure):
+    _fields_ = [('fd', c_int),
+        ('crtc_id', c_int),
+        ('connector_id', c_int),
+        ('atomic_request_ptr', c_void_p),
+        ('render_fd', c_int)]
+
+class MpvOpenGLDRMDrawSurfaceSize(Structure):
+    _fields_ = [('width', c_int), ('height', c_int)]
+
+class MpvOpenGLDRMParamsV2(Structure):
+    _fields_ = [('fd', c_int),
+        ('crtc_id', c_int),
+        ('connector_id', c_int),
+        ('atomic_request_ptr', c_void_p),
+        ('render_fd', c_int)]
+
+    def __init__(self, crtc_id, connector_id, atomic_request_ptr, fd=-1, render_fd=-1):
+        self.crtc_id, self.connector_id = crtc_id, connector_id
+        self.atomic_request_ptr = atomic_request_ptr
+        self.fd, self.render_fd = fd, render_fd
+
+
+class MpvRenderParam(Structure):
+    _fields_ = [('type_id', c_int),
+                ('data', c_void_p)]
+
+    # maps human-readable type name to (type_id, argtype) tuple.
+    # The type IDs come from libmpv/render.h
+    TYPES = {"invalid"                 :(0, None),
+            "api_type"                 :(1, str),
+            "opengl_init_params"       :(2, MpvOpenGLInitParams),
+            "opengl_fbo"               :(3, MpvOpenGLFBO),
+            "flip_y"                   :(4, bool),
+            "depth"                    :(5, int),
+            "icc_profile"              :(6, bytes),
+            "ambient_light"            :(7, int),
+            "x11_display"              :(8, c_void_p),
+            "wl_display"               :(9, c_void_p),
+            "advanced_control"         :(10, bool),
+            "next_frame_info"          :(11, MpvRenderFrameInfo),
+            "block_for_target_time"    :(12, bool),
+            "skip_rendering"           :(13, bool),
+            "drm_display"              :(14, MpvOpenGLDRMParams),
+            "drm_draw_surface_size"    :(15, MpvOpenGLDRMDrawSurfaceSize),
+            "drm_display_v2"           :(16, MpvOpenGLDRMParamsV2)}
+
+    def __init__(self, name, value=None):
+        if name not in self.TYPES:
+            raise ValueError('unknown render param type "{}"'.format(name))
+        self.type_id, cons = self.TYPES[name]
+        if cons is None:
+            self.value = None
+            self.data = c_void_p()
+        elif cons is str:
+            self.value = value
+            self.data = cast(c_char_p(value.encode('utf-8')), c_void_p)
+        elif cons is bytes:
+            self.value = MpvByteArray(value)
+            self.data = cast(pointer(self.value), c_void_p)
+        elif cons is bool:
+            self.value = c_int(int(bool(value)))
+            self.data = cast(pointer(self.value), c_void_p)
+        else:
+            self.value = cons(**value)
+            self.data = cast(pointer(self.value), c_void_p)
+
+def kwargs_to_render_param_array(kwargs):
+    t = MpvRenderParam * (len(kwargs)+1)
+    return t(*kwargs.items(), ('invalid', None))
 
 class MpvFormat(c_int):
     NONE        = 0
     STRING      = 1
     OSD_STRING  = 2
     FLAG        = 3
     INT64       = 4
@@ -208,14 +333,19 @@
         return { self.keys[i].decode('utf-8'):
                 self.values[i].node_value(decoder) for i in range(self.num) }
 
 class MpvByteArray(Structure):
     _fields_ = [('data', c_void_p),
                 ('size', c_size_t)]
 
+    def __init__(self, value):
+        self._value = value
+        self.data = cast(c_char_p(value), c_void_p)
+        self.size = len(value)
+
     def bytes_value(self):
         return cast(self.data, POINTER(c_char))[:self.size]
 
 class MpvNode(Structure):
     def node_value(self, decoder=identity_decoder):
         return MpvNode.node_cast_value(self.val, self.format.value, decoder)
 
@@ -303,22 +433,32 @@
                 ('text', c_char_p)]
 
     def as_dict(self, decoder=identity_decoder):
         return { 'prefix': self.prefix.decode('utf-8'),
                  'level':  self.level.decode('utf-8'),
                  'text':   decoder(self.text).rstrip() }
 
-class MpvEventEndFile(c_int):
-    EOF_OR_INIT_FAILURE = 0
+class MpvEventEndFile(Structure):
+    _fields_ = [('reason', c_int),
+                ('error', c_int)]
+
+    EOF                 = 0
     RESTARTED           = 1
     ABORTED             = 2
     QUIT                = 3
+    ERROR               = 4
+    REDIRECT            = 5
+
+    # For backwards-compatibility
+    @property
+    def value(self):
+        return self.reason
 
     def as_dict(self, decoder=identity_decoder):
-        return {'reason': self.value}
+        return {'reason': self.reason, 'error': self.error}
 
 class MpvEventScriptInputDispatch(Structure):
     _fields_ = [('arg0', c_int),
                 ('type', c_char_p)]
 
     def as_dict(self, decoder=identity_decoder):
         pass # TODO
@@ -326,27 +466,56 @@
 class MpvEventClientMessage(Structure):
     _fields_ = [('num_args', c_int),
                 ('args', POINTER(c_char_p))]
 
     def as_dict(self, decoder=identity_decoder):
         return { 'args': [ self.args[i].decode('utf-8') for i in range(self.num_args) ] }
 
+StreamReadFn = CFUNCTYPE(c_int64, c_void_p, POINTER(c_char), c_uint64)
+StreamSeekFn = CFUNCTYPE(c_int64, c_void_p, c_int64)
+StreamSizeFn = CFUNCTYPE(c_int64, c_void_p)
+StreamCloseFn = CFUNCTYPE(None, c_void_p)
+StreamCancelFn = CFUNCTYPE(None, c_void_p)
+
+class StreamCallbackInfo(Structure):
+    _fields_ = [('cookie', c_void_p),
+                ('read', StreamReadFn),
+                ('seek', StreamSeekFn),
+                ('size', StreamSizeFn),
+                ('close', StreamCloseFn), ]
+#                ('cancel', StreamCancelFn)]
+
+StreamOpenFn = CFUNCTYPE(c_int, c_void_p, c_char_p, POINTER(StreamCallbackInfo))
+
 WakeupCallback = CFUNCTYPE(None, c_void_p)
 
+RenderUpdateFn = CFUNCTYPE(None, c_void_p)
+
 OpenGlCbUpdateFn = CFUNCTYPE(None, c_void_p)
 OpenGlCbGetProcAddrFn = CFUNCTYPE(c_void_p, c_void_p, c_char_p)
 
-def _handle_func(name, args, restype, errcheck, ctx=MpvHandle):
+def _handle_func(name, args, restype, errcheck, ctx=MpvHandle, deprecated=False):
     func = getattr(backend, name)
     func.argtypes = [ctx] + args if ctx else args
     if restype is not None:
         func.restype = restype
     if errcheck is not None:
         func.errcheck = errcheck
-    globals()['_'+name] = func
+    if deprecated:
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if not wrapper.warned: # Only warn on first invocation to prevent spamming
+                warn("Backend C api has been deprecated: " + name, DeprecationWarning, stacklevel=2)
+                wrapper.warned = True
+            return func(*args, **kwargs)
+        wrapper.warned = False
+
+        globals()['_'+name] = wrapper
+    else:
+        globals()['_'+name] = func
 
 def bytes_free_errcheck(res, func, *args):
     notnull_errcheck(res, func, *args)
     rv = cast(res, c_void_p).value
     _mpv_free(res)
     return rv
 
@@ -354,16 +523,16 @@
     if res is None:
         raise RuntimeError('Underspecified error in MPV when calling {} with args {!r}: NULL pointer returned.'\
                 'Please consult your local debugger.'.format(func.__name__, args))
     return res
 
 ec_errcheck = ErrorCode.raise_for_ec
 
-def _handle_gl_func(name, args=[], restype=None):
-    _handle_func(name, args, restype, errcheck=None, ctx=MpvOpenGLCbContext)
+def _handle_gl_func(name, args=[], restype=None, deprecated=False):
+    _handle_func(name, args, restype, errcheck=None, ctx=MpvOpenGLCbContext, deprecated=deprecated)
 
 backend.mpv_client_api_version.restype = c_ulong
 def _mpv_client_api_version():
     ver = backend.mpv_client_api_version()
     return ver>>16, ver&0xFFFF
 
 backend.mpv_free.argtypes = [c_void_p]
@@ -374,15 +543,15 @@
 
 backend.mpv_create.restype = MpvHandle
 _mpv_create = backend.mpv_create
 
 _handle_func('mpv_create_client',           [c_char_p],                                 MpvHandle, notnull_errcheck)
 _handle_func('mpv_client_name',             [],                                         c_char_p, errcheck=None)
 _handle_func('mpv_initialize',              [],                                         c_int, ec_errcheck)
-_handle_func('mpv_detach_destroy',          [],                                         None, errcheck=None)
+_handle_func('mpv_destroy',                 [],                                         None, errcheck=None)
 _handle_func('mpv_terminate_destroy',       [],                                         None, errcheck=None)
 _handle_func('mpv_load_config_file',        [c_char_p],                                 c_int, ec_errcheck)
 _handle_func('mpv_get_time_us',             [],                                         c_ulonglong, errcheck=None)
 
 _handle_func('mpv_set_option',              [c_char_p, MpvFormat, c_void_p],            c_int, ec_errcheck)
 _handle_func('mpv_set_option_string',       [c_char_p, c_char_p],                       c_int, ec_errcheck)
 
@@ -408,22 +577,36 @@
 _handle_func('mpv_request_event',           [MpvEventID, c_int],                        c_int, ec_errcheck)
 _handle_func('mpv_request_log_messages',    [c_char_p],                                 c_int, ec_errcheck)
 _handle_func('mpv_wait_event',              [c_double],                                 POINTER(MpvEvent), errcheck=None)
 _handle_func('mpv_wakeup',                  [],                                         None, errcheck=None)
 _handle_func('mpv_set_wakeup_callback',     [WakeupCallback, c_void_p],                 None, errcheck=None)
 _handle_func('mpv_get_wakeup_pipe',         [],                                         c_int, errcheck=None)
 
-_handle_func('mpv_get_sub_api',             [MpvSubApi],                                c_void_p, notnull_errcheck)
+_handle_func('mpv_stream_cb_add_ro',        [c_char_p, c_void_p, StreamOpenFn],         c_int, ec_errcheck)
 
-_handle_gl_func('mpv_opengl_cb_set_update_callback',    [OpenGlCbUpdateFn, c_void_p])
-_handle_gl_func('mpv_opengl_cb_init_gl',                [c_char_p, OpenGlCbGetProcAddrFn, c_void_p],    c_int)
-_handle_gl_func('mpv_opengl_cb_draw',                   [c_int, c_int, c_int],                          c_int)
-_handle_gl_func('mpv_opengl_cb_render',                 [c_int, c_int],                                 c_int)
-_handle_gl_func('mpv_opengl_cb_report_flip',            [c_ulonglong],                                  c_int)
-_handle_gl_func('mpv_opengl_cb_uninit_gl',              [],                                             c_int)
+_handle_func('mpv_render_context_create',               [MpvRenderCtxHandle, MpvHandle, POINTER(MpvRenderParam)],   c_int, ec_errcheck,     ctx=None)
+_handle_func('mpv_render_context_set_parameter',        [MpvRenderParam],                                           c_int, ec_errcheck,     ctx=MpvRenderCtxHandle)
+_handle_func('mpv_render_context_get_info',             [MpvRenderParam],                                           c_int, ec_errcheck,     ctx=MpvRenderCtxHandle)
+_handle_func('mpv_render_context_set_update_callback',  [RenderUpdateFn, c_void_p],                                 None, errcheck=None,    ctx=MpvRenderCtxHandle)
+_handle_func('mpv_render_context_update',               [],                                                         c_int64, errcheck=None, ctx=MpvRenderCtxHandle)
+_handle_func('mpv_render_context_render',               [POINTER(MpvRenderParam)],                                  c_int, ec_errcheck,     ctx=MpvRenderCtxHandle)
+_handle_func('mpv_render_context_report_swap',          [],                                                         None, errcheck=None,    ctx=MpvRenderCtxHandle)
+_handle_func('mpv_render_context_free',                 [],                                                         None, errcheck=None,    ctx=MpvRenderCtxHandle)
+
+
+# Deprecated in v0.29.0 and may disappear eventually
+if hasattr(backend, 'mpv_get_sub_api'):
+    _handle_func('mpv_get_sub_api',             [MpvSubApi],                                c_void_p, notnull_errcheck, deprecated=True)
+
+    _handle_gl_func('mpv_opengl_cb_set_update_callback',    [OpenGlCbUpdateFn, c_void_p], deprecated=True)
+    _handle_gl_func('mpv_opengl_cb_init_gl',                [c_char_p, OpenGlCbGetProcAddrFn, c_void_p],    c_int, deprecated=True)
+    _handle_gl_func('mpv_opengl_cb_draw',                   [c_int, c_int, c_int],                          c_int, deprecated=True)
+    _handle_gl_func('mpv_opengl_cb_render',                 [c_int, c_int],                                 c_int, deprecated=True)
+    _handle_gl_func('mpv_opengl_cb_report_flip',            [c_ulonglong],                                  c_int, deprecated=True)
+    _handle_gl_func('mpv_opengl_cb_uninit_gl',              [],                                             c_int, deprecated=True)
 
 
 def _mpv_coax_proptype(value, proptype=str):
     """Intelligently coax the given python value into something that can be understood as a proptype property."""
     if type(value) is bytes:
         return value;
     elif type(value) is bool:
@@ -431,17 +614,15 @@
     elif proptype in (str, int, float):
         return str(proptype(value)).encode('utf-8')
     else:
         raise TypeError('Cannot coax value of type {} into property type {}'.format(type(value), proptype))
 
 def _make_node_str_list(l):
     """Take a list of python objects and make a MPV string node array from it.
-
     As an example, the python list ``l = [ "foo", 23, false ]`` will result in the following MPV node object::
-
         struct mpv_node {
             .format = MPV_NODE_ARRAY,
             .u.list = *(struct mpv_node_array){
                 .num = len(l),
                 .keys = NULL,
                 .values = struct mpv_node[len(l)] {
                     { .format = MPV_NODE_STRING, .u.string = l[0] },
@@ -469,47 +650,19 @@
     while True:
         event = _mpv_wait_event(handle, -1).contents
         if event.event_id.value == MpvEventID.NONE:
             raise StopIteration()
         yield event
 
 
-def _event_loop(event_handle, playback_cond, event_callbacks, message_handlers, property_handlers, log_handler):
-    for event in _event_generator(event_handle):
-        try:
-            devent = event.as_dict(decoder=lazy_decoder) # copy data from ctypes
-            eid = devent['event_id']
-            for callback in event_callbacks:
-                callback(devent)
-            if eid in (MpvEventID.SHUTDOWN, MpvEventID.END_FILE):
-                with playback_cond:
-                    playback_cond.notify_all()
-            if eid == MpvEventID.PROPERTY_CHANGE:
-                pc = devent['event']
-                name, value, _fmt = pc['name'], pc['value'], pc['format']
-
-                for handler in property_handlers[name]:
-                    handler(name, value)
-            if eid == MpvEventID.LOG_MESSAGE and log_handler is not None:
-                ev = devent['event']
-                log_handler(ev['level'], ev['prefix'], ev['text'])
-            if eid == MpvEventID.CLIENT_MESSAGE:
-                # {'event': {'args': ['key-binding', 'foo', 'u-', 'g']}, 'reply_userdata': 0, 'error': 0, 'event_id': 16}
-                target, *args = devent['event']['args']
-                if target in message_handlers:
-                    message_handlers[target](*args)
-            if eid == MpvEventID.SHUTDOWN:
-                _mpv_detach_destroy(event_handle)
-                return
-        except Exception as e:
-            traceback.print_exc()
-
 _py_to_mpv = lambda name: name.replace('_', '-')
 _mpv_to_py = lambda name: name.replace('-', '_')
 
+_drop_nones = lambda *args: [ arg for arg in args if arg is not None ]
+
 class _Proxy:
     def __init__(self, mpv):
         super().__setattr__('mpv', mpv)
 
 class _PropertyProxy(_Proxy):
     def __dir__(self):
         return super().__dir__() + [ name.replace('-', '_') for name in self.mpv.property_list ]
@@ -538,37 +691,142 @@
 
     def __getattr__(self, name):
         return self.mpv._get_property(_py_to_mpv(name), decoder=self._decoder)
 
     def __setattr__(self, name, value):
         setattr(self.mpv, _py_to_mpv(name), value)
 
+class GeneratorStream:
+    """Transform a python generator into an mpv-compatible stream object. This only supports size() and read(), and
+    does not support seek(), close() or cancel().
+    """
+
+    def __init__(self, generator_fun, size=None):
+        self._generator_fun = generator_fun
+        self.size = size
+
+    def seek(self, offset):
+        self._read_iter = iter(self._generator_fun())
+        self._read_chunk = b''
+        return 0 # We only support seeking to the first byte atm
+        # implementation in case seeking to arbitrary offsets would be necessary
+        # while offset > 0:
+        #     offset -= len(self.read(offset))
+        # return offset
+
+    def read(self, size):
+        if not self._read_chunk:
+            try:
+                self._read_chunk += next(self._read_iter)
+            except StopIteration:
+                return b''
+        rv, self._read_chunk = self._read_chunk[:size], self._read_chunk[size:]
+        return rv
+
+    def close(self):
+        self._read_iter = iter([]) # make next read() call return EOF
+
+    def cancel(self):
+        self._read_iter = iter([]) # make next read() call return EOF
+        # TODO?
+
+
+class ImageOverlay:
+    def __init__(self, m, overlay_id, img=None, pos=(0, 0)):
+        self.m = m
+        self.overlay_id = overlay_id
+        self.pos = pos
+        self._size = None
+        if img is not None:
+            self.update(img)
+
+    def update(self, img=None, pos=None):
+        from PIL import Image
+        if img is not None:
+            self.img = img
+        img = self.img
+
+        w, h = img.size
+        stride = w*4
+
+        if pos is not None:
+            self.pos = pos
+        x, y = self.pos
+
+        # Pre-multiply alpha channel
+        bg = Image.new('RGBA', (w, h),  (0, 0, 0, 0))
+        out = Image.alpha_composite(bg, img)
+
+        # Copy image to ctypes buffer
+        if img.size != self._size:
+            self._buf = create_string_buffer(w*h*4)
+            self._size = img.size
+
+        self._buf[:] = out.tobytes('raw', 'BGRA')
+        source = '&' + str(addressof(self._buf))
+
+        self.m.overlay_add(self.overlay_id, x, y, source, 0, 'bgra', w, h, stride)
+
+    def remove(self):
+        self.m.remove_overlay(self.overlay_id)
+
+
+class FileOverlay:
+    def __init__(self, m, overlay_id, filename=None, size=None, stride=None, pos=(0,0)):
+        self.m = m
+        self.overlay_id = overlay_id
+        self.pos = pos
+        self.size = size
+        self.stride = stride
+        if filename is not None:
+            self.update(filename)
+
+    def update(self, filename=None, size=None, stride=None, pos=None):
+        if filename is not None:
+            self.filename = filename
+
+        if pos is not None:
+            self.pos = pos
+
+        if size is not None:
+            self.size = size
+
+        if stride is not None:
+            self.stride = stride
+
+        x, y = self.pos
+        w, h = self.size
+        stride = self.stride or 4*w
+
+        self.m.overlay_add(self, self.overlay_id, x, y, self.filename, 0, 'bgra', w, h, stride)
+
+    def remove(self):
+        self.m.remove_overlay(self.overlay_id)
+
+
 class MPV(object):
     """See man mpv(1) for the details of the implemented commands. All mpv properties can be accessed as
     ``my_mpv.some_property`` and all mpv options can be accessed as ``my_mpv['some-option']``.
-
     By default, properties are returned as decoded ``str`` and an error is thrown if the value does not contain valid
     utf-8. To get a decoded ``str`` if possibly but ``bytes`` instead of an error if not, use
     ``my_mpv.lazy.some_property``. To always get raw ``bytes``, use ``my_mpv.raw.some_property``.  To access a
     property's decoded OSD value, use ``my_mpv.osd.some_property``.
-
     To get API information on an option, use ``my_mpv.option_info('option-name')``. To get API information on a
     property, use ``my_mpv.properties['property-name']``. Take care to use mpv's dashed-names instead of the
     underscore_names exposed on the python object.
-
     To make your program not barf hard the first time its used on a weird file system **always** access properties
     containing file names or file tags through ``MPV.raw``.  """
     def __init__(self, *extra_mpv_flags, log_handler=None, start_event_thread=True, loglevel=None, **extra_mpv_opts):
         """Create an MPV instance.
-
         Extra arguments and extra keyword arguments will be passed to mpv as options.
         """
 
         self.handle = _mpv_create()
         self._event_thread = None
+        self._core_shutdown = False
 
         _mpv_set_option_string(self.handle, b'audio-display', b'no')
         istr = lambda o: ('yes' if o else 'no') if type(o) is bool else str(o)
         try:
             for flag in extra_mpv_flags:
                 _mpv_set_option_string(self.handle, flag.encode('utf-8'), b'')
             for k,v in extra_mpv_opts.items():
@@ -579,72 +837,210 @@
         self.osd = _OSDPropertyProxy(self)
         self.file_local = _FileLocalProxy(self)
         self.raw    = _DecoderPropertyProxy(self, identity_decoder)
         self.strict = _DecoderPropertyProxy(self, strict_decoder)
         self.lazy   = _DecoderPropertyProxy(self, lazy_decoder)
 
         self._event_callbacks = []
+        self._event_handler_lock = threading.Lock()
         self._property_handlers = collections.defaultdict(lambda: [])
+        self._quit_handlers = set()
         self._message_handlers = {}
         self._key_binding_handlers = {}
-        self._playback_cond = threading.Condition()
         self._event_handle = _mpv_create_client(self.handle, b'py_event_handler')
-        self._loop = partial(_event_loop, self._event_handle, self._playback_cond, self._event_callbacks,
-                self._message_handlers, self._property_handlers, log_handler)
+        self._log_handler = log_handler
+        self._stream_protocol_cbs = {}
+        self._stream_protocol_frontends = collections.defaultdict(lambda: {})
+        self.register_stream_protocol('python', self._python_stream_open)
+        self._python_streams = {}
+        self._python_stream_catchall = None
+        self.overlay_ids = set()
+        self.overlays = {}
         if loglevel is not None or log_handler is not None:
             self.set_loglevel(loglevel or 'terminal-default')
         if start_event_thread:
             self._event_thread = threading.Thread(target=self._loop, name='MPVEventHandlerThread')
             self._event_thread.setDaemon(True)
             self._event_thread.start()
         else:
             self._event_thread = None
 
+    def _loop(self):
+        for event in _event_generator(self._event_handle):
+            try:
+                devent = event.as_dict(decoder=lazy_decoder) # copy data from ctypes
+                eid = devent['event_id']
+
+                with self._event_handler_lock:
+                    if eid == MpvEventID.SHUTDOWN:
+                        self._core_shutdown = True
+
+                for callback in self._event_callbacks:
+                    callback(devent)
+
+                if eid == MpvEventID.PROPERTY_CHANGE:
+                    pc = devent['event']
+                    name, value, _fmt = pc['name'], pc['value'], pc['format']
+                    for handler in self._property_handlers[name]:
+                        handler(name, value)
+
+                if eid == MpvEventID.LOG_MESSAGE and self._log_handler is not None:
+                    ev = devent['event']
+                    self._log_handler(ev['level'], ev['prefix'], ev['text'])
+
+                if eid == MpvEventID.CLIENT_MESSAGE:
+                    # {'event': {'args': ['key-binding', 'foo', 'u-', 'g']}, 'reply_userdata': 0, 'error': 0, 'event_id': 16}
+                    target, *args = devent['event']['args']
+                    if target in self._message_handlers:
+                        self._message_handlers[target](*args)
+
+                if eid == MpvEventID.SHUTDOWN:
+                    _mpv_destroy(self._event_handle)
+                    return
+
+            except Exception as e:
+                print('Exception inside python-mpv event loop:', file=sys.stderr)
+                traceback.print_exc()
+
+    @property
+    def core_shutdown(self):
+        """Property indicating whether the core has been shut down. Possible causes for this are e.g. the `quit` command
+        or a user closing the mpv window."""
+        return self._core_shutdown
+
+    def check_core_alive(self):
+        """ This method can be used as a sanity check to tests whether the core is still alive at the time it is
+        called."""
+        if self._core_shutdown:
+            raise ShutdownError('libmpv core has been shutdown')
+
+    def wait_until_paused(self):
+        """Waits until playback of the current title is paused or done. Raises a ShutdownError if the core is shutdown while
+        waiting."""
+        self.wait_for_property('core-idle')
+
     def wait_for_playback(self):
-        """Waits until playback of the current title is paused or done."""
-        with self._playback_cond:
-            self._playback_cond.wait()
+        """Waits until playback of the current title is finished. Raises a ShutdownError if the core is shutdown while
+        waiting.
+        """
+        self.wait_for_event('end_file')
+
+    def wait_until_playing(self):
+        """Waits until playback of the current title has started. Raises a ShutdownError if the core is shutdown while
+        waiting."""
+        self.wait_for_property('core-idle', lambda idle: not idle)
 
     def wait_for_property(self, name, cond=lambda val: val, level_sensitive=True):
         """Waits until ``cond`` evaluates to a truthy value on the named property. This can be used to wait for
-        properties such as ``idle_active`` indicating the player is done with regular playback and just idling around
+        properties such as ``idle_active`` indicating the player is done with regular playback and just idling around.
+        Raises a ShutdownError when the core is shutdown while waiting.
         """
+        with self.prepare_and_wait_for_property(name, cond, level_sensitive):
+            pass
+
+    def wait_for_shutdown(self):
+        '''Wait for core to shutdown (e.g. through quit() or terminate()).'''
         sema = threading.Semaphore(value=0)
+
+        @self.event_callback('shutdown')
+        def shutdown_handler(event):
+            sema.release()
+
+        sema.acquire()
+        shutdown_handler.unregister_mpv_events()
+
+    @contextmanager
+    def prepare_and_wait_for_property(self, name, cond=lambda val: val, level_sensitive=True):
+        """Context manager that waits until ``cond`` evaluates to a truthy value on the named property. See
+        prepare_and_wait_for_event for usage.
+        Raises a ShutdownError when the core is shutdown while waiting.
+        """
+        sema = threading.Semaphore(value=0)
+
         def observer(name, val):
             if cond(val):
                 sema.release()
         self.observe_property(name, observer)
+
+        @self.event_callback('shutdown')
+        def shutdown_handler(event):
+            sema.release()
+
+        yield
         if not level_sensitive or not cond(getattr(self, name.replace('-', '_'))):
             sema.acquire()
+
+        self.check_core_alive()
+
+        shutdown_handler.unregister_mpv_events()
         self.unobserve_property(name, observer)
 
+    def wait_for_event(self, *event_types, cond=lambda evt: True):
+        """Waits for the indicated event(s). If cond is given, waits until cond(event) is true. Raises a ShutdownError
+        if the core is shutdown while waiting. This also happens when 'shutdown' is in event_types.
+        """
+        with self.prepare_and_wait_for_event(*event_types, cond=cond):
+            pass
+
+    @contextmanager
+    def prepare_and_wait_for_event(self, *event_types, cond=lambda evt: True):
+        """Context manager that waits for the indicated event(s) like wait_for_event after running. If cond is given,
+        waits until cond(event) is true. Raises a ShutdownError if the core is shutdown while waiting. This also happens
+        when 'shutdown' is in event_types.
+        Compared to wait_for_event this handles the case where a thread waits for an event it itself causes in a
+        thread-safe way. An example from the testsuite is:
+        with self.m.prepare_and_wait_for_event('client_message'):
+            self.m.keypress(key)
+        Using just wait_for_event it would be impossible to ensure the event is caught since it may already have been
+        handled in the interval between keypress(...) running and a subsequent wait_for_event(...) call.
+        """
+        sema = threading.Semaphore(value=0)
+
+        @self.event_callback('shutdown')
+        def shutdown_handler(event):
+            sema.release()
+
+        @self.event_callback(*event_types)
+        def target_handler(evt):
+            if cond(evt):
+                sema.release()
+
+        yield
+        sema.acquire()
+
+        self.check_core_alive()
+
+        shutdown_handler.unregister_mpv_events()
+        target_handler.unregister_mpv_events()
+
     def __del__(self):
         if self.handle:
             self.terminate()
 
     def terminate(self):
         """Properly terminates this player instance. Preferably use this instead of relying on python's garbage
         collector to cause this to be called from the object's destructor.
+        This method will detach the main libmpv handle and wait for mpv to shut down and the event thread to finish.
         """
         self.handle, handle = None, self.handle
         if threading.current_thread() is self._event_thread:
-            # Handle special case to allow event handle to be detached.
-            # This is necessary since otherwise the event thread would deadlock itself.
-            grim_reaper = threading.Thread(target=lambda: _mpv_terminate_destroy(handle))
-            grim_reaper.start()
+            raise UserWarning('terminate() should not be called from event thread (e.g. from a callback function). If '
+                    'you want to terminate mpv from here, please call quit() instead, then sync the main thread '
+                    'against the event thread using e.g. wait_for_shutdown(), then terminate() from the main thread. '
+                    'This call has been transformed into a call to quit().')
+            self.quit()
         else:
             _mpv_terminate_destroy(handle)
             if self._event_thread:
                 self._event_thread.join()
 
     def set_loglevel(self, level):
         """Set MPV's log level. This adjusts which output will be sent to this object's log handlers. If you just want
         mpv's regular terminal output, you don't need to adjust this but just need to pass a log handler to the MPV
         constructur such as ``MPV(log_handler=print)``.
-
         Valid log levels are "no", "fatal", "error", "warn", "info", "v" "debug" and "trace". For details see your mpv's
         client.h header file.
         """
         _mpv_request_log_messages(self._event_handle, level.encode('utf-8'))
 
     def command(self, name, *args):
         """Execute a raw command."""
@@ -666,16 +1062,16 @@
         self.command('seek', amount, reference, precision)
 
     def revert_seek(self):
         """Mapped mpv revert_seek command, see man mpv(1)."""
         self.command('revert_seek');
 
     def frame_step(self):
-        """Mapped mpv frame_step command, see man mpv(1)."""
-        self.command('frame_step')
+        """Mapped mpv frame-step command, see man mpv(1)."""
+        self.command('frame-step')
 
     def frame_back_step(self):
         """Mapped mpv frame_back_step command, see man mpv(1)."""
         self.command('frame_back_step')
 
     def property_add(self, name, value=1):
         """Add the given value to the property's value. On overflow or underflow, clamp the property to the maximum. If
@@ -704,29 +1100,61 @@
     def screenshot_raw(self, includes='subtitles'):
         """Mapped mpv screenshot_raw command, see man mpv(1). Returns a pillow Image object."""
         from PIL import Image
         res = self.node_command('screenshot-raw', includes)
         if res['format'] != 'bgr0':
             raise ValueError('Screenshot in unknown format "{}". Currently, only bgr0 is supported.'
                     .format(res['format']))
-        img = Image.frombytes('RGBA', (res['w'], res['h']), res['data'])
+        img = Image.frombytes('RGBA', (res['stride']//4, res['h']), res['data'])
         b,g,r,a = img.split()
         return Image.merge('RGB', (r,g,b))
 
+    def allocate_overlay_id(self):
+        free_ids = set(range(64)) - self.overlay_ids
+        if not free_ids:
+            raise IndexError('All overlay IDs are in use')
+        next_id, *_ = sorted(free_ids)
+        self.overlay_ids.add(next_id)
+        return next_id
+
+    def free_overlay_id(self, overlay_id):
+        self.overlay_ids.remove(overlay_id)
+
+    def create_file_overlay(self, filename=None, size=None, stride=None, pos=(0,0)):
+        overlay_id = self.allocate_overlay_id()
+        overlay = FileOverlay(self, overlay_id, filename, size, stride, pos)
+        self.overlays[overlay_id] = overlay
+        return overlay
+
+    def create_image_overlay(self, img=None, pos=(0,0)):
+        overlay_id = self.allocate_overlay_id()
+        overlay = ImageOverlay(self, overlay_id, img, pos)
+        self.overlays[overlay_id] = overlay
+        return overlay
+
+    def remove_overlay(self, overlay_id):
+        self.overlay_remove(overlay_id)
+        self.free_overlay_id(overlay_id)
+        del self.overlays[overlay_id]
+
     def playlist_next(self, mode='weak'):
         """Mapped mpv playlist_next command, see man mpv(1)."""
         self.command('playlist_next', mode)
 
     def playlist_prev(self, mode='weak'):
         """Mapped mpv playlist_prev command, see man mpv(1)."""
         self.command('playlist_prev', mode)
 
+    def playlist_play_index(self, idx):
+        """Mapped mpv playlist-play-index command, see man mpv(1)."""
+        self.command('playlist-play-index', idx)
+
     @staticmethod
     def _encode_options(options):
-        return ','.join('{}={}'.format(str(key), str(val)) for key, val in options.items())
+        return ','.join('{}={}'.format(_py_to_mpv(str(key)), str(val)) for key, val in options.items())
 
     def loadfile(self, filename, mode='replace', **options):
         """Mapped mpv loadfile command, see man mpv(1)."""
         self.command('loadfile', filename.encode(fs_enc), mode, MPV._encode_options(options))
 
     def loadlist(self, playlist, mode='replace'):
         """Mapped mpv loadlist command, see man mpv(1)."""
@@ -740,29 +1168,68 @@
         """Mapped mpv playlist_remove command, see man mpv(1)."""
         self.command('playlist_remove', index)
 
     def playlist_move(self, index1, index2):
         """Mapped mpv playlist_move command, see man mpv(1)."""
         self.command('playlist_move', index1, index2)
 
+    def playlist_shuffle(self):
+        """Mapped mpv playlist-shuffle command, see man mpv(1)."""
+        self.command('playlist-shuffle')
+
+    def playlist_unshuffle(self):
+        """Mapped mpv playlist-unshuffle command, see man mpv(1)."""
+        self.command('playlist-unshuffle')
+
     def run(self, command, *args):
         """Mapped mpv run command, see man mpv(1)."""
         self.command('run', command, *args)
 
     def quit(self, code=None):
         """Mapped mpv quit command, see man mpv(1)."""
         self.command('quit', code)
 
     def quit_watch_later(self, code=None):
         """Mapped mpv quit_watch_later command, see man mpv(1)."""
         self.command('quit_watch_later', code)
 
-    def sub_add(self, filename):
+    def stop(self, keep_playlist=False):
+        """Mapped mpv stop command, see man mpv(1)."""
+        if keep_playlist:
+            self.command('stop', 'keep-playlist')
+        else:
+            self.command('stop')
+
+    def audio_add(self, url, flags='select', title=None, lang=None):
+        """Mapped mpv audio_add command, see man mpv(1)."""
+        self.command('audio_add', url.encode(fs_enc), *_drop_nones(flags, title, lang))
+
+    def audio_remove(self, audio_id=None):
+        """Mapped mpv audio_remove command, see man mpv(1)."""
+        self.command('audio_remove', audio_id)
+
+    def audio_reload(self, audio_id=None):
+        """Mapped mpv audio_reload command, see man mpv(1)."""
+        self.command('audio_reload', audio_id)
+
+    def video_add(self, url, flags='select', title=None, lang=None):
+        """Mapped mpv video_add command, see man mpv(1)."""
+        self.command('video_add', url.encode(fs_enc), *_drop_nones(flags, title, lang))
+
+    def video_remove(self, video_id=None):
+        """Mapped mpv video_remove command, see man mpv(1)."""
+        self.command('video_remove', video_id)
+
+    def video_reload(self, video_id=None):
+        """Mapped mpv video_reload command, see man mpv(1)."""
+        self.command('video_reload', video_id)
+
+    def sub_add(self, url, flags='select', title=None, lang=None):
         """Mapped mpv sub_add command, see man mpv(1)."""
-        self.command('sub_add', filename.encode(fs_enc))
+        self.command('sub_add', url.encode(fs_enc), *_drop_nones(flags, title, lang))
 
     def sub_remove(self, sub_id=None):
         """Mapped mpv sub_remove command, see man mpv(1)."""
         self.command('sub_remove', sub_id)
 
     def sub_reload(self, sub_id=None):
         """Mapped mpv sub_reload command, see man mpv(1)."""
@@ -776,26 +1243,68 @@
         """Mapped mpv sub_seek command, see man mpv(1)."""
         self.command('sub_seek', skip)
 
     def toggle_osd(self):
         """Mapped mpv osd command, see man mpv(1)."""
         self.command('osd')
 
+    def print_text(self, text):
+        """Mapped mpv print-text command, see man mpv(1)."""
+        self.command('print-text', text)
+
     def show_text(self, string, duration='-1', level=None):
         """Mapped mpv show_text command, see man mpv(1)."""
         self.command('show_text', string, duration, level)
 
+    def expand_text(self, text):
+        """Mapped mpv expand-text command, see man mpv(1)."""
+        return self.node_command('expand-text', text)
+
+    def expand_path(self, path):
+        """Mapped mpv expand-path command, see man mpv(1)."""
+        return self.node_command('expand-path', path)
+
     def show_progress(self):
         """Mapped mpv show_progress command, see man mpv(1)."""
         self.command('show_progress')
 
+    def rescan_external_files(self, mode='reselect'):
+        """Mapped mpv rescan-external-files command, see man mpv(1)."""
+        self.command('rescan-external-files', mode)
+
     def discnav(self, command):
         """Mapped mpv discnav command, see man mpv(1)."""
         self.command('discnav', command)
 
+    def mouse(x, y, button=None, mode='single'):
+        """Mapped mpv mouse command, see man mpv(1)."""
+        if button is None:
+            self.command('mouse', x, y, mode)
+        else:
+            self.command('mouse', x, y, button, mode)
+
+    def keypress(self, name):
+        """Mapped mpv keypress command, see man mpv(1)."""
+        self.command('keypress', name)
+
+    def keydown(self, name):
+        """Mapped mpv keydown command, see man mpv(1)."""
+        self.command('keydown', name)
+
+    def keyup(self, name=None):
+        """Mapped mpv keyup command, see man mpv(1)."""
+        if name is None:
+            self.command('keyup')
+        else:
+            self.command('keyup', name)
+
+    def keybind(self, name, command):
+        """Mapped mpv keybind command, see man mpv(1)."""
+        self.command('keybind', name, command)
+
     def write_watch_later_config(self):
         """Mapped mpv write_watch_later_config command, see man mpv(1)."""
         self.command('write_watch_later_config')
 
     def overlay_add(self, overlay_id, x, y, file_or_fd, offset, fmt, w, h, stride):
         """Mapped mpv overlay_add command, see man mpv(1)."""
         self.command('overlay_add', overlay_id, x, y, file_or_fd, offset, fmt, w, h, stride)
@@ -813,23 +1322,22 @@
         self.command('script_message_to', target, *args)
 
     def observe_property(self, name, handler):
         """Register an observer on the named property. An observer is a function that is called with the new property
         value every time the property's value is changed. The basic function signature is ``fun(property_name,
         new_value)`` with new_value being the decoded property value as a python object. This function can be used as a
         function decorator if no handler is given.
-
         To unregister the observer, call either of ``mpv.unobserve_property(name, handler)``,
         ``mpv.unobserve_all_properties(handler)`` or the handler's ``unregister_mpv_properties`` attribute::
-
             @player.observe_property('volume')
             def my_handler(new_volume, *):
                 print("It's loud!", volume)
-
             my_handler.unregister_mpv_properties()
+        exit_handler is a function taking no arguments that is called when the underlying mpv handle is terminated (e.g.
+        from calling MPV.terminate() or issuing a "quit" input command).
         """
         self._property_handlers[name].append(handler)
         _mpv_observe_property(self._event_handle, hash(name)&0xffffffffffffffff, name.encode('utf-8'), MpvFormat.NODE)
 
     def property_observer(self, name):
         """Function decorator to register a property observer. See ``MPV.observe_property`` for details."""
         def wrapper(fun):
@@ -851,162 +1359,136 @@
         """Unregister a property observer from *all* observed properties."""
         for name in self._property_handlers:
             self.unobserve_property(name, handler)
 
     def register_message_handler(self, target, handler=None):
         """Register a mpv script message handler. This can be used to communicate with embedded lua scripts. Pass the
         script message target name this handler should be listening to and the handler function.
-
         WARNING: Only one handler can be registered at a time for any given target.
-
         To unregister the message handler, call its ``unregister_mpv_messages`` function::
-
             player = mpv.MPV()
             @player.message_handler('foo')
             def my_handler(some, args):
                 print(args)
-
             my_handler.unregister_mpv_messages()
         """
         self._register_message_handler_internal(target, handler)
 
     def _register_message_handler_internal(self, target, handler):
         self._message_handlers[target] = handler
 
     def unregister_message_handler(self, target_or_handler):
         """Unregister a mpv script message handler for the given script message target name.
-
         You can also call the ``unregister_mpv_messages`` function attribute set on the handler function when it is
         registered.
         """
         if isinstance(target_or_handler, str):
             del self._message_handlers[target_or_handler]
         else:
             for key, val in self._message_handlers.items():
                 if val == target_or_handler:
                     del self._message_handlers[key]
 
     def message_handler(self, target):
         """Decorator to register a mpv script message handler.
-
         WARNING: Only one handler can be registered at a time for any given target.
-
         To unregister the message handler, call its ``unregister_mpv_messages`` function::
-
             player = mpv.MPV()
             @player.message_handler('foo')
             def my_handler(some, args):
                 print(args)
-
             my_handler.unregister_mpv_messages()
         """
         def register(handler):
             self._register_message_handler_internal(target, handler)
             handler.unregister_mpv_messages = lambda: self.unregister_message_handler(handler)
             return handler
         return register
 
     def register_event_callback(self, callback):
         """Register a blanket event callback receiving all event types.
-
         To unregister the event callback, call its ``unregister_mpv_events`` function::
-
             player = mpv.MPV()
             @player.event_callback('shutdown')
             def my_handler(event):
                 print('It ded.')
-
             my_handler.unregister_mpv_events()
         """
         self._event_callbacks.append(callback)
 
     def unregister_event_callback(self, callback):
         """Unregiser an event callback."""
         self._event_callbacks.remove(callback)
 
     def event_callback(self, *event_types):
         """Function decorator to register a blanket event callback for the given event types. Event types can be given
         as str (e.g.  'start-file'), integer or MpvEventID object.
-
         WARNING: Due to the way this is filtering events, this decorator cannot be chained with itself.
-
         To unregister the event callback, call its ``unregister_mpv_events`` function::
-
             player = mpv.MPV()
             @player.event_callback('shutdown')
             def my_handler(event):
                 print('It ded.')
-
             my_handler.unregister_mpv_events()
         """
         def register(callback):
-            types = [MpvEventID.from_str(t) if isinstance(t, str) else t for t in event_types] or MpvEventID.ANY
-            @wraps(callback)
-            def wrapper(event, *args, **kwargs):
-                if event['event_id'] in types:
-                    callback(event, *args, **kwargs)
-            self._event_callbacks.append(wrapper)
-            wrapper.unregister_mpv_events = partial(self.unregister_event_callback, wrapper)
-            return wrapper
+            with self._event_handler_lock:
+                self.check_core_alive()
+                types = [MpvEventID.from_str(t) if isinstance(t, str) else t for t in event_types] or MpvEventID.ANY
+                @wraps(callback)
+                def wrapper(event, *args, **kwargs):
+                    if event['event_id'] in types:
+                        callback(event, *args, **kwargs)
+                self._event_callbacks.append(wrapper)
+                wrapper.unregister_mpv_events = partial(self.unregister_event_callback, wrapper)
+                return wrapper
         return register
 
     @staticmethod
     def _binding_name(callback_or_cmd):
         return 'py_kb_{:016x}'.format(hash(callback_or_cmd)&0xffffffffffffffff)
 
     def on_key_press(self, keydef, mode='force'):
         """Function decorator to register a simplified key binding. The callback is called whenever the key given is
         *pressed*.
-
         To unregister the callback function, you can call its ``unregister_mpv_key_bindings`` attribute::
-
             player = mpv.MPV()
             @player.on_key_press('Q')
             def binding():
                 print('blep')
-
             binding.unregister_mpv_key_bindings()
-
         WARNING: For a single keydef only a single callback/command can be registered at the same time. If you register
         a binding multiple times older bindings will be overwritten and there is a possibility of references leaking. So
         don't do that.
-
         The BIG FAT WARNING regarding untrusted keydefs from the key_binding method applies here as well.
         """
         def register(fun):
             @self.key_binding(keydef, mode)
             @wraps(fun)
-            def wrapper(state='p-', name=None):
+            def wrapper(state='p-', name=None, char=None):
                 if state[0] in ('d', 'p'):
                     fun()
             return wrapper
         return register
 
     def key_binding(self, keydef, mode='force'):
         """Function decorator to register a low-level key binding.
-
         The callback function signature is ``fun(key_state, key_name)`` where ``key_state`` is either ``'U'`` for "key
         up" or ``'D'`` for "key down".
-
         The keydef format is: ``[Shift+][Ctrl+][Alt+][Meta+]<key>`` where ``<key>`` is either the literal character the
         key produces (ASCII or Unicode character), or a symbolic name (as printed by ``mpv --input-keylist``).
-
         To unregister the callback function, you can call its ``unregister_mpv_key_bindings`` attribute::
-
             player = mpv.MPV()
             @player.key_binding('Q')
-            def binding(state, name):
+            def binding(state, name, char):
                 print('blep')
-
             binding.unregister_mpv_key_bindings()
-
         WARNING: For a single keydef only a single callback/command can be registered at the same time. If you register
         a binding multiple times older bindings will be overwritten and there is a possibility of references leaking. So
         don't do that.
-
         BIG FAT WARNING: mpv's key binding mechanism is pretty powerful.  This means, you essentially get arbitrary code
         exectution through key bindings. This interface makes some limited effort to sanitize the keydef given in the
         first parameter, but YOU SHOULD NOT RELY ON THIS IN FOR SECURITY. If your input comes from config files, this is
         completely fine--but, if you are about to pass untrusted input into this parameter, better double-check whether
         this is secure in your case.
         """
         def register(fun):
@@ -1036,27 +1518,99 @@
                     binding_name, '{} script-binding py_event_handler/{}'.format(keydef, binding_name), mode)
         elif isinstance(callback_or_cmd, str):
             self.command('define-section', binding_name, '{} {}'.format(keydef, callback_or_cmd), mode)
         else:
             raise TypeError('register_key_binding expects either an str with an mpv command or a python callable.')
         self.command('enable-section', binding_name, 'allow-hide-cursor+allow-vo-dragging')
 
-    def _handle_key_binding_message(self, binding_name, key_state, key_name=None):
-        self._key_binding_handlers[binding_name](key_state, key_name)
+    def _handle_key_binding_message(self, binding_name, key_state, key_name=None, key_char=None):
+        self._key_binding_handlers[binding_name](key_state, key_name, key_char)
 
     def unregister_key_binding(self, keydef):
         """Unregister a key binding by keydef."""
         binding_name = MPV._binding_name(keydef)
         self.command('disable-section', binding_name)
         self.command('define-section', binding_name, '')
         if binding_name in self._key_binding_handlers:
             del self._key_binding_handlers[binding_name]
             if not self._key_binding_handlers:
                 self.unregister_message_handler('key-binding')
 
+    def register_stream_protocol(self, proto, open_fn=None):
+        """ Register a custom stream protocol as documented in libmpv/stream_cb.h:
+            https://github.com/mpv-player/mpv/blob/master/libmpv/stream_cb.h
+            proto is the protocol scheme, e.g. "foo" for "foo://" urls.
+            This function can either be used with two parameters or it can be used as a decorator on the target
+            function.
+            open_fn is a function taking an URI string and returning an mpv stream object.
+            open_fn may raise a ValueError to signal libmpv the URI could not be opened.
+            The mpv stream protocol is as follows:
+            class Stream:
+                @property
+                def size(self):
+                    return None # unknown size
+                    return size # int with size in bytes
+                def read(self, size):
+                    ...
+                    return read # non-empty bytes object with input
+                    return b'' # empty byte object signals permanent EOF
+                def seek(self, pos):
+                    return new_offset # integer with new byte offset. The new offset may be before the requested offset
+                    in case an exact seek is inconvenient.
+                def close(self):
+                    ...
+                # def cancel(self): (future API versions only)
+                #     Abort a running read() or seek() operation
+                #     ...
+        """
+
+        def decorator(open_fn):
+            @StreamOpenFn
+            def open_backend(_userdata, uri, cb_info):
+                try:
+                    frontend = open_fn(uri.decode('utf-8'))
+                except ValueError:
+                    return ErrorCode.LOADING_FAILED
+
+                def read_backend(_userdata, buf, bufsize):
+                    data = frontend.read(bufsize)
+                    for i in range(len(data)):
+                        buf[i] = data[i]
+                    return len(data)
+
+                cb_info.contents.cookie = None
+                read = cb_info.contents.read = StreamReadFn(read_backend)
+                close = cb_info.contents.close = StreamCloseFn(lambda _userdata: frontend.close())
+
+                seek, size, cancel = None, None, None
+                if hasattr(frontend, 'seek'):
+                    seek = cb_info.contents.seek = StreamSeekFn(lambda _userdata, offx: frontend.seek(offx))
+                if hasattr(frontend, 'size') and frontend.size is not None:
+                    size = cb_info.contents.size = StreamSizeFn(lambda _userdata: frontend.size)
+
+                # Future API versions only
+                # if hasattr(frontend, 'cancel'):
+                #     cb_info.contents.cancel = StreamCancelFn(lambda _userdata: frontend.cancel())
+
+                # keep frontend and callbacks in memory forever (TODO)
+                frontend._registered_callbacks = [read, close, seek, size, cancel]
+                self._stream_protocol_frontends[proto][uri] = frontend
+                return 0
+
+            if proto in self._stream_protocol_cbs:
+                raise KeyError('Stream protocol already registered')
+            self._stream_protocol_cbs[proto] = [open_backend]
+            _mpv_stream_cb_add_ro(self.handle, proto.encode('utf-8'), c_void_p(), open_backend)
+
+            return open_fn
+
+        if open_fn is not None:
+            decorator(open_fn)
+        return decorator
+
     # Convenience functions
     def play(self, filename):
         """Play a path or URL (requires ``ytdl`` option to be set)."""
         self.loadfile(filename)
 
     @property
     def playlist_filenames(self):
@@ -1064,16 +1618,98 @@
         return [element['filename'] for element in self.playlist]
 
     def playlist_append(self, filename, **options):
         """Append a path or URL to the playlist. This does not start playing the file automatically. To do that, use
         ``MPV.loadfile(filename, 'append-play')``."""
         self.loadfile(filename, 'append', **options)
 
+    # "Python stream" logic. This is some porcelain for directly playing data from python generators.
+
+    def _python_stream_open(self, uri):
+        """Internal handler for python:// protocol streams registered through @python_stream(...) and
+        @python_stream_catchall
+        """
+        name, = re.fullmatch('python://(.*)', uri).groups()
+
+        if name in self._python_streams:
+            generator_fun, size = self._python_streams[name]
+        else:
+            if self._python_stream_catchall is not None:
+                generator_fun, size = self._python_stream_catchall(name)
+            else:
+                raise ValueError('Python stream name not found and no catch-all defined')
+
+        return GeneratorStream(generator_fun, size)
+
+    def python_stream(self, name=None, size=None):
+        """Register a generator for the python stream with the given name.
+        name is the name, i.e. the part after the "python://" in the URI, that this generator is registered as.
+        size is the total number of bytes in the stream (if known).
+        Any given name can only be registered once. The catch-all can also only be registered once. To unregister a
+        stream, call the .unregister function set on the callback.
+        The generator signals EOF by returning, manually raising StopIteration or by yielding b'', an empty bytes
+        object.
+        The generator may be called multiple times if libmpv seeks or loops.
+        See also: @mpv.python_stream_catchall
+        @mpv.python_stream('foobar')
+        def reader():
+            for chunk in chunks:
+                yield chunk
+        mpv.play('python://foobar')
+        mpv.wait_for_playback()
+        reader.unregister()
+        """
+        def register(cb):
+            if name in self._python_streams:
+                raise KeyError('Python stream name "{}" is already registered'.format(name))
+            self._python_streams[name] = (cb, size)
+            def unregister():
+                if name not in self._python_streams or\
+                        self._python_streams[name][0] is not cb: # This is just a basic sanity check
+                    raise RuntimeError('Python stream has already been unregistered')
+                del self._python_streams[name]
+            cb.unregister = unregister
+            return cb
+        return register
+
+    def python_stream_catchall(self, cb):
+        """ Register a catch-all python stream to be called when no name matches can be found. Use this decorator on a
+        function that takes a name argument and returns a (generator, size) tuple (with size being None if unknown).
+        An invalid URI can be signalled to libmpv by raising a ValueError inside the callback.
+        See also: @mpv.python_stream(name, size)
+        @mpv.python_stream_catchall
+        def catchall(name):
+            if not name.startswith('foo'):
+                raise ValueError('Unknown Name')
+            def foo_reader():
+                with open(name, 'rb') as f:
+                    while True:
+                        chunk = f.read(1024)
+                        if not chunk:
+                            break
+                        yield chunk
+            return foo_reader, None
+        mpv.play('python://foo23')
+        mpv.wait_for_playback()
+        catchall.unregister()
+        """
+        if self._python_stream_catchall is not None:
+            raise KeyError('A catch-all python stream is already registered')
+
+        self._python_stream_catchall = cb
+        def unregister():
+            if self._python_stream_catchall is not cb:
+                    raise RuntimeError('This catch-all python stream has already been unregistered')
+            self._python_stream_catchall = None
+        cb.unregister = unregister
+        return cb
+
     # Property accessors
     def _get_property(self, name, decoder=strict_decoder, fmt=MpvFormat.NODE):
+        self.check_core_alive()
         out = create_string_buffer(sizeof(MpvNode))
         try:
             cval = _mpv_get_property(self.handle, name.encode('utf-8'), fmt, out)
 
             if fmt is MpvFormat.OSD_STRING:
                 return cast(out, POINTER(c_char_p)).contents.value.decode('utf-8')
             elif fmt is MpvFormat.NODE:
@@ -1082,14 +1718,15 @@
                 return rv
             else:
                 raise TypeError('_get_property only supports NODE and OSD_STRING formats.')
         except PropertyUnavailableError as ex:
             return None
 
     def _set_property(self, name, value):
+        self.check_core_alive()
         ename = name.encode('utf-8')
         if isinstance(value, (list, set, dict)):
             _1, _2, _3, pointer = _make_node_str_list(value)
             _mpv_set_property(self.handle, ename, MpvFormat.NODE, pointer)
         else:
             _mpv_set_property_string(self.handle, ename, _mpv_coax_proptype(value))
 
@@ -1129,7 +1766,57 @@
 
     def option_info(self, name):
         """Get information on the given option."""
         try:
             return self._get_property('option-info/'+name)
         except AttributeError:
             return None
+
+class MpvRenderContext:
+    def __init__(self, mpv, api_type, **kwargs):
+        self._mpv = mpv
+        kwargs['api_type'] = api_type
+
+        buf = cast(create_string_buffer(sizeof(MpvRenderCtxHandle)), POINTER(MpvRenderCtxHandle))
+        _mpv_render_context_create(buf, mpv.handle, kwargs_to_render_param_array(kwargs))
+        self._handle = buf.contents
+
+    def free(self):
+        _mpv_render_context_free(self._handle)
+
+    def __setattr__(self, name, value):
+        if name.startswith('_'):
+            super().__setattr__(name, value)
+
+        elif name == 'update_cb':
+            func = value if value else (lambda: None)
+            self._update_cb = value
+            self._update_fn_wrapper = RenderUpdateFn(lambda _userdata: func())
+            _mpv_render_context_set_update_callback(self._handle, self._update_fn_wrapper, None)
+
+        else:
+            param = MpvRenderParam(name, value)
+            _mpv_render_context_set_parameter(self._handle, param)
+
+    def __getattr__(self, name):
+        if name == 'update_cb':
+            return self._update_cb
+
+        elif name == 'handle':
+            return self._handle
+
+        param = MpvRenderParam(name)
+        data_type = type(param.data.contents)
+        buf = cast(create_string_buffer(sizeof(data_type)), POINTER(data_type))
+        param.data = buf
+        _mpv_render_context_get_info(self._handle, param)
+        return buf.contents.as_dict()
+
+    def update(self):
+        """ Calls mpv_render_context_update and returns the MPV_RENDER_UPDATE_FRAME flag (see render.h) """
+        return bool(_mpv_render_context_update(self._handle) & 1)
+
+    def render(self, **kwargs):
+        _mpv_render_context_render(self._handle, kwargs_to_render_param_array(kwargs))
+
+    def report_swap(self):
+        _mpv_render_context_report_swap(self._handle)
```

### Comparing `feeluown-3.8.8/PKG-INFO` & `feeluown-3.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 3.8.8
+Version: 3.8.9
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
         
@@ -70,12 +70,12 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: battery
-Provides-Extra: webengine
-Provides-Extra: win32
 Provides-Extra: macOS
+Provides-Extra: win32
+Provides-Extra: webengine
+Provides-Extra: dev
```

### Comparing `feeluown-3.8.8/feeluown/nowplaying/linux/introspect.xml` & `feeluown-3.8.9/feeluown/nowplaying/linux/introspect.xml`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/nowplaying/linux/__init__.py` & `feeluown-3.8.9/feeluown/nowplaying/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/nowplaying/linux/mpris2.py` & `feeluown-3.8.9/feeluown/nowplaying/linux/mpris2.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/nowplaying/global_hotkey_mac.py` & `feeluown-3.8.9/feeluown/nowplaying/global_hotkey_mac.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/collection.py` & `feeluown-3.8.9/feeluown/collection.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/plugin.py` & `feeluown-3.8.9/feeluown/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         :param module: 插件模块对象，它有 enable 和 disable 方法
         :param desc: 插件描述
         :param author: 插件作者
         :param homepage: 插件主页
         :param dist_name: 插件发行版名字
         """
         self.alias = alias
-        self.name = module.__name__
+        # FIXME(cosven): use entry point name as plugin name, instead of the module name.
+        self.name = module.__name__.split('.')[-1]
         self._module = module
         self.version = version
         self.desc = desc
         self.author = author
         self.homepage = homepage
         self.dist_name = dist_name
         self.is_enabled = False
```

### Comparing `feeluown-3.8.8/feeluown/player/metadata.py` & `feeluown-3.8.9/feeluown/player/metadata.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/recently_played.py` & `feeluown-3.8.9/feeluown/player/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/base_player.py` & `feeluown-3.8.9/feeluown/player/base_player.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/radio.py` & `feeluown-3.8.9/feeluown/player/radio.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/__init__.py` & `feeluown-3.8.9/feeluown/player/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/mpvplayer.py` & `feeluown-3.8.9/feeluown/player/mpvplayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 import locale
 import logging
 
-from feeluown.utils.utils import use_mpv_old
-from .metadata import MetadataFields, Metadata
-
-if use_mpv_old():
-    from mpv_old import (  # type: ignore
-        MPV,
-        MpvEventID,
-        MpvEventEndFile,
-        _mpv_set_property_string,
-        _mpv_set_option_string,
-        _mpv_client_api_version,
-    )
-else:
-    from mpv import (  # type: ignore
-        MPV,
-        MpvEventID,
-        MpvEventEndFile,
-        _mpv_set_property_string,
-        _mpv_set_option_string,
-        _mpv_client_api_version,
-    )
+from mpv import (  # type: ignore
+    MPV,
+    MpvEventID,
+    MpvEventEndFile,
+    _mpv_set_property_string,
+    _mpv_set_option_string,
+    _mpv_client_api_version,
+)
 
 from feeluown.utils.dispatch import Signal
 from feeluown.media import Media, VideoAudioManifest
 from .base_player import AbstractPlayer, State
+from .metadata import MetadataFields, Metadata
 
 
 logger = logging.getLogger(__name__)
 
 
 class MpvPlayer(AbstractPlayer):
     """
```

### Comparing `feeluown-3.8.8/feeluown/player/lyric.py` & `feeluown-3.8.9/feeluown/player/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/fm.py` & `feeluown-3.8.9/feeluown/player/fm.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/player/playlist.py` & `feeluown-3.8.9/feeluown/player/playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from feeluown.excs import ProviderIOError
 from feeluown.utils import aio
 from feeluown.utils.dispatch import Signal
 from feeluown.utils.utils import DedupList
 from feeluown.player import Metadata, MetadataFields
 from feeluown.library import MediaNotFound, SongProtocol, ModelType, NotSupported
+from feeluown.media import Media
 from feeluown.models.uri import reverse
 
 logger = logging.getLogger(__name__)
 
 
 class PlaybackMode(IntEnum):
     """
@@ -436,16 +437,17 @@
                     self.songs_added.emit(index + 1, 1)
                 target_song = standby
             else:
                 self._app.show_msg('Song standby not found')
         except ProviderIOError as e:
             # FIXME: This may cause infinite loop when the prepare media always fails
             logger.error(f'prepare media failed: {e}, try next song')
-        except:  # noqa
+        except Exception as e:  # noqa
             # When the exception is unknown, we mark the song as bad.
+            self._app.show_msg(f'prepare media failed due to unknown error: {e}')
             logger.exception('prepare media failed due to unknown error, '
                              'so we mark the song as a bad one')
             self.mark_as_bad(song)
             self.next()
             return
         else:
             assert media, "media must not be empty"
@@ -487,16 +489,21 @@
             # The song.artists_name should return a list of strings
             MetadataFields.artists: [song.artists_name_display or ''],
             MetadataFields.album: song.album_name_display or '',
         })
         try:
             song = await aio.run_fn(self._app.library.song_upgrade, song)
             if song.album is not None:
-                album = self._app.library.album_upgrade(song.album)
+                album = await aio.run_fn(self._app.library.album_upgrade, song.album)
                 artwork = album.cover
+                # For model v1, the cover can be a Media object.
+                # For example, in fuo_local plugin, the album.cover is a Media
+                # object with url set to fuo://local/songs/{identifier}/data/cover.
+                if isinstance(artwork, Media):
+                    artwork = artwork.url
             else:
                 artwork = ''
         except NotSupported:
             # The song or the album can't be upgraded.
             pass
         except:  # noqa
             logger.exception(f"prepare metadata for song '{str(song)}' failed")
```

### Comparing `feeluown-3.8.8/feeluown/media.py` & `feeluown-3.8.9/feeluown/media.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/models/base.py` & `feeluown-3.8.9/feeluown/models/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/models/uri.py` & `feeluown-3.8.9/feeluown/models/uri.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/models/models.py` & `feeluown-3.8.9/feeluown/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,16 @@
 
 class SongModel(BaseModel, MultiQualityMixin):
     QualityCls = Quality.Audio
 
     class Meta:
         model_type = ModelType.song.value
         fields = ['album', 'artists', 'lyric', 'comments', 'title', 'url',
-                  'duration', 'mv', 'media']
+                  'duration', 'mv', 'media',
+                  'disc', 'genre', 'date', 'track', ]
         fields_display = ['title', 'artists_name', 'album_name', 'duration_ms']
 
         support_multi_quality = False
 
     @property
     def artists_name(self):
         return _get_artists_name(self.artists or [])
```

### Comparing `feeluown-3.8.8/feeluown/models/__init__.py` & `feeluown-3.8.9/feeluown/models/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/fuoexec/functions.py` & `feeluown-3.8.9/feeluown/fuoexec/functions.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/fuoexec/signal_manager.py` & `feeluown-3.8.9/feeluown/fuoexec/signal_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         """Connect all slots.
         """
         if self._signal is None:
             raise RuntimeError("no signal is bound")
 
         # Connect slot which are not symbol.
         # These slots are connected directly.
-        for slot, aioqueue in self._slot_list:
-            self._signal.connect(slot, weak=True, aioqueue=aioqueue)
+        for slot, kwargs in self._slot_list:
+            self._signal.connect(slot, **kwargs)
         self._slot_list.clear()
 
         # Connect slots which are symbol currently.
         self._signal.connect(self.slot_symbols_delegate, weak=False)
 
     def connect_slot(self, slot: Callable, **kwargs):
         if self._signal is not None:
```

### Comparing `feeluown-3.8.8/feeluown/fuoexec/fuoexec.py` & `feeluown-3.8.9/feeluown/fuoexec/fuoexec.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/entry_points/run_app.py` & `feeluown-3.8.9/feeluown/entry_points/run_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/entry_points/base.py` & `feeluown-3.8.9/feeluown/entry_points/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/entry_points/run.py` & `feeluown-3.8.9/feeluown/entry_points/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from feeluown.utils.patch import patch_janus, patch_qeventloop
+from feeluown.utils.patch import patch_janus, patch_qeventloop, patch_mutagen
 patch_janus()
+patch_mutagen()
 
 try:
     patch_qeventloop()
 except ImportError:
     # qasync/qt is not installed
     # FIXME: should not catch the error at here
     pass
```

### Comparing `feeluown-3.8.8/feeluown/library/model_protocol.py` & `feeluown-3.8.9/feeluown/library/model_protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/library/models.py` & `feeluown-3.8.9/feeluown/library/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -260,14 +260,19 @@
 class SongModel(BaseNormalModel):
     meta: Any = ModelMeta.create(ModelType.song, is_normal=True)
     title: str
     album: Optional[BriefAlbumModel]
     artists: List[BriefArtistModel]
     duration: int  # milliseconds
 
+    genre: str = ''
+    date: str = ''  # For example: 2020-12-11 00:00:00, 2020-12-11T00:00:00Z
+    track: str = '1/1'  # The number of the track on the album.
+    disc: str = '1/1'
+
     @property
     def artists_name(self):
         return fmt_artists(self.artists)
 
     @property
     def album_name(self):
         return self.album.name if self.album else ''
@@ -365,14 +370,23 @@
     # Since modelv1 playlist does not have creator field, it is set to optional.
     creator: Optional[BriefUserModel]
     name: str
     cover: str
     description: str
 
 
+class SimpleSearchResult(_BaseModel):
+    q: str
+    songs: List[BriefSongModel] = []
+    albums: List[BriefAlbumModel] = []
+    artists: List[BriefAlbumModel] = []
+    playlists: List[BriefPlaylistModel] = []
+    videos: List[BriefVideoModel] = []
+
+
 _type_modelcls_mapping = {
     ModelType.song: (SongModel, BriefSongModel),
     ModelType.album: (AlbumModel, BriefAlbumModel),
     ModelType.artist: (ArtistModel, BriefArtistModel),
     ModelType.video: (VideoModel, BriefVideoModel),
     ModelType.playlist: (PlaylistModel, BriefPlaylistModel),
     ModelType.user: (UserModel, BriefUserModel),
```

### Comparing `feeluown-3.8.8/feeluown/library/flags.py` & `feeluown-3.8.9/feeluown/library/flags.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,29 +17,14 @@
     playlists_rd = 0x00000080
 
     multi_quality = 0x0001000
     similar = 0x00002000
     hot_comments = 0x00008000
     web_url = 0x00010000
     model_v2 = 0x00004000
-    """
-    The provider uses ModelV2 for a specific resource.
-
-    When model_v2 is on, the way of fetching attributes is completely changed.
-    All fetching operations are performed by methods of library.
-
-    Before, if you want to get the title of a song, you should do::
-
-        title = await aio.run_fn(lambda: song.title)
-
-    Now if the provider use ModelV2, you can do::
-
-        upgraded_song = await aio.run_fn(library.song_upgrade, song)
-        title = upgrade_song.title
-    """
 
     current_user = 0x00100000
 
     # Impl: x_add_song(x, song)
     add_song = 0x01000000
     remove_song = 0x02000000
```

### Comparing `feeluown-3.8.8/feeluown/library/__init__.py` & `feeluown-3.8.9/feeluown/library/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 from .models import ModelFlags, BaseModel, ModelType, \
     SongModel, BriefSongModel, \
     BriefArtistModel, BriefAlbumModel, \
     BriefCommentModel, CommentModel, \
     BriefUserModel, UserModel, \
     LyricModel, VideoModel, BriefVideoModel, \
     ArtistModel, AlbumModel, PlaylistModel, BriefPlaylistModel, \
-    fmt_artists_names, \
+    fmt_artists_names, AlbumType, SimpleSearchResult, \
     get_modelcls_by_type, \
     V2SupportedModelTypes
 from .excs import NotSupported, NoUserLoggedIn, ModelNotFound, \
     ProviderAlreadyExists, ResourceNotFound, MediaNotFound
 from .provider_protocol import *
```

### Comparing `feeluown-3.8.8/feeluown/library/provider.py` & `feeluown-3.8.9/feeluown/library/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/library/model_state.py` & `feeluown-3.8.9/feeluown/library/model_state.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/library/provider_protocol.py` & `feeluown-3.8.9/feeluown/library/provider_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,24 @@
 
 ID = str
 _FlagProtocolMapping: Dict[Tuple[ModelType, PF], type] = {}
 
 
 def check_flag(provider, model_type: ModelType, flag: PF) -> bool:
     """Check if provider supports X"""
+
+    # A provider should declare explicitly whether it uses model v2 or not.
+    if flag is PF.model_v2:
+        try:
+            use_model_v2 = provider.use_model_v2(model_type)
+        except AttributeError:  # noqa
+            # The provider may not implement the `use_model_v2` interface.
+            return False
+        return use_model_v2
+
     protocol_cls = _FlagProtocolMapping[(model_type, flag)]
     return isinstance(provider, protocol_cls)
 
 
 def eq(model_type: ModelType, flag: PF):
     """Decorate a protocol class and associate it with a provider flag"""
     def wrapper(cls):
@@ -189,24 +199,33 @@
     @abstractmethod
     def artist_create_songs_rd(self, artist: BriefArtistProtocol):
         """Create songs reader of the artist
         """
         raise NotImplementedError
 
 
-@eq(ModelType.artist, PF.songs_rd)
+@eq(ModelType.artist, PF.albums_rd)
 @runtime_checkable
 class SupportsArtistAlbumsReader(Protocol):
     @abstractmethod
     def artist_create_albums_rd(self, artist: BriefArtistProtocol):
         """Create albums reader of the artist
         """
         raise NotImplementedError
 
 
+@runtime_checkable
+class SupportsArtistContributedAlbumsReader(Protocol):
+    @abstractmethod
+    def artist_create_contributed_albums_rd(self, artist: BriefArtistProtocol):
+        """Create contributed albums reader of the artist
+        """
+        raise NotImplementedError
+
+
 #
 # Protocols for Video related functions.
 #
 
 @eq(ModelType.video, PF.get)
 @runtime_checkable
 class SupportsVideoGet(Protocol):
```

### Comparing `feeluown-3.8.8/feeluown/library/library.py` & `feeluown-3.8.9/feeluown/library/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import warnings
 from functools import partial, lru_cache
 from typing import cast, Optional, Union
 
+from feeluown.excs import ModelCannotUpgrade
 from feeluown.media import Media
 from feeluown.models import SearchType, ModelType
 from feeluown.utils import aio
 from feeluown.utils.dispatch import Signal
 from feeluown.utils.utils import log_exectime
 from feeluown.utils.reader import create_reader
 from .provider import AbstractProvider
@@ -14,27 +15,28 @@
 from .excs import (
     NotSupported, MediaNotFound, NoUserLoggedIn, ProviderAlreadyExists,
     ProviderNotFound, ModelNotFound
 )
 from .flags import Flags as PF
 from .models import (
     ModelFlags as MF, BaseModel, BriefSongModel, UserModel,
-    get_modelcls_by_type, V2SupportedModelTypes,
+    get_modelcls_by_type,
 )
 from .model_protocol import (
     BriefVideoProtocol, ModelProtocol, BriefSongProtocol, SongProtocol, UserProtocol,
     LyricProtocol, VideoProtocol, BriefAlbumProtocol, BriefArtistProtocol
 )
+from .model_state import ModelState
 from .provider_protocol import (
-    check_flag,
+    check_flag as check_flag_impl,
     SupportsCurrentUser,
     SupportsSongLyric, SupportsSongMV, SupportsSongMultiQuality,
     SupportsPlaylistRemoveSong, SupportsPlaylistAddSong, SupportsPlaylistSongsReader,
     SupportsArtistSongsReader, SupportsArtistAlbumsReader,
-    SupportsVideoMultiQuality,
+    SupportsVideoMultiQuality, SupportsArtistContributedAlbumsReader,
 )
 
 
 logger = logging.getLogger(__name__)
 
 FULL_SCORE = 10
 MIN_SCORE = 5
@@ -396,18 +398,21 @@
              provider has. In the future, we may use typing.Protocol.
              So you should use :meth:`check_flags` method to check ability
              instead of compare provider flags directly.
         """
         provider = self.get(source)
         if provider is None:
             return False
-        if isinstance(provider, ProviderV2):
-            return provider.check_flags(model_type, flags)
-        # Always return false when the provider is not a v2 instance.
-        return False
+
+        # Check each flag.
+        for value in PF.__members__.values():
+            if value in PF(flags):
+                if check_flag_impl(provider, model_type, flags) is False:
+                    return False
+        return True
 
     def check_flags_by_model(self, model: ModelProtocol, flags: PF) -> bool:
         """Alias for check_flags"""
         warnings.warn('please use isintance(provider, protocol_cls)')
         return self.check_flags(model.source,
                                 ModelType(model.meta.model_type),
                                 flags)
@@ -485,18 +490,20 @@
 
         :raises NotSupported:
         :raises ProviderNotFound:
         """
         provider = self.get_or_raise(song.source)
         if isinstance(provider, SupportsSongMV):
             mv = provider.song_get_mv(song)
-        else:
+        elif not self.check_flags(song.source, song.meta.model_type, PF.model_v2):
             song_v1 = self.cast_model_to_v1(song)
             mv = song_v1.mv
             mv = cast(Optional[VideoProtocol], mv)
+        else:
+            mv = None
         return mv
 
     def song_get_lyric(self, song: BriefSongModel) -> Optional[LyricProtocol]:
         """
 
         Return None when lyric does not exist instead of raising exceptions,
         because it is predictable.
@@ -541,26 +548,38 @@
             artist = self.cast_model_to_v1(artist)
             if artist.meta.allow_create_songs_g:
                 reader = create_reader(artist.create_songs_g())
             else:
                 reader = create_reader(artist.songs)
         return reader
 
-    def artist_create_albums_rd(self, artist):
+    def artist_create_albums_rd(self, artist, contributed=False):
         """Create albums reader for artist model.
         """
         provider = self.get_or_raise(artist.source)
-        if isinstance(provider, SupportsArtistAlbumsReader):
-            reader = provider.artist_create_albums_rd(artist)
+        if contributed is False:
+            if isinstance(provider, SupportsArtistAlbumsReader):
+                reader = provider.artist_create_albums_rd(artist)
+            else:
+                artist = self.cast_model_to_v1(artist)
+                if artist.meta.allow_create_albums_g:
+                    reader = create_reader(artist.create_albums_g())
+                else:
+                    raise NotSupported("can't create albums reader for artist")
         else:
-            artist = self.cast_model_to_v1(artist)
-            if artist.meta.allow_create_albums_g:
-                reader = create_reader(artist.create_albums_g())
+            if isinstance(provider, SupportsArtistContributedAlbumsReader):
+                reader = provider.artist_create_contributed_albums_rd(artist)
             else:
-                raise NotSupported("can't create albums reader for artist")
+                artist = self.cast_model_to_v1(artist)
+                # Old code check if provider supports contributed_albums in this way.
+                if hasattr(artist, 'contributed_albums') and artist.contributed_albums:
+                    reader = create_reader(artist.create_contributed_albums_g())
+                else:
+                    raise NotSupported(
+                        "can't create contributed albums reader for artist")
         return reader
 
     # --------
     # Playlist
     # --------
 
     def playlist_upgrade(self, playlist):
@@ -622,16 +641,16 @@
         :raise NotSupported: provider has not .get for this model type
         :raise ResourceNotFound: model does not exist
         """
         provider = self.get_or_raise(pid)
         model = None
         try_v1way = True
         if isinstance(provider, ProviderV2):
-            if provider.check_flags(mtype, PF.model_v2):
-                if provider.check_flags(mtype, PF.get):
+            if provider.use_model_v2(mtype):
+                if self.check_flags(pid, mtype, PF.get):
                     try_v1way = False
                     model = provider.model_get(mtype, mid)
 
         # Try to use the ModelV1.get API to get the model.
         if try_v1way and isinstance(provider, AbstractProvider):
             try:
                 model_cls = provider.get_model_cls(mtype)
@@ -644,68 +663,72 @@
 
     def model_get_cover(self, model):
         """Get the cover url of model
 
         :param model: model which has a 'cover' field.
         :return: cover url if exists, else ''.
         """
-        cover = ''
         if MF.v2 in model.meta.flags:
-            if MF.normal in model.meta.flags:
-                cover = model.cover
-            else:
-                # TODO: upgrade artist model.
-                # Currently supported model types: (ModelType.album, ModelType.video).
-                if ModelType(model.meta.model_type) in V2SupportedModelTypes:
+            if MF.normal not in model.meta.flags:
+                try:
                     um = self._model_upgrade(model)
-                    # FIXME: remove this hack lator.
-                    if ModelType(model.meta.model_type) is ModelType.artist:
-                        cover = um.pic_url
-                    else:
-                        cover = um.cover
+                except (ModelCannotUpgrade, NotSupported):
+                    return ''
+            else:
+                um = model
+            # FIXME: remove this hack lator.
+            if ModelType(model.meta.model_type) is ModelType.artist:
+                cover = um.pic_url
+            else:
+                cover = um.cover
         else:
             cover = model.cover
             # Check if cover is a media object.
             if cover and not isinstance(cover, str):
                 cover = cover.url
         return cover
 
     def _model_upgrade(self, model):
         """
-        Thinking: currently, the caller must catch the NotSupported error.
+        :raises NotSupported: provider does't impl SupportGetProtocol for the model type
+        :raises CannotUpgrade: the model can't be upgraded
         """
-        try_v1way = True
-        upgraded_model = None
-        if model.meta.flags & MF.v2:
-            if MF.normal in model.meta.flags:
-                upgraded_model = model
-                try_v1way = False
-            else:
-                provider = self.getv2_or_raise(model.source)
-                # When the provider does not support 'get' for this model.
-                # Do not raise NotSupported here and try to use the v1 way.
-                #
-                # For example, provider X may support 'get' for SongModel, then
-                # the song.artists can return list of BriefArtistModel.
-                if check_flag(provider, ModelType(model.meta.model_type), PF.get):
-                    upgraded_model = provider.model_get(
-                        model.meta.model_type, model.identifier)
-                    try_v1way = False
-
-        if try_v1way is True:
-            v1model = self.cast_model_to_v1(model)
-            modelcls = get_modelcls_by_type(ModelType(model.meta.model_type))
-            fields = [f for f in list(modelcls.__fields__)
-                      if f not in list(BaseModel.__fields__)]
-            for field in fields:
-                getattr(v1model, field)
-            upgraded_model = v1model
-        else:
-            assert upgraded_model is not None
-        return upgraded_model
+        # Upgrade model in v1 way if it is a v1 model.
+        if MF.v2 not in model.meta.flags:
+            return self._model_upgrade_in_v1_way(model)
+
+        # Return model directly if it is already a normal model.
+        if MF.normal in model.meta.flags:
+            return model
+
+        provider = self.getv2_or_raise(model.source)
+        model_type = ModelType(model.meta.model_type)
+        is_support = check_flag_impl(provider, model_type, PF.get)
+        if is_support:
+            upgraded_model = provider.model_get(model_type, model.identifier)
+            if upgraded_model is None:
+                model.state = ModelState.not_exists
+                raise ModelCannotUpgrade('model does not exist')
+            return upgraded_model
+
+        # Fallback to v1 way if the provider does not support PF.get.
+        # For example, provider X may support 'get' for SongModel and it
+        # does not support 'get' for ArtistModel temporarily. It returns
+        # a SongModel and the song.artists returns list of BriefArtistModel,
+        # in this condition, BriefArtistModel should be upgraded in v1 way.
+        return self._model_upgrade_in_v1_way(model)
+
+    def _model_upgrade_in_v1_way(self, model):
+        v1model = self.cast_model_to_v1(model)
+        modelcls = get_modelcls_by_type(ModelType(model.meta.model_type))
+        fields = [f for f in list(modelcls.__fields__)
+                  if f not in list(BaseModel.__fields__)]
+        for field in fields:
+            getattr(v1model, field)
+        return v1model
 
     # --------
     # Video
     # --------
     def video_upgrade(self, video):
         return self._model_upgrade(video)
```

### Comparing `feeluown-3.8.8/feeluown/argparser.py` & `feeluown-3.8.9/feeluown/argparser.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/version.py` & `feeluown-3.8.9/feeluown/version.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/dslv2.py` & `feeluown-3.8.9/feeluown/server/dslv2.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/protocol.py` & `feeluown-3.8.9/feeluown/server/protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/dslv1/parser.py` & `feeluown-3.8.9/feeluown/server/dslv1/parser.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/dslv1/codegen.py` & `feeluown-3.8.9/feeluown/server/dslv1/codegen.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/dslv1/lexer.py` & `feeluown-3.8.9/feeluown/server/dslv1/lexer.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/show.py` & `feeluown-3.8.9/feeluown/server/handlers/show.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/base.py` & `feeluown-3.8.9/feeluown/server/handlers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/exec_.py` & `feeluown-3.8.9/feeluown/server/handlers/exec_.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/search.py` & `feeluown-3.8.9/feeluown/server/handlers/search.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/handle.py` & `feeluown-3.8.9/feeluown/server/handlers/handle.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/help.py` & `feeluown-3.8.9/feeluown/server/handlers/help.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/player.py` & `feeluown-3.8.9/feeluown/server/handlers/player.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/playlist.py` & `feeluown-3.8.9/feeluown/server/handlers/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/handlers/sub.py` & `feeluown-3.8.9/feeluown/server/handlers/sub.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/excs.py` & `feeluown-3.8.9/feeluown/server/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/data_structure.py` & `feeluown-3.8.9/feeluown/server/data_structure.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/__init__.py` & `feeluown-3.8.9/feeluown/server/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/pubsub/publishers.py` & `feeluown-3.8.9/feeluown/server/pubsub/publishers.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/pubsub/gateway.py` & `feeluown-3.8.9/feeluown/server/pubsub/gateway.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/server/server.py` & `feeluown-3.8.9/feeluown/server/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/excs.py` & `feeluown-3.8.9/feeluown/excs.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,21 @@
 
     For example, a model identifier is invalid.
 
     .. versionadded:: 3.7.7
     """
 
 
+class ModelCannotUpgrade(LibraryException):
+    """Model cannot be upgraded
+
+    .. versionadded:: 3.8.9
+    """
+
+
 class NotSupported(LibraryException):
     """Provider does not support the operation
     """
 
 
 class MediaNotFound(ResourceNotFound):
     pass
```

### Comparing `feeluown-3.8.8/feeluown/cli/install.py` & `feeluown-3.8.9/feeluown/cli/install.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/cli/cli.py` & `feeluown-3.8.9/feeluown/cli/cli.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/__init__.py` & `feeluown-3.8.9/feeluown/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import logging.config
 
 from .consts import LOG_FILE
 
 
-__version__ = '3.8.8'
+__version__ = '3.8.9'
 
 
 dict_config = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
```

### Comparing `feeluown-3.8.8/feeluown/app/app.py` & `feeluown-3.8.9/feeluown/app/app.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/app/server_app.py` & `feeluown-3.8.9/feeluown/app/server_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/app/gui_app.py` & `feeluown-3.8.9/feeluown/app/gui_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,17 @@
 
     def run(self):
         super().run()
         self.show()
 
     def load_state(self):
         super().load_state()
-        self.browser.goto(page='/player_playlist')
+        coll_library = self.coll_uimgr.get_coll_library()
+        coll_id = self.coll_uimgr.get_coll_id(coll_library)
+        self.browser.goto(page=f'/colls/{coll_id}')
 
     def closeEvent(self, _):
         if not self.config.ENABLE_TRAY:
             self.exit()
 
     def mouseReleaseEvent(self, e):
         if not self.rect().contains(e.pos()):
```

### Comparing `feeluown-3.8.8/feeluown/app/config.py` & `feeluown-3.8.9/feeluown/app/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/app/cli_app.py` & `feeluown-3.8.9/feeluown/app/cli_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/json_.py` & `feeluown-3.8.9/feeluown/serializers/json_.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/plain.py` & `feeluown-3.8.9/feeluown/serializers/plain.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/_plain_formatter.py` & `feeluown-3.8.9/feeluown/serializers/_plain_formatter.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/base.py` & `feeluown-3.8.9/feeluown/serializers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/python.py` & `feeluown-3.8.9/feeluown/serializers/python.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/model_helpers.py` & `feeluown-3.8.9/feeluown/serializers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/__init__.py` & `feeluown-3.8.9/feeluown/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/serializers/objs.py` & `feeluown-3.8.9/feeluown/serializers/objs.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/tray.py` & `feeluown-3.8.9/feeluown/gui/tray.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/comment_list.py` & `feeluown-3.8.9/feeluown/gui/widgets/comment_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 
 from PyQt5.QtCore import QAbstractListModel, QModelIndex, Qt, QSize, \
     QPoint, QRect
-from PyQt5.QtGui import QPalette, QPen, QFont
-from PyQt5.QtWidgets import QStyledItemDelegate, QListView, QSizePolicy, QFrame
+from PyQt5.QtGui import QPalette, QPen, QFont, QFontMetrics
+from PyQt5.QtWidgets import QStyledItemDelegate, QListView, QSizePolicy, QFrame, \
+    QApplication
 
 from feeluown.gui.helpers import ItemViewNoScrollMixin, Paddings, Margins
 
 
 def human_readable_number_v1(n):
     levels = [(100000000, '亿'),
               (10000, '万')]
@@ -46,15 +47,15 @@
 class CommentListDelegate(QStyledItemDelegate):
     def __init__(self, parent):
         super().__init__(parent=parent)
 
         self._margin_h = 0
         self._margin_v = 10
         self._name_content_margin = 5
-        self._name_height = 15
+        self._name_height = QFontMetrics(QApplication.font()).height()
         self._parent_comment_paddings = Paddings(8, 3, 8, 3)
         self._parent_comment_margins = Margins(20, 5, 10, 5)
 
     def paint(self, painter, option, index):
         painter.save()
         comment = index.data(Qt.UserRole)
         fm = option.fontMetrics
@@ -196,15 +197,14 @@
             row_count -= 1
             height += self.sizeHintForRow(row_count)
         return height
 
 
 if __name__ == '__main__':
     import time
-    from PyQt5.QtWidgets import QApplication
     from feeluown.utils.reader import wrap
     from feeluown.library.models import CommentModel, BriefUserModel, BriefCommentModel
 
     user = BriefUserModel(identifier='fuo-bot',
                           source='fuo',
                           name='随风而去')
     content = ('有没有一首歌会让你很想念，有没有一首歌你会假装听不见，'
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/mpv.py` & `feeluown-3.8.9/feeluown/gui/widgets/mpv.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/collections.py` & `feeluown-3.8.9/feeluown/gui/widgets/collections.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/video.py` & `feeluown-3.8.9/feeluown/gui/widgets/video.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,41 +2,46 @@
 from PyQt5.QtGui import QColor, QPalette
 from PyQt5.QtWidgets import QVBoxLayout, QPushButton, QWidget, \
     QHBoxLayout, QOpenGLWidget, QLabel
 
 from feeluown.player import State
 from feeluown.gui.widgets.progress_slider import ProgressSlider
 from feeluown.gui.widgets.size_grip import SizeGrip
+from feeluown.gui.widgets.textbtn import TextButton
 from .labels import ProgressLabel, DurationLabel
 
 
 class VideoPlayerCtlBar(QWidget):
+
     def __init__(self, app, parent=None):
         super().__init__(parent=parent)
 
         self._app = app
 
         # Create widgets.
         self._toggle_btn = QPushButton()
         self._progress_slider = ProgressSlider(app)
         self._progress_label = ProgressLabel(app, self)
         self._duration_label = DurationLabel(app, self)
+        #: Toggle fullscreen button.
+        self._fullscreen_btn = TextButton("全屏")
         self._size_grip = SizeGrip(parent=self)
         self._layout = QVBoxLayout(self)
         self._bottom_layout = QHBoxLayout()
 
         # Do initialization for widgets.
         self._toggle_btn.setCheckable(True)
         self._setup_ui()
 
         self._app.player.state_changed.connect(
             lambda x: self._toggle_btn.setChecked(x == State.playing),
             weak=False,
             aioqueue=True)
         self._toggle_btn.clicked.connect(self._app.player.toggle)
+        self._fullscreen_btn.clicked.connect(self._app.watch_mgr.toggle_pip_fullscreen)
 
     def _setup_ui(self):
         self.setAutoFillBackground(True)
         # TODO: rename the ObjectName.
         self._toggle_btn.setObjectName('video_pp_btn')
 
         # Setup layout.
@@ -52,24 +57,28 @@
         self._bottom_layout.addSpacing(8)
         self._bottom_layout.addWidget(self._progress_label)
         self._bottom_layout.addSpacing(2)
         self._bottom_layout.addWidget(QLabel('/', self))
         self._bottom_layout.addSpacing(2)
         self._bottom_layout.addWidget(self._duration_label)
         self._bottom_layout.addStretch(1)
+        self._bottom_layout.addWidget(self._fullscreen_btn)
+        self._bottom_layout.addSpacing(8)
         self._bottom_layout.addWidget(self._size_grip)
 
         # Setup widgets size.
         self._size_grip.setFixedSize(20, 20)
+        self._fullscreen_btn.setFixedHeight(20)
         # Button size should be same as the value defined in style sheet.
         self._toggle_btn.setFixedSize(24, 24)
 
         # Customize the palette.
         palette = self.palette()
         palette.setColor(QPalette.Text, QColor('white'))
+        palette.setColor(QPalette.ButtonText, QColor('white'))
         palette.setColor(QPalette.WindowText, QColor('white'))
         bg_color = QColor('black')
         bg_color.setAlpha(180)  # Make it semi-transparent.
         palette.setColor(QPalette.Window, bg_color)
         self.setPalette(palette)
         # It seems children don't inherit the palette, so we set palette for
         # children explicitly.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/magicbox.py` & `feeluown-3.8.9/feeluown/gui/widgets/magicbox.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/meta.py` & `feeluown-3.8.9/feeluown/gui/widgets/meta.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/cover_label.py` & `feeluown-3.8.9/feeluown/gui/widgets/cover_label.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/tabbar.py` & `feeluown-3.8.9/feeluown/gui/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/volume_button.py` & `feeluown-3.8.9/feeluown/gui/widgets/volume_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/table_toolbar.py` & `feeluown-3.8.9/feeluown/gui/widgets/table_toolbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/video_list.py` & `feeluown-3.8.9/feeluown/gui/widgets/video_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/separator.py` & `feeluown-3.8.9/feeluown/gui/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/artist.py` & `feeluown-3.8.9/feeluown/gui/widgets/artist.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/album.py` & `feeluown-3.8.9/feeluown/gui/widgets/album.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def filterAcceptsRow(self, source_row, source_parent):
         accepted = super().filterAcceptsRow(source_row, source_parent)
         source_model = self.sourceModel()
         index = source_model.index(source_row, parent=source_parent)
         album = index.data(Qt.UserRole)
         if accepted and self.types:
-            accepted = AlbumType(album.type) in self.types
+            accepted = AlbumType(album.type_) in self.types
         return accepted
 
 
 class AlbumListView(ImgListView):
     show_album_needed = pyqtSignal([object])
 
     def __init__(self, *args, **kwargs):
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/menu.py` & `feeluown-3.8.9/feeluown/gui/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/settings.py` & `feeluown-3.8.9/feeluown/gui/widgets/settings.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/statusline_items/plugin.py` & `feeluown-3.8.9/feeluown/gui/widgets/statusline_items/plugin.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/statusline_items/notify.py` & `feeluown-3.8.9/feeluown/gui/widgets/statusline_items/notify.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/labels.py` & `feeluown-3.8.9/feeluown/gui/widgets/labels.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/my_music.py` & `feeluown-3.8.9/feeluown/gui/widgets/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/imglist.py` & `feeluown-3.8.9/feeluown/gui/widgets/imglist.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,25 +74,26 @@
             self.no_more_item.emit()
             return
         items_len = len(items)
         colors = [random.choice(list(COLORS.values())) for _ in range(0, items_len)]
         self.colors.extend(colors)
         self.on_items_fetched(items)
         for item in items:
-            aio.create_task(self.fetch_image(
-                item,
-                self._fetch_image_callback(item),
-                uid=reverse(item) + '/cover'))
+            aio.create_task(self.fetch_image(item, self._fetch_image_callback(item)))
 
     def _fetch_image_callback(self, item):
         def cb(content):
+            uri = reverse(item)
+            if content is None:
+                self.pixmaps[uri] = None
+                return
+
             img = QImage()
             img.loadFromData(content)
             pixmap = QPixmap(img)
-            uri = reverse(item)
             self.pixmaps[uri] = pixmap
             row = self._items.index(item)
             top_left = self.createIndex(row, 0)
             bottom_right = self.createIndex(row, 0)
             self.dataChanged.emit(top_left, bottom_right)
         return cb
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/progress_slider.py` & `feeluown-3.8.9/feeluown/gui/widgets/progress_slider.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/provider.py` & `feeluown-3.8.9/feeluown/gui/widgets/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from PyQt5.QtCore import Qt, QSize, QRectF, QRect, QPoint
 from PyQt5.QtGui import QPainter, QTextOption, QPalette, QBrush, QColor, \
     QGuiApplication  # noqa
 from PyQt5.QtWidgets import QStyledItemDelegate, QListView
 from PyQt5.QtSvg import QSvgRenderer
 
 from feeluown.library import ModelType, ProviderFlags as PF
-from feeluown.gui.helpers import ItemViewNoScrollMixin, resize_font, SOLARIZED_COLORS
+from feeluown.gui.helpers import ItemViewNoScrollMixin, SOLARIZED_COLORS
 from .textlist import TextlistModel
 
 
 class ProvidersModel(TextlistModel):
     def __init__(self, library, parent=None):
         super().__init__(parent)
         self._library = library
@@ -45,16 +45,16 @@
 
 
 class ProvidersDelegate(QStyledItemDelegate):
     def __init__(self, parent=None, library=None):
         super().__init__(parent)
         self._library = library
 
-        self._radius = 22
-        self._padding = 6
+        self._radius = 24
+        self._padding = 7
 
         self.__body_radius = self._radius - self._padding
         self.__text_rect_x = self.__body_radius - self.__body_radius / math.sqrt(2)
         self.__text_rect_width = 2 * (self.__body_radius / math.sqrt(2))
 
     def paint(self, painter, option, index):
         painter.setRenderHint(QPainter.Antialiasing)
@@ -83,15 +83,15 @@
             pen.setColor(non_text_color)
             painter.setPen(pen)
             painter.drawRoundedRect(body_rect, w//2, h//2)
             painter.restore()
 
             painter.save()
             font = painter.font()
-            resize_font(font, -3)
+            font.setPixelSize(10)
             painter.setFont(font)
             text_option = QTextOption()
             text_option.setWrapMode(QTextOption.WrapAtWordBoundaryOrAnywhere)
             text_option.setAlignment(Qt.AlignCenter)
 
             text_rect = QRectF(self.__text_rect_x, self.__text_rect_x,
                                self.__text_rect_width, self.__text_rect_width)
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/textlist.py` & `feeluown-3.8.9/feeluown/gui/widgets/textlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/lyric.py` & `feeluown-3.8.9/feeluown/gui/widgets/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/frameless.py` & `feeluown-3.8.9/feeluown/gui/widgets/frameless.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         self.setWindowFlags(Qt.WindowStaysOnTopHint | Qt.FramelessWindowHint)
         self._layout = QVBoxLayout(self)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.setSpacing(0)
 
         self.setMouseTracking(True)
 
-        QShortcut(QKeySequence.Cancel, self).activated.connect(self.hide)
+        QShortcut(QKeySequence.Cancel, self).activated.connect(
+            self.on_cancel_key_pressed)
 
     def attach_widget(self, widget):
         """set inner widget"""
         self._widget = widget
         self._widget.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self._layout.insertWidget(0, self._widget)
 
@@ -54,14 +55,20 @@
 
     def mouseReleaseEvent(self, e):
         self._old_pos = None
 
     def resizeEvent(self, e):
         super().resizeEvent(e)
 
+    def on_cancel_key_pressed(self):
+        if Qt.WindowFullScreen & self.windowState():
+            self.setWindowState(self.windowState() ^ Qt.WindowFullScreen)
+        else:
+            self.hide()
+
 
 if __name__ == '__main__':
     from PyQt5.QtWidgets import QApplication, QLabel
 
     app = QApplication([])
     widget = QLabel("hello world!")
     window = ResizableFramelessContainer()
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/playlist_button.py` & `feeluown-3.8.9/feeluown/gui/widgets/playlist_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/weblogin.py` & `feeluown-3.8.9/feeluown/gui/widgets/weblogin.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/playlists.py` & `feeluown-3.8.9/feeluown/gui/widgets/playlists.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/playlist.py` & `feeluown-3.8.9/feeluown/gui/widgets/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/messageline.py` & `feeluown-3.8.9/feeluown/gui/widgets/messageline.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/songs.py` & `feeluown-3.8.9/feeluown/gui/widgets/songs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from functools import partial
 
 from PyQt5.QtCore import (
     pyqtSignal, Qt, QVariant, QEvent,
     QAbstractTableModel, QAbstractListModel, QModelIndex,
     QSize, QRect, QPoint, QPointF, QSortFilterProxyModel,
 )
-from PyQt5.QtGui import QPainter, QPalette, QPen, QMouseEvent, QPolygonF
+from PyQt5.QtGui import QPainter, QPalette, QMouseEvent, QPolygonF
 from PyQt5.QtWidgets import (
     QAction, QFrame, QHBoxLayout, QAbstractItemView, QHeaderView,
     QPushButton, QTableView, QWidget, QMenu, QListView,
-    QStyle, QSizePolicy, QStyledItemDelegate,
+    QStyle, QSizePolicy, QStyledItemDelegate
 )
 
 from feeluown.utils import aio
 from feeluown.utils.dispatch import Signal
 from feeluown.library import ModelState, ModelFlags
 from feeluown.models import ModelExistence
 
@@ -235,16 +235,16 @@
             self._items.pop(row)
             count -= 1
         self.endRemoveRows()
         return True
 
     def flags(self, index):
         # Qt.NoItemFlags is ItemFlag and we should return ItemFlags
-        no_item_flags = Qt.ItemIsSelectable
-        if index.column() in (Column.source, Column.index, Column.duration):
+        no_item_flags = Qt.ItemIsSelectable | Qt.ItemIsEnabled
+        if index.column() in (Column.index, Column.source, Column.duration):
             return no_item_flags
 
         # Default flags.
         flags = Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemIsDragEnabled
         song = index.data(Qt.UserRole)
         # If song's state is `not_exists` or `cant_upgrade`, the album and
         # artist columns are disabled.
@@ -463,63 +463,49 @@
             if index.isValid():
                 artist = index.data(Qt.UserRole)
                 self.view.show_artist_needed.emit(artist)
         super().setModelData(editor, model, index)
 
     def paint(self, painter, option, index):
         super().paint(painter, option, index)
-
         painter.setRenderHint(QPainter.Antialiasing)
         hovered = index.row() == self.row_hovered
 
         # Draw play button on Column.index when the row is hovered.
         if hovered and index.column() == Column.index:
             painter.save()
-            # Override contents.
-            if option.state & QStyle.State_Selected:  # type: ignore
-                bgcolor = option.palette.color(QPalette.Active, QPalette.Highlight)
-                fgcolor = option.palette.color(QPalette.Active, QPalette.HighlightedText)
-            else:
-                bgcolor = option.palette.color(QPalette.Active, QPalette.Base)
-                fgcolor = option.palette.color(QPalette.Active, QPalette.Text)
-            painter.setBrush(bgcolor)
+            # Override the content drawed by super().paint.
             painter.setPen(Qt.NoPen)
+            # HELP(cosven): when an item was hovered, super().paint may draw
+            # a semi-transparent rect over the item or draw a different color
+            # for the text. The rect/text color may not be in the palette.
+            # I checked the qt source code, and I think this behaviour is
+            # platform indenpent.It is drawed by something like KDE, kvantum.
+            # We have no way to draw a similar look (or please help find a way).
+            if index.row() % 2 == 0:
+                painter.setBrush(option.palette.color(QPalette.Base))
+            else:
+                painter.setBrush(option.palette.color(QPalette.AlternateBase))
             painter.drawRect(option.rect)
             # Draw play button.
+            painter.setBrush(option.palette.color(QPalette.Text))
             triangle_edge = 12
             triangle_height = 10
-            painter.setBrush(fgcolor)
             # Move the triangle right 2px and it looks better.
             painter.translate(
                 2 + option.rect.x() + (option.rect.width() - triangle_height)//2,
                 option.rect.y() + (option.rect.height() - triangle_edge)//2
             )
             triangle = QPolygonF([QPointF(0, 0),
                                   QPointF(triangle_height, triangle_edge//2),
                                   QPointF(0, triangle_edge)])
             painter.drawPolygon(triangle)
             painter.restore()
 
-        # Draw a line under each row. If it is hovered, highlight the line.
-        painter.save()
-        pen = QPen()
-        line_color = option.palette.color(QPalette.Active, QPalette.Text)
-        line_color.setAlpha(30)
-        pen.setColor(line_color)
-        painter.setPen(pen)
-        bottom_left = option.rect.bottomLeft()
-        bottom_right = option.rect.bottomRight()
-        if index.model().columnCount() - 1 == index.column():
-            bottom_right = QPoint(bottom_right.x(), bottom_right.y())
-        if index.column() == 0:
-            bottom_left = QPoint(bottom_left.x(), bottom_right.y())
-        painter.drawLine(bottom_left, bottom_right)
-        painter.restore()
-
-        # Draw the mask over the row.
+        # Since the selection behaviour is SelectRows, so draw the mask over the row.
         if hovered:
             painter.save()
             mask_color = option.palette.color(QPalette.Active, QPalette.Text)
             mask_color.setAlpha(20)
             painter.setPen(Qt.NoPen)
             painter.setBrush(mask_color)
             painter.drawRect(option.rect)
@@ -572,15 +558,14 @@
         super().__init__(parent)
         QTableView.__init__(self, parent)
 
         self._app = app
 
         # override ItemViewNoScrollMixin variables
         self._least_row_count = 6
-        self._row_height = 40
 
         # slot functions
         self.remove_song_func = None
 
         self.delegate = SongsTableDelegate(app, self)
         self.setItemDelegate(self.delegate)
         self.about_to_show_menu = Signal()
@@ -590,17 +575,17 @@
         self.entered.connect(lambda index: self.row_hovered.emit(index.row()))
 
     def _setup_ui(self):
         self.horizontalHeader().setSectionResizeMode(QHeaderView.ResizeToContents)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setFrameShape(QFrame.NoFrame)
+        self.setAlternatingRowColors(True)
         self.verticalHeader().hide()
         self.horizontalHeader().hide()
-        self.verticalHeader().setDefaultSectionSize(self._row_height)
         self.setWordWrap(False)
         self.setTextElideMode(Qt.ElideRight)
         self.setMouseTracking(True)
         self.setEditTriggers(QAbstractItemView.SelectedClicked)
         self.setSelectionMode(QAbstractItemView.ExtendedSelection)
         # Note that the selection behavior affects drop behavior.
         # You may need to to change the Model.flags and mimeData methods
```

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/statusline.py` & `feeluown-3.8.9/feeluown/gui/widgets/statusline.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/widgets/login.py` & `feeluown-3.8.9/feeluown/gui/widgets/login.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/image.py` & `feeluown-3.8.9/feeluown/gui/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 from functools import partial
 import logging
 import os
 import time
 from hashlib import md5
 
-from feeluown.models import resolve
 from feeluown.consts import CACHE_DIR
 
 
 logger = logging.getLogger(__name__)
 
 
 class ImgManager(object):
@@ -27,16 +26,22 @@
         if fpath is not None:
             with open(fpath, 'rb') as f:
                 content = f.read()
             return content
         return None
 
     async def get(self, img_url, img_name):
-        if img_url.startswith('fuo://'):
-            return resolve(img_url)
+        if img_url.startswith('fuo://local'):
+            # Before, `models.uri.resolve` is uesd to handle these non-std paths,
+            # and it is not elegant in fact :(
+            # HACK(cosven): please think about a better way in the future.
+            provider = self._app.library.get('local')
+            if provider is None:
+                return None
+            return provider.handle_with_path(img_url[11:])
         fpath = self.cache.get(img_name)
         if fpath is not None:
             logger.info('read image:%s from cache', img_name)
             with open(fpath, 'rb') as f:
                 content = f.read()
             self.cache.update(img_name)
             return content
```

### Comparing `feeluown-3.8.8/feeluown/gui/pages/song_explore.py` & `feeluown-3.8.9/feeluown/gui/pages/song_explore.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from feeluown.gui.widgets.cover_label import CoverLabelV2
 from feeluown.gui.widgets.comment_list import CommentListView, CommentListModel
 from feeluown.gui.widgets.songs import SongListView, SongListModel
 
 logger = logging.getLogger(__name__)
 
 
-async def render(req, **kwargs):  # pylint: disable=too-many-locals
+async def render(req, **kwargs):  # pylint: disable=too-many-locals,too-many-branches
     app = req.ctx['app']
     song = req.ctx['model']
 
     try:
         provider = app.library.get_or_raise(song.source)
     except ProviderNotFound as e:
         view = InlineErrorMessageView()
@@ -93,15 +93,16 @@
                 sentences.append(sentence)
             view.lyric_label.set_lyric('\n'.join(sentences))
 
     # Show album cover in the end since it's an expensive CPU/IO operation.
     # FIXME: handle NotSupported exception
     if song.album is not None:
         album = await aio.run_fn(app.library.album_upgrade, song.album)
-        aio.create_task(view.cover_label.show_cover(album.cover, reverse(album)))
+        if album.cover:
+            aio.create_task(view.cover_label.show_cover(album.cover, reverse(album)))
 
 
 class ScrollArea(QScrollArea, BgTransparentMixin):
     def __init__(self, app, parent=None):
         super().__init__(parent=parent)
 
         self._app = app
```

### Comparing `feeluown-3.8.8/feeluown/gui/pages/model.py` & `feeluown-3.8.9/feeluown/gui/pages/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,21 @@
 
         self.render_tab_bar()
 
         if tab_index == 0:
             self.show_desc(self.model.description)
         elif tab_index == 1:
             await self._show_songs()
-        elif tab_index == 2:
+        elif tab_index in (2, 3):
+            contributed = tab_index == 3
             self.toolbar.filter_albums_needed.connect(
                 lambda types: self.albums_table.model().filter_by_types(types))
-            reader = await aio.run_fn(self._app.library.artist_create_albums_rd, artist)
+            reader = await aio.run_fn(
+                self._app.library.artist_create_albums_rd, artist, contributed)
             self.show_albums(reader)
-        elif tab_index == 3:
-            if hasattr(artist, 'contributed_albums') and artist.contributed_albums:
-                # This model must be v1.
-                self.show_albums(artist.create_contributed_albums_g())
 
         # finally, we render cover
         cover = artist.pic_url
         if cover:
             await self.show_cover(cover,
                                   reverse(artist) + '/cover',
                                   as_background=True)
```

### Comparing `feeluown-3.8.8/feeluown/gui/pages/coll_mixed.py` & `feeluown-3.8.9/feeluown/gui/pages/coll_mixed.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/uimodels/collection.py` & `feeluown-3.8.9/feeluown/gui/uimodels/collection.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/uimodels/my_music.py` & `feeluown-3.8.9/feeluown/gui/uimodels/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/uimodels/provider.py` & `feeluown-3.8.9/feeluown/gui/uimodels/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/uimodels/playlist.py` & `feeluown-3.8.9/feeluown/gui/uimodels/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/page_containers/table.py` & `feeluown-3.8.9/feeluown/gui/page_containers/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 import warnings
 from contextlib import suppress
 
 from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QImage, QPixmap
+from PyQt5.QtGui import QImage, QPixmap, QPalette
 from PyQt5.QtWidgets import QFrame, QVBoxLayout, QLabel, QApplication
 from requests.exceptions import RequestException
 
 from feeluown.utils import aio
 from feeluown.utils.reader import wrap
 from feeluown.media import Media, MediaType
 from feeluown.excs import ProviderIOError
@@ -235,14 +235,16 @@
     def __init__(self, parent=None):
         super().__init__(parent=parent)
 
         self.setContentsMargins(30, 15, 30, 10)
         self.setWordWrap(True)
         self.setTextInteractionFlags(Qt.TextSelectableByMouse)
 
+        self.palette().setColor(QPalette.Background, self.palette().color(QPalette.Base))
+
 
 class TableContainer(QFrame, BgTransparentMixin):
     def __init__(self, app, parent=None):
         super().__init__(parent)
 
         self._app = app
         self._renderer = None
@@ -300,15 +302,14 @@
         self.desc_widget.hide()
 
         self._layout = QVBoxLayout(self)
         self._v_layout = QVBoxLayout()
 
         self._v_layout.addWidget(self.meta_widget)
         self._v_layout.addWidget(self.toolbar)
-        self._v_layout.addSpacing(10)
         self._v_layout.addWidget(self.desc_widget)
 
         # Since QTableView has a margin on the left and right(see SongsTableDelegate),
         # so set the v_layout left margin to same value(0) to align widgets.
         self._v_layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addLayout(self._v_layout)
         for table in self._tables:
@@ -490,17 +491,17 @@
                         self._app.playlist.clear()
                         self._app.playlist.set_models(songs)
             self._app.playlist.play_model(song)
         else:
             try:
                 song = await aio.run_in_executor(
                     None, self._app.library.song_upgrade, song)
-            except NotSupported:
+            except NotSupported as e:
                 assert ModelFlags.v2 & song.meta.flags
-                self._app.show_msg('资源提供放不支持该功能')
+                self._app.show_msg(f'资源提供方不支持该功能: {str(e)}')
                 logger.info(f'provider:{song.source} does not support song_get')
                 song.state = ModelState.cant_upgrade
             except (ProviderIOError, RequestException) as e:
                 # FIXME: we should only catch ProviderIOError here,
                 # but currently, some plugins such fuo-qqmusic may raise
                 # requests.RequestException
                 logger.exception('upgrade song failed')
```

### Comparing `feeluown-3.8.8/feeluown/gui/ui.py` & `feeluown-3.8.9/feeluown/gui/ui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import logging
 from PyQt5.QtWidgets import QSizePolicy, QSplitter, QVBoxLayout
 
-from feeluown.utils.utils import use_mpv_old
 from feeluown.gui.widgets.separator import Separator
 from feeluown.gui.widgets.settings import SettingsDialog
 from feeluown.gui.widgets.messageline import MessageLine
 
-if use_mpv_old():
-    from feeluown.gui.widgets.mpv_old import MpvOpenGLWidget
-else:
-    from feeluown.gui.widgets.mpv import MpvOpenGLWidget
+from feeluown.gui.widgets.mpv import MpvOpenGLWidget
 
 from feeluown.gui.uimain.sidebar import LeftPanel
 from feeluown.gui.uimain.page_view import RightPanel
 from feeluown.gui.uimain.player_bar import TopPanel
+from feeluown.gui.uimain.playlist_overlay import PlaylistOverlay
 
 
 logger = logging.getLogger(__name__)
 
 
 class Ui:
 
@@ -27,47 +24,59 @@
         self._top_separator = Separator(parent=app)
         self._splitter = QSplitter(app)
 
         # NOTE: 以位置命名的部件应该只用来组织界面布局，不要
         # 给其添加任何功能性的函数
         self._message_line = MessageLine()
         self.top_panel = TopPanel(app, app)
-        self.sidebar = self._left_panel_con = LeftPanel(self._app,)
+        self.sidebar = self._left_panel_con = LeftPanel(self._app)
         self.left_panel = self._left_panel_con.p
         self.page_view = self.right_panel = RightPanel(self._app, self._splitter)
         self.toolbar = self.bottom_panel = self.right_panel.bottom_panel
         self.mpv_widget = MpvOpenGLWidget(self._app)
         self.frameless_container = None
+        self.playlist_overlay = PlaylistOverlay(app, parent=app)
 
         # alias
         self.magicbox = self.bottom_panel.magicbox
         self.player_bar = self.pc_panel = self.top_panel.pc_panel
         self.table_container = self.right_panel.table_container
         # backward compatible, old name is songs_table_container
         self.songs_table_container = self.table_container
         self.songs_table = self.table_container.songs_table
         self.back_btn = self.bottom_panel.back_btn
         self.forward_btn = self.bottom_panel.forward_btn
         self.toggle_video_btn = self.pc_panel.toggle_video_btn
 
-        self.pc_panel.playlist_btn.clicked.connect(
-            lambda: self._app.browser.goto(page='/player_playlist'))
+        self.pc_panel.playlist_btn.clicked.connect(self.raise_playlist_view)
         self.toolbar.settings_btn.clicked.connect(
             self._open_settings_dialog)
         self.toolbar.toggle_sidebar_btn.clicked.connect(self._toggle_sidebar)
 
         self._setup_ui()
 
+    def raise_playlist_view(self):
+        if not self.playlist_overlay.isVisible():
+            width = max(self._app.width() // 4, 330)
+            x = self._app.width() - width
+            height = self._app.height()
+            self.playlist_overlay.setGeometry(x, 0, width, height)
+            self.playlist_overlay.show()
+            self.playlist_overlay.setFocus()
+            # Put the widget on top.
+            self.playlist_overlay.raise_()
+
     def _setup_ui(self):
         self._app.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
 
         self._splitter.setHandleWidth(0)
         self._splitter.addWidget(self._left_panel_con)
         self._splitter.addWidget(self.right_panel)
         self._message_line.hide()
+        self.playlist_overlay.hide()
 
         self.right_panel.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         # self._layout.addWidget(self.bottom_panel)
         self._layout.addWidget(self._splitter)
         self._layout.addWidget(self.mpv_widget)
         self._layout.addWidget(self._message_line)
@@ -75,15 +84,15 @@
         self._layout.addWidget(self.top_panel)
 
         self._layout.setSpacing(0)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self.top_panel.layout().setSpacing(0)
         self.top_panel.layout().setContentsMargins(0, 0, 0, 0)
 
-        self._app.resize(880, 600)
+        self._app.resize(960, 600)
 
     def _open_settings_dialog(self):
         dialog = SettingsDialog(self._app, self._app)
         dialog.exec()
 
     def _toggle_sidebar(self):
         if self.sidebar.isVisible():
```

### Comparing `feeluown-3.8.8/feeluown/gui/uimain/toolbar.py` & `feeluown-3.8.9/feeluown/gui/uimain/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QWidget, QPushButton, QHBoxLayout, QStackedWidget
 
 from feeluown.gui.widgets.magicbox import MagicBox
 from feeluown.gui.widgets.statusline import StatusLine
 
 
 class ToolbarButton(QPushButton):
@@ -53,19 +54,20 @@
         # self._layout.addStretch(0)
         self._layout.addSpacing(80)
         self._layout.addWidget(self.status_line)
         self._layout.addWidget(self.toggle_sidebar_btn)
         self._layout.addWidget(self.settings_btn)
 
         # assume the magicbox height is about 30
-        h_margin, v_margin = 5, 10
+        h_margin, v_margin = 5, 7
         height = self.magicbox.height()
 
-        self.setFixedHeight(height + v_margin * 2 + 10)
+        self.setFixedHeight(height + v_margin * 2 + 8)
         self._layout.setContentsMargins(h_margin, v_margin, h_margin, v_margin)
+        self._layout.setAlignment(self._stacked_widget, Qt.AlignVCenter)
         self._layout.setSpacing(0)
 
     def _show_next_stacked_widget(self):
         current_index = self._stacked_widget.currentIndex()
         if current_index < self._stacked_widget.count() - 1:
             next_index = current_index + 1
         else:
```

### Comparing `feeluown-3.8.8/feeluown/gui/uimain/sidebar.py` & `feeluown-3.8.9/feeluown/gui/uimain/sidebar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 
 from PyQt5.QtCore import QSize, Qt
 from PyQt5.QtWidgets import QFrame, QLabel, QVBoxLayout, QSizePolicy, QScrollArea, \
     QHBoxLayout
 
-from feeluown.gui.helpers import use_mac_theme
 from feeluown.gui.widgets.playlists import PlaylistsView
 from feeluown.gui.widgets.provider import ProvidersView
 from feeluown.gui.widgets.collections import CollectionsView
 from feeluown.gui.widgets.my_music import MyMusicView
 from feeluown.gui.widgets.textbtn import TextButton
 
 
@@ -19,31 +18,36 @@
     def __init__(self, label, view, parent=None):
         super().__init__(parent)
 
         self._label = label
         self._view = view
         self._toggle_btn = TextButton(self.btn_text_hide, self)
 
+        self._toggle_btn.clicked.connect(self.toggle_view)
+        self.setup_ui()
+
+    def setup_ui(self):
+        self._label.setFixedHeight(25)
+
         self._layout = QVBoxLayout(self)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.setSpacing(0)
-        self._h_layout = QHBoxLayout()
-        label.setFixedHeight(25)
-        self._h_layout.addWidget(label)
-        self._h_layout.addStretch(0)
-        self._h_layout.addWidget(self._toggle_btn)
-        self._h_layout.addSpacing(10)
-        self._layout.addLayout(self._h_layout)
-        self._layout.addWidget(view)
-        self._layout.addStretch(0)
+
+        self._t_h_layout = QHBoxLayout()
+        self._b_h_layout = QHBoxLayout()
+        self._t_h_layout.addWidget(self._label)
+        self._t_h_layout.addStretch(0)
+        self._t_h_layout.addWidget(self._toggle_btn)
+        self._b_h_layout.addWidget(self._view)
+
+        self._layout.addLayout(self._t_h_layout)
+        self._layout.addLayout(self._b_h_layout)
         # XXX: 本意是让 ListViewContainer 下方不要出现多余的空间
         self.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
 
-        self._toggle_btn.clicked.connect(self.toggle_view)
-
     def toggle_view(self):
         if self._view.isVisible():
             self.hide_view()
         else:
             self.show_view()
 
     def show_view(self):
@@ -71,15 +75,15 @@
 
         # HELP(cosven): size policy is not working
         # self.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Expanding)
         self.setMaximumWidth(280)
 
     def sizeHint(self):
         size = super().sizeHint()
-        width = min(self._app.width() // 4, 240)
+        width = min(self._app.width() * 22 // 100, 240)
         return QSize(width, size.height())
 
 
 class _LeftPanel(QFrame):
 
     def __init__(self, app, parent=None):
         super().__init__(parent)
@@ -114,17 +118,16 @@
         self.providers_view.setModel(self._app.pvd_uimgr.model)
         self.playlists_view.setModel(self._app.pl_uimgr.model)
         self.my_music_view.setModel(self._app.mymusic_uimgr.model)
         self.collections_view.setModel(self._app.coll_uimgr.model)
 
         self._layout = QVBoxLayout(self)
 
-        if use_mac_theme():
-            self._layout.setSpacing(0)
-            self._layout.setContentsMargins(6, 4, 0, 0)
+        self._layout.setSpacing(0)
+        self._layout.setContentsMargins(16, 16, 16, 0)
         self._layout.addWidget(self.providers_con)
         self._layout.addWidget(self.collections_con)
         self._layout.addWidget(self.my_music_con)
         self._layout.addWidget(self.playlists_con)
         self._layout.addStretch(0)
 
         self.providers_view.setFrameShape(QFrame.NoFrame)
```

### Comparing `feeluown-3.8.8/feeluown/gui/uimain/page_view.py` & `feeluown-3.8.9/feeluown/gui/uimain/page_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,85 @@
 import logging
 import sys
 
-from PyQt5.QtCore import Qt, QRect, QSize, QModelIndex, QEasingCurve
+from PyQt5.QtCore import Qt, QRect, QSize, QEasingCurve, QEvent
 from PyQt5.QtGui import QPainter, QBrush, QColor, QLinearGradient, QPalette
-from PyQt5.QtWidgets import QFrame, QVBoxLayout, QScrollArea, QStackedLayout
+from PyQt5.QtWidgets import QFrame, QVBoxLayout, QStackedLayout
 
 from feeluown.utils import aio
 from feeluown.models import ModelType
 from feeluown.utils.reader import wrap
 
 from feeluown.gui.theme import Light
-from feeluown.gui.helpers import BgTransparentMixin, ItemViewNoScrollMixin
+from feeluown.gui.helpers import BgTransparentMixin, BaseScrollAreaForNoScrollItemView
 from feeluown.gui.uimain.toolbar import BottomPanel
 from feeluown.gui.page_containers.table import TableContainer
+from feeluown.gui.base_renderer import VFillableBg
 
 logger = logging.getLogger(__name__)
 
 
 def add_alpha(color, alpha):
     new_color = QColor(color)
     new_color.setAlpha(alpha)
     return new_color
 
 
-class ScrollArea(QScrollArea, BgTransparentMixin):
-    """
-    该 ScrollArea 和 TableContainer 是紧密耦合的一个组件，
-    目标是为了让整个 Table 内容都处于一个滚动的窗口内。
-
-    TODO: 给这个 ScrollArea 添加更多注释，对它进行一些重构
-    """
+class ScrollArea(BaseScrollAreaForNoScrollItemView, BgTransparentMixin):
     def __init__(self, app, parent=None):
         super().__init__(parent=parent)
         self._app = app
 
         self.setWidgetResizable(True)
         self.setFrameShape(QFrame.NoFrame)
 
         self.t = TableContainer(app, self)
         self.setWidget(self.t)
+        #: widgets that may affect the itemview height
+        self._other_widgets = [self.t.meta_widget, self.t.toolbar]
+        for w in self._other_widgets:
+            w.installEventFilter(self)
 
-        self.verticalScrollBar().valueChanged.connect(self.on_v_scrollbar_value_changed)
         # As far as I know, KDE and GNOME can't auto hide the scrollbar,
         # and they show an old-fation vertical scrollbar.
         # HELP: implement an auto-hide scrollbar for Linux
         if sys.platform.lower() != 'darwin':
             self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
 
-    def on_v_scrollbar_value_changed(self, value):
-        maximum = self.verticalScrollBar().maximum()
-        if maximum == value:
-            table = self.t.current_table
-            if table is None:
-                return
-            model = table.model()
-            if model is not None and model.canFetchMore(QModelIndex()):
-                model.fetchMore(QModelIndex())
+    def get_itemview(self):
+        return self.t.current_table
+
+    def height_for_itemview(self):
+        height = self.height()
+        for w in self._other_widgets:
+            if w.isVisible():
+                height -= w.height()
+        return height
 
     def wheelEvent(self, e):
         super().wheelEvent(e)
         self._app.ui.bottom_panel.update()
 
-    def resizeEvent(self, e):
-        super().resizeEvent(e)
-        table = self.t.current_table
-        if table is not None and isinstance(table, ItemViewNoScrollMixin):
-            table.suggest_min_height(self.height_for_table())
-
-    def height_for_table(self):
-        """a proper height for the table widget"""
-        # spacing is 10
+    def eventFilter(self, obj, event):
+        if event.type() == QEvent.Resize:
+            self.maybe_resize_itemview()
+        return False
+
+    def fillable_bg_height(self):
+        """Implement VFillableBg protocol"""
+        height = 0
         table_container = self.t
-        table_proper_height = self.height() - 10
         if table_container.meta_widget.isVisible():
-            table_proper_height -= table_container.meta_widget.height()
+            height += table_container.meta_widget.height()
+        extra = table_container.current_extra
+        if extra is not None and extra.isVisible():
+            height += extra.height()
         if table_container.toolbar.isVisible():
-            table_proper_height -= table_container.toolbar.height()
-        if table_container.desc_widget.isVisible():
-            table_proper_height -= table_container.desc_widget.height()
-        return table_proper_height
+            height += table_container.toolbar.height()
+        return height
 
 
 class RightPanel(QFrame):
     def __init__(self, app, parent=None):
         super().__init__(parent)
 
         self._app = app
@@ -170,35 +167,29 @@
         painter = QPainter(self)
         painter.setPen(Qt.NoPen)
         painter.setRenderHint(QPainter.Antialiasing)
         painter.setRenderHint(QPainter.SmoothPixmapTransform)
 
         # calculate available size
         draw_width = self.width()
-        draw_height = 10  # spacing defined in table container
-        draw_height += self.bottom_panel.height()
-        if self.table_container.meta_widget.isVisible():
-            draw_height += self.table_container.meta_widget.height()
-        extra = self.table_container.current_extra
-        if extra is not None and extra.isVisible():
-            draw_height += extra.height()
-        if self.table_container.toolbar.isVisible():
-            draw_height += self.table_container.toolbar.height()
+        draw_height = self.bottom_panel.height()
+        if isinstance(self._stacked_layout.currentWidget(), VFillableBg):
+            draw_height += self._stacked_layout.currentWidget().fillable_bg_height()
 
         scrolled = self.scrollarea.verticalScrollBar().value()
         max_scroll_height = draw_height - self.bottom_panel.height()
 
         # Draw the whole background with QPalette.Base color.
         painter.save()
         painter.setBrush(self.palette().brush(QPalette.Base))
         painter.drawRect(self.rect())
         painter.restore()
 
-        # Do not draw the pixmap when it is not shown.
-        if scrolled >= max_scroll_height:
+        # Do not draw the pixmap or overlay when it scrolled a lot.
+        if scrolled > max_scroll_height:
             painter.save()
             painter.setBrush(self.palette().brush(QPalette.Window))
             painter.drawRect(self.bottom_panel.rect())
             painter.restore()
             return
 
         if self._pixmap is not None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `feeluown-3.8.8/feeluown/gui/uimain/player_bar.py` & `feeluown-3.8.9/feeluown/gui/uimain/player_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     QPushButton, QSizePolicy, QMenu,
 )
 from feeluown.gui.widgets.cover_label import CoverLabelV2
 
 from feeluown.utils import aio
 from feeluown.excs import ProviderIOError
 from feeluown.media import MediaType
-from feeluown.player import PlaybackMode, State
+from feeluown.player import State
 from feeluown.gui.widgets.lyric import Window as LyricWindow
 from feeluown.gui.widgets.menu import SongMenuInitializer
 from feeluown.gui.helpers import resize_font
 from feeluown.gui.widgets import TextButton
 from feeluown.gui.widgets.playlist_button import PlaylistButton
 from feeluown.gui.widgets.volume_button import VolumeButton
 from feeluown.gui.widgets.progress_slider import ProgressSlider
@@ -233,32 +233,23 @@
         super().__init__(parent)
         self._app = app
 
         class IconButton(QPushButton):
             def __init__(self, *args, **kwargs):
                 super().__init__(*args, **kwargs)
 
-        self._playback_modes = list(PlaybackMode.__members__.values())
-        self._pm_alias_map = {
-            PlaybackMode.one_loop: '单曲循环',
-            PlaybackMode.sequential: '顺序播放',
-            PlaybackMode.loop: '循环播放',
-            PlaybackMode.random: '随机播放',
-        }
         self.lyric_window = LyricWindow()
         self.lyric_window.hide()
 
         # initialize sub widgets
         self._layout = QHBoxLayout(self)
         self.previous_btn = IconButton(self)
         self.pp_btn = IconButton(self)
         self.next_btn = IconButton(self)
 
-        #: playback mode switch button
-        self.pms_btn = TextButton(self)
         self.volume_btn = VolumeButton(self)
         self.playlist_btn = PlaylistButton(self._app, self)
         #: mark song as favorite button
         self.like_btn = LikeButton(self._app, self)
         self.mv_btn = TextButton('MV', self)
         self.toggle_lyric_btn = LyricButton(self._app, self)
         self.download_btn = QPushButton(self)
@@ -268,25 +259,23 @@
         self.toggle_pip_btn = TextButton('◲', self)
 
         self.previous_btn.setObjectName('previous_btn')
         self.pp_btn.setObjectName('pp_btn')
         self.next_btn.setObjectName('next_btn')
         self.playlist_btn.setObjectName('playlist_btn')
         self.volume_btn.setObjectName('volume_btn')
-        self.pms_btn.setObjectName('pms_btn')
         self.download_btn.setObjectName('download_btn')
         self.like_btn.setObjectName('like_btn')
         self.mv_btn.setObjectName('mv_btn')
         self.toggle_lyric_btn.setObjectName('toggle_lyric_btn')
         self.toggle_video_btn.setObjectName('toggle_video_btn')
         self.toggle_pip_btn.setObjectName('toggle_pip_btn')
 
         self.progress_slider = ProgressSlider(app=app, parent=self)
 
-        self.pms_btn.setToolTip('修改播放模式')
         self.volume_btn.setToolTip('调整音量')
         self.playlist_btn.setToolTip('显示当前播放列表')
 
         self.mv_btn.setToolTip('播放 MV')
         self.download_btn.setToolTip('下载歌曲（未实现，欢迎 PR）')
         self.pp_btn.setCheckable(True)
         self.download_btn.setCheckable(True)
@@ -302,31 +291,27 @@
         # we should enable focus since we want to have shortcut keys
         self.setFocusPolicy(Qt.StrongFocus)
         self.song_source_label.setObjectName('song_source_label')
 
         self.next_btn.clicked.connect(self._app.playlist.next)
         self.previous_btn.clicked.connect(self._app.playlist.previous)
         self.pp_btn.clicked.connect(self._app.player.toggle)
-        self.pms_btn.clicked.connect(self._switch_playback_mode)
         self.volume_btn.change_volume_needed.connect(
             lambda volume: setattr(self._app.player, 'volume', volume))
 
         player = self._app.player
         playlist = self._app.playlist
-        playlist.playback_mode_changed.connect(self.on_playback_mode_changed,
-                                               aioqueue=True)
         playlist.song_changed.connect(self.on_player_song_changed, aioqueue=True)
         player.state_changed.connect(self._on_player_state_changed, aioqueue=True)
         player.metadata_changed.connect(self.on_metadata_changed, aioqueue=True)
         player.volume_changed.connect(self.volume_btn.on_volume_changed)
         self._app.live_lyric.sentence_changed.connect(self.lyric_window.set_sentence)
         self.lyric_window.play_previous_needed.connect(playlist.previous)
         self.lyric_window.play_next_needed.connect(playlist.next)
 
-        self._update_pms_btn_text()
         self._setup_ui()
 
     def _setup_ui(self):
         self.cover_label.setFixedWidth(44)
         self.cover_label.setMaximumHeight(44)
         self.song_source_label.setFixedHeight(20)
         self.progress_slider.setFixedHeight(20)  # half of parent height
@@ -399,43 +384,23 @@
         self._layout.addSpacing(7)
         self._layout.addLayout(self._sub_layout)
         self._layout.setStretchFactor(self._sub_layout, 1)
         self._layout.addSpacing(7)
         self._layout.addLayout(self._progress_v_layout)
         self._layout.addStretch(0)
         self._layout.addSpacing(18)
-        self._layout.addWidget(self.pms_btn)
-        self._layout.addSpacing(8)
         self._layout.addWidget(self.playlist_btn)
         self._layout.addSpacing(8)
         self._layout.addWidget(self.toggle_video_btn)
         self._layout.addSpacing(8)
         self._layout.addWidget(self.toggle_pip_btn)
         self._layout.addSpacing(18)
         self._layout.setSpacing(0)
         self._layout.setContentsMargins(0, 0, 0, 0)
 
-    def _switch_playback_mode(self):
-        playlist = self._app.playlist
-        pm_total = len(self._playback_modes)
-        pm_idx = self._playback_modes.index(playlist.playback_mode)
-        if pm_idx < pm_total - 1:
-            pm_idx += 1
-        else:
-            pm_idx = 0
-        playlist.playback_mode = self._playback_modes[pm_idx]
-
-    def on_playback_mode_changed(self, _):
-        self._update_pms_btn_text()
-
-    def _update_pms_btn_text(self):
-        playback_mode = self._app.playlist.playback_mode
-        alias = self._pm_alias_map[playback_mode]
-        self.pms_btn.setText(alias)
-
     def on_player_song_changed(self, song):
         task_spec = self._app.task_mgr.get_or_create('update-mv-btn-status')
         task_spec.bind_coro(self.update_mv_btn_status(song))
 
     def on_metadata_changed(self, metadata):
         if not metadata:
             self.song_source_label.setText('歌曲来源')
```

### Comparing `feeluown-3.8.8/feeluown/gui/watch.py` & `feeluown-3.8.9/feeluown/gui/watch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 from contextlib import contextmanager
 from enum import IntEnum
 
+from PyQt5.QtCore import Qt
+
 from feeluown.player.mpvplayer import _mpv_set_property_string
 from feeluown.gui.widgets.frameless import ResizableFramelessContainer
 
 logger = logging.getLogger(__name__)
 
 
 class Mode(IntEnum):
@@ -115,17 +117,17 @@
 
     def exit_pip_mode(self):
         """exit picture in picture mode"""
         self._pip_container.hide()
         self._app.ui.mpv_widget.hide()
         logger.info("exit video-show picture in picture mode")
 
-    #
-    # signal callbacks
-    #
+    def toggle_pip_fullscreen(self):
+        self._pip_container.setWindowState(
+            self._pip_container.windowState() ^ Qt.WindowFullScreen)
 
     def play_mv(self):
         song = self._app.player.current_song
         if song is None:
             return
 
         # The mv button only shows when there is a valid mv object
```

### Comparing `feeluown-3.8.8/feeluown/gui/theme.py` & `feeluown-3.8.9/feeluown/gui/theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
             if sys.platform == 'darwin':
                 if get_osx_theme() == 1:
                     theme = DARK
                 else:
                     theme = LIGHT
             else:
                 theme = self.guess_system_theme()
-                if theme == Dark:
-                    theme = MacOSDark
+                if theme == DARK:
+                    theme = Dark
         else:  # user settings have highest priority
             theme = self._app.config.THEME
         self.load_theme(theme)
 
     def load_theme(self, theme):
         if theme == DARK:
             self.load_dark()
```

### Comparing `feeluown-3.8.8/feeluown/gui/mimedata.py` & `feeluown-3.8.9/feeluown/gui/mimedata.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/browser.py` & `feeluown-3.8.9/feeluown/gui/browser.py`

 * *Files 7% similar despite different names*

```diff
@@ -182,15 +182,14 @@
 
     def initialize(self):
         """browser should be initialized after all ui components are created
 
         1. bind routes with renderer
         """
         from feeluown.gui.pages.search import render as render_search
-        from feeluown.gui.pages.player_playlist import render as render_player_playlist
         from feeluown.gui.pages.model import render as render_model
         from feeluown.gui.pages.coll_mixed import render as render_coll_mixed
         from feeluown.gui.pages.song_explore import render as render_song_explore
 
         model_prefix = f'{MODEL_PAGE_PREFIX}<provider>'
 
         async def dummy_render(req, *args, **kwargs):
@@ -200,11 +199,10 @@
             (f'{model_prefix}/<ns>/<identifier>', render_model),
             # These routes will be removed in v3.9
             (f'{model_prefix}/songs/<identifier>/similar', dummy_render),
             (f'{model_prefix}/songs/<identifier>/hot_comments', dummy_render),
             (f'{model_prefix}/songs/<identifier>/explore', render_song_explore),
             ('/colls/<identifier>', render_coll_mixed),
             ('/search', render_search),
-            ('/player_playlist', render_player_playlist),
         ]
         for url, renderer in urlpatterns:
             self.route(url)(renderer)
```

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/last.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/last.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/feeluown.icns` & `feeluown-3.8.9/feeluown/gui/assets/icons/feeluown.icns`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/pause.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/pause.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/cur_playlist_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/cur_playlist_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/like.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/like.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/download_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/download_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/play.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/play.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/volume.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/volume.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/already_download.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/already_download.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/tray-dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/tray-dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/last_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/last_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/feeluown.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/feeluown.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/feeluown.ico` & `feeluown-3.8.9/feeluown/gui/assets/icons/feeluown.ico`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/next.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/next.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/tray-light.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/tray-light.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/like_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/like_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/like_checked_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/like_checked_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/like_checked.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/like_checked.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/play_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/play_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/next_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/next_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/volume_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/volume_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/download.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/download.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/pause_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/pause_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/cur_playlist.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/cur_playlist.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/icons/already_downloaded_dark.png` & `feeluown-3.8.9/feeluown/gui/assets/icons/already_downloaded_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/themes/common.qss` & `feeluown-3.8.9/feeluown/gui/assets/themes/common.qss`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 QWidget {
     /* font-size: 13px; */
     /* tips: you can turn on border for debugging */
     /* border: 1px solid red; */
 }
 
 LeftPanel QLabel {
+    color: #888;
+}
+
+LeftPanel QLabel {
     padding-top: 3px;
     padding-bottom: 3px;
-    font-size: 12px;
-    font-weight: bold;
 }
 
-LeftPanel QListView {
-    margin-left: 5px;
+LeftPanel QLabel, LeftPanel ListViewContainer TextButton {
+    font-size: 12px;
 }
 
 LeftPanel QListView, QSplitter::handle {
     background-color: transparent;
 }
 
-DescLabel {
-    background-color: palette(base);
-}
-
 MagicBox {
     background: transparent;
     border-bottom: 1px dashed #777;
 }
 MagicBox:focus {
     border-bottom: 1px solid #777;
     background: palette(window);
@@ -78,30 +76,39 @@
 TextButton:hover, ToolbarButton:hover {
     border: 1px solid #777;
 }
 TextButton:checked {
     border: 1px solid #d75a4a;  /* same as like_btn red color */
     color: #d75a4a;
 }
+
+LeftPanel ListViewContainer TextButton, ClickableHeader TextButton {
+    border: none;
+    color: #888;
+}
+LeftPanel ListViewContainer TextButton:hover, ClickableHeader TextButton:hover {
+    color: palette(text);
+    border: none;
+}
+ClickableHeader TextButton:checked {
+    color: palette(text);
+    border: none;
+}
+
 #mv_btn, #toggle_lyric_btn {
     font-size: 9px;
 }
 #mv_btn {
     padding: 0px 3px;
 }
 #toggle_lyric_btn {
     padding: 0px 5px;
 }
 #toggle_video_btn, #toggle_pip_btn {
     padding: 0px 3px;
 }
 
-LeftPanel ListViewContainer TextButton {
-    padding: 0px 2px;
-    border: none;
-}
-
 VideoCtlToolbar QPushButton {
     width: 24px;
     height: 24px;
     outline: none;
 }
```

### Comparing `feeluown-3.8.8/feeluown/gui/assets/themes/light.qss` & `feeluown-3.8.9/feeluown/gui/assets/themes/light.qss`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/assets/themes/macos_dark.colors` & `feeluown-3.8.9/feeluown/gui/assets/themes/macos_dark.colors`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826088%*

 * *Differences: {"'Active'": "{'AlternateBase': '#292929'}",*

 * * "'Disabled'": "{'AlternateBase': '#292929'}",*

 * * "'Inactive'": "{'AlternateBase': '#292929'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "Active": {
-        "AlternateBase": "#989898",
+        "AlternateBase": "#292929",
         "Background": "#323232",
         "Base": "#1e1e1e",
         "BrightText": "#373737",
         "Button": "#323232",
         "ButtonText": "#ffffff",
         "Dark": "#bfbfbf",
         "Foreground": "#ffffff",
@@ -21,15 +21,15 @@
         "Text": "#ffffff",
         "ToolTipBase": "#ffffff",
         "ToolTipText": "#000000",
         "Window": "#323232",
         "WindowText": "#ffffff"
     },
     "Disabled": {
-        "AlternateBase": "#989898",
+        "AlternateBase": "#292929",
         "Background": "#323232",
         "Base": "#323232",
         "BrightText": "#373737",
         "Button": "#323232",
         "ButtonText": "#717171",
         "Dark": "#bfbfbf",
         "Foreground": "#ffffff",
@@ -46,15 +46,15 @@
         "Text": "#ffffff",
         "ToolTipBase": "#ffffff",
         "ToolTipText": "#000000",
         "Window": "#323232",
         "WindowText": "#ffffff"
     },
     "Inactive": {
-        "AlternateBase": "#989898",
+        "AlternateBase": "#292929",
         "Background": "#323232",
         "Base": "#1e1e1e",
         "BrightText": "#373737",
         "Button": "#323232",
         "ButtonText": "#ffffff",
         "Dark": "#bfbfbf",
         "Foreground": "#ffffff",
```

### Comparing `feeluown-3.8.8/feeluown/gui/assets/themes/dark.qss` & `feeluown-3.8.9/feeluown/gui/assets/themes/dark.qss`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/base_renderer.py` & `feeluown-3.8.9/feeluown/gui/base_renderer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from abc import abstractmethod
+from typing import runtime_checkable, Protocol
+
 from feeluown.gui.widgets.tabbar import Tab, TabBar
 
 
 class LibraryTabRendererMixin:
 
     def init_tabbar_signal_binding(self):
         for tab_id, signal in self.get_tabid_signal_mapping().items():
@@ -56,7 +59,21 @@
         for tab in self.tabs:
             tab_bar.addTab(tab[0])
         tab_bar.setCurrentIndex(self.tab_index)
         tab_bar.tabBarClicked.connect(self.render_by_tab_index)
 
     def render_by_tab_index(self, tab_index):
         raise NotImplementedError
+
+
+@runtime_checkable
+class VFillableBg(Protocol):
+    """Protocol for widgets which has vertical fillable background
+
+    This protocol indicates the background of the widget is transparent. The parent
+    widget can fill color for the widget.
+
+    .. versionadded:: 3.8.9
+    """
+    @abstractmethod
+    def fillable_bg_height(self) -> int:
+        raise NotImplementedError
```

### Comparing `feeluown-3.8.8/feeluown/gui/hotkey.py` & `feeluown-3.8.9/feeluown/gui/hotkey.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/gui/helpers.py` & `feeluown-3.8.9/feeluown/gui/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 和应用逻辑相关的一些工具函数
 """
 import asyncio
 import itertools
 import random
 import sys
 import logging
-from contextlib import suppress
-from requests.exceptions import RequestException
 
 try:
     # helper module should work in no-window mode
     from PyQt5.QtCore import QModelIndex, QSize, Qt, pyqtSignal, QSortFilterProxyModel, \
         QAbstractListModel
     from PyQt5.QtGui import QPalette, QFontMetrics
-    from PyQt5.QtWidgets import QApplication
+    from PyQt5.QtWidgets import QApplication, QScrollArea
 except ImportError:
     pass
 
 from feeluown.utils import aio
 from feeluown.excs import ProviderIOError
-from feeluown.library import NotSupported
+from feeluown.library import NotSupported, ModelType, BaseModel
+from feeluown.models.uri import reverse
 
 logger = logging.getLogger(__name__)
 
 
 async def async_run(func, loop=None, executor=None):
     """异步的获取 model 属性值
 
@@ -38,24 +37,14 @@
     return await loop.run_in_executor(executor, func)
 
 
 class ActionError(Exception):
     pass
 
 
-def use_mac_theme():
-    """判断是否需要使用 mac 主题
-
-    目前只是简单为 mac 做一些定制，但如果真的要引入 theme 这个概念，
-    单这一个函数是不够的。
-    """
-    return True
-    return sys.platform == 'darwin'
-
-
 def is_macos():
     """Check if operating system is macOS
 
     .. versionadded: v3.7.10
     """
     return sys.platform == 'darwin'
 
@@ -92,31 +81,88 @@
 class BgTransparentMixin:
     def __init__(self, *args, **kwargs):
         palette = self.palette()
         palette_set_bg_color(palette, Qt.transparent)
         self.setPalette(palette)
 
 
+class BaseScrollAreaForNoScrollItemView(QScrollArea):
+    """A scroll area base class for itemview with no_scroll_v=True
+
+    Subclass must implement the following methods:
+    * itemview
+    * height_for_itemview
+    Also note the API is not stable.
+
+    .. versionadded:: 3.8.9
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.verticalScrollBar().valueChanged.connect(self.on_v_scrollbar_value_changed)
+
+    def get_itemview(self):
+        raise NotImplementedError
+
+    def height_for_itemview(self):
+        raise NotImplementedError
+
+    def resizeEvent(self, e):
+        super().resizeEvent(e)
+        self.maybe_resize_itemview()
+
+    def maybe_resize_itemview(self):
+        """Resize itemview to make sure it has a chance to fetch more items
+
+        When the itemview has no more items, do not need to resize it.
+        """
+        itemview = self.get_itemview()
+        if itemview is not None:
+            model = itemview.model()
+            if model is not None and model.canFetchMore(QModelIndex()):
+                # +1 to make sure user can scroll, then user has a change to
+                # trigger itemview fetch more.
+                itemview.suggest_min_height(self.height_for_itemview() + 1)
+                itemview.adjust_height()
+
+    def maybe_trigger_itemview_fetch_more(self):
+        itemview = self.get_itemview()
+        if itemview is not None:
+            model = itemview.model()
+            if model is not None and model.canFetchMore(QModelIndex()):
+                model.fetchMore(QModelIndex())
+
+    def on_v_scrollbar_value_changed(self, value):
+        maximum = self.verticalScrollBar().maximum()
+        if maximum == value:
+            self.maybe_trigger_itemview_fetch_more()
+
+
 class ItemViewNoScrollMixin:
     """
     `no_scroll_v` means that the itemview's size(height) is always enough to hold
     all fetched items. When new items are fetched, the itemview size is
     automatically adjueted.
 
     The itemview with no_scroll_v=True is usually used with an outside ScrollArea.
     """
     def __init__(self, *args, no_scroll_v=True, row_height=0, least_row_count=0,
-                 reserved=30, **kwargs):
+                 fixed_row_count=0, reserved=30, **kwargs):
         """
         :params no_scroll_v: enable on no_scroll_v feature or not
+        :params fixed_row_count: set row_height when fixed_row_count is set
 
         .. versionadded:: 3.7.8
            The *row_height*, *least_row_count*, *reserved* parameter were added.
+
+        .. versionadded:: 3.8.9
+           The *fixed_row_count* parameter was added.
         """
         self._least_row_count = least_row_count
+        self._fixed_row_count = fixed_row_count
         self._row_height = row_height
         self._reserved = reserved
 
         self._min_height = 0
 
         self._no_scroll_v = no_scroll_v
 
@@ -137,23 +183,27 @@
     #         self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
 
     def adjust_height(self):
         if self.model() is None:
             return
 
         if self.model().canFetchMore(QModelIndex()):
-            # according to QAbstractItemView source code,
-            # qt will trigger fetchMore when the last row is
-            # inside the viewport, so we always hide the last
-            # two row to ensure fetch-more will not be
-            # triggered automatically
-            index = self._last_visible_index()
-            rect = self.visualRect(index)
-            height = self.sizeHint().height() - int(rect.height() * 1.5) - self._reserved
-            self.setFixedHeight(max(height, self.min_height()))
+            if self._fixed_row_count == 0:
+                # according to QAbstractItemView source code,
+                # qt will trigger fetchMore when the last row is
+                # inside the viewport, so we always hide the last
+                # two row to ensure fetch-more will not be
+                # triggered automatically
+                index = self._last_visible_index()
+                rect = self.visualRect(index)
+                height = self.sizeHint().height() - int(rect.height() * 1.5) - \
+                    self._reserved
+                self.setFixedHeight(max(height, self.min_height()))
+            else:
+                self.setFixedHeight(self._row_height * self._fixed_row_count)
         else:
             height = self.sizeHint().height()
             self.setFixedHeight(height)
         self.updateGeometry()
 
     def on_rows_changed(self, *args):
         if self._no_scroll_v is True:
@@ -183,18 +233,21 @@
     def sizeHint(self):
         super_size_hint = super().sizeHint()
         if self._no_scroll_v is False:
             return super_size_hint
 
         height = min_height = self.min_height()
         if self.model() is not None:
-            index = self._last_visible_index()
-            rect = self.visualRect(index)
-            height = rect.y() + rect.height() + self._reserved
-            height = max(min_height, height)
+            if self._fixed_row_count == 0:
+                index = self._last_visible_index()
+                rect = self.visualRect(index)
+                height = rect.y() + rect.height() + self._reserved
+                height = max(min_height, height)
+            else:
+                height = self._row_height * self._fixed_row_count
         return QSize(super_size_hint.width(), height)
 
     def _last_visible_index(self):
         source_model = self.model()
         row_index = source_model.rowCount() - 1
         if isinstance(source_model, QAbstractListModel):
             column_index = 0
@@ -337,30 +390,78 @@
             self._fetch_more_cb(None)
         else:
             self._fetch_more_cb(items)
 
 
 def fetch_cover_wrapper(app):
     """
-    Your should only use this helper within ImgListModel.
+    Your should only use this helper within ImgListModel and SongMiniCardListModel.
     """
     img_mgr, library = app.img_mgr, app.library
 
-    async def fetch_model_cover(model, cb, uid):
-        # try get from cache first
-        content = img_mgr.get_from_cache(uid)
+    async def fetch_model_cover(model, cb):
+        # Get image unique id.
+        model_is_song = False
+        song_is_v2 = False
+        upgraded_song = None
+        if ModelType(model.meta.model_type) is ModelType.song:
+            model_is_song = True
+            if isinstance(model, BaseModel):
+                song_is_v2 = True
+                img_uid, _ = model.cache_get('album_uid')
+            else:
+                img_uid = None
+        else:
+            img_uid = reverse(model) + '/cover'
+        if img_uid is None:
+            assert model_is_song
+            try:
+                upgraded_song = await aio.run_fn(library.song_upgrade, model)
+                album = upgraded_song.album
+            except NotSupported:
+                album = None
+            if album is None:
+                cb(None)
+                return
+
+            img_uid = reverse(album) + '/cover'
+            if song_is_v2:
+                model.cache_set('album_uid', img_uid)
+
+        # Check image cache with image unique ID.
+        content = img_mgr.get_from_cache(img_uid)
         if content is not None:
-            return cb(content)
-        # FIXME: sleep random second to avoid send too many request to provider
-        await asyncio.sleep(random.randrange(100) / 100)
-        with suppress(ProviderIOError, RequestException, NotSupported):
-            url = await aio.run_fn(library.model_get_cover, model)
-            if url:
-                content = await img_mgr.get(url, uid)
-                cb(content)
+            cb(content)
+            return
+
+        # Get image url.
+        img_url = None
+        if model_is_song and song_is_v2:
+            img_url, _ = model.cache_get('album_cover')
+        if img_url is None:
+            if model_is_song:
+                model_with_img = upgraded_song.album
+            else:
+                model_with_img = model
+            try:
+                img_url = await aio.run_fn(library.model_get_cover, model_with_img)
+            except NotSupported:
+                img_url = ''
+            if model_is_song:
+                model.cache_set('album_cover', img_url)
+
+        # Fetch image by url and invoke cb.
+        if img_url:
+            # FIXME: sleep random second to avoid send too many request to provider
+            await asyncio.sleep(random.randrange(100) / 100)
+            content = await img_mgr.get(img_url, img_uid)
+            cb(content)
+        else:
+            cb(None)
+
     return fetch_model_cover
 
 
 # https://ethanschoonover.com/solarized/
 SOLARIZED_COLORS = {
     'yellow':    '#b58900',
     'orange':    '#cb4b16',
```

### Comparing `feeluown-3.8.8/feeluown/config.py` & `feeluown-3.8.9/feeluown/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/task.py` & `feeluown-3.8.9/feeluown/task.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/utils/aio.py` & `feeluown-3.8.9/feeluown/utils/aio.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/utils/reader.py` & `feeluown-3.8.9/feeluown/utils/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     #             'max_per_read': self._max_per_read,
     #             'read_times': read_times}
 
     def _read_range(self, start, end):
         # TODO: make this method thread safe
         assert start <= end, "start should less than end"
         try:
-            logger.info('trigger read_func(%d, %d)', start, end)
+            logger.debug('trigger read_func(%d, %d)', start, end)
             objs = self._read_func(start, end)
         except:  # noqa: E722
             raise ReadFailed('read_func raise error')
         else:
             expected = end - start
             actual = len(objs)
             if expected != actual:
```

### Comparing `feeluown-3.8.8/feeluown/utils/dispatch.py` & `feeluown-3.8.9/feeluown/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/utils/router.py` & `feeluown-3.8.9/feeluown/utils/router.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/utils/sync.py` & `feeluown-3.8.9/feeluown/utils/sync.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/utils/request.py` & `feeluown-3.8.9/feeluown/utils/request.py`

 * *Files identical despite different names*

### Comparing `feeluown-3.8.8/feeluown/utils/utils.py` & `feeluown-3.8.9/feeluown/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,27 +20,14 @@
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     # TODO: this may block for 2 second if port is not used on Windows
     rv = sock.connect_ex(('127.0.0.1', port))
     sock.close()
     return rv == 0
 
 
-def use_mpv_old():
-    try:
-        import mpv  # noqa
-    except AttributeError as e:
-        # libmpv<1.28 'undefined symbol: mpv_render_context_create'
-        # libmpv<1.29 'undefined symbol: mpv_destroy'
-        msg = str(e)
-        if 'undefined symbol' in msg:
-            logger.info(f'use mpv old because of err: {msg}')
-            return True
-    return False
-
-
 def parse_ms(ms):
     minute = int(ms / 60000)
     second = int((ms % 60000) / 1000)
     return minute, second
 
 
 def log_exectime(func):
```

### Comparing `feeluown-3.8.8/feeluown.egg-info/SOURCES.txt` & `feeluown-3.8.9/feeluown.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+LICENSE
 README.md
 mpv.py
-mpv_old.py
 setup.cfg
 setup.py
 feeluown/__init__.py
 feeluown/__main__.py
 feeluown/argparser.py
 feeluown/collection.py
 feeluown/config.py
@@ -79,57 +79,60 @@
 feeluown/gui/assets/icons/volume.png
 feeluown/gui/assets/icons/volume_dark.png
 feeluown/gui/assets/themes/common.qss
 feeluown/gui/assets/themes/dark.qss
 feeluown/gui/assets/themes/light.qss
 feeluown/gui/assets/themes/macos_dark.colors
 feeluown/gui/page_containers/__init__.py
+feeluown/gui/page_containers/scroll_area.py
 feeluown/gui/page_containers/table.py
 feeluown/gui/pages/__init__.py
 feeluown/gui/pages/coll_mixed.py
 feeluown/gui/pages/model.py
-feeluown/gui/pages/player_playlist.py
 feeluown/gui/pages/search.py
 feeluown/gui/pages/song_explore.py
 feeluown/gui/uimain/__init__.py
 feeluown/gui/uimain/page_view.py
 feeluown/gui/uimain/player_bar.py
+feeluown/gui/uimain/playlist_overlay.py
 feeluown/gui/uimain/sidebar.py
 feeluown/gui/uimain/toolbar.py
 feeluown/gui/uimodels/__init__.py
 feeluown/gui/uimodels/collection.py
 feeluown/gui/uimodels/my_music.py
 feeluown/gui/uimodels/playlist.py
 feeluown/gui/uimodels/provider.py
 feeluown/gui/widgets/__init__.py
+feeluown/gui/widgets/accordion.py
 feeluown/gui/widgets/album.py
 feeluown/gui/widgets/artist.py
 feeluown/gui/widgets/collections.py
 feeluown/gui/widgets/comment_list.py
 feeluown/gui/widgets/cover_label.py
 feeluown/gui/widgets/frameless.py
+feeluown/gui/widgets/header.py
 feeluown/gui/widgets/imglist.py
 feeluown/gui/widgets/labels.py
 feeluown/gui/widgets/login.py
 feeluown/gui/widgets/lyric.py
 feeluown/gui/widgets/magicbox.py
 feeluown/gui/widgets/menu.py
 feeluown/gui/widgets/messageline.py
 feeluown/gui/widgets/meta.py
 feeluown/gui/widgets/mpv.py
-feeluown/gui/widgets/mpv_old.py
 feeluown/gui/widgets/my_music.py
 feeluown/gui/widgets/playlist.py
 feeluown/gui/widgets/playlist_button.py
 feeluown/gui/widgets/playlists.py
 feeluown/gui/widgets/progress_slider.py
 feeluown/gui/widgets/provider.py
 feeluown/gui/widgets/separator.py
 feeluown/gui/widgets/settings.py
 feeluown/gui/widgets/size_grip.py
+feeluown/gui/widgets/song_minicard_list.py
 feeluown/gui/widgets/songs.py
 feeluown/gui/widgets/statusline.py
 feeluown/gui/widgets/tabbar.py
 feeluown/gui/widgets/table_toolbar.py
 feeluown/gui/widgets/textbtn.py
 feeluown/gui/widgets/textlist.py
 feeluown/gui/widgets/video.py
@@ -146,14 +149,19 @@
 feeluown/library/library.py
 feeluown/library/model_protocol.py
 feeluown/library/model_state.py
 feeluown/library/models.py
 feeluown/library/provider.py
 feeluown/library/provider_protocol.py
 feeluown/library/provider_v2.py
+feeluown/local/__init__.py
+feeluown/local/db.py
+feeluown/local/provider.py
+feeluown/local/schemas.py
+feeluown/local/ui.py
 feeluown/models/__init__.py
 feeluown/models/base.py
 feeluown/models/models.py
 feeluown/models/uri.py
 feeluown/nowplaying/__init__.py
 feeluown/nowplaying/global_hotkey_mac.py
 feeluown/nowplaying/linux/__init__.py
@@ -208,17 +216,18 @@
 feeluown/uimodels/__init__.py
 feeluown/uimodels/collection.py
 feeluown/uimodels/my_music.py
 feeluown/uimodels/playlist.py
 feeluown/uimodels/provider.py
 feeluown/utils/__init__.py
 feeluown/utils/aio.py
+feeluown/utils/audio.py
 feeluown/utils/compat.py
 feeluown/utils/dispatch.py
-feeluown/utils/janus.py
+feeluown/utils/lang.py
 feeluown/utils/patch.py
 feeluown/utils/reader.py
 feeluown/utils/request.py
 feeluown/utils/router.py
 feeluown/utils/sync.py
 feeluown/utils/typing_.py
 feeluown/utils/utils.py
```

### Comparing `feeluown-3.8.8/feeluown.egg-info/PKG-INFO` & `feeluown-3.8.9/feeluown.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 3.8.8
+Version: 3.8.9
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
         
@@ -70,12 +70,12 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: battery
-Provides-Extra: webengine
-Provides-Extra: win32
 Provides-Extra: macOS
+Provides-Extra: win32
+Provides-Extra: webengine
+Provides-Extra: dev
```

### Comparing `feeluown-3.8.8/setup.py` & `feeluown-3.8.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     description='*nix music player',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPL-3.0",
     author='feeluown',
     author_email='yinshaowen241@gmail.com',
     packages=find_packages(exclude=('tests*',)),
-    py_modules=['mpv', 'mpv_old'],
+    py_modules=['mpv'],
     package_data={
         '': ['nowplaying/linux/*.xml',
              'gui/assets/icons/*.png',
              'gui/assets/icons/*.ico',
              'gui/assets/icons/*.icns',
              'gui/assets/themes/*.qss',
              'gui/assets/themes/*.colors',
@@ -55,18 +55,18 @@
     install_requires=[
         'janus',
         'requests',
         'qasync',
         'tomlkit',
         'packaging',
         'pydantic>=1.8.1',
+        'mutagen>=1.37',
     ],
     extras_require={
-        'battery': ['fuo-local>=0.2.1',
-                    'fuo-netease>=0.4.2',
+        'battery': ['fuo-netease>=0.4.2',
                     'fuo-qqmusic>=0.2',
                     'fuo-kuwo>=0.1.1',
                     ],
         'macOS': ['pyobjc-framework-Cocoa', 'pyobjc-framework-Quartz'],
         'win32': ['pyshortcuts'],
         'webengine': ['PyQtWebEngine'],
         'dev': [
@@ -95,10 +95,13 @@
     },
     entry_points={
         'console_scripts': [
             "feeluown=feeluown.__main__:main",
             "fuo=feeluown.__main__:main",
             "feeluown-genicon=feeluown.cli.install:generate_icon",
             # "feeluown-update=feeluown.install:update"
+        ],
+        'fuo.plugins_v1': [
+            'local = feeluown.local',
         ]
     },
 )
```

### Comparing `feeluown-3.8.8/README.md` & `feeluown-3.8.9/README.md`

 * *Files identical despite different names*

