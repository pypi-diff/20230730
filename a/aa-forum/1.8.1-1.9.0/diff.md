# Comparing `tmp/aa_forum-1.8.1.tar.gz` & `tmp/aa_forum-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_forum-1.8.1.tar", last modified: Sun Jun 26 22:40:34 2022, max compression
+gzip compressed data, was "aa_forum-1.9.0.tar", last modified: Mon Jul 11 06:35:31 2022, max compression
```

## Comparing `aa_forum-1.8.1.tar` & `aa_forum-1.9.0.tar`

### file list

```diff
@@ -1,198 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.029498 aa_forum-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    13018 2022-06-26 22:40:17.000000 aa_forum-1.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-26 22:40:17.000000 aa_forum-1.8.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-26 22:40:17.000000 aa_forum-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-26 22:40:17.000000 aa_forum-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15337 2022-06-26 22:40:34.029498 aa_forum-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13996 2022-06-26 22:40:17.000000 aa_forum-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    54038 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/admin-board-options.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   111021 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/admin-view.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    30790 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/feature-announcement-board.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   113759 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/forum-index.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    57392 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/start-new-topic.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    93987 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/topic-overview.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   122941 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/docs/images/topic-view.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum/helper/
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/helper/eve_images.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/helper/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/helper/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/helper/webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    13063 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/migrations/0002_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/migrations/0003_board_discord_webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/migrations/0005_announcement_boards.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17703 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/scripts/drop_tables.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/scripts/fake_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/static/aa_forum/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/cs.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     1078 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/el.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     1024 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt-br.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     1153 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     1539 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/vi.js
--rwxr-xr-x   0 runner    (1001) docker     (121)      916 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/zh.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    22802 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/static/aa_forum/css/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    12546 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/css/aa-forum.css
--rw-r--r--   0 runner    (1001) docker     (121)     6952 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/css/aa-forum.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/static/aa_forum/images/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/images/new.gif
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/images/new_none.png
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/images/new_some.png
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/images/off.png
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/images/on.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/
--rw-r--r--   0 runner    (1001) docker     (121)     7246 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.jquery.json
--rw-r--r--   0 runner    (1001) docker     (121)    35653 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.js
--rw-r--r--   0 runner    (1001) docker     (121)    14081 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     9333 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/sumoselect.css
--rw-r--r--   0 runner    (1001) docker     (121)     7335 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/sumoselect.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/templates/aa_forum/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/administration/
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.021498 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/topic/
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/categories.html
--rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/new-category.html
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/breadcrumb.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/form/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
--rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/board.html
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/forum-index.html
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
--rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/search/
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/search/pagination.html
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/search/search-form.html
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/search/search-result.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.013498 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/administration/
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/administration/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/board.html
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/modify-message.html
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/new-topic.html
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/topic.html
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/search/
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templates/aa_forum/view/search/results.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.025498 aa_forum-1.8.1/aa_forum/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templatetags/aa_forum_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templatetags/aa_forum_template_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templatetags/aa_forum_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/templatetags/aa_forum_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.029498 aa_forum-1.8.1/aa_forum/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    23041 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (121)    29345 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)    14523 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     7127 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_views_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    44329 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/test_views_forum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6085 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.029498 aa_forum-1.8.1/aa_forum/views/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14342 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/views/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    39418 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/views/forum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-06-26 22:40:17.000000 aa_forum-1.8.1/aa_forum/views/search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:40:34.017498 aa_forum-1.8.1/aa_forum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15337 2022-06-26 22:40:33.000000 aa_forum-1.8.1/aa_forum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7467 2022-06-26 22:40:34.000000 aa_forum-1.8.1/aa_forum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 22:40:33.000000 aa_forum-1.8.1/aa_forum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 22:40:32.000000 aa_forum-1.8.1/aa_forum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-26 22:40:33.000000 aa_forum-1.8.1/aa_forum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-26 22:40:33.000000 aa_forum-1.8.1/aa_forum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-26 22:40:17.000000 aa_forum-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-06-26 22:40:34.029498 aa_forum-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.480958 aa_forum-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-11 06:35:10.000000 aa_forum-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    15337 2022-07-11 06:35:31.480958 aa_forum-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13996 2022-07-11 06:35:10.000000 aa_forum-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.464958 aa_forum-1.9.0/aa_forum/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    54038 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/admin-board-options.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   111021 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/admin-view.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    30790 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/feature-announcement-board.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   113759 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/forum-index.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    57392 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/start-new-topic.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    93987 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/topic-overview.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   122941 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/docs/images/topic-view.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.464958 aa_forum-1.9.0/aa_forum/helper/
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/helper/eve_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/helper/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/helper/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/helper/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.464958 aa_forum-1.9.0/aa_forum/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    13063 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/migrations/0002_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/migrations/0003_board_discord_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/migrations/0005_announcement_boards.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17703 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.464958 aa_forum-1.9.0/aa_forum/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/scripts/drop_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/scripts/fake_messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/static/aa_forum/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.468958 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.468958 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/cs.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1078 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/el.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1024 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt-br.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1153 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1539 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/vi.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)      916 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/zh.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    22802 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/static/aa_forum/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)    12546 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/css/aa-forum.css
+-rw-r--r--   0 runner    (1001) docker     (121)     6952 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/css/aa-forum.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/static/aa_forum/images/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/images/new.gif
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/images/new_none.png
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/images/new_some.png
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/images/off.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/images/on.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/
+-rw-r--r--   0 runner    (1001) docker     (121)     7246 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/templates/aa_forum/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/templates/aa_forum/bundles/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/administration/
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/topic/
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.472958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/
+-rw-r--r--   0 runner    (1001) docker     (121)     5319 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/categories.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/new-category.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/breadcrumb.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/form/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/board.html
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/forum-index.html
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/search/
+-rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/search/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/search/search-form.html
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/search/search-result.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.460958 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.476958 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/administration/
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/administration/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.480958 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/board.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/modify-message.html
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/new-topic.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/topic.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.480958 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/search/
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templates/aa_forum/view/search/results.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.480958 aa_forum-1.9.0/aa_forum/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templatetags/aa_forum_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templatetags/aa_forum_template_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templatetags/aa_forum_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/templatetags/aa_forum_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.480958 aa_forum-1.9.0/aa_forum/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23041 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29345 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14523 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7127 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_views_admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44329 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/test_views_forum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6085 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.480958 aa_forum-1.9.0/aa_forum/views/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14342 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/views/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39418 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/views/forum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-07-11 06:35:10.000000 aa_forum-1.9.0/aa_forum/views/search.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 06:35:31.464958 aa_forum-1.9.0/aa_forum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15337 2022-07-11 06:35:31.000000 aa_forum-1.9.0/aa_forum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7182 2022-07-11 06:35:31.000000 aa_forum-1.9.0/aa_forum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 06:35:31.000000 aa_forum-1.9.0/aa_forum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 06:35:31.000000 aa_forum-1.9.0/aa_forum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-11 06:35:31.000000 aa_forum-1.9.0/aa_forum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-11 06:35:31.000000 aa_forum-1.9.0/aa_forum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-11 06:35:10.000000 aa_forum-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-07-11 06:35:31.480958 aa_forum-1.9.0/setup.cfg
```

### Comparing `aa_forum-1.8.1/LICENSE` & `aa_forum-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/PKG-INFO` & `aa_forum-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_forum
-Version: 1.8.1
+Version: 1.9.0
 Summary: Simple forum for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-forum
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_forum-1.8.1/README.md` & `aa_forum-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/admin.py` & `aa_forum-1.9.0/aa_forum/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/auth_hooks.py` & `aa_forum-1.9.0/aa_forum/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/constants.py` & `aa_forum-1.9.0/aa_forum/constants.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/admin-board-options.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/admin-board-options.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/admin-view.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/admin-view.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/feature-announcement-board.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/feature-announcement-board.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/forum-index.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/forum-index.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/start-new-topic.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/start-new-topic.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/topic-overview.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/topic-overview.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/docs/images/topic-view.jpg` & `aa_forum-1.9.0/aa_forum/docs/images/topic-view.jpg`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/forms.py` & `aa_forum-1.9.0/aa_forum/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/helper/eve_images.py` & `aa_forum-1.9.0/aa_forum/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/helper/text.py` & `aa_forum-1.9.0/aa_forum/helper/text.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/helper/webhook.py` & `aa_forum-1.9.0/aa_forum/helper/webhook.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/managers.py` & `aa_forum-1.9.0/aa_forum/managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/migrations/0001_initial.py` & `aa_forum-1.9.0/aa_forum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/migrations/0002_default_settings.py` & `aa_forum-1.9.0/aa_forum/migrations/0002_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py` & `aa_forum-1.9.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/migrations/0005_announcement_boards.py` & `aa_forum-1.9.0/aa_forum/migrations/0005_announcement_boards.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/models.py` & `aa_forum-1.9.0/aa_forum/models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/scripts/fake_messages.py` & `aa_forum-1.9.0/aa_forum/scripts/fake_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/signals.py` & `aa_forum-1.9.0/aa_forum/signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon-hdpi.png` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon.png` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ar.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/bg.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/cs.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/de.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/el.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/en.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/es.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/et.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/eu.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fi.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fr.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/he.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/hu.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/it.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ja.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ko.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nb.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nl.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nn.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pl.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt-br.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ru.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/sk.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/tr.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/uk.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/vi.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/zh.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.min.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/ckeditor/plugins/youtube/plugin.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/css/aa-forum.css` & `aa_forum-1.9.0/aa_forum/static/aa_forum/css/aa-forum.css`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/css/aa-forum.min.css` & `aa_forum-1.9.0/aa_forum/static/aa_forum/css/aa-forum.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/images/new_none.png` & `aa_forum-1.9.0/aa_forum/static/aa_forum/images/new_none.png`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/images/new_some.png` & `aa_forum-1.9.0/aa_forum/static/aa_forum/images/new_some.png`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/images/off.png` & `aa_forum-1.9.0/aa_forum/static/aa_forum/images/off.png`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/images/on.png` & `aa_forum-1.9.0/aa_forum/static/aa_forum/images/on.png`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js` & `aa_forum-1.9.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/categories.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/categories.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/administration/new-category.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/administration/new-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/breadcrumb.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/board.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/menu.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/partials/search/pagination.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/partials/search/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/administration/index.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/modify-message.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 {% extends "aa_forum/base.html" %}
 
 {% load aa_forum_versioned_static %}
 {% load static %}
 {% load i18n %}
 
-{% block page_title %}{% translate "Forum (Administration)" %}{% endblock %}
+{% block page_title %}{% translate "Modify Message » Forum" %}{% endblock %}
 
 {% block aa_forum_header %}
     <br>
 
     {% include "aa_forum/partials/menu.html" %}
+    {% include "aa_forum/partials/breadcrumb.html" with category=board.category board=board topic=message.topic modify_message=True %}
 {% endblock %}
 
 {% block aa_forum_body %}
-    <script type="application/javascript">
-        let aaForumAdminSettings = {}
-    </script>
-
-    {% include "aa_forum/partials/administration/categories.html" %}
+    {% include "aa_forum/partials/forum/topic/modify-message.html" %}
 {% endblock %}
 
 {% block extra_css %}
-    {% include "bundles/jquery-ui-css.html" %}
-
     <link rel="stylesheet" type="text/css" href="{% aa_forum_static 'aa_forum/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% static 'aa_forum/libs/sumoselect/3.0.2-66/sumoselect.min.css' %}">
     <link rel="stylesheet" type="text/css" href="{% aa_forum_static 'aa_forum/css/aa-forum.min.css' %}">
 {% endblock %}
 
 {% block extra_javascript %}
-    {% include "bundles/jquery-ui-js.html" %}
-
-    <script type="application/javascript" src="{% static 'aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.min.js' %}"></script>
-    <script type="application/javascript" src="{% aa_forum_static 'aa_forum/javascript/aa-forum-admin.min.js' %}"></script>
+    <script type="application/javascript" src="{% static 'ckeditor/ckeditor-init.js' %}"></script>
+    <script type="application/javascript" src="{% static 'ckeditor/ckeditor/ckeditor.js' %}"></script>
 {% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% extends "aa_forum/base.html" %} {% load aa_forum_versioned_static %} {% load
-static %} {% load i18n %} {% block page_title %}{% translate "Forum
-(Administration)" %}{% endblock %} {% block aa_forum_header %}
-{% include "aa_forum/partials/menu.html" %} {% endblock %} {% block
-aa_forum_body %}
- {% include "aa_forum/partials/administration/categories.html" %} {% endblock
-%} {% block extra_css %} {% include "bundles/jquery-ui-css.html" %}
+static %} {% load i18n %} {% block page_title %}{% translate "Modify Message Â»
+Forum" %}{% endblock %} {% block aa_forum_header %}
+{% include "aa_forum/partials/menu.html" %} {% include "aa_forum/partials/
+breadcrumb.html" with category=board.category board=board topic=message.topic
+modify_message=True %} {% endblock %} {% block aa_forum_body %} {% include
+"aa_forum/partials/forum/topic/modify-message.html" %} {% endblock %} {% block
+extra_css %}
 
-
- {% endblock %} {% block extra_javascript %} {% include "bundles/jquery-ui-
-js.html" %}
+ {% endblock %} {% block extra_javascript %}
  {% endblock %}
```

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/board.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/index.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/modify-message.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,49 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6161 5f66  {% extends "aa_f
 00000010: 6f72 756d 2f62 6173 652e 6874 6d6c 2220  orum/base.html" 
 00000020: 257d 0a0a 7b25 206c 6f61 6420 6161 5f66  %}..{% load aa_f
 00000030: 6f72 756d 5f76 6572 7369 6f6e 6564 5f73  orum_versioned_s
 00000040: 7461 7469 6320 257d 0a7b 2520 6c6f 6164  tatic %}.{% load
-00000050: 2073 7461 7469 6320 257d 0a7b 2520 6c6f   static %}.{% lo
-00000060: 6164 2069 3138 6e20 257d 0a0a 7b25 2062  ad i18n %}..{% b
-00000070: 6c6f 636b 2070 6167 655f 7469 746c 6520  lock page_title 
-00000080: 257d 7b25 2074 7261 6e73 6c61 7465 2022  %}{% translate "
-00000090: 4d6f 6469 6679 204d 6573 7361 6765 20c2  Modify Message .
-000000a0: bb20 466f 7275 6d22 2025 7d7b 2520 656e  . Forum" %}{% en
-000000b0: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
-000000c0: 6f63 6b20 6161 5f66 6f72 756d 5f68 6561  ock aa_forum_hea
-000000d0: 6465 7220 257d 0a20 2020 203c 6272 3e0a  der %}.    <br>.
-000000e0: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
-000000f0: 2261 615f 666f 7275 6d2f 7061 7274 6961  "aa_forum/partia
-00000100: 6c73 2f6d 656e 752e 6874 6d6c 2220 257d  ls/menu.html" %}
-00000110: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
-00000120: 2261 615f 666f 7275 6d2f 7061 7274 6961  "aa_forum/partia
-00000130: 6c73 2f62 7265 6164 6372 756d 622e 6874  ls/breadcrumb.ht
-00000140: 6d6c 2220 7769 7468 2063 6174 6567 6f72  ml" with categor
-00000150: 793d 626f 6172 642e 6361 7465 676f 7279  y=board.category
-00000160: 2062 6f61 7264 3d62 6f61 7264 2074 6f70   board=board top
-00000170: 6963 3d6d 6573 7361 6765 2e74 6f70 6963  ic=message.topic
-00000180: 206d 6f64 6966 795f 6d65 7373 6167 653d   modify_message=
-00000190: 5472 7565 2025 7d0a 7b25 2065 6e64 626c  True %}.{% endbl
-000001a0: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
-000001b0: 2061 615f 666f 7275 6d5f 626f 6479 2025   aa_forum_body %
-000001c0: 7d0a 2020 2020 7b25 2069 6e63 6c75 6465  }.    {% include
-000001d0: 2022 6161 5f66 6f72 756d 2f70 6172 7469   "aa_forum/parti
-000001e0: 616c 732f 666f 7275 6d2f 746f 7069 632f  als/forum/topic/
-000001f0: 6d6f 6469 6679 2d6d 6573 7361 6765 2e68  modify-message.h
-00000200: 746d 6c22 2025 7d0a 7b25 2065 6e64 626c  tml" %}.{% endbl
-00000210: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
-00000220: 2065 7874 7261 5f63 7373 2025 7d0a 2020   extra_css %}.  
-00000230: 2020 3c6c 696e 6b20 7265 6c3d 2273 7479    <link rel="sty
-00000240: 6c65 7368 6565 7422 2074 7970 653d 2274  lesheet" type="t
-00000250: 6578 742f 6373 7322 2068 7265 663d 227b  ext/css" href="{
-00000260: 2520 6161 5f66 6f72 756d 5f73 7461 7469  % aa_forum_stati
-00000270: 6320 2761 615f 666f 7275 6d2f 6373 732f  c 'aa_forum/css/
-00000280: 6161 2d62 6f6f 7473 7472 6170 2d66 6978  aa-bootstrap-fix
-00000290: 2e6d 696e 2e63 7373 2720 257d 223e 0a20  .min.css' %}">. 
-000002a0: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
-000002b0: 796c 6573 6865 6574 2220 7479 7065 3d22  ylesheet" type="
-000002c0: 7465 7874 2f63 7373 2220 6872 6566 3d22  text/css" href="
-000002d0: 7b25 2061 615f 666f 7275 6d5f 7374 6174  {% aa_forum_stat
-000002e0: 6963 2027 6161 5f66 6f72 756d 2f63 7373  ic 'aa_forum/css
-000002f0: 2f61 612d 666f 7275 6d2e 6d69 6e2e 6373  /aa-forum.min.cs
-00000300: 7327 2025 7d22 3e0a 7b25 2065 6e64 626c  s' %}">.{% endbl
-00000310: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
-00000320: 2065 7874 7261 5f6a 6176 6173 6372 6970   extra_javascrip
-00000330: 7420 257d 0a20 2020 203c 7363 7269 7074  t %}.    <script
-00000340: 2074 7970 653d 2261 7070 6c69 6361 7469   type="applicati
-00000350: 6f6e 2f6a 6176 6173 6372 6970 7422 2073  on/javascript" s
-00000360: 7263 3d22 7b25 2073 7461 7469 6320 2763  rc="{% static 'c
-00000370: 6b65 6469 746f 722f 636b 6564 6974 6f72  keditor/ckeditor
-00000380: 2d69 6e69 742e 6a73 2720 257d 223e 3c2f  -init.js' %}"></
-00000390: 7363 7269 7074 3e0a 2020 2020 3c73 6372  script>.    <scr
-000003a0: 6970 7420 7479 7065 3d22 6170 706c 6963  ipt type="applic
-000003b0: 6174 696f 6e2f 6a61 7661 7363 7269 7074  ation/javascript
-000003c0: 2220 7372 633d 227b 2520 7374 6174 6963  " src="{% static
-000003d0: 2027 636b 6564 6974 6f72 2f63 6b65 6469   'ckeditor/ckedi
-000003e0: 746f 722f 636b 6564 6974 6f72 2e6a 7327  tor/ckeditor.js'
-000003f0: 2025 7d22 3e3c 2f73 6372 6970 743e 0a7b   %}"></script>.{
-00000400: 2520 656e 6462 6c6f 636b 2025 7d0a       % endblock %}.
+00000050: 2069 3138 6e20 257d 0a0a 7b25 2062 6c6f   i18n %}..{% blo
+00000060: 636b 2070 6167 655f 7469 746c 6520 257d  ck page_title %}
+00000070: 7b25 2074 7261 6e73 6c61 7465 2022 4d6f  {% translate "Mo
+00000080: 6469 6679 2054 6f70 6963 20c2 bb20 466f  dify Topic .. Fo
+00000090: 7275 6d22 2025 7d7b 2520 656e 6462 6c6f  rum" %}{% endblo
+000000a0: 636b 2025 7d0a 0a7b 2520 626c 6f63 6b20  ck %}..{% block 
+000000b0: 6161 5f66 6f72 756d 5f68 6561 6465 7220  aa_forum_header 
+000000c0: 257d 0a20 2020 203c 6272 3e0a 0a20 2020  %}.    <br>..   
+000000d0: 207b 2520 696e 636c 7564 6520 2261 615f   {% include "aa_
+000000e0: 666f 7275 6d2f 7061 7274 6961 6c73 2f6d  forum/partials/m
+000000f0: 656e 752e 6874 6d6c 2220 257d 0a20 2020  enu.html" %}.   
+00000100: 207b 2520 696e 636c 7564 6520 2261 615f   {% include "aa_
+00000110: 666f 7275 6d2f 7061 7274 6961 6c73 2f62  forum/partials/b
+00000120: 7265 6164 6372 756d 622e 6874 6d6c 2220  readcrumb.html" 
+00000130: 7769 7468 2063 6174 6567 6f72 793d 626f  with category=bo
+00000140: 6172 642e 6361 7465 676f 7279 2062 6f61  ard.category boa
+00000150: 7264 3d62 6f61 7264 2074 6f70 6963 3d6d  rd=board topic=m
+00000160: 6573 7361 6765 2e74 6f70 6963 206d 6f64  essage.topic mod
+00000170: 6966 795f 6d65 7373 6167 653d 5472 7565  ify_message=True
+00000180: 2025 7d0a 7b25 2065 6e64 626c 6f63 6b20   %}.{% endblock 
+00000190: 257d 0a0a 7b25 2062 6c6f 636b 2061 615f  %}..{% block aa_
+000001a0: 666f 7275 6d5f 626f 6479 2025 7d0a 2020  forum_body %}.  
+000001b0: 2020 7b25 2069 6e63 6c75 6465 2022 6161    {% include "aa
+000001c0: 5f66 6f72 756d 2f70 6172 7469 616c 732f  _forum/partials/
+000001d0: 666f 7275 6d2f 746f 7069 632f 6d6f 6469  forum/topic/modi
+000001e0: 6679 2d74 6f70 6963 2e68 746d 6c22 2025  fy-topic.html" %
+000001f0: 7d0a 7b25 2065 6e64 626c 6f63 6b20 257d  }.{% endblock %}
+00000200: 0a0a 7b25 2062 6c6f 636b 2065 7874 7261  ..{% block extra
+00000210: 5f63 7373 2025 7d0a 2020 2020 3c6c 696e  _css %}.    <lin
+00000220: 6b20 7265 6c3d 2273 7479 6c65 7368 6565  k rel="styleshee
+00000230: 7422 2074 7970 653d 2274 6578 742f 6373  t" type="text/cs
+00000240: 7322 2068 7265 663d 227b 2520 6161 5f66  s" href="{% aa_f
+00000250: 6f72 756d 5f73 7461 7469 6320 2761 615f  orum_static 'aa_
+00000260: 666f 7275 6d2f 6373 732f 6161 2d62 6f6f  forum/css/aa-boo
+00000270: 7473 7472 6170 2d66 6978 2e6d 696e 2e63  tstrap-fix.min.c
+00000280: 7373 2720 257d 223e 0a20 2020 203c 6c69  ss' %}">.    <li
+00000290: 6e6b 2072 656c 3d22 7374 796c 6573 6865  nk rel="styleshe
+000002a0: 6574 2220 7479 7065 3d22 7465 7874 2f63  et" type="text/c
+000002b0: 7373 2220 6872 6566 3d22 7b25 2061 615f  ss" href="{% aa_
+000002c0: 666f 7275 6d5f 7374 6174 6963 2027 6161  forum_static 'aa
+000002d0: 5f66 6f72 756d 2f63 7373 2f61 612d 666f  _forum/css/aa-fo
+000002e0: 7275 6d2e 6d69 6e2e 6373 7327 2025 7d22  rum.min.css' %}"
+000002f0: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+00000300: 0a                                       .
```

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/new-topic.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/new-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/topic.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templates/aa_forum/view/search/results.html` & `aa_forum-1.9.0/aa_forum/templates/aa_forum/view/search/results.html`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templatetags/aa_forum_search.py` & `aa_forum-1.9.0/aa_forum/templatetags/aa_forum_search.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templatetags/aa_forum_template_variables.py` & `aa_forum-1.9.0/aa_forum/templatetags/aa_forum_template_variables.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/templatetags/aa_forum_user.py` & `aa_forum-1.9.0/aa_forum/templatetags/aa_forum_user.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_helpers.py` & `aa_forum-1.9.0/aa_forum/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_integration.py` & `aa_forum-1.9.0/aa_forum/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_managers.py` & `aa_forum-1.9.0/aa_forum/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_models.py` & `aa_forum-1.9.0/aa_forum/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_signals.py` & `aa_forum-1.9.0/aa_forum/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_templatetags.py` & `aa_forum-1.9.0/aa_forum/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_views_admin.py` & `aa_forum-1.9.0/aa_forum/tests/test_views_admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/test_views_forum.py` & `aa_forum-1.9.0/aa_forum/tests/test_views_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/tests/utils.py` & `aa_forum-1.9.0/aa_forum/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/urls.py` & `aa_forum-1.9.0/aa_forum/urls.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/views/admin.py` & `aa_forum-1.9.0/aa_forum/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/views/forum.py` & `aa_forum-1.9.0/aa_forum/views/forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum/views/search.py` & `aa_forum-1.9.0/aa_forum/views/search.py`

 * *Files identical despite different names*

### Comparing `aa_forum-1.8.1/aa_forum.egg-info/PKG-INFO` & `aa_forum-1.9.0/aa_forum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-forum
-Version: 1.8.1
+Version: 1.9.0
 Summary: Simple forum for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-forum
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_forum-1.8.1/aa_forum.egg-info/SOURCES.txt` & `aa_forum-1.9.0/aa_forum.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-CHANGELOG.md
-CODEOWNERS
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 aa_forum/__init__.py
 aa_forum/admin.py
 aa_forum/app_settings.py
 aa_forum/apps.py
@@ -83,20 +80,17 @@
 aa_forum/static/aa_forum/images/new_some.png
 aa_forum/static/aa_forum/images/off.png
 aa_forum/static/aa_forum/images/on.png
 aa_forum/static/aa_forum/javascript/aa-forum-admin.js
 aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
 aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
 aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
-aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.jquery.json
-aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.js
-aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/jquery.sumoselect.min.js
-aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/sumoselect.css
-aa_forum/static/aa_forum/libs/sumoselect/3.0.2-66/sumoselect.min.css
 aa_forum/templates/aa_forum/base.html
+aa_forum/templates/aa_forum/bundles/sumoselect-css.html
+aa_forum/templates/aa_forum/bundles/sumoselect-js.html
 aa_forum/templates/aa_forum/modals/administration/delete-board.html
 aa_forum/templates/aa_forum/modals/administration/delete-category.html
 aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
 aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
 aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
 aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
 aa_forum/templates/aa_forum/partials/breadcrumb.html
```

### Comparing `aa_forum-1.8.1/setup.cfg` & `aa_forum-1.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 long_description_content_type = text/markdown
 author = Peter Pfeufer
 author_email = development@ppfeufer.de
 maintainer = Peter Pfeufer
 maintainer_email = development@ppfeufer.de
 license = GPL-3.0
 license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -33,25 +34,28 @@
 	eveonline
 	forum
 project_urls = 
 	Issue / Bug Reports = https://github.com/ppfeufer/aa-forum/issues
 	Changelog = https://github.com/ppfeufer/aa-forum/blob/master/CHANGELOG.md
 
 [options]
-packages = find:
+packages = find_namespace:
 install_requires = 
-	allianceauth>=2.11.0
+	allianceauth>=2.14.0
 	allianceauth-app-utils>=1.12.0
 	dhooks-lite>=0.6.1
 	django-ckeditor>=6.2.0
 	unidecode>=1.3.3
 python_requires = ~=3.7
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
-include = aa_forum
+include = aa_forum*
+
+[options.package_data]
+* = *
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

