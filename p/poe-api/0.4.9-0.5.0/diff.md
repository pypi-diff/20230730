# Comparing `tmp/poe_api-0.4.9-py3-none-any.whl.zip` & `tmp/poe_api-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,44 +1,80 @@
-Zip file size: 41727 bytes, number of entries: 42
--rw-r--r--  2.0 unx    23935 b- defN 23-Jul-08 14:53 poe.py
--rw-r--r--  2.0 unx     1093 b- defN 23-May-27 23:16 poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-04 03:20 poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--  2.0 unx       97 b- defN 23-May-27 23:16 poe_graphql/BioFragment.graphql
--rw-r--r--  2.0 unx       73 b- defN 23-May-27 23:16 poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--  2.0 unx      100 b- defN 23-May-27 23:16 poe_graphql/ChatFragment.graphql
--rw-r--r--  2.0 unx    11486 b- defN 23-Jun-04 03:16 poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--  2.0 unx      686 b- defN 23-May-27 23:16 poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--  2.0 unx      154 b- defN 23-May-27 23:16 poe_graphql/ChatViewQuery.graphql
--rw-r--r--  2.0 unx      160 b- defN 23-May-27 23:16 poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--  2.0 unx      123 b- defN 23-May-27 23:16 poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--  2.0 unx      146 b- defN 23-Jun-04 03:20 poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--  2.0 unx     1083 b- defN 23-May-27 23:37 poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--  2.0 unx      103 b- defN 23-May-27 23:16 poe_graphql/HandleFragment.graphql
--rw-r--r--  2.0 unx      306 b- defN 23-May-27 23:16 poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--  2.0 unx     1885 b- defN 23-May-27 23:16 poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--  2.0 unx      135 b- defN 23-May-27 23:16 poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--  2.0 unx      194 b- defN 23-May-27 23:16 poe_graphql/MessageFragment.graphql
--rw-r--r--  2.0 unx      145 b- defN 23-May-27 23:16 poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--  2.0 unx      216 b- defN 23-May-27 23:16 poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--  2.0 unx     1666 b- defN 23-Jun-04 03:22 poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--  2.0 unx      841 b- defN 23-Jun-04 03:23 poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--  2.0 unx      912 b- defN 23-Jun-04 03:19 poe_graphql/SendMessageMutation.graphql
--rw-r--r--  2.0 unx      263 b- defN 23-May-27 23:16 poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--  2.0 unx      213 b- defN 23-May-27 23:16 poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--  2.0 unx      308 b- defN 23-May-27 23:16 poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--  2.0 unx      159 b- defN 23-May-27 23:16 poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--  2.0 unx      162 b- defN 23-May-27 23:16 poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--  2.0 unx       95 b- defN 23-May-27 23:16 poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--  2.0 unx      147 b- defN 23-May-27 23:16 poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--  2.0 unx      368 b- defN 23-May-27 23:16 poe_graphql/UserSnippetFragment.graphql
--rw-r--r--  2.0 unx      400 b- defN 23-May-27 23:16 poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--  2.0 unx     1038 b- defN 23-May-27 23:16 poe_graphql/ViewerStateFragment.graphql
--rw-r--r--  2.0 unx      657 b- defN 23-May-27 23:16 poe_graphql/ViewerStateUpdatedSubscription.graphql
+Zip file size: 64017 bytes, number of entries: 78
+-rw-r--r--  2.0 unx    24913 b- defN 23-Jul-24 15:53 poe.py
+-rw-r--r--  2.0 unx    25283 b- defN 23-Jul-29 22:19 poe/__init__.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jul-23 18:41 poe/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-23 18:41 poe/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--  2.0 unx      180 b- defN 23-Jul-23 18:41 poe/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-23 18:41 poe/poe_graphql/BioFragment.graphql
+-rw-r--r--  2.0 unx       73 b- defN 23-Jul-23 18:41 poe/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 18:41 poe/poe_graphql/ChatFragment.graphql
+-rw-r--r--  2.0 unx    11486 b- defN 23-Jul-23 18:41 poe/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--  2.0 unx      686 b- defN 23-Jul-23 18:41 poe/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-23 18:41 poe/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--  2.0 unx      160 b- defN 23-Jul-23 18:41 poe/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--  2.0 unx      123 b- defN 23-Jul-23 18:41 poe/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--  2.0 unx      146 b- defN 23-Jul-23 18:41 poe/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--  2.0 unx     1083 b- defN 23-Jul-23 18:41 poe/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-23 18:41 poe/poe_graphql/HandleFragment.graphql
+-rw-r--r--  2.0 unx      306 b- defN 23-Jul-23 18:41 poe/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--  2.0 unx     1885 b- defN 23-Jul-23 18:41 poe/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--  2.0 unx      135 b- defN 23-Jul-23 18:41 poe/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--  2.0 unx      194 b- defN 23-Jul-23 18:41 poe/poe_graphql/MessageFragment.graphql
+-rw-r--r--  2.0 unx      145 b- defN 23-Jul-23 18:41 poe/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--  2.0 unx      216 b- defN 23-Jul-23 18:41 poe/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--  2.0 unx     1759 b- defN 23-Jul-23 18:41 poe/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--  2.0 unx      941 b- defN 23-Jul-23 18:41 poe/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--  2.0 unx      912 b- defN 23-Jul-23 18:41 poe/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-23 18:41 poe/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--  2.0 unx      213 b- defN 23-Jul-23 18:41 poe/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-23 18:41 poe/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-23 18:41 poe/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-23 18:41 poe/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-23 18:41 poe/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--  2.0 unx      147 b- defN 23-Jul-23 18:41 poe/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--  2.0 unx      180 b- defN 23-Jul-23 18:41 poe/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--  2.0 unx      368 b- defN 23-Jul-23 18:41 poe/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--  2.0 unx      400 b- defN 23-Jul-23 18:41 poe/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-23 18:41 poe/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--  2.0 unx      657 b- defN 23-Jul-23 18:41 poe/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jul-23 18:41 poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-23 18:41 poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--  2.0 unx      180 b- defN 23-Jul-23 18:41 poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-23 18:41 poe_graphql/BioFragment.graphql
+-rw-r--r--  2.0 unx       73 b- defN 23-Jul-23 18:41 poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 18:41 poe_graphql/ChatFragment.graphql
+-rw-r--r--  2.0 unx    11486 b- defN 23-Jul-23 18:41 poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--  2.0 unx      686 b- defN 23-Jul-23 18:41 poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-23 18:41 poe_graphql/ChatViewQuery.graphql
+-rw-r--r--  2.0 unx      160 b- defN 23-Jul-23 18:41 poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--  2.0 unx      123 b- defN 23-Jul-23 18:41 poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--  2.0 unx      146 b- defN 23-Jul-23 18:41 poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--  2.0 unx     1083 b- defN 23-Jul-23 18:41 poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-23 18:41 poe_graphql/HandleFragment.graphql
+-rw-r--r--  2.0 unx      306 b- defN 23-Jul-23 18:41 poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--  2.0 unx     1885 b- defN 23-Jul-23 18:41 poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--  2.0 unx      135 b- defN 23-Jul-23 18:41 poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--  2.0 unx      194 b- defN 23-Jul-23 18:41 poe_graphql/MessageFragment.graphql
+-rw-r--r--  2.0 unx      145 b- defN 23-Jul-23 18:41 poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--  2.0 unx      216 b- defN 23-Jul-23 18:41 poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--  2.0 unx     1759 b- defN 23-Jul-23 18:41 poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--  2.0 unx      941 b- defN 23-Jul-23 18:41 poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--  2.0 unx      912 b- defN 23-Jul-23 18:41 poe_graphql/SendMessageMutation.graphql
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-23 18:41 poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--  2.0 unx      213 b- defN 23-Jul-23 18:41 poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-23 18:41 poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-23 18:41 poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-23 18:41 poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-23 18:41 poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--  2.0 unx      147 b- defN 23-Jul-23 18:41 poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--  2.0 unx      180 b- defN 23-Jul-23 18:41 poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--  2.0 unx      368 b- defN 23-Jul-23 18:41 poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--  2.0 unx      400 b- defN 23-Jul-23 18:41 poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-23 18:41 poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--  2.0 unx      657 b- defN 23-Jul-23 18:41 poe_graphql/ViewerStateUpdatedSubscription.graphql
 -rw-r--r--  2.0 unx        0 b- defN 23-May-27 23:16 poe_graphql/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-08 14:56 poe_api-0.4.9.dist-info/LICENSE
--rw-r--r--  2.0 unx    18418 b- defN 23-Jul-08 14:56 poe_api-0.4.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 14:56 poe_api-0.4.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-08 14:56 poe_api-0.4.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3969 b- defN 23-Jul-08 14:56 poe_api-0.4.9.dist-info/RECORD
-42 files, 107857 bytes uncompressed, 35185 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-30 00:31 poe_api-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20227 b- defN 23-Jul-30 00:31 poe_api-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 00:31 poe_api-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-30 00:31 poe_api-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7621 b- defN 23-Jul-30 00:31 poe_api-0.5.0.dist-info/RECORD
+78 files, 166231 bytes uncompressed, 51477 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,10 +1,118 @@
 Filename: poe.py
 Comment: 
 
+Filename: poe/__init__.py
+Comment: 
+
+Filename: poe/poe_graphql/AddHumanMessageMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/AddMessageBreakMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/AutoSubscriptionMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/BioFragment.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ChatAddedSubscription.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ChatFragment.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ChatListPaginationQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ChatPaginationQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ChatViewQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/DeleteHumanMessagesMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/DeleteMessageMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/DeleteUserMessagesMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ExploreBotsListPaginationQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/HandleFragment.graphql
+Comment: 
+
+Filename: poe/poe_graphql/LoginWithVerificationCodeMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/MessageAddedSubscription.graphql
+Comment: 
+
+Filename: poe/poe_graphql/MessageDeletedSubscription.graphql
+Comment: 
+
+Filename: poe/poe_graphql/MessageFragment.graphql
+Comment: 
+
+Filename: poe/poe_graphql/MessageRemoveVoteMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/MessageSetVoteMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/PoeBotCreateMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/PoeBotEditMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SendMessageMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ShareMessagesMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SignupWithVerificationCodeMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/StaleChatUpdateMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SubscriptionsMutation.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SummarizePlainPostQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SummarizeQuotePostQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/SummarizeSharePostQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/UserSnippetFragment.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ViewerInfoQuery.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ViewerStateFragment.graphql
+Comment: 
+
+Filename: poe/poe_graphql/ViewerStateUpdatedSubscription.graphql
+Comment: 
+
 Filename: poe_graphql/AddHumanMessageMutation.graphql
 Comment: 
 
 Filename: poe_graphql/AddMessageBreakMutation.graphql
 Comment: 
 
 Filename: poe_graphql/AutoSubscriptionMutation.graphql
@@ -105,23 +213,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.4.9.dist-info/LICENSE
+Filename: poe_api-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.4.9.dist-info/METADATA
+Filename: poe_api-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.4.9.dist-info/WHEEL
+Filename: poe_api-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.4.9.dist-info/top_level.txt
+Filename: poe_api-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.4.9.dist-info/RECORD
+Filename: poe_api-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -1,8 +1,9 @@
 import re, json, random, logging, time, queue, threading, traceback, hashlib, string, random, os
+import quickjs
 import requests
 import tls_client as requests_tls
 import secrets
 import websocket
 import uuid
 import random
 from pathlib import Path
@@ -13,73 +14,75 @@
 queries = {}
 
 logging.basicConfig()
 logger = logging.getLogger()
 
 user_agent = "This will be ignored! See the README for info on how to set custom headers."
 headers = {
-  "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0",
-  "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+  "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
+  "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
   "Accept-Encoding": "gzip, deflate, br",
-  "Accept-Language": "en-US,en;q=0.5",
-  "Te": "trailers",
+  "Accept-Language": "en-US,en;q=0.9",
+  "Sec-Ch-Ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"112\"",
+  "Sec-Ch-Ua-Mobile": "?0",
+  "Sec-Ch-Ua-Platform": "\"Linux\"",
   "Upgrade-Insecure-Requests": "1"
 }
-client_identifier = "firefox_102"
+client_identifier = "chrome112"
 
 def load_queries():
   for path in queries_path.iterdir():
     if path.suffix != ".graphql":
       continue
     with open(path) as f:
       queries[path.stem] = f.read()
 
 def generate_payload(query_name, variables):
   if query_name == "recv":
     return generate_recv_payload(variables)
   return {
     "query": queries[query_name],
+    "queryName": query_name,
     "variables": variables
   }
 
 def generate_recv_payload(variables):
   payload = [
     {
       "category": "poe/bot_response_speed",
       "data": variables,
     }
   ]
-  
+
   if random.random() > 0.9:
     payload.append({
       "category": "poe/statsd_event",
       "data": {
         "key": "poe.speed.web_vitals.INP",
         "value": random.randint(100, 125),
         "category": "time",
         "path": "/[handle]",
         "extra_data": {},
       },
     })
 
   return payload
 
-
 def request_with_retries(method, *args, **kwargs):
   attempts = kwargs.get("attempts") or 10
   url = args[0]
   for i in range(attempts):
     r = method(*args, **kwargs)
     if r.status_code == 200:
       return r
     if r.status_code == 307:
       if r.headers.get("Location").startswith("/login"):
         raise RuntimeError("Invalid or missing token.")
     logger.warn(f"Server returned a status code of {r.status_code} while downloading {url}. Retrying ({i+1}/{attempts})...")
-  
+
   raise RuntimeError(f"Failed to download {url} too many times.")
 
 def generate_nonce(length:int=16):
   return "".join(secrets.choice(string.ascii_letters + string.digits) for i in range(length))
 
 def get_config_path():
   if os.name == "nt":
@@ -88,45 +91,45 @@
 
 def set_saved_device_id(user_id, device_id):
   device_id_path = get_config_path() / "device_id.json"
   device_ids = {}
   if device_id_path.exists():
     with open(device_id_path) as f:
       device_ids = json.loads(f.read())
-  
+
   device_ids[user_id] = device_id
   device_id_path.parent.mkdir(parents=True, exist_ok=True)
   with open(device_id_path, "w") as f:
     f.write(json.dumps(device_ids, indent=2))
 
 def get_saved_device_id(user_id):
   device_id_path = get_config_path() / "device_id.json"
   device_ids = {}
   if device_id_path.exists():
     with open(device_id_path) as f:
       device_ids = json.loads(f.read())
-  
+
   if user_id in device_ids:
     return device_ids[user_id]
-  
+
   device_id = str(uuid.uuid4())
   device_ids[user_id] = device_id
   device_id_path.parent.mkdir(parents=True, exist_ok=True)
   with open(device_id_path, "w") as f:
     f.write(json.dumps(device_ids, indent=2))
-  
+
   return device_id
 
 class Client:
   gql_url = "https://poe.com/api/gql_POST"
   gql_recv_url = "https://poe.com/api/receive_POST"
   home_url = "https://poe.com"
   settings_url = "https://poe.com/api/settings"
 
-  def __init__(self, token, proxy=None, headers=headers, device_id=None, client_identifier=client_identifier):
+  def __init__(self, token, proxy=None, headers=headers, device_id=None, client_identifier=client_identifier, formkey=None):
     self.ws_connecting = False
     self.ws_connected = False
     self.ws_error = False
     self.connect_count = 0
     self.setup_count = 0
 
     self.token = token
@@ -135,21 +138,22 @@
     self.client_identifier = client_identifier
 
     self.active_messages = {}
     self.message_queues = {}
     self.suggestion_callbacks = {}
 
     self.headers = {**headers, **{
-      "Referrer": "https://poe.com/",
-      "Origin": "https://poe.com",
-      "Host": "poe.com",
-      "Sec-Fetch-Dest": "empty",
-      "Sec-Fetch-Mode": "cors",
+      "Cache-Control": "no-cache",
+      "Sec-Fetch-Dest": "document",
+      "Sec-Fetch-Mode": "navigate",
       "Sec-Fetch-Site": "same-origin",
+      "Sec-Fetch-User": "?1",
     }}
+    self.formkey_salt = None
+    self.formkey = formkey
 
     self.connect_ws()
 
   def setup_session(self):
     logger.info("Setting up session...")
     if self.client_identifier:
       self.session = requests_tls.Session(client_identifier=self.client_identifier)
@@ -186,65 +190,78 @@
 
     self.gql_headers = {
       "poe-formkey": self.formkey,
       "poe-tchannel": self.channel["channel"],
     }
     self.gql_headers = {**self.gql_headers, **self.headers}
     self.subscribe()
-  
+
   def get_device_id(self):
     user_id = self.viewer["poeUser"]["id"]
     device_id = get_saved_device_id(user_id)
     return device_id
-    
-  def extract_formkey(self, html):
-    script_regex = r'<script>if\(.+\)throw new Error;(.+)</script>'
-    script_text = re.search(script_regex, html).group(1)
-    key_regex = r'var .="([0-9a-f]+)",'
-    key_text = re.search(key_regex, script_text).group(1)
-    cipher_regex = r'.\[(\d+)\]=.\[(\d+)\]'
-    cipher_pairs = re.findall(cipher_regex, script_text)
-
-    formkey_list = [""] * len(cipher_pairs)
-    for pair in cipher_pairs:
-      formkey_index, key_index = map(int, pair)
-      formkey_list[formkey_index] = key_text[key_index]
-    formkey = "".join(formkey_list)[:-1] # credit to @aditiaryan on realizing my mistake
-    
+
+  #i find it funny how the contents of this function will lead 
+  #to the formkey function getting changed a few hours later
+  def extract_formkey(self, html, app_script):
+    script_regex = r'<script>(.+?)</script>'
+    vars_regex = r'window\._([a-zA-Z0-9]{10})="([a-zA-Z0-9]{10})"'
+    key, value = re.findall(vars_regex, app_script)[0]
+
+    script_text = """
+      let QuickJS = undefined, process = undefined;
+      let window = {
+        document: {a:1},
+        navigator: {
+          userAgent: "a"
+        }
+      };
+    """
+    script_text += f"window._{key} = '{value}';"
+    script_text += "".join(re.findall(script_regex, html))
+
+    function_regex = r'(window\.[a-zA-Z0-9]{17})=function'
+    function_text = re.search(function_regex, script_text).group(1)
+    script_text += f"{function_text}();"
+
+    context = quickjs.Context()
+    formkey = context.eval(script_text)
     return formkey
 
   def get_next_data(self, overwrite_vars=False):
     logger.info("Downloading next_data...")
-    
+
     r = request_with_retries(self.session.get, self.home_url)
     json_regex = r'<script id="__NEXT_DATA__" type="application\/json">(.+?)</script>'
     json_text = re.search(json_regex, r.text).group(1)
     next_data = json.loads(json_text)
 
     if overwrite_vars:
-      self.formkey = self.extract_formkey(r.text)
+      if not self.formkey:
+        script_src_regex = r'src="(https://psc2\.cf2\.poecdn\.net/[a-f0-9]{40}/_next/static/chunks/pages/_app-[a-f0-9]{16}\.js)"'
+        script_src = re.search(script_src_regex, r.text).group(1)
+        r2 = request_with_retries(self.session.get, script_src)
+        self.formkey = self.extract_formkey(r.text, r2.text)
+
       if "payload" in next_data["props"]["pageProps"]:
         self.viewer = next_data["props"]["pageProps"]["payload"]["viewer"]
       else:
         self.viewer = next_data["props"]["pageProps"]["data"]["viewer"]
       self.user_id = self.viewer["poeUser"]["id"]
       self.next_data = next_data
 
     return next_data
-  
-  def get_bot(self, display_name):
-    url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/{display_name}.json'
-    
+
+  def get_bot(self, handle):
+    url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/{handle}.json'
+
     data = request_with_retries(self.session.get, url).json()
-    if "payload" in data["pageProps"]:
-      chat_data = data["pageProps"]["payload"]["chatOfBotHandle"]
-    else:
-      chat_data = data["pageProps"]["data"]["chatOfBotHandle"]
+    chat_data = data["pageProps"]["data"]["chatOfBotHandle"]
     return chat_data
-    
+
   def get_bots(self, download_next_data=True):
     logger.info("Downloading all bots...")
     if download_next_data:
       next_data = self.get_next_data(overwrite_vars=True)
     else:
       next_data = self.next_data
 
@@ -253,136 +270,131 @@
     bot_list_url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/index.json'
     bot_list = self.viewer["availableBotsConnection"]["edges"]
 
     threads = []
     bots = {}
 
     def get_bot_thread(bot):
-      chat_data = self.get_bot(bot["node"]["displayName"])
+      chat_data = self.get_bot(bot["node"]["handle"])
       bots[chat_data["defaultBotObject"]["nickname"]] = chat_data
 
     for bot in bot_list:
       thread = threading.Thread(target=get_bot_thread, args=(bot,), daemon=True)
       threads.append(thread)
-    
+
     for thread in threads:
       thread.start()
     for thread in threads:
       thread.join()
-    
+
     self.bots = bots
-    self.bot_names = self.get_bot_names()          
+    self.bot_names = self.get_bot_names()
     return bots
-  
+
   def get_bot_by_codename(self, bot_codename):
     if bot_codename in self.bots:
       return self.bots[bot_codename]
-    
+
     #todo: cache this so it isn't re-downloaded every time
     return self.get_bot(bot_codename)
 
   def get_bot_names(self):
     bot_names = {}
     for bot_nickname in self.bots:
       bot_obj = self.bots[bot_nickname]["defaultBotObject"]
       bot_names[bot_nickname] = bot_obj["displayName"]
     return bot_names
-  
+
   def explore_bots(self, end_cursor=None, count=25):
     if not end_cursor:
       url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/explore_bots.json'
       r = request_with_retries(self.session.get, url).json()
-      if "payload" in r["pageProps"]:
-        key = "payload"
-        nodes = r["pageProps"]["payload"]["exploreBotsConnection"]["edges"]
-      else:
-        key = "data"
-        nodes = r["pageProps"]["data"]["exploreBotsConnection"]["edges"]
+      data = r["pageProps"].get("payload") or r["pageProps"]["data"]
+      nodes = data["exploreBotsConnection"]["edges"]
       bots = [node["node"] for node in nodes]
       bots = bots[:count]
       return {
         "bots": bots,
-        "end_cursor": r["pageProps"][key]["exploreBotsConnection"]["pageInfo" ]["endCursor"],
+        "end_cursor": data["exploreBotsConnection"]["pageInfo" ]["endCursor"],
       }
 
     else:
       # Use graphql to get the next page
       result = self.send_query("ExploreBotsListPaginationQuery", {
-        "count": count, 
+        "count": count,
         "cursor": end_cursor
       })
       result = result["data"]["exploreBotsConnection"]
 
       bots = [node["node"] for node in result["edges"]]
       return {
         "bots": bots,
         "end_cursor": result["pageInfo"]["endCursor"],
       }
-  
+
   def get_remaining_messages(self, chatbot):
     chat_data = self.get_bot_by_codename(chatbot)
     return chat_data["defaultBotObject"]["messageLimit"]["numMessagesRemaining"]
-      
+
   def get_channel_data(self, channel=None):
     logger.info("Downloading channel data...")
     r = request_with_retries(self.session.get, self.settings_url)
     data = r.json()
 
     return data["tchannelData"]
-  
+
   def get_websocket_url(self, channel=None):
     if channel is None:
       channel = self.channel
     query = f'?min_seq={channel["minSeq"]}&channel={channel["channel"]}&hash={channel["channelHash"]}'
-    return f'wss://{self.ws_domain}.tch.{channel["baseHost"]}/up/{channel["boxName"]}/updates'+query
+    return f'ws://{self.ws_domain}.tch.{channel["baseHost"]}/up/{channel["boxName"]}/updates'+query
 
   def send_query(self, query_name, variables, attempts=20):
     for i in range(attempts):
       json_data = generate_payload(query_name, variables)
       payload = json.dumps(json_data, separators=(",", ":"))
-      
-      base_string = payload + self.gql_headers["poe-formkey"] + "WpuLMiXEKKE98j56k"
-      
+
+      base_string = payload + self.gql_headers["poe-formkey"] + "Jb1hi3fg1MxZpzYfy"
+
       headers = {
         "content-type": "application/json",
         "poe-tag-id": hashlib.md5(base_string.encode()).hexdigest()
       }
       headers = {**self.gql_headers, **headers}
-      
+
       if query_name == "recv":
         r = request_with_retries(self.session.post, self.gql_recv_url, data=payload, headers=headers)
         return None
-      else:
-        r = request_with_retries(self.session.post, self.gql_url, data=payload, headers=headers)
-      
+
+      r = request_with_retries(self.session.post, self.gql_url, data=payload, headers=headers)
       data = r.json()
       if data["data"] == None:
-        logger.warn(f'{query_name} returned an error: {data["errors"][0]["message"]} | Retrying ({i+1}/20)')
+        logger.warn(f'{query_name} returned an error: {data["errors"][0]["message"]} | Retrying ({i+1}/20) | Response: {data}')
         time.sleep(2)
         continue
 
       return r.json()
-    
+
     raise RuntimeError(f'{query_name} failed too many times.')
-  
+
   def subscribe(self):
     logger.info("Subscribing to mutations")
     result = self.send_query("SubscriptionsMutation", {
       "subscriptions": [
         {
           "subscriptionName": "messageAdded",
           "query": queries["MessageAddedSubscription"]
         },
         {
           "subscriptionName": "viewerStateUpdated",
           "query": queries["ViewerStateUpdatedSubscription"]
         }
       ]
     })
-  
+
   def ws_run_thread(self):
     kwargs = {}
     if self.proxy:
       proxy_parsed = urlparse(self.proxy)
       kwargs = {
         "proxy_type": proxy_parsed.scheme,
         "http_proxy_host": proxy_parsed.hostname,
@@ -432,34 +444,34 @@
       timer += 0.01
       if timer > timeout:
         self.ws_connecting = False
         self.ws_connected = False
         self.ws_error = True
         ws.close()
         raise RuntimeError("Timed out waiting for websocket to connect.")
-  
+
   def disconnect_ws(self):
     self.ws_connecting = False
     self.ws_connected = False
     if self.ws:
       self.ws.close()
-  
+
   def on_ws_connect(self, ws):
     self.ws_connecting = False
     self.ws_connected = True
-  
+
   def on_ws_close(self, ws, close_status_code, close_message):
     logger.warn(f"Websocket closed with status {close_status_code}: {close_message}")
 
     self.ws_connecting = False
     self.ws_connected = False
     if self.ws_error:
       self.ws_error = False
       self.connect_ws()
-  
+
   def on_ws_error(self, ws, error):
     self.ws_connecting = False
     self.ws_connected = False
     self.ws_error = True
 
   def on_message(self, ws, msg):
     try:
@@ -471,15 +483,15 @@
       for message_str in data["messages"]:
         message_data = json.loads(message_str)
         if message_data["message_type"] != "subscriptionUpdate":
           continue
         message = message_data["payload"]["data"]["messageAdded"]
 
         #handle suggested replies
-        if "suggestedReplies" in message and type(message["suggestedReplies"]) == list and len(message["suggestedReplies"]) > 0:
+        if "suggestedReplies" in message and type(message["suggestedReplies"]) == list and len(message["suggestedReplies"]) > 0 and message["messageId"] in self.suggestion_callbacks:
           self.suggestion_callbacks[message["messageId"]](message["suggestedReplies"][-1])
           if len(message["suggestedReplies"]) >= 3:
             del self.suggestion_callbacks[message["messageId"]]
 
         copied_dict = self.active_messages.copy()
         for key, value in copied_dict.items():
           #add the message to the appropriate queue
@@ -515,24 +527,28 @@
       time.sleep(0.01)
 
     self.connect_ws()
 
     logger.info(f"Sending message to {chatbot}: {message}")
 
     chat_id = self.get_bot_by_codename(chatbot)["chatId"]
-    message_data = self.send_query("SendMessageMutation", {
-      "bot": chatbot,
-      "query": message,
-      "chatId": chat_id,
-      "source": None,
-      "clientNonce": generate_nonce(),
-      "sdid": self.device_id,
-      "withChatBreak": with_chat_break,
-    })
-    del self.active_messages["pending"]
+    try:
+      message_data = self.send_query("SendMessageMutation", {
+        "bot": chatbot,
+        "query": message,
+        "chatId": chat_id,
+        "source": None,
+        "clientNonce": generate_nonce(),
+        "sdid": self.device_id,
+        "withChatBreak": with_chat_break,
+      })
+      del self.active_messages["pending"]
+    except Exception as e:
+      del self.active_messages["pending"]
+      raise e
 
     if not message_data["data"]["messageEdgeCreate"]["message"]:
       raise RuntimeError(f"Daily limit reached for {chatbot}.")
     try:
       human_message = message_data["data"]["messageEdgeCreate"]["message"]
       human_message_id = human_message["node"]["messageId"]
     except TypeError:
@@ -565,15 +581,15 @@
       message_id = message["messageId"]
 
       # set a suggestion callback on response
       if callable(suggest_callback) and not message_id in self.suggestion_callbacks:
         self.suggestion_callbacks[message_id] = suggest_callback
 
       yield message
-    
+
     def recv_post_thread():
       bot_message_id = self.active_messages[human_message_id]
 
       # wait 2 seconds after sending the request
       time.sleep(2.5)
 
       # send recv_post after receiving the last message
@@ -586,33 +602,33 @@
         "full_response_word_count": len(last_text.split(" ")) + 1,
         "human_message_id": human_message_id,
         "bot_message_id": bot_message_id,
         "chat_id": chat_id,
         "bot_response_status": "success",
       })
       time.sleep(0.5)
-    
+
     t = threading.Thread(target=recv_post_thread, daemon=True)
     t.start()
     if not async_recv:
       t.join()
 
     del self.active_messages[human_message_id]
     del self.message_queues[human_message_id]
-  
+
   def send_chat_break(self, chatbot):
     logger.info(f"Sending chat break to {chatbot}")
     result = self.send_query("AddMessageBreakMutation", {
       "chatId": self.get_bot_by_codename(chatbot)["chatId"]}
     )
     return result["data"]["messageBreakEdgeCreate"]["message"]
 
   def get_message_history(self, chatbot, count=25, cursor=None):
     logger.info(f"Downloading {count} messages from {chatbot}")
-    
+
     messages = []
     if cursor == None:
       if not chatbot in self.bots:
         chat_data = self.get_bot(chatbot)
       else:
         chat_data = self.get_bot(self.bot_names[chatbot])
 
@@ -647,86 +663,96 @@
     logger.info(f"Deleting messages: {message_ids}")
     if not type(message_ids) is list:
       message_ids = [int(message_ids)]
 
     result = self.send_query("DeleteMessageMutation", {
       "messageIds": message_ids
     })
-  
+
   def purge_conversation(self, chatbot, count=-1):
     logger.info(f"Purging messages from {chatbot}")
     last_messages = self.get_message_history(chatbot, count=50)[::-1]
     while last_messages:
       message_ids = []
       for message in last_messages:
         if count == 0:
           break
-        count -= 1  
+        count -= 1
         message_ids.append(message["node"]["messageId"])
 
       self.delete_message(message_ids)
-            
+
       if count == 0:
         return
       last_messages = self.get_message_history(chatbot, count=50)[::-1]
-      
+
     logger.info(f"No more messages left to delete.")
 
-  def create_bot(self, handle, prompt="", base_model="chinchilla", description="", 
+  def create_bot(self, handle, prompt, display_name=None, base_model="chinchilla", description="",
                   intro_message="", api_key=None, api_bot=False, api_url=None,
                   prompt_public=True, pfp_url=None, linkification=False,
-                  markdown_rendering=True, suggested_replies=False, private=False):
+                  markdown_rendering=True, suggested_replies=False, private=False,
+                  temperature=None):
     result = self.send_query("PoeBotCreateMutation", {
       "model": base_model,
+      "displayName": display_name,
       "handle": handle,
       "prompt": prompt,
       "isPromptPublic": prompt_public,
       "introduction": intro_message,
       "description": description,
       "profilePictureUrl": pfp_url,
       "apiUrl": api_url,
       "apiKey": api_key,
       "isApiBot": api_bot,
       "hasLinkification": linkification,
       "hasMarkdownRendering": markdown_rendering,
       "hasSuggestedReplies": suggested_replies,
-      "isPrivateBot": private
+      "isPrivateBot": private,
+      "temperature": temperature
     })
 
     data = result["data"]["poeBotCreate"]
     if data["status"] != "success":
       raise RuntimeError(f"Poe returned an error while trying to create a bot: {data['status']}")
     self.get_bots()
     return data
 
-  def edit_bot(self, bot_id, handle, prompt="", base_model="chinchilla", description="", 
+  def edit_bot(self, bot_id, handle, prompt, display_name=None, base_model="chinchilla", description="",
                 intro_message="", api_key=None, api_url=None, private=False,
                 prompt_public=True, pfp_url=None, linkification=False,
-                markdown_rendering=True, suggested_replies=False):
+                markdown_rendering=True, suggested_replies=False, temperature=None, new_handle=None):
+
+    if bot_id is None and handle is not None:
+      bot_id = self.get_bot(handle)["defaultBotObject"]["botId"]
+    new_handle = new_handle or handle
+    
     result = self.send_query("PoeBotEditMutation", {
       "baseBot": base_model,
       "botId": bot_id,
-      "handle": handle,
+      "handle": new_handle,
+      "displayName": display_name,
       "prompt": prompt,
       "isPromptPublic": prompt_public,
       "introduction": intro_message,
       "description": description,
       "profilePictureUrl": pfp_url,
       "apiUrl": api_url,
       "apiKey": api_key,
       "hasLinkification": linkification,
       "hasMarkdownRendering": markdown_rendering,
       "hasSuggestedReplies": suggested_replies,
-      "isPrivateBot": private
+      "isPrivateBot": private,
+      "temperature": temperature
     })
 
     data = result["data"]["poeBotEdit"]
     if data["status"] != "success":
       raise RuntimeError(f"Poe returned an error while trying to edit a bot: {data['status']}")
     self.get_bots()
     return data
-  
+
   def purge_all_conversations(self):
     logger.info("Purging all conversations")
     self.send_query("DeleteUserMessagesMutation", {})
 
-load_queries()
+load_queries()
```

## poe_graphql/PoeBotCreateMutation.graphql

```diff
@@ -1,24 +1,26 @@
 mutation CreateBotMain_poeBotCreate_Mutation(
   $model: String!
+  $displayName: String
   $handle: String!
   $prompt: String!
   $isPromptPublic: Boolean!
   $introduction: String!
   $description: String!
   $profilePictureUrl: String
   $apiUrl: String
   $apiKey: String
   $isApiBot: Boolean
   $hasLinkification: Boolean
   $hasMarkdownRendering: Boolean
   $hasSuggestedReplies: Boolean
   $isPrivateBot: Boolean
+  $temperature: Float
 ) {
-  poeBotCreate(model: $model, handle: $handle, promptPlaintext: $prompt, isPromptPublic: $isPromptPublic, introduction: $introduction, description: $description, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, isApiBot: $isApiBot, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot) {
+  poeBotCreate(model: $model, handle: $handle, displayName: $displayName, promptPlaintext: $prompt, isPromptPublic: $isPromptPublic, introduction: $introduction, description: $description, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, isApiBot: $isApiBot, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot, temperature: $temperature) {
     status
     bot {
       id
       ...BotHeader_bot
     }
   }
 }
@@ -49,15 +51,15 @@
       url
     }
   }
   ...botHelpers_useDeletion_bot
 }
 
 fragment BotLink_bot on Bot {
-  displayName
+  handle
 }
 
 fragment IdAnnotation_node on Node {
   __isNode: __typename
   id
 }
 
@@ -65,8 +67,8 @@
   deletionState
 }
 
 fragment botHelpers_useViewerCanAccessPrivateBot on Bot {
   isPrivateBot
   viewerIsCreator
   isSystemBot
-}
+}
```

## poe_graphql/PoeBotEditMutation.graphql

```diff
@@ -1,24 +1,27 @@
 mutation EditBotMain_poeBotEdit_Mutation(
   $botId: BigInt!
   $handle: String!
+  $displayName: String
   $description: String!
   $introduction: String!
   $isPromptPublic: Boolean!
   $baseBot: String!
   $profilePictureUrl: String
   $prompt: String!
   $apiUrl: String
   $apiKey: String
   $hasLinkification: Boolean
   $hasMarkdownRendering: Boolean
   $hasSuggestedReplies: Boolean
   $isPrivateBot: Boolean
+  $temperature: Float
 ) {
-  poeBotEdit(botId: $botId, handle: $handle, description: $description, introduction: $introduction, isPromptPublic: $isPromptPublic, model: $baseBot, promptPlaintext: $prompt, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot) {
+  poeBotEdit(botId: $botId, handle: $handle, displayName: $displayName, description: $description, introduction: $introduction, isPromptPublic: $isPromptPublic, model: $baseBot, promptPlaintext: $prompt, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot, temperature: $temperature) {
     status
     bot {
       handle
       id
     }
   }
 }
+
```

## Comparing `poe_api-0.4.9.dist-info/LICENSE` & `poe_api-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.4.9.dist-info/METADATA` & `poe_api-0.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.4.9
+Version: 0.5.0
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: websocket-client
-Requires-Dist: requests[socks]
 Requires-Dist: python-socks
+Requires-Dist: quickjs
+Requires-Dist: requests[socks]
 Requires-Dist: tls-client
+Requires-Dist: websocket-client
 
 # Python Poe API
 
 [![PyPi Version](https://img.shields.io/pypi/v/poe-api.svg)](https://pypi.org/project/poe-api/)
 
 This is a reverse engineered API wrapper for Quora's Poe, which allows you free access to OpenAI's ChatGPT and GPT-4, as well as Anthropic's Claude.
 
@@ -63,34 +64,42 @@
  - Use pre-existing third party bots
 
 ## Installation:
 You can install this library by running the following command:
 ```
 pip3 install poe-api
 ```
+This library depends on `quickjs`, which does not have prebuilt binaries available for Python 3.11. Pip will attempt to compile it, but will fail if `python-dev` is not installed.
+
+On Linux, you can install it via the instructions listed here: https://stackoverflow.com/questions/21530577/fatal-error-python-h-no-such-file-or-directory
+
+On Windows and MacOS, `python-dev` should be included with your existing Python installation.
 
 ## Documentation:
 Examples can be found in the `/examples` directory. To run these examples, pass in your token as a command-line argument.
 ```
 python3 examples/temporary_message.py "TOKEN_HERE"
 ```
 
 ### Finding Your Token:
 Log into [Poe](https://poe.com) on any desktop web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `p-b` cookie in the following menus:
  - Chromium: Devtools > Application > Cookies > poe.com
  - Firefox: Devtools > Storage > Cookies
  - Safari: Devtools > Storage > Cookies
 
+Note that excessive usage of this library may lead to your account getting banned. It is recommended that you set your own rate limits, and that you use an alt account that you don't value. See [issue #118](https://github.com/ading2210/poe-api/issues/118) for more details. If your requests are infrequent, the risk for a ban is very low.
+
 ### Using the Client:
 To use this library, simply import `poe` and create a `poe.Client` instance. The Client class accepts the following arguments:
  - `token` - The token to use. 
  - `proxy = None` - The proxy to use, in the format `protocol://host:port`. The `socks5h` protocol is recommended, as it also proxies the DNS queries.
  - `device_id = None` - The device ID to use. If this is not specified, it will be randomly generated and stored on the disk. 
  - `headers = headers` - The headers to use. This defaults to the headers specified in `poe.headers`.
  - `client_identifier = client_identifier` - The client identifier that will be passed into the TLS client library. This defaults to the one specified in `poe.client_identifier`.
+ - `formkey = None` - The formkey to use. Only supply this option if initializing the client without it fails. You can find this value by going into your browser's devtools, looking in the network tab for a `gql_POST` request, and taking the value of the `poe-formkey` request header. The formkey that you use must come from a browser that matches the headers that you've set in `poe.headers`. Keep in mind that the default browser is Chromium 112.
 
 Regular Example:
 ```python
 import poe
 client = poe.Client("TOKEN_HERE")
 ```
 
@@ -106,21 +115,22 @@
 The client downloads all of the available bots upon initialization and stores them within `client.bots`. A dictionary that maps bot codenames to their display names can be found at `client.bot_names`. If you want to refresh these values, you can call `client.get_bots`. This function takes the following arguments:
  - `download_next_data = True` - Whether or not to re-download the `__NEXT_DATA__`, which is required if the bot list has changed. 
 
 ```python
 print(json.dumps(client.bot_names, indent=2))
 """
 {
-  "capybara": "Sage",
-  "a2": "Claude-instant",
-  "nutria": "Dragonfly",
-  "a2_100k": "Claude-instant-100k",
-  "beaver": "GPT-4",
+  "capybara": "Assistant",
   "chinchilla": "ChatGPT",
-  "a2_2": "Claude+"
+  "beaver": "GPT-4",
+  "a2_100k": "Claude-instant-100k",
+  "a2": "Claude-instant",
+  "agouti": "ChatGPT-16k",
+  "a2_2": "Claude-2-100k",
+  "acouchy": "Google-PaLM"
 }
 """
 ```
 
 Note that, on free accounts, Claude+ (a2_2) has a limit of 3 messages per day and GPT-4 (beaver) has a limit of 1 message per day. Claude-instant-100k (c2_100k) is completely inaccessible for free accounts. For all the other chatbots, there seems to be a rate limit of 10 messages per minute.
 
 #### Using 3rd Party Bots:
@@ -160,48 +170,53 @@
 
 Since display names are the same as the codenames for custom bots, you can simply pass the bot's display name into `client.send_message` to send it a message.
 
 #### Creating New Bots:
 You can create a new bot using the `client.create_bot` function, which accepts the following arguments:
  - `handle` - The handle of the new bot.
  - `prompt = ""` - The prompt for the new bot.
- - `base_model = "chinchilla"` - The model that the new bot uses. This must be either `"chinchilla"` (ChatGPT)  or `"a2"` (Claude).
+ - `display_name = None` - The display name for the new bot.
+ - `base_model = "chinchilla"` - The model that the new bot uses. This must be either `"chinchilla"` (ChatGPT) or `"a2"` (Claude). If you've subscribed, you can use `"beaver"` (ChatGPT4) or  "a2_2"` (Claude-2-100k).
  - `description = ""` - The description for the new bot.
  - `intro_message = ""` - The intro message for the new bot. If this is an empty string then the bot will not have an intro message.
  - `prompt_public = True` - Whether or not the prompt should be publicly visible. 
  - `pfp_url = None` - The URL for the bot's profile picture. Currently, there is no way to actually upload a custom image using this library.
  - `linkification = False` - Whether or not the bot should turn some text in the response into clickable links.
  - `markdown_rendering = True` - Whether or not to enable markdown rendering for the bot's responses.
  - `suggested_replies = False` - Whether or not the bot should suggest possible replies after each response.
  - `private = False` - Whether or not the bot should be private.
+ - `temperature = None`: - The temperature for the new bot.
 
 Use these arguments if you want the new bot to use your own API (as detailed [here](https://github.com/poe-platform/api-bot-tutorial)):
  - `api_key = None` - The API key for the new bot. 
  - `api_bot = False` - Whether or not the bot has API functionally enabled.
  - `api_url = None` - The API URL for the new bot.
 
 A full example of how to create and edit bots is located at `examples/create_bot.py`.
 ```python
 new_bot = client.create_bot(bot_name, "prompt goes here", base_model="a2")
 ```
 
 #### Editing a Bot:
 You can edit a custom bot using the `client.edit_bot` function, which accepts the following arguments:
- - `bot_id` - The `botId` of the bot to edit.
- - `handle` - The handle of the bot to edit.
- - `prompt` - The prompt for the new bot.
- - `base_model = "chinchilla"` - The new model that the bot uses. This must be either `"chinchilla"` (ChatGPT)  or `"a2"` (Claude). Previously, it was possible to set this to `"beaver"` (GPT-4), which would bypass the free account restrictions, but this is now patched.
+ - `bot_id` - The `botId` of the bot to edit. This can also be set to `None`.
+ - `handle` - The handle for the bot you're editing.
+ - `prompt` - The new prompt for the bot.
+ - `new_handle = None` - The new handle for the bot. By default the handle will not change.
+ - `display_name = None` - The new display name for the bot.
+ - `base_model = "chinchilla"` - The new model that the bot uses. This must be either `"chinchilla"` (ChatGPT) or `"a2"` (Claude). If you've subscribed, you can use `"beaver"` (ChatGPT4) or  "a2_2"` (Claude-2-100k).
  - `description = ""` - The new description for the bot.
  - `intro_message = ""` - The new intro message for the bot. If this is an empty string then the bot will not have an intro message.
  - `prompt_public = True` - Whether or not the prompt should be publicly visible. 
  - `pfp_url = None` - The URL for the bot's profile picture. Currently, there is no way to actually upload a custom image using this library.
  - `linkification = False` - Whether or not the bot should turn some text in the response into clickable links.
  - `markdown_rendering = True` - Whether or not to enable markdown rendering for the bot's responses.
  - `suggested_replies = False` - Whether or not the bot should suggest possible replies after each response.
  - `private = False` - Whether or not the bot should be private.
+ - `temperature = None`: - The new temperature for the this bot.
 
 Bot API related arguments:
  - `api_key = None` - The new API key for the bot. 
  - `api_url = None` - The new API URL for the bot.
 
 A full example of how to create and edit bots is located at `examples/create_bot.py`.
 ```python
@@ -337,31 +352,32 @@
 If you want to change the headers that are spoofed, set `poe.headers` after importing the library. 
 
 To use your browser's own headers, visit [this site](https://headers.uniqueostrich18.repl.co/), and copy-paste its contents.
 ```python
 import poe
 poe.headers = {
   "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0",
-  "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+  'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*q=0.8,application/signed-exchange;v=b3;q=0.7',
   "Accept-Encoding": "gzip, deflate, br",
-  "Accept-Language": "en-US,en;q=0.5",
-  "Te": "trailers",
+  'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
   "Upgrade-Insecure-Requests": "1"
 }
 ```
 
 The following headers will be ignored and overwritten:
 ```python
 {
   "Referrer": "https://poe.com/",
   "Origin": "https://poe.com",
   "Host": "poe.com",
-  "Sec-Fetch-Dest": "empty",
-  "Sec-Fetch-Mode": "cors",
-  "Sec-Fetch-Site": "same-origin"
+  "Cache-Control": "no-cache",
+  "Sec-Fetch-Dest": "document",
+  "Sec-Fetch-Mode": "navigate",
+  "Sec-Fetch-Site": "same-origin",
+  "Sec-Fetch-User": "?1",
 }
 ```
 
 Previously, this was done through `poe.user_agent`, but that variable is now completely ignored.
 
 You'd also want to change `poe.client_identifier` to match the user-agent that you have set. See the [Python-TLS-Client documentation](https://github.com/FlorianREGAZ/Python-Tls-Client#examples) for some sample values. Keep in mind that spoofing Chrome/Firefox versions >= 110 may be detectable. 
 ```python
```

