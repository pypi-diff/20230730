# Comparing `tmp/extract_msg-0.41.5.tar.gz` & `tmp/extract_msg-0.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_msg-0.41.5.tar", last modified: Sun Jun 11 17:19:39 2023, max compression
+gzip compressed data, was "extract_msg-0.42.0.tar", last modified: Sat Jul 29 23:17:13 2023, max compression
```

## Comparing `extract_msg-0.41.5.tar` & `extract_msg-0.42.0.tar`

### file list

```diff
@@ -1,71 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 17:19:38.998645 extract_msg-0.41.5/
--rw-rw-rw-   0        0        0    76104 2023-06-11 17:19:36.000000 extract_msg-0.41.5/CHANGELOG.md
--rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.41.5/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.41.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12267 2023-06-11 17:19:38.999643 extract_msg-0.41.5/PKG-INFO
--rw-rw-rw-   0        0        0    11460 2023-06-11 17:19:36.000000 extract_msg-0.41.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 17:19:38.950775 extract_msg-0.41.5/extract_msg/
--rw-rw-rw-   0        0        0     2254 2023-06-11 17:19:36.000000 extract_msg-0.41.5/extract_msg/__init__.py
--rw-rw-rw-   0        0        0     3542 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:19:38.976705 extract_msg-0.41.5/extract_msg/_rtf/
--rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/_rtf/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/_rtf/create_doc.py
--rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/_rtf/inject_rtf.py
--rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/_rtf/token.py
--rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/_rtf/tokenize_rtf.py
--rw-rw-rw-   0        0        0     6954 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/appointment.py
--rw-rw-rw-   0        0        0    13262 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/attachment.py
--rw-rw-rw-   0        0        0    16369 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/attachment_base.py
--rw-rw-rw-   0        0        0     3169 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/calendar.py
--rw-rw-rw-   0        0        0    21050 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/calendar_base.py
--rw-rw-rw-   0        0        0    27572 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/constants.py
--rw-rw-rw-   0        0        0    50103 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/contact.py
--rw-rw-rw-   0        0        0    58866 2023-05-25 02:02:13.000000 extract_msg-0.41.5/extract_msg/enums.py
--rw-rw-rw-   0        0        0     3377 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:19:38.979696 extract_msg-0.41.5/extract_msg/logging-config/
--rw-rw-rw-   0        0        0     2082 2023-05-09 19:47:37.000000 extract_msg-0.41.5/extract_msg/logging-config/logging-nt.json
--rw-rw-rw-   0        0        0     2058 2023-05-09 19:47:37.000000 extract_msg-0.41.5/extract_msg/logging-config/logging-posix.json
--rw-rw-rw-   0        0        0     3588 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/meeting_cancellation.py
--rw-rw-rw-   0        0        0     1628 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/meeting_exception.py
--rw-rw-rw-   0        0        0     3771 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/meeting_forward.py
--rw-rw-rw-   0        0        0     2043 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/meeting_related.py
--rw-rw-rw-   0        0        0     6784 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/meeting_request.py
--rw-rw-rw-   0        0        0     2415 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/meeting_response.py
--rw-rw-rw-   0        0        0      375 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/message.py
--rw-rw-rw-   0        0        0    59297 2023-06-11 17:19:36.000000 extract_msg-0.41.5/extract_msg/message_base.py
--rw-rw-rw-   0        0        0      201 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/message_signed.py
--rw-rw-rw-   0        0        0     7201 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/message_signed_base.py
--rw-rw-rw-   0        0        0    39208 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/msg.py
--rw-rw-rw-   0        0        0    12647 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/named.py
--rw-rw-rw-   0        0        0    41608 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/ole_writer.py
--rw-rw-rw-   0        0        0     2578 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/post.py
--rw-rw-rw-   0        0        0     6723 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/prop.py
--rw-rw-rw-   0        0        0     7602 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/properties.py
--rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.41.5/extract_msg/py.typed
--rw-rw-rw-   0        0        0    12677 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/recipient.py
--rw-rw-rw-   0        0        0     8976 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/signed_attachment.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:19:38.997650 extract_msg-0.41.5/extract_msg/structures/
--rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/__init__.py
--rw-rw-rw-   0        0        0    11677 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/_helpers.py
--rw-rw-rw-   0        0        0     6676 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/business_card.py
--rw-rw-rw-   0        0        0    19038 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/entry_id.py
--rw-rw-rw-   0        0        0     6161 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/misc_id.py
--rw-rw-rw-   0        0        0     7370 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/recurrence_pattern.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/report_tag.py
--rw-rw-rw-   0        0        0     1391 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/system_time.py
--rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/time_zone_definition.py
--rw-rw-rw-   0        0        0     2440 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/time_zone_struct.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/structures/tz_rule.py
--rw-rw-rw-   0        0        0    13190 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/task.py
--rw-rw-rw-   0        0        0     4162 2023-05-09 19:54:43.000000 extract_msg-0.41.5/extract_msg/task_request.py
--rw-rw-rw-   0        0        0    56485 2023-06-11 16:43:24.000000 extract_msg-0.41.5/extract_msg/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:19:38.968727 extract_msg-0.41.5/extract_msg.egg-info/
--rw-rw-rw-   0        0        0    12267 2023-06-11 17:19:38.000000 extract_msg-0.41.5/extract_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2023-06-11 17:19:38.000000 extract_msg-0.41.5/extract_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 17:19:38.000000 extract_msg-0.41.5/extract_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-11 17:19:38.000000 extract_msg-0.41.5/extract_msg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      237 2023-06-11 17:19:38.000000 extract_msg-0.41.5/extract_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 17:19:38.000000 extract_msg-0.41.5/extract_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-06-11 16:43:24.000000 extract_msg-0.41.5/requirements.txt
--rw-rw-rw-   0        0        0      167 2023-06-11 17:19:39.001639 extract_msg-0.41.5/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.41.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.839953 extract_msg-0.42.0/
+-rw-rw-rw-   0        0        0    83564 2023-07-29 23:17:08.000000 extract_msg-0.42.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.42.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.42.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12250 2023-07-29 23:17:13.841401 extract_msg-0.42.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11428 2023-07-29 23:17:08.000000 extract_msg-0.42.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.680050 extract_msg-0.42.0/extract_msg/
+-rw-rw-rw-   0        0        0     1937 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/__init__.py
+-rw-rw-rw-   0        0        0     3629 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.728475 extract_msg-0.42.0/extract_msg/_rtf/
+-rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/_rtf/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/_rtf/create_doc.py
+-rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/_rtf/inject_rtf.py
+-rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/_rtf/token.py
+-rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/_rtf/tokenize_rtf.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.745803 extract_msg-0.42.0/extract_msg/attachments/
+-rw-rw-rw-   0        0        0     5756 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/__init__.py
+-rw-rw-rw-   0        0        0     7343 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/attachment.py
+-rw-rw-rw-   0        0        0    23050 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/attachment_base.py
+-rw-rw-rw-   0        0        0     1188 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/broken_att.py
+-rw-rw-rw-   0        0        0     6056 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/custom_att.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.751755 extract_msg-0.42.0/extract_msg/attachments/custom_att_handler/
+-rw-rw-rw-   0        0        0     2591 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/custom_att_handler/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/custom_att_handler/custom_handler.py
+-rw-rw-rw-   0        0        0     4754 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
+-rw-rw-rw-   0        0        0     5009 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/emb_msg_att.py
+-rw-rw-rw-   0        0        0     9052 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/signed_att.py
+-rw-rw-rw-   0        0        0     1162 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/unsupported_att.py
+-rw-rw-rw-   0        0        0     2442 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/attachments/web_att.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.758736 extract_msg-0.42.0/extract_msg/constants/
+-rw-rw-rw-   0        0        0     5670 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/constants/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/constants/ps.py
+-rw-rw-rw-   0        0        0     1078 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/constants/re.py
+-rw-rw-rw-   0        0        0     3237 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/constants/st.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.631965 extract_msg-0.42.0/extract_msg/data/
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.761728 extract_msg-0.42.0/extract_msg/data/logging-config/
+-rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/data/logging-config/logging-nt.json
+-rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/data/logging-config/logging-posix.json
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.764722 extract_msg-0.42.0/extract_msg/encoding/
+-rw-rw-rw-   0        0        0    12602 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.778684 extract_msg-0.42.0/extract_msg/encoding/_dt/
+-rw-rw-rw-   0        0        0      116 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_mac_ce.py
+-rw-rw-rw-   0        0        0     2785 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_mac_cyrillic.py
+-rw-rw-rw-   0        0        0     2721 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_mac_greek.py
+-rw-rw-rw-   0        0        0     2627 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_mac_iceland.py
+-rw-rw-rw-   0        0        0     2628 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_mac_turkish.py
+-rw-rw-rw-   0        0        0     2422 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_win874_dec.py
+-rw-rw-rw-   0        0        0   298022 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/_dt/_win950_dec.py
+-rw-rw-rw-   0        0        0    12122 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/encoding/utils.py
+-rw-rw-rw-   0        0        0    58987 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/enums.py
+-rw-rw-rw-   0        0        0     4048 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.812594 extract_msg-0.42.0/extract_msg/msg_classes/
+-rw-rw-rw-   0        0        0     1249 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/__init__.py
+-rw-rw-rw-   0        0        0     6722 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/appointment.py
+-rw-rw-rw-   0        0        0     2930 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/calendar.py
+-rw-rw-rw-   0        0        0    19319 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/calendar_base.py
+-rw-rw-rw-   0        0        0    46043 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/contact.py
+-rw-rw-rw-   0        0        0     3590 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/meeting_cancellation.py
+-rw-rw-rw-   0        0        0     1630 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/meeting_exception.py
+-rw-rw-rw-   0        0        0     3737 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/meeting_forward.py
+-rw-rw-rw-   0        0        0     1900 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/meeting_related.py
+-rw-rw-rw-   0        0        0     6577 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/meeting_request.py
+-rw-rw-rw-   0        0        0     2223 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/meeting_response.py
+-rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/message.py
+-rw-rw-rw-   0        0        0    55795 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/message_base.py
+-rw-rw-rw-   0        0        0      201 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/message_signed.py
+-rw-rw-rw-   0        0        0     5016 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/message_signed_base.py
+-rw-rw-rw-   0        0        0    37987 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/msg.py
+-rw-rw-rw-   0        0        0     2610 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/post.py
+-rw-rw-rw-   0        0        0     1675 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/sticky_note.py
+-rw-rw-rw-   0        0        0    12686 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/task.py
+-rw-rw-rw-   0        0        0     4017 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/msg_classes/task_request.py
+-rw-rw-rw-   0        0        0    41660 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/ole_writer.py
+-rw-rw-rw-   0        0        0     8558 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/open_msg.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.816583 extract_msg-0.42.0/extract_msg/properties/
+-rw-rw-rw-   0        0        0      549 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/properties/__init__.py
+-rw-rw-rw-   0        0        0    15147 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/properties/named.py
+-rw-rw-rw-   0        0        0     6806 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/properties/prop.py
+-rw-rw-rw-   0        0        0     7627 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/properties/properties_store.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.42.0/extract_msg/py.typed
+-rw-rw-rw-   0        0        0    13687 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/recipient.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.838955 extract_msg-0.42.0/extract_msg/structures/
+-rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/structures/__init__.py
+-rw-rw-rw-   0        0        0    11737 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/_helpers.py
+-rw-rw-rw-   0        0        0     6682 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/business_card.py
+-rw-rw-rw-   0        0        0    19050 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/entry_id.py
+-rw-rw-rw-   0        0        0     6179 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/misc_id.py
+-rw-rw-rw-   0        0        0     7352 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/recurrence_pattern.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/structures/report_tag.py
+-rw-rw-rw-   0        0        0     1397 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/system_time.py
+-rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.42.0/extract_msg/structures/time_zone_definition.py
+-rw-rw-rw-   0        0        0     2443 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/time_zone_struct.py
+-rw-rw-rw-   0        0        0     3254 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/structures/tz_rule.py
+-rw-rw-rw-   0        0        0    48405 2023-07-29 23:17:08.000000 extract_msg-0.42.0/extract_msg/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:17:13.699997 extract_msg-0.42.0/extract_msg.egg-info/
+-rw-rw-rw-   0        0        0    12250 2023-07-29 23:17:13.000000 extract_msg-0.42.0/extract_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3136 2023-07-29 23:17:13.000000 extract_msg-0.42.0/extract_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 23:17:13.000000 extract_msg-0.42.0/extract_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-29 23:17:13.000000 extract_msg-0.42.0/extract_msg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      270 2023-07-29 23:17:13.000000 extract_msg-0.42.0/extract_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-29 23:17:13.000000 extract_msg-0.42.0/extract_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      193 2023-07-29 23:17:08.000000 extract_msg-0.42.0/requirements.txt
+-rw-rw-rw-   0        0        0      218 2023-07-29 23:17:13.842401 extract_msg-0.42.0/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.42.0/setup.py
```

### Comparing `extract_msg-0.41.5/CHANGELOG.md` & `extract_msg-0.42.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,63 @@
+**v0.42.0**
+* [[TeamMsgExtractor #372](https://github.com/TeamMsgExtractor/msg-extractor/issues/372)] Changed the way that the save functions return a value. This makes the return value from all save functions much more informative, allowing a user to separate if a file or folder (or if more than one) was saved from the function. It also guarantees that all classes from this module will return the relevant path(s) if data is actually saved.
+* [[TeamMsgExtractor #288](https://github.com/TeamMsgExtractor/msg-extractor/issues/288)] Added feature to allow attachment save functions to simply overwrite existing files of the same name. This can be done with the `overwriteExisting` keyword argument from code or the `--overwrite-existing` option from the command line.
+* [[TeamMsgExtractor #40](https://github.com/TeamMsgExtractor/msg-extractor/issues/40)] Added new submodule `custom_attachments`. This submodule provides an extendable way to handle custom attachment types, attachment types whose structure and formatting are not defined in the Microsoft documentation for MSG files. This includes a handler to at least partially cover support for Outlook images.
+* [[TeamMsgExtractor #373](https://github.com/TeamMsgExtractor/msg-extractor/issues/373)] Added the `encoding` submodule for encoding tasks, including proper support for Microsoft's implementation of CP950. This gets added to the codecs list as "windows-950".
+    * Added infrastructure to make it easy to add variable-byte (up to two bytes) encodings and single-byte encodings.
+    * Added the following encodings:
+        * windows-874
+        * x-mac-ce
+        * x-mac-cyrillic
+        * x-mac-greek
+        * x-mac-icelandic
+        * x-mac-turkish
+* Fixed an issue in the save functions that left the possibility for the zip files to not end up closing if the save function created it and then had an exception.
+* Added new property `AttachmentBase.clsid` which returns the listed CLSID value of the data stream/storage of the attachment.
+* Changed internal behavior of `MSGFile.attachments`. This should not cause any noticeable changes to the output.
+* Refactored code significantly to make it more organized.
+* Changed the exports from the main module to only include an important subset of the module. For other items, you'll have to import the submodule that it falls under to access it. Submodules export all important pieces, so it will be easier to find.
+    * This includes having many modules be under entirely new paths. Some of these changes have been done with no deprecation, something I generally try to avoid. This is happening at the same time as the public api is significantly changing, which makes it more acceptable.
+* Fixed `__main__` using the wrong enum for error behavior.
+* Fixed `Named.get` being severely out of date (it's not used anywhere by the module which is why it wasn't noticed).
+* Fixed `Named.__getitem__` being entirely case-sensitive.
+* Switched much of the internal code (and the `treePath` property of all classes that have it) to using `weakref.ReferenceType` to avoid hard cyclic references.
+* Fixed `Recipient._getTypedStream` never returning a value.
+* Added additional type hints in various places.
+* Modified tests.py to only run if it is run as a file instead of imported.
+* Changed `knownMsgClass` to a private function since it is explicitly not being exported by any part of the module.
+* Removed unused function `getFullClassName`.
+* Fixes to the HTML body when saving as HTML will no longer require the `preparedHtml`/`--prepared-html` option.
+* Removed unused exceptions.
+* Entirely reoganized the way attachments are initialized, including the class that will be used in various circumstances. Embedded MSG files, custom attachments, and web attachments will all use dedicated classes that are subclasses of `AttachmentBase`.
+    * With this change, the way to specify a new `Attachment` class is to override the function used when creating attachments. This can be done by passing `attachmentInit = myFunction` as an option to `openMsg`. This function MUST return an instance of `AttachmentBase`.
+* Added first implementation of web attachments. Saving is not currently possible, but basic relevant property access is now possible. Saving will not be stopped by this attachment if `skipNotImplemented = True` is passed to the save function.
+* Changed the option to suppress `RTFDE` errors to fall under the `ErrorBehavior` enum. Usage of the original option will be allowable, but is being marked as deprecated. However, it is still a dedicated option from the command line.
+    * Also fixed the option not properly ignoring some `RTFDE` errors, specifically the ones that it is normal for the module to throw.
+* Removed some constants that are not used by the module.
+* Updated to support `RTFDE` version `0.1.0`. Users encountering random errors from that module should find that those errors have disappeared. If you get errors from it still, bring up the issue on their GitHub.
+* Fixed bug that would cause weird behavior if you gave an empty string as the path for an MSG file.
+* Added support for `IPM.StickyNote`.
+* Fixed an issue that would cause MSG file to never close if an error happened during any of the `__init__` functions for MSG classes.
+* Removed unneeded `chardet` dependency.
+* Removed `Contact.__init__` as it didn't provide any unique behavior.
+* Changed the documentation of `openMsg` to specify that it accepts all options recognized by `MSGFile` subclasses, allowing the doc string to not be modified every time one of them is changed.
+    * Changed the documentation of various `__init__` methods to do the same thing.
+* Added `dataType` property to `AttachmentBase` and `SignedAttachment` for checking the class that the data will be, if accessible. Returns `None` if the data is inaccessible, including because accessing it would throw an exception.
+* Added new enum `InsecureFeatures` and option `insecureFeatures`. This option will allow certain features with security implications to be used for files that you trust. Currently the only feature it supports is the usage of `PIL`/`Pillow` to open and modify images. All features like this will be opt-in to reduce possible vulnerabilities.
+* Modified all custom exceptions the module uses to derive from a single base class for better organization.
+    * Added new exceptions to handle some of the situations previously handled by base Python exceptions.
+* Changed internal handling of the `prefix` option for `MSGFile.__init__` (and therefore `openMsg`). If you are not setting this manually, you should notice little difference.
+* Made enums less strict and converted all using `fromBits` to be `IntFlag` enums.
+* Fixed `CalendarBase.keywords` being blatantly incorrect (it was so bad I don't know how it slipped through).
+* Fixed `Contact.gender` being blatantly incorrect.
+* Fixed sender not being properly decoded in some circumstances.
+* Changed behavior of `MSGFile` to have `olefile` raise defects of type `DEFECT_INCORRECT` and above instead of just `DEFECT_FATAL`. Uncaught issues of `DEFECT_INCORRECT` can often cause the module to have parsing issues that may be misleading, this just ensures the issue is clarified. This behavior can be reverted back to the previous with `ErrorBehavior.OLE_DEFECT_INCORRECT`.
+* Fixed potential issues that may have made is possible for certain attachments to ignore filename conflict resolution code.
+
 **v0.41.5**
 * Fixed an issue from version `0.41.3` where the header being present but missing the `From` field would cause an exception.
 
 **v0.41.4**
 * Fixed an issue in the last version that would break the decoding function if the contents were not encoded.
 * Updated `tzlocal` and allow future updates for `compressed_rtf` and `ebcdic`.
```

### Comparing `extract_msg-0.41.5/LICENSE.txt` & `extract_msg-0.42.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/PKG-INFO` & `extract_msg-0.42.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: extract_msg
-Version: 0.41.5
+Version: 0.42.0
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: mime
+Provides-Extra: image
 License-File: LICENSE.txt
 
 |License: GPL v3| |PyPI3| |PyPI2|
 
 extract-msg
 =============
 
@@ -70,70 +71,62 @@
 
 
 #########REWRITE COMMAND LINE USAGE#############
 Currently, the README is in the process of being redone. For now, please
 refer to the usage information provided from the program's help dialog:
 ::
 
-    usage: extract_msg [-h] [--use-content-id] [--validate] [--json] [--file-logging] [-v] [--log LOG] [--config CONFIGPATH]
-                       [--out OUTPATH] [--use-filename] [--dump-stdout] [--html] [--pdf] [--wk-path WKPATH]
-                       [--wk-options [WKOPTIONS ...]] [--prepared-html] [--charset CHARSET] [--raw] [--rtf] [--allow-fallback]
-                       [--skip-body-not-found] [--zip ZIP] [--save-header] [--attachments-only] [--skip-hidden] [--no-folders]
-                       [--skip-embedded] [--extract-embedded] [--skip-not-implemented] [--out-name OUTNAME | --glob] [--ignore-rtfde]
-                       [--progress]
-                       msg [msg ...]
-
-    extract_msg: Extracts emails and attachments saved in Microsoft Outlook's .msg files. https://github.com/TeamMsgExtractor/msg-
-    extractor
-
-    positional arguments:
-      msg                   An MSG file to be parsed.
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      --use-content-id, --cid
-                            Save attachments by their Content ID, if they have one. Useful when working with the HTML body.
-      --validate            Turns on file validation mode. Turns off regular file output.
-      --json                Changes to write output files as json.
-      --file-logging        Enables file logging. Implies --verbose level 1.
-      -v, --verbose         Turns on console logging. Specify more than once for higher verbosity.
-      --log LOG             Set the path to write the file log to.
-      --config CONFIGPATH   Set the path to load the logging config from.
-      --out OUTPATH         Set the folder to use for the program output. (Default: Current directory)
-      --use-filename        Sets whether the name of each output is based on the msg filename.
-      --dump-stdout         Tells the program to dump the message body (plain text) to stdout. Overrides saving arguments.
-      --html                Sets whether the output should be HTML. If this is not possible, will error.
-      --pdf                 Saves the body as a PDF. If this is not possible, will error.
-      --wk-path WKPATH      Overrides the path for finding wkhtmltopdf.
-      --wk-options [WKOPTIONS ...]
-                            Sets additional options to be used in wkhtmltopdf. Should be a series of options and values, replacing the -
-                            or -- in the beginning with + or ++, respectively. For example: --wk-options "+O Landscape"
-      --prepared-html       When used in conjunction with --html, sets whether the HTML output should be prepared for embedded
-                            attachments.
-      --charset CHARSET     Character set to use for the prepared HTML in the added tag. (Default: utf-8)
-      --raw                 Sets whether the output should be raw. If this is not possible, will error.
-      --rtf                 Sets whether the output should be RTF. If this is not possible, will error.
-      --allow-fallback      Tells the program to fallback to a different save type if the selected one is not possible.
-      --skip-body-not-found
-                            Skips saving the body if the body cannot be found, rather than throwing an error.
-      --zip ZIP             Path to use for saving to a zip file.
-      --save-header         Store the header in a separate file.
-      --attachments-only    Specify to only save attachments from an msg file.
-      --skip-hidden         Skips any attachment marked as hidden (usually ones embedded in the body).
-      --no-folders          Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with
-                            --out-name.
-      --skip-embedded       Skips all embedded MSG files when saving attachments.
-      --extract-embedded    Extracts the embedded MSG files as MSG files instead of running their save functions.
-      --skip-not-implemented, --skip-ni
-                            Skips any attachments that are not implemented, allowing saving of the rest of the message.
-      --out-name OUTNAME    Name to be used with saving the file output. Cannot be used if you are saving more than one file.
-      --glob, --wildcard    Interpret all paths as having wildcards. Incompatible with --out-name.
-      --ignore-rtfde        Ignores all errors thrown from RTFDE when trying to save. Useful for allowing fallback to continue when an
-                            exception happens.
-      --progress            Shows what file the program is currently working on during it's progress.
+     usage: extract_msg [-h] [--use-content-id] [--json] [--file-logging] [-v] [--log LOG] [--config CONFIGPATH] [--out OUTPATH] [--use-filename] [--dump-stdout] [--html] [--pdf] [--wk-path WKPATH] [--wk-options [WKOPTIONS ...]]
+                        [--prepared-html] [--charset CHARSET] [--raw] [--rtf] [--allow-fallback] [--skip-body-not-found] [--zip ZIP] [--save-header] [--attachments-only] [--skip-hidden] [--no-folders] [--skip-embedded] [--extract-embedded]
+                        [--overwrite-existing] [--skip-not-implemented] [--out-name OUTNAME | --glob] [--ignore-rtfde] [--progress]
+                        msg [msg ...]
+
+     extract_msg: Extracts emails and attachments saved in Microsoft Outlook's .msg files. https://github.com/TeamMsgExtractor/msg-extractor
+
+     positional arguments:
+       msg                   An MSG file to be parsed.
+
+     options:
+       -h, --help            show this help message and exit
+       --use-content-id, --cid
+                             Save attachments by their Content ID, if they have one. Useful when working with the HTML body.
+       --json                Changes to write output files as json.
+       --file-logging        Enables file logging. Implies --verbose level 1.
+       -v, --verbose         Turns on console logging. Specify more than once for higher verbosity.
+       --log LOG             Set the path to write the file log to.
+       --config CONFIGPATH   Set the path to load the logging config from.
+       --out OUTPATH         Set the folder to use for the program output. (Default: Current directory)
+       --use-filename        Sets whether the name of each output is based on the msg filename.
+       --dump-stdout         Tells the program to dump the message body (plain text) to stdout. Overrides saving arguments.
+       --html                Sets whether the output should be HTML. If this is not possible, will error.
+       --pdf                 Saves the body as a PDF. If this is not possible, will error.
+       --wk-path WKPATH      Overrides the path for finding wkhtmltopdf.
+       --wk-options [WKOPTIONS ...]
+                             Sets additional options to be used in wkhtmltopdf. Should be a series of options and values, replacing the - or -- in the beginning with + or ++, respectively. For example: --wk-options "+O Landscape"
+       --prepared-html       When used in conjunction with --html, sets whether the HTML output should be prepared for embedded attachments.
+       --charset CHARSET     Character set to use for the prepared HTML in the added tag. (Default: utf-8)
+       --raw                 Sets whether the output should be raw. If this is not possible, will error.
+       --rtf                 Sets whether the output should be RTF. If this is not possible, will error.
+       --allow-fallback      Tells the program to fallback to a different save type if the selected one is not possible.
+       --skip-body-not-found
+                             Skips saving the body if the body cannot be found, rather than throwing an error.
+       --zip ZIP             Path to use for saving to a zip file.
+       --save-header         Store the header in a separate file.
+       --attachments-only    Specify to only save attachments from an msg file.
+       --skip-hidden         Skips any attachment marked as hidden (usually ones embedded in the body).
+       --no-folders          Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with --out-name.
+       --skip-embedded       Skips all embedded MSG files when saving attachments.
+       --extract-embedded    Extracts the embedded MSG files as MSG files instead of running their save functions.
+       --overwrite-existing  Disables filename conflict resolution code for attachments when saving a file, causing files to be overwriten if two attachments with the same filename are on an MSG file.
+       --skip-not-implemented, --skip-ni
+                             Skips any attachments that are not implemented, allowing saving of the rest of the message.
+       --out-name OUTNAME    Name to be used with saving the file output. Cannot be used if you are saving more than one file.
+       --glob, --wildcard    Interpret all paths as having wildcards. Incompatible with --out-name.
+       --ignore-rtfde        Ignores all errors thrown from RTFDE when trying to save. Useful for allowing fallback to continue when an exception happens.
+       --progress            Shows what file the program is currently working on during it's progress.
 
 **To use this in your own script**, start by using:
 
 ::
 
      import extract_msg
 
@@ -261,16 +254,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.5-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.5/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.0-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.42.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.5/README.rst` & `extract_msg-0.42.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -55,70 +55,62 @@
 
 
 #########REWRITE COMMAND LINE USAGE#############
 Currently, the README is in the process of being redone. For now, please
 refer to the usage information provided from the program's help dialog:
 ::
 
-    usage: extract_msg [-h] [--use-content-id] [--validate] [--json] [--file-logging] [-v] [--log LOG] [--config CONFIGPATH]
-                       [--out OUTPATH] [--use-filename] [--dump-stdout] [--html] [--pdf] [--wk-path WKPATH]
-                       [--wk-options [WKOPTIONS ...]] [--prepared-html] [--charset CHARSET] [--raw] [--rtf] [--allow-fallback]
-                       [--skip-body-not-found] [--zip ZIP] [--save-header] [--attachments-only] [--skip-hidden] [--no-folders]
-                       [--skip-embedded] [--extract-embedded] [--skip-not-implemented] [--out-name OUTNAME | --glob] [--ignore-rtfde]
-                       [--progress]
-                       msg [msg ...]
-
-    extract_msg: Extracts emails and attachments saved in Microsoft Outlook's .msg files. https://github.com/TeamMsgExtractor/msg-
-    extractor
-
-    positional arguments:
-      msg                   An MSG file to be parsed.
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      --use-content-id, --cid
-                            Save attachments by their Content ID, if they have one. Useful when working with the HTML body.
-      --validate            Turns on file validation mode. Turns off regular file output.
-      --json                Changes to write output files as json.
-      --file-logging        Enables file logging. Implies --verbose level 1.
-      -v, --verbose         Turns on console logging. Specify more than once for higher verbosity.
-      --log LOG             Set the path to write the file log to.
-      --config CONFIGPATH   Set the path to load the logging config from.
-      --out OUTPATH         Set the folder to use for the program output. (Default: Current directory)
-      --use-filename        Sets whether the name of each output is based on the msg filename.
-      --dump-stdout         Tells the program to dump the message body (plain text) to stdout. Overrides saving arguments.
-      --html                Sets whether the output should be HTML. If this is not possible, will error.
-      --pdf                 Saves the body as a PDF. If this is not possible, will error.
-      --wk-path WKPATH      Overrides the path for finding wkhtmltopdf.
-      --wk-options [WKOPTIONS ...]
-                            Sets additional options to be used in wkhtmltopdf. Should be a series of options and values, replacing the -
-                            or -- in the beginning with + or ++, respectively. For example: --wk-options "+O Landscape"
-      --prepared-html       When used in conjunction with --html, sets whether the HTML output should be prepared for embedded
-                            attachments.
-      --charset CHARSET     Character set to use for the prepared HTML in the added tag. (Default: utf-8)
-      --raw                 Sets whether the output should be raw. If this is not possible, will error.
-      --rtf                 Sets whether the output should be RTF. If this is not possible, will error.
-      --allow-fallback      Tells the program to fallback to a different save type if the selected one is not possible.
-      --skip-body-not-found
-                            Skips saving the body if the body cannot be found, rather than throwing an error.
-      --zip ZIP             Path to use for saving to a zip file.
-      --save-header         Store the header in a separate file.
-      --attachments-only    Specify to only save attachments from an msg file.
-      --skip-hidden         Skips any attachment marked as hidden (usually ones embedded in the body).
-      --no-folders          Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with
-                            --out-name.
-      --skip-embedded       Skips all embedded MSG files when saving attachments.
-      --extract-embedded    Extracts the embedded MSG files as MSG files instead of running their save functions.
-      --skip-not-implemented, --skip-ni
-                            Skips any attachments that are not implemented, allowing saving of the rest of the message.
-      --out-name OUTNAME    Name to be used with saving the file output. Cannot be used if you are saving more than one file.
-      --glob, --wildcard    Interpret all paths as having wildcards. Incompatible with --out-name.
-      --ignore-rtfde        Ignores all errors thrown from RTFDE when trying to save. Useful for allowing fallback to continue when an
-                            exception happens.
-      --progress            Shows what file the program is currently working on during it's progress.
+     usage: extract_msg [-h] [--use-content-id] [--json] [--file-logging] [-v] [--log LOG] [--config CONFIGPATH] [--out OUTPATH] [--use-filename] [--dump-stdout] [--html] [--pdf] [--wk-path WKPATH] [--wk-options [WKOPTIONS ...]]
+                        [--prepared-html] [--charset CHARSET] [--raw] [--rtf] [--allow-fallback] [--skip-body-not-found] [--zip ZIP] [--save-header] [--attachments-only] [--skip-hidden] [--no-folders] [--skip-embedded] [--extract-embedded]
+                        [--overwrite-existing] [--skip-not-implemented] [--out-name OUTNAME | --glob] [--ignore-rtfde] [--progress]
+                        msg [msg ...]
+
+     extract_msg: Extracts emails and attachments saved in Microsoft Outlook's .msg files. https://github.com/TeamMsgExtractor/msg-extractor
+
+     positional arguments:
+       msg                   An MSG file to be parsed.
+
+     options:
+       -h, --help            show this help message and exit
+       --use-content-id, --cid
+                             Save attachments by their Content ID, if they have one. Useful when working with the HTML body.
+       --json                Changes to write output files as json.
+       --file-logging        Enables file logging. Implies --verbose level 1.
+       -v, --verbose         Turns on console logging. Specify more than once for higher verbosity.
+       --log LOG             Set the path to write the file log to.
+       --config CONFIGPATH   Set the path to load the logging config from.
+       --out OUTPATH         Set the folder to use for the program output. (Default: Current directory)
+       --use-filename        Sets whether the name of each output is based on the msg filename.
+       --dump-stdout         Tells the program to dump the message body (plain text) to stdout. Overrides saving arguments.
+       --html                Sets whether the output should be HTML. If this is not possible, will error.
+       --pdf                 Saves the body as a PDF. If this is not possible, will error.
+       --wk-path WKPATH      Overrides the path for finding wkhtmltopdf.
+       --wk-options [WKOPTIONS ...]
+                             Sets additional options to be used in wkhtmltopdf. Should be a series of options and values, replacing the - or -- in the beginning with + or ++, respectively. For example: --wk-options "+O Landscape"
+       --prepared-html       When used in conjunction with --html, sets whether the HTML output should be prepared for embedded attachments.
+       --charset CHARSET     Character set to use for the prepared HTML in the added tag. (Default: utf-8)
+       --raw                 Sets whether the output should be raw. If this is not possible, will error.
+       --rtf                 Sets whether the output should be RTF. If this is not possible, will error.
+       --allow-fallback      Tells the program to fallback to a different save type if the selected one is not possible.
+       --skip-body-not-found
+                             Skips saving the body if the body cannot be found, rather than throwing an error.
+       --zip ZIP             Path to use for saving to a zip file.
+       --save-header         Store the header in a separate file.
+       --attachments-only    Specify to only save attachments from an msg file.
+       --skip-hidden         Skips any attachment marked as hidden (usually ones embedded in the body).
+       --no-folders          Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with --out-name.
+       --skip-embedded       Skips all embedded MSG files when saving attachments.
+       --extract-embedded    Extracts the embedded MSG files as MSG files instead of running their save functions.
+       --overwrite-existing  Disables filename conflict resolution code for attachments when saving a file, causing files to be overwriten if two attachments with the same filename are on an MSG file.
+       --skip-not-implemented, --skip-ni
+                             Skips any attachments that are not implemented, allowing saving of the rest of the message.
+       --out-name OUTNAME    Name to be used with saving the file output. Cannot be used if you are saving more than one file.
+       --glob, --wildcard    Interpret all paths as having wildcards. Incompatible with --out-name.
+       --ignore-rtfde        Ignores all errors thrown from RTFDE when trying to save. Useful for allowing fallback to continue when an exception happens.
+       --progress            Shows what file the program is currently working on during it's progress.
 
 **To use this in your own script**, start by using:
 
 ::
 
      import extract_msg
 
@@ -246,16 +238,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.5-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.5/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.0-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.42.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.5/extract_msg/__main__.py` & `extract_msg-0.42.0/extract_msg/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __all__ = [
     'main',
 ]
 
+
 import os
 import sys
 import traceback
 import zipfile
 
-from extract_msg import __doc__, utils
-from extract_msg.enums import AttachErrorBehavior
+from extract_msg import __doc__, openMsg, utils
+from extract_msg.enums import ErrorBehavior
 
 
 def main() -> None:
     # Setup logging to stdout, indicate running from cli
     CLI_LOGGING = 'extract_msg_cli'
     args = utils.getCommandArgs(sys.argv[1:])
 
@@ -45,14 +46,15 @@
         'charset': args.charset,
         'contentId': args.cid,
         'customFilename': args.outName,
         'customPath': out,
         'extractEmbedded': args.extractEmbedded,
         'html': args.html,
         'json': args.json,
+        'overwriteExisting': args.overwriteExisting,
         'pdf': args.pdf,
         'preparedHtml': args.preparedHtml,
         'rtf': args.rtf,
         'saveHeader': args.saveHeader,
         'skipBodyNotFound': args.skipBodyNotFound,
         'skipEmbedded': args.skipEmbedded,
         'skipHidden': args.skipHidden,
@@ -60,21 +62,21 @@
         'useMsgFilename': args.useFilename,
         'wkOptions': args.wkOptions,
         'wkPath': args.wkPath,
         'zip': _zip,
     }
 
     openKwargs = {
-        'ignoreRtfDeErrors': args.ignoreRtfDeErrors,
+        'errorBehavior': ErrorBehavior.RTFDE if args.ignoreRtfDeErrors else ErrorBehavior.THROW,
     }
 
     # If we are skipping the NotImplementedError attachments, we need to
     # suppress the error.
     if args.skipNotImplemented:
-        openKwargs['attachmentErrorBehavior'] = AttachErrorBehavior.NOT_IMPLEMENTED
+        openKwargs['errorBehavior'] |= ErrorBehavior.ATTACH_NOT_IMPLEMENTED
 
     def strSanitize(inp):
         """
         Small function to santize parts of a string when failing to print
         them.
         """
         return ''.join((x if x.isascii() else
@@ -87,15 +89,15 @@
             # This may throw an error sometimes and not othertimes.
             # Unclear why, so let's just silence it.
             try:
                 print(f'Saving file "{x}"...')
             except UnicodeEncodeError:
                 print(f'Saving file "{strSanitize(x)}" (failed to print without repr)...')
         try:
-            with utils.openMsg(x, **openKwargs) as msg:
+            with openMsg(x, **openKwargs) as msg:
                 if args.dumpStdout:
                     print(msg.body)
                 elif args.noFolders:
                     msg.saveAttachments(**kwargs)
                 else:
                     msg.save(**kwargs)
         except Exception as e:
```

### Comparing `extract_msg-0.41.5/extract_msg/_rtf/create_doc.py` & `extract_msg-0.42.0/extract_msg/_rtf/create_doc.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/_rtf/inject_rtf.py` & `extract_msg-0.42.0/extract_msg/_rtf/inject_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/_rtf/token.py` & `extract_msg-0.42.0/extract_msg/_rtf/token.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/_rtf/tokenize_rtf.py` & `extract_msg-0.42.0/extract_msg/_rtf/tokenize_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/appointment.py` & `extract_msg-0.42.0/extract_msg/msg_classes/appointment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,99 @@
 __all__ = [
     'AppointmentMeeting',
 ]
 
 
 import datetime
+import functools
 
 from typing import Optional
 
-from . import constants
-from .enums import AppointmentStateFlag, RecurPatternType, ResponseStatus
+from ..constants import HEADER_FORMAT_TYPE, ps
 from .calendar import Calendar
-from .structures.entry_id import EntryID
+from ..enums import AppointmentStateFlag, RecurPatternType, ResponseStatus
+from ..structures.entry_id import EntryID
 
 
 class AppointmentMeeting(Calendar):
     """
     Parser for Microsoft Outlook Appointment or Meeting files.
 
     Both Appointment and Meeting have the same class type but Meeting has
     additional properties. These properties are meaningless on an Appointment
     object.
     """
 
-    @property
+    @functools.cached_property
     def appointmentCounterProposal(self) -> bool:
         """
         Indicates to the organizer that there are counter proposals that have
         not been accepted or rejected by the organizer.
         """
-        return self._ensureSetNamed('_appointmentCounterProposal', '8257', constants.PSETID_APPOINTMENT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('8257', ps.PSETID_APPOINTMENT, bool, False)
 
-    @property
+    @functools.cached_property
     def appointmentLastSequence(self) -> Optional[int]:
         """
         The last sequence number that was sent to any attendee.
         """
-        return self._ensureSetNamed('_appointmentLastSequence', '8203', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8203', ps.PSETID_APPOINTMENT)
 
-    @property
+    @functools.cached_property
     def appointmentProposalNumber(self) -> Optional[int]:
         """
         The number of attendees who have sent counter propostals that have not
         been accepted or rejected by the organizer.
         """
-        return self._ensureSetNamed('_appointmentProposalNumber', '8259', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8259', ps.PSETID_APPOINTMENT)
 
-    @property
+    @functools.cached_property
     def appointmentReplyName(self) -> Optional[datetime.datetime]:
         """
         The user who last replied to the meeting request or meeting update.
         """
-        return self._ensureSetNamed('_appointmentReplyName', '8230', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8230', ps.PSETID_APPOINTMENT)
 
-    @property
+    @functools.cached_property
     def appointmentReplyTime(self) -> Optional[datetime.datetime]:
         """
         The date and time at which the attendee responded to a received Meeting
         Request object of Meeting Update object in UTC.
         """
-        return self._ensureSetNamed('_appointmentReplyTime', '8220', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8220', ps.PSETID_APPOINTMENT)
 
-    @property
+    @functools.cached_property
     def appointmentSequenceTime(self) -> Optional[datetime.datetime]:
         """
         The date and time at which the appointmentSequence property was last
         modified.
         """
-        return self._ensureSetNamed('_appointmentSequenceTime', '8202', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8202', ps.PSETID_APPOINTMENT)
 
-    @property
+    @functools.cached_property
     def autoFillLocation(self) -> bool:
         """
         A value of True indicates that the value of the location property is set
         to the value of the displayName property from the recipientRow structure
         that represents a Resource object.
 
         A value of False indicates that the value of the location property is
         not automatically set.
         """
-        return self._ensureSetNamed('_autoFillLocation', '823A', constants.PSETID_APPOINTMENT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('823A', ps.PSETID_APPOINTMENT, bool, False)
 
-    @property
+    @functools.cached_property
     def fInvited(self) -> bool:
         """
         Whether a Meeting Request object has been sent out.
         """
-        return self._ensureSetNamed('_fInvited', '8229', constants.PSETID_APPOINTMENT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('8229', ps.PSETID_APPOINTMENT, bool, False)
 
     @property
-    def headerFormatProperties(self) -> constants.HEADER_FORMAT_TYPE:
+    def headerFormatProperties(self) -> HEADER_FORMAT_TYPE:
         """
         Returns a dictionary of properties, in order, to be formatted into the
         header. Keys are the names to use in the header while the values are one
         of the following:
         None: Signifies no data was found for the property and it should be
             omitted from the header.
         str: A string to be formatted into the header using the string encoding.
@@ -157,21 +158,21 @@
                 'Resources': self.bcc,
             },
             '-importance-': {
                 'Importance': self.importanceString,
             },
         }
 
-    @property
+    @functools.cached_property
     def isMeeting(self) -> bool:
         """
         Attempts to determine if the object is a Meeting. True if meeting, False
         if appointment.
         """
         return self.appointmentStateFlags and AppointmentStateFlag.MEETING in self.appointmentStateFlags
 
-    @property
+    @functools.cached_property
     def originalStoreEntryID(self) -> Optional[EntryID]:
         """
         The EntryID of the delegator's message store.
         """
-        return self._ensureSetNamed('_originalStoreEntryID', '8237', constants.PSETID_APPOINTMENT, overrideClass = EntryID.autoCreate)
+        return self._getNamedAs('8237', ps.PSETID_APPOINTMENT, EntryID.autoCreate)
```

### Comparing `extract_msg-0.41.5/extract_msg/attachment_base.py` & `extract_msg-0.42.0/extract_msg/properties/named.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,418 +1,417 @@
 from __future__ import annotations
 
 
 __all__ = [
-    'AttachmentBase',
+    'Named',
+    'NamedProperties',
+    'NamedPropertyBase',
+    'NumericalNamedProperty',
+    'StringNamedProperty',
 ]
 
 
-import datetime
+import copy
 import logging
+import pprint
 
-from functools import partial
-from typing import Optional, Tuple, TYPE_CHECKING
+from typing import Any, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
-from .enums import AttachmentType, ErrorBehavior, PropertiesType
-from .exceptions import StandardViolationError
-from .named import NamedProperties
-from .prop import FixedLengthProp
-from .properties import Properties
-from .utils import tryGetMimetype, verifyPropertyId, verifyType
+from .. import constants
+from ..enums import NamedPropertyType
+from ..utils import bytesToGuid, divide, makeWeakRef, properHex
+from compressed_rtf.crc32 import crc32
 
 
 # Allow for nice type checking.
 if TYPE_CHECKING:
-    from .msg import MSGFile
+    from ..msg_classes.msg import MSGFile
+    from ..attachments.attachment_base import AttachmentBase
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
-class AttachmentBase:
+class Named:
     """
-    Stores the attachment data of a Message instance.
-    Should the attachment be an embeded message, the
-    class used to create it will be the same as the
-    Message class used to create the attachment.
+    Class for handling access to the named properties themselves.
     """
 
-    def __init__(self, msg, dir_):
-        """
-        :param msg: the Message instance that the attachment belongs to.
-        :param dir_: the directory inside the msg file where the attachment is located.
-        """
-        self.__msg = msg
-        self.__dir = dir_
-        if not self.exists('__properties_version1.0'):
-            if (msg.errorBehavior & ErrorBehavior.STANDARDS_VIOLATION):
-                logger.error('Attachments MUST have a property stream.')
-            else:
-                raise StandardViolationError('Attachments MUST have a property stream.') from None
-        self.__props = Properties(self._getStream('__properties_version1.0'), PropertiesType.ATTACHMENT)
-        self.__namedProperties = NamedProperties(msg.named, self)
-        self.__treePath = msg.treePath + (self,)
-
-    def _ensureSet(self, variable, streamID, stringStream = True, **kwargs):
-        """
-        Ensures that the variable exists, otherwise will set it using the
-        specified stream. After that, return said variable.
-
-        If the specified stream is not a string stream, make sure to set
-        :param stringStream: to False.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            if stringStream:
-                value = self._getStringStream(streamID)
-            else:
-                value = self._getStream(streamID)
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
-
-    def _ensureSetNamed(self, variable, propertyName : str, guid : str, **kwargs):
-        """
-        Ensures that the variable exists, otherwise will set it using the named
-        property. After that, return said variable.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            value = self.namedProperties.get((propertyName, guid))
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
-
-    def _ensureSetProperty(self, variable, propertyName, **kwargs):
-        """
-        Ensures that the variable exists, otherwise will set it using the
-        property. After that, return said variable.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            try:
-                value = self.props[propertyName].value
-            except (KeyError, AttributeError):
-                value = None
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
-
-    def _ensureSetTyped(self, variable, _id, **kwargs):
-        """
-        Like the other ensure set functions, but designed for when something
-        could be multiple types (where only one will be present). This way you
-        have no need to set the type, it will be handled for you.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            value = self._getTypedData(_id)
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
+    __dir = '__nameid_version1.0'
 
-    def _getStream(self, filename) -> Optional[bytes]:
-        return self.__msg._getStream([self.__dir, filename])
+    def __init__(self, msg : MSGFile):
+        self.__msg = makeWeakRef(msg)
+        # Get the basic streams. If all are emtpy, then nothing to do.
+        guidStream = self._getStream('__substg1.0_00020102') or self._getStream('__substg1.0_00020102', False)
+        entryStream = self._getStream('__substg1.0_00030102') or self._getStream('__substg1.0_00030102', False)
+        self.guidStream = guidStream
+        self.entryStream = entryStream
+        self.namesStream = self._getStream('__substg1.0_00040102') or self._getStream('__substg1.0_00040102', False)
+        # The if else stuff is for protection against None.
+        guidStreamLength = len(guidStream) if guidStream else 0
+        entryStreamLength = len(entryStream) if entryStream else 0
+
+        self.__propertiesDict = {}
+        self.__properties = []
+        self.__guids = tuple()
+        self.__names = {}
+
+        # Check that we even have any entries. If there are none, nothing to do.
+        if entryStream:
+            guids = tuple([None, constants.ps.PS_MAPI, constants.ps.PS_PUBLIC_STRINGS] + [bytesToGuid(x) for x in divide(guidStream, 16)])
+            entries : List[Dict[str, Any]]= []
+            for rawStream in divide(entryStream, 8):
+                tmp = constants.st.STNP_ENT.unpack(rawStream)
+                entry = {
+                    'id': tmp[0],
+                    'pid': tmp[2],
+                    'guid_index': tmp[1] >> 1,
+                    'pkind': NamedPropertyType(tmp[1] & 1), # 0 if numerical, 1 if string.
+                    'rawStream': rawStream,
+                }
+                entry['guid'] = guids[entry['guid_index']]
+                entries.append(entry)
+
+            self.entries = entries
+            self.__guids = guids
+
+            for entry in entries:
+                self.__properties.append(StringNamedProperty(entry, self.__getName(entry['id'])) if entry['pkind'] == NamedPropertyType.STRING_NAMED else NumericalNamedProperty(entry))
+
+            for property in self.__properties:
+                name = property.name if isinstance(property, StringNamedProperty) else property.propertyID
+                self.__propertiesDict[(name, property.guid)] = property
+
+    def __contains__(self, key) -> bool:
+        return key in self.__propertiesDict
+
+    def __getitem__(self, propertyName : Tuple[str, str]):
+        # Validate the key.
+        if not hasattr(propertyName, '__len__') or len(propertyName) != 2:
+            raise TypeError('Named property key must be a tuple of two strings.')
+
+        # Case insensitive search of the dictionary.
+        propertyName = (propertyName[0].upper(), propertyName[1].upper())
+        for key in self.__propertiesDict.keys():
+             if propertyName == (key[0].upper(), key[1].upper()):
+                    return self.__propertiesDict[key]
+
+        raise KeyError(propertyName)
+
+    def __iter__(self):
+        return self.__propertiesDict.__iter__()
+
+    def __len__(self) -> int:
+        return self.__propertiesDict.__len__()
+
+    def __getName(self, offset : int) -> str:
+        """
+        Parses the offset into the named stream and returns the name found.
+        """
+        # We used to parse names by handing it as an array, as specified by the
+        # documentation, but this new method allows for a little bit more wiggle
+        # room in terms of what is accepted by the module.
+        if offset & 3 != 0:
+            # If the offset is not a multiple of 4, that is an error, but we are
+            # reducing it to a warning.
+            logger.warning(f'Malformed named properties detected due to bad offset ({offset}). Ignoring.')
+        # Check that offset is in string stream.
+        if offset > len(self.namesStream):
+            raise ValueError('Failed to parse named property: offset was not in string stream.')
+
+        # Get the length, in bytes, of the string.
+        length = constants.st.STNP_NAM.unpack(self.namesStream[offset:offset + 4])[0]
+        offset += 4
+
+        # Make sure the string can be read entirely. If it can't, something was
+        # corrupt.
+        if offset + length > len(self.namesStream):
+            raise ValueError(f'Failed to parse named property: length ({length}) of string overflows the string stream. This is probably due to a bad offset.')
+
+        return self.namesStream[offset:offset + length].decode('utf-16-le')
+
+    def _getStream(self, filename, prefix = True) -> Optional[bytes]:
+        """
+        Gets a binary representation of the requested filename.
+
+        This should ALWAYS return a bytes object if it was found, otherwise
+        returns None.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
+        """
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Named instance has been garbage collected.')
+        return msg._getStream([self.__dir, filename], prefix = prefix)
 
-    def _getStringStream(self, filename) -> Optional[str]:
+    def _getStringStream(self, filename, prefix = True) -> Optional[str]:
         """
         Gets a string representation of the requested filename.
-        Checks for both ASCII and Unicode representations and returns
-        a value if possible.  If there are both ASCII and Unicode
-        versions, then :param prefer: specifies which will be
-        returned.
-        """
-        return self.__msg._getStringStream([self.__dir, filename])
-
-    def _getTypedData(self, id, _type = None):
-        """
-        Gets the data for the specified id as the type that it is
-        supposed to be. :param id: MUST be a 4 digit hexadecimal
-        string.
-
-        If you know for sure what type the data is before hand,
-        you can specify it as being one of the strings in the
-        constant FIXED_LENGTH_PROPS_STRING or
-        VARIABLE_LENGTH_PROPS_STRING.
-        """
-        verifyPropertyId(id)
-        id = id.upper()
-        found, result = self._getTypedStream('__substg1.0_' + id, _type)
-        if found:
-            return result
-        else:
-            found, result = self._getTypedProperty(id, _type)
-            return result if found else None
 
-    def _getTypedProperty(self, propertyID, _type = None):
-        """
-        Gets the property with the specified id as the type that it
-        is supposed to be. :param id: MUST be a 4 digit hexadecimal
-        string.
-
-        If you know for sure what type the property is before hand,
-        you can specify it as being one of the strings in the
-        constant FIXED_LENGTH_PROPS_STRING or
-        VARIABLE_LENGTH_PROPS_STRING.
-        """
-        verifyPropertyId(propertyID)
-        verifyType(_type)
-        propertyID = propertyID.upper()
-        for x in (propertyID + _type,) if _type is not None else self.props:
-            if x.startswith(propertyID):
-                prop = self.props[x]
-                return True, (prop.value if isinstance(prop, FixedLengthProp) else prop)
-        return False, None
-
-    def _getTypedStream(self, filename, _type = None):
-        """
-        Gets the contents of the specified stream as the type that
-        it is supposed to be.
-
-        Rather than the full filename, you should only feed this
-        function the filename sans the type. So if the full name
-        is "__substg1.0_001A001F", the filename this function
-        should receive should be "__substg1.0_001A".
-
-        If you know for sure what type the stream is before hand,
-        you can specify it as being one of the strings in the
-        constant FIXED_LENGTH_PROPS_STRING or
-        VARIABLE_LENGTH_PROPS_STRING.
-
-        If you have not specified the type, the type this function
-        returns in many cases cannot be predicted. As such, when
-        using this function it is best for you to check the type
-        that it returns. If the function returns None, that means
-        it could not find the stream specified.
-        """
-        return self.__msg._getTypedStream([self.__dir, filename], True, _type)
+        Rather than the full filename, you should only feed this function the
+        filename sans the type. So if the full name is "__substg1.0_001A001F",
+        the filename this function should receive should be "__substg1.0_001A".
+
+        This should ALWAYS return a string if it was found, otherwise returns
+        None.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
+        """
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Named instance has been garbage collected.')
+        return msg._getStringStream([self.__dir, filename], prefix = prefix)
 
     def exists(self, filename) -> bool:
         """
-        Checks if stream exists inside the attachment folder.
+        Checks if stream exists inside the named properties folder.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self.__msg.exists([self.__dir, filename])
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Named instance has been garbage collected.')
+        return msg.exists([self.__dir, filename])
 
     def sExists(self, filename) -> bool:
         """
-        Checks if the string stream exists inside the attachment folder.
-        """
-        return self.__msg.sExists([self.__dir, filename])
+        Checks if the string stream exists inside the named properties folder.
 
-    def existsTypedProperty(self, id, _type = None) -> bool:
-        """
-        Determines if the stream with the provided id exists. The return of this
-        function is 2 values, the first being a boolean for if anything was
-        found, and the second being how many were found.
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self.__msg.existsTypedProperty(id, self.__dir, _type, True, self.__props)
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Named instance has been garbage collected.')
+        return msg.sExists([self.__dir, filename])
 
-    @property
-    def attachmentEncoding(self) -> Optional[bytes]:
+    def get(self, propertyName, default = None):
         """
-        The encoding information about the attachment object. Will return
-        b'*\x86H\x86\xf7\x14\x03\x0b\x01' if encoded in MacBinary format,
-        otherwise it is unset.
+        Tries to get a named property based on its key. Returns :param default:
+        if not found. Key is a tuple of the name and the property set GUID.
         """
-        return self._ensureSet('_attachmentEncoding', '__substg1.0_37020102', False)
+        try:
+            return self[propertyName]
+        except KeyError:
+            return default
 
-    @property
-    def additionalInformation(self) -> Optional[str]:
-        """
-        The additional information about the attachment. This property MUST be
-        an empty string if attachmentEncoding is not set. Otherwise it MUST be
-        set to a string of the format ":CREA:TYPE" where ":CREA" is the
-        four-letter Macintosh file creator code and ":TYPE" is a four-letter
-        Macintosh type code.
-        """
-        return self._ensureSet('_additionalInformation', '__substg1.0_370F')
+    def keys(self):
+        return self.__propertiesDict.keys()
 
-    @property
-    def cid(self) -> Optional[str]:
+    def pprintKeys(self):
         """
-        Returns the Content ID of the attachment, if it exists.
+        Uses the pprint function on a sorted list of keys.
         """
-        return self._ensureSet('_cid', '__substg1.0_3712')
+        pprint.pprint(sorted(self.__propertiesDict.keys()))
 
-    contendId = cid
+    def values(self):
+        return self.__propertiesDict.values()
 
     @property
     def dir(self):
         """
-        Returns the directory inside the msg file where the attachment is
-        located.
+        Returns the directory inside the msg file where the named properties are located.
         """
         return self.__dir
 
     @property
-    def displayName(self) -> Optional[str]:
+    def msg(self) -> MSGFile:
         """
-        Returns the display name of the folder.
+        Returns the Message instance the attachment belongs to.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self._ensureSet('_displayName', '__substg1.0_3001')
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Named instance has been garbage collected.')
+        return msg
 
     @property
-    def exceptionReplaceTime(self) -> Optional[datetime.datetime]:
+    def namedProperties(self) -> Dict:
+        """
+        Returns a copy of the dictionary containing all the named properties.
         """
-        The original date and time at which the instance in the recurrence
-        pattern would have occurred if it were not an exception.
+        return copy.deepcopy(self.__propertiesDict)
+
 
-        Only applicable if the attachment is an Exception object.
+
+class NamedProperties:
+    """
+    An instance that uses a Named instance and an extract-msg class to read the
+    data of named properties.
+    """
+    def __init__(self, named, streamSource : Union[MSGFile, AttachmentBase]):
+        """
+        :param named: The named instance to refer to for named properties
+            entries.
+        :param streamSource: The source to use for acquiring the data of a named
+            property.
         """
-        return self._ensureSetProperty('_exceptionReplaceTime', '7FF90040')
+        self.__named = named
+        self.__streamSource = makeWeakRef(streamSource)
 
-    @property
-    def extension(self) -> Optional[str]:
+    def __getitem__(self, item):
         """
-        The reported extension for the file.
+        Get a named property using the [] operator. Item must be a named
+        property instance or a tuple with 2 items: the name and the GUID string.
+
+        :raises ReferenceError: The associated instance for getting actual
+            property data has been garbage collected.
         """
-        return self._ensureSet('_extension', '__substg1.0_3703')
+        if (source := self.__streamSource()) is None:
+            raise ReferenceError('The stream source for the NamedProperties instance has been garbage collected.')
+        if isinstance(item, NamedPropertyBase):
+            return source._getTypedData(item.propertyStreamID)
+        else:
+            return source._getTypedData(self.__named[item].propertyStreamID)
 
-    @property
-    def hidden(self) -> bool:
+    def get(self, item, default = None):
         """
-        Indicates whether an Attachment object is hidden from the end user.
+        Get a named property, returning the value of :param default: if not
+        found. Item must be a tuple with 2 items: the name and the GUID string.
+
+        :raises ReferenceError: The associated instance for getting actual
+            property data has been garbage collected.
         """
-        return self._ensureSetProperty('_hidden', '7FFE000B', overrideClass = bool, preserveNone = False)
+        try:
+            return self[item]
+        except KeyError:
+            return default
+
+
+
+class NamedPropertyBase:
+    def __init__(self, entry):
+        self.__entry = entry
+        self.__guidIndex = entry['guid_index']
+        self.__namedPropertyID = entry['pid']
+        self.__guid = entry['guid']
+        self.__propertyStreamID = f'{0x8000 + self.__namedPropertyID:04X}'
 
     @property
-    def isAttachmentContactPhoto(self) -> bool:
+    def guid(self) -> str:
         """
-        Whether the attachment is a contact photo for a Contact object.
+        The guid of the property's property set.
         """
-        return self._ensureSetProperty('_isAttachmentContactPhoto', '7FFF000B', overrideClass = bool, preserveNone = False)
+        return self.__guid
 
     @property
-    def longFilename(self) -> Optional[str]:
+    def guidIndex(self) -> int:
         """
-        Returns the long file name of the attachment, if it exists.
+        The guid index of the property's property set.
         """
-        return self._ensureSet('_longFilename', '__substg1.0_3707')
+        return self.__guidIndex
 
     @property
-    def mimetype(self) -> Optional[str]:
+    def namedPropertyID(self) -> int:
         """
-        The content-type mime header of the attachment, if specified.
+        The named property id.
         """
-        return self._ensureSet('_mimetype', '__substg1.0_370E', overrideClass = partial(tryGetMimetype, self), preserveNone = False)
+        return self.__namedPropertyID
 
     @property
-    def msg(self) -> MSGFile:
+    def propertyStreamID(self) -> str:
         """
-        Returns the Message instance the attachment belongs to.
+        An ID usable for grabbing the value stream.
         """
-        return self.__msg
+        return self.__propertyStreamID
+
+    @property
+    def rawEntry(self) -> dict:
+        return copy.deepcopy(self.__entry)
 
     @property
-    def name(self) -> Optional[str]:
+    def rawEntryStream(self) -> bytes:
         """
-        The best name available for the file. Uses long filename before short.
+        The raw data used for the entry.
         """
-        if self.type is AttachmentType.MSG:
-            if self.displayName:
-                return self.displayName + '.msg'
-        return self.longFilename or self.shortFilename
+        return self.__entry['rawStream']
 
     @property
-    def namedProperties(self) -> NamedProperties:
+    def type(self) -> NamedPropertyType:
         """
-        The NamedAttachmentProperties instance for this attachment.
+        The type of named property.
         """
-        return self.__namedProperties
+        raise NotImplementedError('NamedPropertyBase cannot be used directly. Subclass it before using it.')
+
+
+
+class StringNamedProperty(NamedPropertyBase):
+    def __init__(self, entry, name):
+        super().__init__(entry)
+        self.__name = name
+
+        # Finally got this to be correct after asking about it on a Microsoft
+        # forum. Apparently it uses the same CRC-32 as the Compressed RTF
+        # standard does, so we can just use the function defined in the
+        # compressed-rtf Python module.
+        #
+        # First thing to note is that the name should only ever be lowered if it
+        # is part of the PS_INTERNET_HEADERS property set **AND** it is
+        # generated by certain versions of Outlook. As such, a little bit of
+        # additional code will need to run to determine exactly what the stream
+        # ID should be if it is in that property set.
+        if self.guid == constants.ps.PS_INTERNET_HEADERS:
+            # To be sure if it needs to be lower the most effective method would
+            # be to just get the Stream ID and then check if the entry is in
+            # there. If it isn't, then check the regular case and see. If it is
+            # not in either... well, we don't use it for anything so it will
+            # just be a warning, and the Stream ID will be set to 0.
+            #
+            # TODO: Unfortunately, doing this will need to be put off until a
+            # different version, preferably after Python 2 support is removed,
+            # as this will require restructuring a lot of internal code. For now
+            # we just assume that it is lowercase.
+            self.__streamID = 0x1000 + (crc32(name.lower().encode('utf-16-le')) ^ (self.guidIndex << 1 | 1)) % 0x1F
+
+        else:
+            # No special logic here to determine what to do.
+            self.__streamID = 0x1000 + (crc32(name.encode('utf-16-le')) ^ (self.guidIndex << 1 | 1)) % 0x1F
 
     @property
-    def payloadClass(self) -> Optional[str]:
+    def name(self) -> str:
         """
-        The class name of an object that can display the contents of the
-        message.
+        The name of the property.
         """
-        return self._ensureSet('_payloadClass', '__substg1.0_371A')
+        return self.__name
 
     @property
-    def props(self) -> Properties:
+    def streamID(self) -> int:
         """
-        Returns the Properties instance of the attachment.
+        Returns the streamID of the named property. This may not be accurate.
         """
-        return self.__props
+        return self.__streamID
 
     @property
-    def renderingPosition(self) -> Optional[int]:
+    def type(self) -> NamedPropertyType:
         """
-        The offset, in redered characters, to use when rendering the attachment
-        within the main message text. A value of 0xFFFFFFFF indicates a hidden
-        attachment that is not to be rendered.
+        Returns the type of the named property. This will either be NUMERICAL_NAMED or STRING_NAMED.
         """
-        return self._ensureSetProperty('_renderingPosition', '370B0003')
+        return NamedPropertyType.STRING_NAMED
+
+
+
+class NumericalNamedProperty(NamedPropertyBase):
+    def __init__(self, entry):
+        super().__init__(entry)
+        self.__propertyID = properHex(entry['id'], 4).upper()
+        self.__streamID = 0x1000 + (entry['id'] ^ (self.guidIndex << 1)) % 0x1F
 
     @property
-    def shortFilename(self) -> Optional[str]:
+    def propertyID(self) -> str:
         """
-        Returns the short file name of the attachment, if it exists.
+        The actualy property id of the named property.
         """
-        return self._ensureSet('_shortFilename', '__substg1.0_3704')
+        return self.__propertyID
 
     @property
-    def treePath(self) -> Tuple:
+    def streamID(self) -> int:
         """
-        A path, as a tuple of instances, needed to get to this instance through
-        the MSGFile-Attachment tree.
+        Returns the streamID of the named property. This may not be accurate
         """
-        return self.__treePath
+        return self.__streamID
 
     @property
-    def type(self) -> AttachmentType:
+    def type(self) -> NamedPropertyType:
         """
-        Returns the (internally used) type of the data.
+        Returns the type of the named property. This will either be NUMERICAL_NAMED or STRING_NAMED.
         """
-        return AttachmentType.UNKNOWN
+        return NamedPropertyType.NUMERICAL_NAMED
```

### Comparing `extract_msg-0.41.5/extract_msg/enums.py` & `extract_msg-0.42.0/extract_msg/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,83 @@
 __all__ = [
-    'AddressBookType', 'AppointmentAuxilaryFlag', 'AppointmentColor',
-    'AppointmentStateFlag', 'AttachErrorBehavior', 'AttachmentType',
-    'BCImageAlignment', 'BCImageSource', 'BCLabelFormat', 'BCTemplateID',
-    'BCTextFormat', 'BodyTypes', 'BusyStatus', 'ClientIntentFlag', 'Color',
-    'ContactAddressIndex', 'ContactLinkState', 'DeencapType',
-    'DirectoryEntryType', 'DisplayType', 'ElectronicAddressProperties',
-    'EntryIDType', 'EntryIDTypeHex', 'ErrorCode', 'ErrorCodeType', 'Gender',
-    'IconIndex', 'Importance', 'Intelligence', 'MacintoshEncoding',
-    'MeetingObjectChange', 'MeetingRecipientType', 'MeetingType',
-    'MessageFormat', 'MessageType', 'NamedPropertyType', 'OORBodyFormat',
-    'PostalAddressID', 'Priority', 'PropertiesType', 'RecipientRowFlagType',
-    'RecipientType', 'RecurCalendarType', 'RecurDOW', 'RecurEndType',
-    'RecurFrequency', 'RecurMonthNthWeek', 'RecurPatternTypeSpecificWeekday',
-    'RecurPatternType', 'ResponseStatus', 'ResponseType', 'RuleActionType',
-    'Sensitivity', 'ServerProcessingAction', 'SideEffect', 'TaskAcceptance',
-    'TaskHistory', 'TaskMode', 'TaskMultipleRecipients', 'TaskOwnership',
-    'TaskRequestType', 'TaskState', 'TaskStatus', 'TZFlag',
+    'AddressBookType',
+    'AppointmentAuxilaryFlag',
+    'AppointmentColor',
+    'AppointmentStateFlag',
+    'AttachmentPermissionType',
+    'AttachmentType',
+    'BCImageAlignment',
+    'BCImageSource',
+    'BCLabelFormat',
+    'BCTemplateID',
+    'BCTextFormat',
+    'BodyTypes',
+    'BusyStatus',
+    'ClientIntentFlag',
+    'Color',
+    'ContactAddressIndex',
+    'ContactLinkState',
+    'DeencapType',
+    'DirectoryEntryType',
+    'DisplayType',
+    'DVAspect',
+    'ElectronicAddressProperties',
+    'EntryIDType',
+    'EntryIDTypeHex',
+    'ErrorBehavior',
+    'ErrorCode',
+    'ErrorCodeType',
+    'Gender',
+    'IconIndex',
+    'Importance',
+    'InsecureFeatures',
+    'Intelligence',
+    'MacintoshEncoding',
+    'MeetingObjectChange',
+    'MeetingRecipientType',
+    'MeetingType',
+    'MessageFormat',
+    'MessageType',
+    'NamedPropertyType',
+    'NoteColor',
+    'OORBodyFormat',
+    'PostalAddressID',
+    'Priority',
+    'PropertiesType',
+    'RecipientRowFlagType',
+    'RecipientType',
+    'RecurCalendarType',
+    'RecurDOW',
+    'RecurEndType',
+    'RecurFrequency',
+    'RecurMonthNthWeek',
+    'RecurPatternTypeSpecificWeekday',
+    'RecurPatternType',
+    'ResponseStatus',
+    'ResponseType',
+    'RuleActionType',
+    'SaveType',
+    'Sensitivity',
+    'ServerProcessingAction',
+    'SideEffect',
+    'TaskAcceptance',
+    'TaskHistory',
+    'TaskMode',
+    'TaskMultipleRecipients',
+    'TaskOwnership',
+    'TaskRequestType',
+    'TaskState',
+    'TaskStatus',
+    'TZFlag',
 ]
 
 
 import enum
 
-from typing import Set, Union
+from typing import Union
 
 
 class AddressBookType(enum.Enum):
     """
     The type of object that an address book entry ID represents. MUST be one of
     these or it is invalid.
     """
@@ -39,40 +91,25 @@
     CONTAINER = 0x100
     TEMPLATE = 0x101
     ONE_OFF_USER = 0x102
     SEARCH = 0x200
 
 
 
-class AppointmentAuxilaryFlag(enum.Enum):
+class AppointmentAuxilaryFlag(enum.IntFlag):
     """
     Describes the auxilary state of the object.
 
     COPIED: The Calendar object was copied from another Calendar folder.
     FORCE_MEETING_RESPONSE: The client of server can require that a Meeting
         Response object be sent to the organizer when a response is chosen.
     FORWARDED: The object was forwarded by the organizer or another recipient.
     REPAIR_UPDATE_MESSAGE: The meeting request is a Repair Update Message sent
         from a server-side calendar repair system.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['AppointmentAuxilaryFlag']:
-        """
-        Takes an int and returns a set of the flags.
-        """
-        flags = set()
-        for x in range(7):
-            bit = value & (1 << x)
-            if bit:
-                if x in (3, 4, 6):
-                    raise ValueError('Reserved bit was set.')
-                flags.add(cls(bit))
-
-        return flags
-
     COPIED = 0b1
     FORCE_MEETING_RESPONSE = 0b10
     FORWARDED = 0b100
     REPAIR_UPDATE_MESSAGE = 0b100000
 
 
 
@@ -87,33 +124,36 @@
     OLIVE = 0x00000007
     PURPLE = 0x00000008
     TEAL = 0x00000009
     YELLOW = 0x0000000A
 
 
 
-class AppointmentStateFlag(enum.Enum):
+class AppointmentStateFlag(enum.IntFlag):
     """
     MEETING: The object is a Meeting object or meeting-related object.
     RECEIVED: The represented object was received from someone else.
     CANCELED: The Meeting object that is represented has been canceled.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['AppointmentStateFlag']:
-        """
-        Takes an int and returns a set of the flags.
-        """
-        return {cls(1 << x) for x in range(3) if (value & (1 << x)) != 0}
-
     MEETING = 0b1
     RECEIVED = 0b10
     CANCELED = 0b100
 
 
 
+class AttachmentPermissionType(enum.Enum):
+    """
+    The permission type data associated with a web reference attachment.
+    """
+    NONE = 0
+    VIEW = 1
+    EDIT = 2
+
+
+
 class AttachmentType(enum.Enum):
     """
     The type represented by the attachment.
 
     DATA: An attachment stored as plain bytes in the MSG file.
     MSG: A normally embedded MSG file.
     WEB: An attachment referencing a resource on the web.
@@ -127,14 +167,15 @@
     DATA = 0
     MSG = 1
     WEB = 2
     SIGNED = 3
     BROKEN = 4
     UNSUPPORTED = 5
     SIGNED_EMBEDDED = 6
+    CUSTOM = 7
 
     UNKNOWN = 0xFFFFFFFF
 
 
 
 class BCImageAlignment(enum.Enum):
     STRETCH = 0x00
@@ -267,19 +308,18 @@
 class BodyTypes(enum.IntFlag):
     """
     Enum representing the types of bodies found in a message. This does not
     include bodies generated from other sources, and so is a good detection
     method for generated bodies (if you check a body and it is not null, but it
     is not listed in the enum, then it was generated from another body).
 
-    This is an IntFlag enum, so to check if a body was found use the & operator
-    with the body you are checking and ensuring the result isn't BodyTypes.None.
-    You can also convert the result to a bool. For example:
+    This is an IntFlag enum, so to check if a body was found use the in operator
+    with the body you are checking. For example:
 
-    >>> rtfFound = bool(msg.detectedBodies & BodyTypes.RTF)
+    >>> rtfFound = BodyTypes.RTF msg.detectedBodies
     """
     NONE = 0b000
     PLAIN = 0b001
     RTF = 0b010
     HTML = 0b100
     ALL = 0b111
 
@@ -300,15 +340,15 @@
     OL_TENTATIVE = 0x00000001
     OL_BUSY = 0x00000002
     OL_OUT_OF_OFFICE = 0x00000003
     OL_WORKING_ELSEWHERE = 0x00000004
 
 
 
-class ClientIntentFlag(enum.Enum):
+class ClientIntentFlag(enum.IntFlag):
     """
     An action a user has taken on a Meeting object.
 
     MANAGER: The user is the owner of the Meeting object's Calendar folder. If
         set, DELEGATE SHOULD NOT be set.
     DELEGATE: The user is a delegate acting on a Meeting object in a delegator's
         Calendar folder. If set, MANAGER SHOULD NOT be set.
@@ -323,21 +363,14 @@
     MODIFIED_END_TIME: The user modified the end time.
     MODIFIED_LOCATION: The user changed the location of the meeting.
     RESPONDED_EXCEPTION_DECLINE: The user declined an exception to a recurring
         series.
     CANCELED: The user canceled a meeting request.
     EXCEPTION_CANCELED: The user canceled an exception to a recurring series.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['ClientIntentFlag']:
-        """
-        Takes an int and returns a set of the flags.
-        """
-        return {cls(1 << x) for x in range(13) if (value & (1 << x))}
-
     MANAGER = 0b1
     DELEGATE = 0b10
     DELETED_WITH_NO_RESPONSE = 0b100
     DELETED_EXCEPTION_WITH_NO_RESPONSE = 0b1000
     RESPONDED_TENTATIVE = 0b10000
     RESPONSED_ACCEPT = 0b100000
     RESPONDED_DECLINE = 0b1000000
@@ -351,14 +384,15 @@
 
 
 class Color(enum.IntEnum):
     RED = 0
     BLACK = 1
 
 
+
 class ContactAddressIndex(enum.Enum):
     EMAIL_1 = 0
     EMAIL_2 = 1
     EMAIL_3 = 2
     FAX_1 = 3
     FAX_2 = 4
     FAX_3 = 5
@@ -411,29 +445,25 @@
     CONTAINER = 0x0100
     TEMPLATE = 0x0101
     ADDRESS_TEMPLATE = 0x0102
     SEARCH = 0x0200
 
 
 
-class ElectronicAddressProperties(enum.Enum):
-    @classmethod
-    def fromBits(cls, value : int) -> Set['ElectronicAddressProperties']:
-        """
-        Converts an int, with the left most bit referring to 0x00000000, to a
-        set of this enum.
+class DVAspect(enum.IntEnum):
+    """
+    Part of the extra data for Outlook signatures. Different sources seem to
+    disagree on the meanings, so I'm sticking to the meanings in the official
+    Microsoft documentation of the DVASPECT enumeration.
+    """
+    CONTENT = 1
+    ICON = 4
 
-        :raises ValueError: The value was less than 0.
-        """
-        if value < 0:
-            raise ValueError('Value must not be negative.')
-        # This is a quick compressed way to convert the bits in the int into
-        # a tuple of instances of this class should any bit be a 1.
-        return {cls(int(index)) for index, val in enumerate(bin(value)[:1:-1]) if val == '1'}
 
+class ElectronicAddressProperties(enum.Enum):
     EMAIL_1 = 0x00000000
     EMAIL_2 = 0x00000001
     EMAIL_3 = 0x00000002
     BUSINESS_FAX = 0x00000003
     HOME_FAX = 0x00000004
     PRIMARY_FAX = 0x00000005
 
@@ -485,30 +515,45 @@
     WRAPPED = 'C091ADD3519DCF11A4A900AA0047FAA4'
 
 
 
 class ErrorBehavior(enum.IntFlag):
     """
     The behavior to follow when handling an error in an MSG file and it's
-    attachments. This is an int flag enum, so the options you want will be ORed
-    with each other.
+    attachments. Specifying an option indicates the behavior for the situation
+    is to log a message, if anything, instead of raising an exception. This is
+    an int flag enum, so the options you want will be ORed with each other.
 
     THROW: Throw the exception regardless of type.
     ATTACH_NOT_IMPLEMENTED: Silence the exception for NotImplementedError.
     ATTACH_BROKEN: Silence the exception for broken attachments.
-    ATTACH_SUPPRESS_ALL: Silence the exception for NotImplementedError and for broken
-        attachments.
-    STANDARDS_VIOLATION
-    """
-    THROW = 0b000
-    ATTACH_NOT_IMPLEMENTED = 0b001
-    ATTACH_BROKEN = 0b010
-    ATTACH_SUPPRESS_ALL = 0b011
-    STANDARDS_VIOLATION = 0b100
-    SUPPRESS_ALL = 0b111
+    ATTACH_SUPPRESS_ALL: Silence the exception for NotImplementedError and for
+        broken attachments.
+    RTFDE_MALFORMED: Silences errors about malformed RTF data.
+    RTFDE_UNKNOWN_ERROR: Silences errors from RTFDE that are not normal.
+    RTFDE: Silences all errors from RTFDE.
+    STANDARDS_VIOLATION: Silences StandardViolationError where acceptable.
+    OLE_DEFECT_INCORRECT: Silences defects of type DEFECT_INCORRECT that are
+        enabled by default. This can lead to strange bugs.
+    SUPPRESS_ALL: Silences all of the above.
+    """
+    THROW = 0b000000
+    # Attachments.
+    ATTACH_NOT_IMPLEMENTED = 0b000001
+    ATTACH_BROKEN = 0b000010
+    ATTACH_SUPPRESS_ALL = 0b000011
+    # RTFDE.
+    RTFDE_MALFORMED = 0b000100
+    RTFDE_UNKNOWN_ERROR = 0b001000
+    RTFDE = 0b001100
+    # General.
+    STANDARDS_VIOLATION = 0b010000
+    OLE_DEFECT_INCORRECT = 0b100000
+
+    SUPPRESS_ALL = 0b111111
 
 
 
 class ErrorCode(enum.Enum):
     SUCCESS = 0x00000000
     GENERAL_FAILURE = 0x80004005
     OUT_OF_MEMORY = 0x8007000E
@@ -1146,14 +1191,37 @@
 class Importance(enum.Enum):
     LOW = 0
     MEDIUM = 1
     HIGH = 2
 
 
 
+class InsecureFeatures(enum.IntFlag):
+    """
+    Insecure options that can be enabled for an MSG file.
+
+    Using ALL is not recommended unless you check this list before updating to
+    a new version of the module, as new features may have been added. It is
+    also not recommended to use these on files you do not trust.
+
+    The following features are avilable:
+    NONE: No insecure features are allowed (default).
+    PIL_IMAGE_PARSING: Various operations requiring PIL or Pillow that will read
+        image data from parts of the MSG file. These operations are usually
+        constructing new images or are converting from one format to another.
+        This may expose you to security issues from those libraries.
+
+    ALL: All of the previously listed features will be enabled for the MSG file.
+    """
+    NONE = 0b0000
+    PIL_IMAGE_PARSING = 0b0001
+    ALL = 0b1111
+
+
+
 class Intelligence(enum.Enum):
     ERROR = -1
     DUMB = 0
     SMART = 1
 
 
 
@@ -1164,46 +1232,29 @@
     BIN_HEX = 0
     UUENCODE = 1
     APPLE_SINGLE = 2
     APPLE_DOUBLE = 3
 
 
 
-class MeetingObjectChange(enum.Enum):
+class MeetingObjectChange(enum.IntFlag):
     """
     Indicates a property that has changed on a meeting object.
 
     START: The start has changed.
     END: The end has changed.
     RECUR: The recurrence pattern has changed.
     LOCATION: The location has changed.
     SUBJECT: The subject has changed.
     REQUIRED_ATTENDEE: One or more required attendees were added.
     OPTIONAL_ATTENDEE: One or more optional attendees were added.
     BODY: The body was modified.
     RESPONSE: The responseRequested or replyRequested property has changed.
     ALLOW_PROPOSE: The appointmentNotAllowPropose property has changed.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['MeetingObjectChange']:
-        """
-        Takes an int and returns a set of the changes.
-        """
-        changes = set()
-        for x in range(32):
-            if x in (8, 11) or (12 < x < 31):
-                continue
-            bit = value & (1 << x)
-            if bit:
-                if x in (12, 31):
-                    raise ValueError('Reserved bit was set.')
-                changes.add(cls(bit))
-
-        return changes
-
     START = 0b1
     END = 0b10
     RECUR = 0b100
     LOCATION = 0b1000
     SUBJECT = 0b10000
     REQUIRED_ATTENDEE = 0b100000
     OPTIONAL_ATTENDEE = 0b1000000
@@ -1266,14 +1317,23 @@
 
 class NamedPropertyType(enum.Enum):
     NUMERICAL_NAMED = 0
     STRING_NAMED = 1
 
 
 
+class NoteColor(enum.Enum):
+    BLUE = 0
+    GREEN = 1
+    PINK = 2
+    YELLOW = 3
+    WHITE = 4
+
+
+
 class OORBodyFormat(enum.Enum):
     """
     The body format for One Off Recipients.
     """
     TEXT_ONLY = 0b0011
     HTML_ONLY = 0b0111
     TEXT_AND_HTML = 0b1011
@@ -1398,25 +1458,18 @@
     SECOND = 0x00000002
     THIRD = 0x00000003
     FOURTH = 0x00000004
     LAST = 0x00000005
 
 
 
-class RecurPatternTypeSpecificWeekday(enum.Enum):
+class RecurPatternTypeSpecificWeekday(enum.IntFlag):
     """
     See [MS-OXOCAL] for details.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['RecurPatternTypeSpecificWeekday']:
-        """
-        Takes an int and returns a set of the weekdays.
-        """
-        return {cls(1 << x) for x in range(1, 8) if (value & (1 << x))}
-
     SATURDAY = 0b10
     FRIDAY = 0b100
     THURSDAY = 0b1000
     WEDNESDAY = 0b10000
     TUESDAY = 0b100000
     MONDAY = 0b1000000
     SUNDAY = 0b10000000
@@ -1479,44 +1532,62 @@
     OP_DELEGATE = 0x08
     OP_TAG = 0x09
     OP_DELETE = 0x0A
     OP_MARK_AS_READ = 0x0B
 
 
 
+class SaveType(enum.Enum):
+    """
+    Specifies the way that a function saved the data. Used to determine how the
+    return value from a save function should be read.
+
+    CUSTOM: An unlisted save method was used, and the second value is
+        unspecified.
+    NONE: No data was saved, and the second tuple value should be None.
+    FILE: A single file was save, and the location is the second value.
+    FILES: Multiple files were created, and the second value is a list of the
+        locations.
+    FOLDER: A folder was created to store data, and the location is the second
+        value.
+    FOLDERS: Multiple folders were created to store data, and the second value
+        is a list of the locations.
+    """
+    CUSTOM = -1
+    NONE = 0
+    FILE = 1
+    FILES = 2
+    FOLDER = 3
+    FOLDERS = 4
+
+
+
 class Sensitivity(enum.Enum):
     NORMAL = 0
     PERSONAL = 1
     PRIVATE = 2
     CONFIDENTIAL = 3
 
 
 
-class ServerProcessingAction(enum.Enum):
+class ServerProcessingAction(enum.IntFlag):
     """
     Actions taken on a meeting-related object.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['ServerProcessingAction']:
-        """
-        Takes an int and returns a set of the weekdays.
-        """
-        return {cls(1 << x) for x in range(16) if (value & (1 << x))}
-
     DELEGATOR_WANTS_COPY = 0x00000002
     CREATED_ON_PRINCIPLE = 0x00000010
     UPDATED_CAL_ITEM = 0x00000080
     COPIED_OLD_PROPERTIES = 0x00000100
     SEND_AUTO_RESPONSE = 0x00000400
     REVIVED_EXCEPTION = 0x00000800
     PROCESSED_MEETING_FORWARD_NOTIFICATION = 0x00001000
 
 
 
-class SideEffect(enum.Enum):
+class SideEffect(enum.IntFlag):
     """
     A flag for how a Message object is handled by the client in relation to
     certain user interface actions.
 
     OPEN_TO_DELETE: The client opens the Message object when deleting.
     NO_FRAME: No UI is associated with the Message object.
     COERCE_TO_INDEX: The client moves the Message object to the Inbox folder
@@ -1534,21 +1605,14 @@
         unless the OPEN_TO_COPY flag is set.
     CANNOT_UNDO_MOVE: The client cannot undo a move operation. Must not be set
         unless the OPEN_TO_MOVE flag is set.
     HAS_SCRIPT: The Message object contains end-user script.
     OPEN_TO_PERM_DELETE: The client opens the Message object to permanently
         delete it.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['SideEffect']:
-        """
-        Takes an int and returns a set of the side effects.
-        """
-        return {cls(1 << x) for x in range(15) if (value & (1 << x))}
-
     OPEN_TO_DELETE = 0b1
     NO_FRAME = 0b1000
     COERCE_TO_INDEX = 0b10000
     OPEN_TO_COPY = 0b100000
     OPEN_TO_MOVE = 0b1000000
     OPEN_FOR_CTX_MENU = 0b100000000
     CANNOT_UNDO_DELETE = 0b10000000000
@@ -1600,22 +1664,15 @@
     ACCEPTED = 2
     REJECTED = 3
     EMBEDDED_UPDATE = 4
     SELF_ASSIGNED = 5
 
 
 
-class TaskMultipleRecipients(enum.Enum):
-    @classmethod
-    def fromBits(cls, value : int) -> Set['TaskMultipleRecipients']:
-        """
-        Takes an int and returns a set of the flags.
-        """
-        return {cls(1 << x) for x in range(2) if (value & (1 << x))}
-
+class TaskMultipleRecipients(enum.IntFlag):
     SENT = 0x00000001
     RECEIVED = 0x00000002
 
 
 
 class TaskOwnership(enum.Enum):
     """
@@ -1698,28 +1755,21 @@
     IN_PROGRESS = 0x00000001
     COMPLETE = 0x00000002
     WAITING_ON_OTHER = 0x00000003
     DEFERRED = 0x00000004
 
 
 
-class TZFlag(enum.Enum):
+class TZFlag(enum.IntFlag):
     """
     Flags for a TZRule object as defined in [MS-OXOCAL].
 
     RECUR_CURRENT_TZREG: The rule is associated with a recurring series.
     EFFECTIVE_TZREG: The rule is the effective rule.
     """
-    @classmethod
-    def fromBits(cls, value : int) -> Set['TZFlag']:
-        """
-        Takes an int and returns a set of the flags.
-        """
-        return {cls(1 << x) for x in range(2) if (value & (1 << x))}
-
     RECUR_CURRENT_TZREG = 0b1
     EFFECTIVE_TZREG = 0b10
 
 
 
 class _EnumDeprecator:
     """
@@ -1760,15 +1810,15 @@
         warnings.warn(self.__warnMessage, DeprecationWarning)
 
         return self.__new.__getitem__(self.__nameConv.get(name, name))
 
 
 
 
-# Deprecated Enums
+# Deprecated Enums. These are not exported but may be directly accessed.
 AttachErrorBehavior = _EnumDeprecator(
     'AttachErrorBehavior',
     ErrorBehavior,
     {
         'BROKEN': 'ATTACH_SUPPRESS_ALL',
         'NOT_IMPLEMENTED': 'ATTACH_NOT_IMPLEMENTED',
     },
```

### Comparing `extract_msg-0.41.5/extract_msg/exceptions.py` & `extract_msg-0.42.0/extract_msg/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 extract_msg.exceptions
 ~~~~~~~~~~~~~~~~~~~
 This module contains the set of extract_msg exceptions.
 """
 
 __all__ = [
-    'BadHtmlError',
+    'ExMsgBaseException',
+
     'ConversionError',
     'DataNotFoundError',
     'DeencapMalformedData',
     'DeencapNotEncapsulated',
     'ExecutableNotFound',
     'IncompatibleOptionsError',
     'InvalidFileFormatError',
@@ -23,116 +24,127 @@
     'UnsupportedEncodingError',
     'UnknownTypeError',
     'UnsupportedMSGTypeError',
     'UnrecognizedMSGTypeError',
     'WKError',
 ]
 
+# Base exception types.
 
-import logging
-
-
-# Add logger bus.
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
-
+class ExMsgBaseException(Exception):
+    """
+    The base class for all custom exceptions the module uses.
+    """
 
-class BadHtmlError(ValueError):
+# I would want this to also be a subclass of NotImplementedError, but Python
+# docs say that CPython can make that a bit problematic due to things from the C
+# side of the code.
+class FeatureNotImplemented(ExMsgBaseException):
     """
-    HTML failed to pass validation.
+    The base class for a feature not yet being implemented in the module.
     """
 
-class ConversionError(Exception):
+# More specific exceptions.
+
+
+class ConversionError(ExMsgBaseException):
     """
     An error occured during type conversion.
     """
 
-class DataNotFoundError(Exception):
+class DataNotFoundError(ExMsgBaseException):
     """
     Requested stream type was unavailable.
     """
 
-class DeencapMalformedData(Exception):
+class DeencapMalformedData(ExMsgBaseException):
     """
     Data to deencapsulate was malformed in some way.
     """
 
-class DeencapNotEncapsulated(Exception):
+class DeencapNotEncapsulated(ExMsgBaseException):
     """
     Data to deencapsulate did not contain any encapsulated data.
     """
 
-class ExecutableNotFound(Exception):
+class ExecutableNotFound(ExMsgBaseException):
     """
     Could not find the specified executable.
     """
 
-class IncompatibleOptionsError(Exception):
+class IncompatibleOptionsError(ExMsgBaseException):
     """
     Provided options are incompatible with each other.
     """
 
-class InvalidFileFormatError(OSError):
+class InvalidFileFormatError(ExMsgBaseException):
     """
     An Invalid File Format Error occurred.
     """
 
-class InvaildPropertyIdError(Exception):
+class InvaildPropertyIdError(ExMsgBaseException):
     """
     The provided property ID was invalid.
     """
 
-class InvalidVersionError(Exception):
+class PrefixError(ExMsgBaseException):
+    """
+    An issue was detected with the provided prefix. This should never occur if
+    you have no manually provided a prefix.
+    """
+
+class SecurityError(ExMsgBaseException):
     """
-    The version specified is invalid.
+    A code path was triggered that would use an insecure feature, but that
+    insecure feature was not enabled.
     """
 
 class StandardViolationError(InvalidFileFormatError):
     """
     A critical violation of the MSG standards was detected and could not be
     recovered from. Recoverable violations will result in log messages instead.
 
-    Any that could reasonably be skipped, although are likely to still cause 
+    Any that could reasonably be skipped, although are likely to still cause
     errors down the line, can be suppressed.
     """
 
-class TZError(Exception):
+class TZError(ExMsgBaseException):
     """
     Specifically not an OSError to avoid being caught by parts of the module.
     This error represents a fatal error in the datetime parsing as it usually
     means your installation of tzlocal or tzdata are broken. If you have
     received this error after using PyInstaller, you must include the resource
     files for tzdata for it to work properly. See TeamMsgExtractor#272 and
     TeamMsgExtractor#169 for information on why you are getting this error.
     """
 
-class UnknownCodepageError(Exception):
+class UnknownCodepageError(ExMsgBaseException):
     """
     The codepage provided was not one we know of.
     """
 
-class UnsupportedEncodingError(NotImplementedError):
+class UnsupportedEncodingError(FeatureNotImplemented):
     """
     The codepage provided is known but is not supported.
     """
 
-class UnknownTypeError(Exception):
+class UnknownTypeError(ExMsgBaseException):
     """
     The type specified is not one that is recognized.
     """
 
-class UnsupportedMSGTypeError(NotImplementedError):
+class UnsupportedMSGTypeError(FeatureNotImplemented):
     """
     An exception that is raised when an MSG class is recognized by not
     supported.
     """
 
-class UnrecognizedMSGTypeError(TypeError):
+class UnrecognizedMSGTypeError(ExMsgBaseException):
     """
     An exception that is raised when the module cannot determine how to properly
     open a specific class of msg file.
     """
 
-class WKError(RuntimeError):
+class WKError(ExMsgBaseException):
     """
     An error occured while running wkhtmltopdf.
     """
```

### Comparing `extract_msg-0.41.5/extract_msg/logging-config/logging-nt.json` & `extract_msg-0.42.0/extract_msg/data/logging-config/logging-nt.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/logging-config/logging-posix.json` & `extract_msg-0.42.0/extract_msg/data/logging-config/logging-posix.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/meeting_cancellation.py` & `extract_msg-0.42.0/extract_msg/msg_classes/meeting_cancellation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = [
     'MeetingCancellation',
 ]
 
 
-from . import constants
-from .enums import RecurPatternType, ResponseStatus
+from .. import constants
+from ..enums import RecurPatternType, ResponseStatus
 from .meeting_related import MeetingRelated
 
 
 # The documentation for this only specifies restrictions on existing properties,
 # so we just mostly leave this alone.
 class MeetingCancellation(MeetingRelated):
     """
```

### Comparing `extract_msg-0.41.5/extract_msg/meeting_exception.py` & `extract_msg-0.42.0/extract_msg/msg_classes/meeting_exception.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 __all__ = [
     'MeetingException',
 ]
 
 
 import datetime
+import functools
 
 from typing import Optional
 
-from . import constants
+from .. import constants
+from ..enums import SaveType
 from .meeting_related import MeetingRelated
 
 
 class MeetingException(MeetingRelated):
     """
     Class for handling Meeting Exceptions.
     """
 
-    def save(self, *args, **kwargs):
+    def save(self, **_) -> constants.SAVE_TYPE:
         """
         Meeting Exceptions are hidden attachments with no save behaviors. As
         such, for saving we literally just return the object and do nothing
         else.
 
         If you want something to happen for saving, you can call the save of a
         parent class or write your own code.
         """
-        return self
+        return (SaveType.NONE, None)
 
-    @property
+    @functools.cached_property
     def exceptionReplaceTime(self) -> Optional[datetime.datetime]:
         """
         The date and time within the recurrence pattern that the exception will
         replace. The value is specified in UTC.
         """
-        return self._ensureSetNamed('_exceptionReplaceTime', '8228', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8228', constants.ps.PSETID_APPOINTMENT)
 
-    @property
+    @functools.cached_property
     def fExceptionalBody(self) -> bool:
         """
         Indicates that the Exception Embedded Message object has a body that
         differs from the Recurring Calendar object. If True, the Exception MUST
         have a body.
         """
-        return self._ensureSetNamed('_fExceptionalBody', '8206', constants.PSETID_APPOINTMENT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('8206', constants.ps.PSETID_APPOINTMENT, bool, False)
 
-    @property
+    @functools.cached_property
     def fInvited(self) -> bool:
         """
         Indicates if invitations have been sent for this exception.
         """
-        return self._ensureSetNamed('_fInvited', '8229', constants.PSETID_APPOINTMENT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('8229', constants.ps.PSETID_APPOINTMENT, bool, False)
```

### Comparing `extract_msg-0.41.5/extract_msg/meeting_forward.py` & `extract_msg-0.42.0/extract_msg/msg_classes/meeting_forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 __all__ = [
     'MeetingForwardNotification',
 ]
 
 
+import functools
+
 from typing import Optional
 
-from . import constants
+from .. import constants
 from .meeting_related import MeetingRelated
-from .enums import RecurPatternType
+from ..enums import RecurPatternType
 
 
 class MeetingForwardNotification(MeetingRelated):
     """
     Class for handling Meeting Forward Notification objects.
     """
 
-    @property
+    @functools.cached_property
     def forwardNotificationRecipients(self) -> Optional[bytes]:
         """
         Bytes containing a list of RecipientRow structures that indicate the
         recipients of a meeting forward.
 
         Incomplete, looks to be the same structure as
         appointmentUnsendableRecipients, so we need more examples of this.
         """
-        return self._ensureSetNamed('_forwardNotificationRecipients', '8261', constants.PSETID_APPOINTMENT)
+        return self._getNamedAs('8261', constants.ps.PSETID_APPOINTMENT)
 
     @property
     def headerFormatProperties(self) -> constants.HEADER_FORMAT_TYPE:
         """
         Returns a dictionary of properties, in order, to be formatted into the
         header. Keys are the names to use in the header while the values are one
         of the following:
@@ -84,14 +86,14 @@
                 'Resources': self.bcc,
             },
             '-importance-': {
                 'Importance': self.importanceString,
             },
         }
 
-    @property
+    @functools.cached_property
     def promptSendUpdate(self) -> bool:
         """
         Indicates that the Meeting Forward Notification object was out-of-date
         when it was received.
         """
-        return self._ensureSetNamed('_promptSendUpdate', '8045', constants.PSETID_COMMON, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('8045', constants.ps.PSETID_COMMON, bool, False)
```

### Comparing `extract_msg-0.41.5/extract_msg/meeting_related.py` & `extract_msg-0.42.0/extract_msg/msg_classes/meeting_related.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 __all__ = [
     'MeetingRelated',
 ]
 
 
 import datetime
+import functools
 
-from typing import Optional, Set
+from typing import Optional
 
-from . import constants
+from ..constants import ps
 from .calendar_base import CalendarBase
-from .enums import ServerProcessingAction
+from ..enums import ServerProcessingAction
 
 
 class MeetingRelated(CalendarBase):
     """
     Base class for meeting-related objects.
     """
 
-    @property
+    @functools.cached_property
     def attendeeCriticalChange(self) -> Optional[datetime.datetime]:
         """
         The date and time at which the meeting-related object was sent.
         """
-        return self._ensureSetNamed('_attendeeCriticalChange', '0001', constants.PSETID_MEETING)
+        return self._getNamedAs('0001', ps.PSETID_MEETING)
 
-    @property
+    @functools.cached_property
     def processed(self) -> bool:
         """
         Indicates whether a client has processed a meeting-related object.
         """
-        return self._ensureSetProperty('_processed', '7D01000B', overrideClass = bool, preserveNone = False)
+        return self._getPropertyAs('7D01000B', bool, False)
 
-    @property
+    @functools.cached_property
     def serverProcessed(self) -> bool:
         """
         Indicates that the Meeting Request object or Meeting Update object has
         been processed.
         """
-        return self._ensureSetNamed('_serverProcessed', '85CC', constants.PSETID_CALENDAR_ASSISTANT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('85CC', ps.PSETID_CALENDAR_ASSISTANT, bool, False)
 
-    @property
-    def serverProcessingActions(self) -> Optional[Set[ServerProcessingAction]]:
+    @functools.cached_property
+    def serverProcessingActions(self) -> Optional[ServerProcessingAction]:
         """
-        A set of which actions have been taken on the Meeting Request object or
-        Meeting Update object.
+        A union of which actions have been taken on the Meeting Request object
+        or Meeting Update object.
         """
-        return self._ensureSetNamed('_serverProcessingActions', '85CD', constants.PSETID_CALENDAR_ASSISTANT, overrideClass = ServerProcessingAction.fromBits)
+        return self._getNamedAs('85CD', ps.PSETID_CALENDAR_ASSISTANT, ServerProcessingAction)
 
-    @property
+    @functools.cached_property
     def timeZone(self) -> Optional[int]:
         """
         Specifies information about the time zone of a recurring meeting.
 
         See PidLidTimeZone in [MS-OXOCAL] for details.
         """
-        return self._ensureSetNamed('_timeZone', '000C', constants.PSETID_MEETING)
+        return self._getNamedAs('000C', ps.PSETID_MEETING)
 
-    @property
+    @functools.cached_property
     def where(self) -> Optional[str]:
         """
         PidLidWhere. Should be the same as location.
         """
-        return self._ensureSetNamed('_where', '0002', constants.PSETID_MEETING)
+        return self._getNamedAs('0002', ps.PSETID_MEETING)
```

### Comparing `extract_msg-0.41.5/extract_msg/meeting_request.py` & `extract_msg-0.42.0/extract_msg/msg_classes/meeting_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 __all__ = [
     'MeetingRequest',
 ]
 
 
 import datetime
+import functools
 
-from typing import List, Optional, Set
+from typing import Optional
 
-from . import constants
+from ..constants import HEADER_FORMAT_TYPE, ps
 from .meeting_related import MeetingRelated
-from .enums import BusyStatus, MeetingObjectChange, MeetingType, RecurCalendarType, RecurPatternType, ResponseStatus
+from ..enums import BusyStatus, MeetingObjectChange, MeetingType, RecurCalendarType, RecurPatternType, ResponseStatus
 
 
 class MeetingRequest(MeetingRelated):
     """
     Class for handling Meeting Request and Meeting Update objects.
     """
 
-    @property
+    @functools.cached_property
     def appointmentMessageClass(self) -> Optional[str]:
         """
         Indicates the value of the PidTagMessageClass property of the Meeting
         object that is to be generated from the Meeting Request object. MUST
         start with "IPM.Appointment".
         """
-        return self._ensureSetNamed('_appointmentMessageClass', '0024', constants.PSETID_MEETING)
+        return self._getNamedAs('0024', ps.PSETID_MEETING)
 
-    @property
+    @functools.cached_property
     def calendarType(self) -> Optional[RecurCalendarType]:
         """
         The value of the CalendarType field from the PidLidAppointmentRecur
         property if the Meeting Request object represents a recurring series or
         an exception.
         """
-        return self._ensureSetNamed('_calendarType', '001C', constants.PSETID_MEETING, overrideClass = RecurCalendarType)
+        return self._getNamedAs('001C', ps.PSETID_MEETING, RecurCalendarType)
 
-    @property
-    def changeHighlight(self) -> Optional[Set[MeetingObjectChange]]:
+    @functools.cached_property
+    def changeHighlight(self) -> Optional[MeetingObjectChange]:
         """
         Soecifies a bit field that indicates how the Meeting object has been
         changed.
 
-        Returns a set of flags.
+        Returns a union of the set flags.
         """
-        return self._ensureSetNamed('_changeHighlight', '8204', constants.PSETID_APPOINTMENT, overrideClass = MeetingObjectChange.fromBits)
+        return self._getNamedAs('8204', ps.PSETID_APPOINTMENT, MeetingObjectChange)
 
-    @property
+    @functools.cached_property
     def forwardInstance(self) -> bool:
         """
         Indicates that the Meeting Request object represents an exception to a
         recurring series, and it was forwarded (even when forwarded by the
         organizer) rather than being an invitation sent by the organizer.
         """
-        return self._ensureSetNamed('_forwardInstance', '820A', constants.PSETID_APPOINTMENT, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('820A', ps.PSETID_APPOINTMENT, bool, False)
 
     @property
-    def headerFormatProperties(self) -> constants.HEADER_FORMAT_TYPE:
+    def headerFormatProperties(self) -> HEADER_FORMAT_TYPE:
         """
         Returns a dictionary of properties, in order, to be formatted into the
         header. Keys are the names to use in the header while the values are one
         of the following:
         None: Signifies no data was found for the property and it should be
             omitted from the header.
         str: A string to be formatted into the header using the string encoding.
@@ -128,45 +129,45 @@
             },
             '-importance-': {
                 'Importance': self.importanceString,
             },
         }
 
 
-    @property
+    @functools.cached_property
     def intendedBusyStatus(self) -> Optional[BusyStatus]:
         """
         The value of the busyStatus on the Meeting object in the organizer's
         calendar at the time the Meeting Request object or Meeting Update object
         was sent.
         """
-        return self._ensureSetNamed('_intendedBusyStatus', '8224', constants.PSETID_APPOINTMENT, overrideClass = BusyStatus)
+        return self._getNamedAs('8224', ps.PSETID_APPOINTMENT, BusyStatus)
 
-    @property
+    @functools.cached_property
     def meetingType(self) -> Optional[MeetingType]:
         """
         The type of Meeting Request object or Meeting Update object.
         """
-        return self._ensureSetNamed('_meetingType', '0026', constants.PSETID_MEETING, overrideClass = MeetingType)
+        return self._getNamedAs('0026', ps.PSETID_MEETING, MeetingType)
 
-    @property
+    @functools.cached_property
     def oldLocation(self) -> Optional[str]:
         """
         The original value of the location property before a meeting update.
         """
-        return self._ensureSetNamed('_oldLocation', '0028', constants.PSETID_MEETING)
+        return self._getNamedAs('0028', ps.PSETID_MEETING)
 
-    @property
+    @functools.cached_property
     def oldWhenEndWhole(self) -> Optional[datetime.datetime]:
         """
         The original value of the appointmentEndWhole property before a meeting
         update.
         """
-        return self._ensureSetNamed('_oldWhenEndWhole', '002A', constants.PSETID_MEETING)
+        return self._getNamedAs('002A', ps.PSETID_MEETING)
 
-    @property
+    @functools.cached_property
     def oldWhenStartWhole(self) -> Optional[datetime.datetime]:
         """
         The original value of the appointmentStartWhole property before a
         meeting update.
         """
-        return self._ensureSetNamed('_oldWhenStartWhole', '0029', constants.PSETID_MEETING)
+        return self._getNamedAs('0029', ps.PSETID_MEETING)
```

### Comparing `extract_msg-0.41.5/extract_msg/message_base.py` & `extract_msg-0.42.0/extract_msg/msg_classes/message_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from __future__ import annotations
-
-
 __all__ = [
     'MessageBase',
 ]
 
 
 import base64
 import datetime
@@ -16,33 +13,34 @@
 import os
 import pathlib
 import re
 import subprocess
 import zipfile
 
 import bs4
-import chardet
 import compressed_rtf
 import RTFDE
 
 from email.parser import Parser as EmailParser
 from typing import Callable, List, Optional, Union
 
-from . import constants
-from ._rtf.create_doc import createDocument
-from ._rtf.inject_rtf import injectStartRTF
-from .enums import BodyTypes, DeencapType, RecipientType
-from .exceptions import (
-        BadHtmlError, DataNotFoundError, DeencapMalformedData,
-        DeencapNotEncapsulated, IncompatibleOptionsError, WKError
+from .. import constants
+from .._rtf.create_doc import createDocument
+from .._rtf.inject_rtf import injectStartRTF
+from ..enums import (
+        BodyTypes, DeencapType, ErrorBehavior, RecipientType, SaveType
+    )
+from ..exceptions import (
+        DataNotFoundError, DeencapMalformedData, DeencapNotEncapsulated,
+        IncompatibleOptionsError, WKError
     )
 from .msg import MSGFile
-from .structures.report_tag import ReportTag
-from .recipient import Recipient
-from .utils import (
+from ..structures.report_tag import ReportTag
+from ..recipient import Recipient
+from ..utils import (
         addNumToDir, addNumToZipDir, createZipOpen, decodeRfc2047, findWk,
         htmlSanitize, inputToBytes, inputToString, isEncapsulatedRtf,
         prepareFilename, rtfSanitizeHtml, rtfSanitizePlain, validateHtml
     )
 
 from imapclient.imapclient import decode_utf7
 
@@ -54,123 +52,112 @@
 class MessageBase(MSGFile):
     """
     Base class for Message like msg files.
     """
 
     def __init__(self, path, **kwargs):
         """
-        :param path: path to the msg file in the system or is the raw msg file.
-        :param prefix: used for extracting embeded msg files
-            inside the main one. Do not set manually unless
-            you know what you are doing.
-        :param parentMsg: Used for syncronizing named properties instances. Do
-            not set this unless you know what you are doing.
-        :param attachmentClass: Optional, the class the Message object
-            will use for attachments. You probably should
-            not change this value unless you know what you
-            are doing.
-        :param filename: Optional, the filename to be used by default when
-            saving.
-        :param delayAttachments: Optional, delays the initialization of
-            attachments until the user attempts to retrieve them. Allows MSG
-            files with bad attachments to be initialized so the other data can
-            be retrieved.
-        :param overrideEncoding: Optional, an encoding to use instead of the one
-            specified by the msg file. Do not report encoding errors caused by
-            this.
-        :param attachmentErrorBehavior: Optional, the behavior to use in the
-            event of an error when parsing the attachments.
+        Supports all of the options from :method MSGFile.__init__: with some
+        additional ones.
+
         :param recipientSeparator: Optional, separator string to use between
             recipients.
-        :param ignoreRtfDeErrors: Optional, specifies that any errors that occur
-            from the usage of RTFDE should be ignored (default: False).
         :param deencapsulationFunc: Optional, if specified must be a callable
             that will override the way that HTML/text is deencapsulated from the
             RTF body. This function must take exactly 2 arguments, the first
             being the RTF body from the message and the second being an instance
             of the enum DeencapType that will tell the function what type of
             body is desired. The function should return a string for plain text
             and bytes for HTML. If any problems occur, the function *must*
             either return None or raise one of the appropriate functions from
             extract_msg.exceptions. All other exceptions must be handled
             internally or they will not be caught. The original deencapsulation
             method will not run if this is set.
         """
+        if 'ignoreRtfDeErrors' in kwargs:
+            import warnings
+            warnings.warn(':param ignoreRtfDeErrors: is deprecated. Use :param ErrorBehavior: instead.', DeprecationWarning)
+
+            if kwargs.get('ignoreRtfDeErrors', False):
+                errorBehavior = kwargs.get('errorBehavior', ErrorBehavior.THROW)
+                errorBehavior |= ErrorBehavior.RTFDE
+                kwargs['errorBehavior'] = errorBehavior
+
         super().__init__(path, **kwargs)
-        recipientSeparator = ';'
-        self.__recipientSeparator = kwargs.get('recipientSeparator', ';')
-        self.__ignoreRtfDeErrors = kwargs.get('ignoreRtfDeErrors', False)
-        self.__deencap = kwargs.get('deencapsulationFunc')
-        # Initialize properties in the order that is least likely to cause bugs.
-        # TODO have each function check for initialization of needed data so
-        # these lines will be unnecessary.
-        self.props
-        self.header
-        self.recipients
-
-        self.to
-        self.cc
-        self.sender
-        self.date
-        # This variable keeps track of what the new line character should be.
-        self.__crlf = '\n'
+        # The rest needs to be in a try-except block to ensure the file closes
+        # if an error occurs.
         try:
-            self.body
-        except Exception as e:
-            # Prevent an error in the body from preventing opening.
-            logger.exception('Critical error accessing the body. File opened but accessing the body will throw an exception.')
-        self.named
-        self.namedProperties
+            self.__recipientSeparator = kwargs.get('recipientSeparator', ';')
+            self.__deencap = kwargs.get('deencapsulationFunc')
+            # Initialize properties in the order that is least likely to cause bugs.
+            # TODO have each function check for initialization of needed data so
+            # these lines will be unnecessary.
+            self.props
+            self.header
+            self.recipients
+
+            self.to
+            self.cc
+            self.sender
+            self.date
+            # This variable keeps track of what the new line character should be.
+            self._crlf = '\n'
+            try:
+                self.body
+            except Exception as e:
+                # Prevent an error in the body from preventing opening.
+                logger.exception('Critical error accessing the body. File opened but accessing the body will throw an exception.')
+            self.named
+            self.namedProperties
+        except:
+            try:
+                self.close()
+            except:
+                pass
+            raise
 
     def _genRecipient(self, recipientType, recipientInt : RecipientType) -> Optional[str]:
         """
         Returns the specified recipient field.
         """
-        private = '_' + recipientType
         recipientInt = RecipientType(recipientInt)
-        try:
-            return getattr(self, private)
-        except AttributeError:
-            value = None
-            # Check header first.
-            if self.headerInit():
-                value = self.header[recipientType]
-                if value:
-                    value = decodeRfc2047(value)
-                    value = value.replace(',', self.__recipientSeparator)
-
-            # If the header had a blank field or didn't have the field, generate
-            # it manually.
-            if not value:
-                # Check if the header has initialized.
-                if self.headerInit():
-                    logger.info(f'Header found, but "{recipientType}" is not included. Will be generated from other streams.')
-
-                # Get a list of the recipients of the specified type.
-                foundRecipients = tuple(recipient.formatted for recipient in self.recipients if recipient.type == recipientInt)
-
-                # If we found recipients, join them with the recipient separator
-                # and a space.
-                if len(foundRecipients) > 0:
-                    value = (self.__recipientSeparator + ' ').join(foundRecipients)
-
-            # Code to fix the formatting so it's all a single line. This allows
-            # the user to format it themself if they want. This should probably
-            # be redone to use re or something, but I can do that later. This
-            # shouldn't be a huge problem for now.
+        value = None
+        # Check header first.
+        if self.headerInit():
+            value = self.header[recipientType]
             if value:
-                value = value.replace(' \r\n\t', ' ').replace('\r\n\t ', ' ').replace('\r\n\t', ' ')
-                value = value.replace('\r\n', ' ').replace('\r', ' ').replace('\n', ' ')
-                while value.find('  ') != -1:
-                    value = value.replace('  ', ' ')
+                value = decodeRfc2047(value)
+                value = value.replace(',', self.__recipientSeparator)
+
+        # If the header had a blank field or didn't have the field, generate
+        # it manually.
+        if not value:
+            # Check if the header has initialized.
+            if self.headerInit():
+                logger.info(f'Header found, but "{recipientType}" is not included. Will be generated from other streams.')
 
-            # Set the field in the class.
-            setattr(self, private, value)
+            # Get a list of the recipients of the specified type.
+            foundRecipients = tuple(recipient.formatted for recipient in self.recipients if recipient.type == recipientInt)
 
-            return value
+            # If we found recipients, join them with the recipient separator
+            # and a space.
+            if len(foundRecipients) > 0:
+                value = (self.__recipientSeparator + ' ').join(foundRecipients)
+
+        # Code to fix the formatting so it's all a single line. This allows
+        # the user to format it themself if they want. This should probably
+        # be redone to use re or something, but I can do that later. This
+        # shouldn't be a huge problem for now.
+        if value:
+            value = value.replace(' \r\n\t', ' ').replace('\r\n\t ', ' ').replace('\r\n\t', ' ')
+            value = value.replace('\r\n', ' ').replace('\r', ' ').replace('\n', ' ')
+            while value.find('  ') != -1:
+                value = value.replace('  ', ' ')
+
+        return value
 
     def deencapsulateBody(self, rtfBody : bytes, bodyType : DeencapType) -> Optional[Union[bytes, str]]:
         """
         A function to deencapsulate the specified body from the rtfBody. Returns
         a string for plain text and bytes for HTML. If specified, uses the
         deencapsulation override function. Returns None if nothing could be
         deencapsulated.
@@ -197,15 +184,15 @@
                         return self.__deencap(rtfBody, DeencapType.HTML)
                     except DeencapMalformedData:
                         logger.exception('Custom deencapsulation function reported encapsulated data was malformed.')
                     except DeencapNotEncapsulated:
                         logger.exception('Custom deencapsulation function reported data is not encapsulated.')
                 else:
                     if self.deencapsulatedRtf and self.deencapsulatedRtf.content_type == 'html':
-                        return self.deencapsulatedRtf.html.encode('utf-8')
+                        return self.deencapsulatedRtf.html
 
             if bodyType == DeencapType.PLAIN:
                 logger.info('Could not deencapsulate plain text from RTF body.')
             else:
                 logger.info('Could not deencapsulate HTML from RTF body.')
         else:
             logger.info('No RTF body to deencapsulate from.')
@@ -290,15 +277,15 @@
             'cc': inputToString(self.cc, self.stringEncoding),
             'bcc': inputToString(self.bcc, self.stringEncoding),
             'subject': inputToString(self.subject, self.stringEncoding),
             'date': inputToString(self.date, self.stringEncoding),
             'body': decode_utf7(self.body),
         })
 
-    def getSaveBody(self, **kwargs) -> bytes:
+    def getSaveBody(self, **_) -> bytes:
         """
         Returns the plain text body that will be used in saving based on the
         arguments.
 
         :param kwargs: Used to allow kwargs expansion in the save function.
             Arguments absorbed by this are simply ignored.
         """
@@ -309,31 +296,28 @@
         suffix = crlf + '-----------------' + crlf + crlf
         joinStr = crlf
         formatter = (lambda name, value : f'{name}: {value}')
 
         header = self.getInjectableHeader(prefix, joinStr, suffix, formatter).encode('utf-8')
         return header + inputToBytes(self.body, 'utf-8')
 
-    def getSaveHtmlBody(self, preparedHtml : bool = False, charset : str = 'utf-8', **kwargs) -> bytes:
+    def getSaveHtmlBody(self, preparedHtml : bool = False, charset : str = 'utf-8', **_) -> bytes:
         """
         Returns the HTML body that will be used in saving based on the
         arguments.
 
         :param preparedHtml: Whether or not the HTML should be prepared for
             standalone use (add tags, inject images, etc.).
         :param charset: If the html is being prepared, the charset to use for
             the Content-Type meta tag to insert. This exists to ensure that
             something parsing the html can properly determine the encoding (as
             not having this tag can cause errors in some programs). Set this to
             `None` or an empty string to not insert the tag (Default: 'utf-8').
         :param kwargs: Used to allow kwargs expansion in the save function.
             Arguments absorbed by this are simply ignored.
-
-        :raises BadHtmlError: if :param preparedHtml: is False and the HTML
-            fails to validate.
         """
         if self.htmlBody:
             # Inject the header into the data.
             data = self.injectHtmlHeader(prepared = preparedHtml)
 
             # If we are preparing the HTML, then we should
             if preparedHtml and charset:
@@ -360,15 +344,15 @@
 
                     data = bs.prettify('utf-8')
 
             return data
         else:
             return self.htmlBody
 
-    def getSavePdfBody(self, **kwargs) -> bytes:
+    def getSavePdfBody(self, wkPath = None, wkOptions = None, **kwargs) -> bytes:
         """
         Returns the PDF body that will be used in saving based on the arguments.
 
         :param wkPath: Used to manually specify the path of the wkhtmltopdf
             executable. If not specified, the function will try to find it.
             Useful if wkhtmltopdf is not on the path. If :param pdf: is False,
             this argument is ignored.
@@ -379,18 +363,17 @@
             Arguments absorbed by this are simply ignored.
 
         :raises ExecutableNotFound: The wkhtmltopdf executable could not be
             found.
         :raises WKError: Something went wrong in creating the PDF body.
         """
         # Immediately try to find the executable.
-        wkPath = findWk(kwargs.get('wkPath'))
+        wkPath = findWk(wkPath)
 
         # First thing is first, we need to parse our wkOptions if they exist.
-        wkOptions = kwargs.get('wkOptions')
         if wkOptions:
             try:
                 # Try to convert to a list, whatever it is, and fail if it is
                 # not possible.
                 parsedWkOptions = [*wkOptions]
             except TypeError:
                 raise TypeError(f':param wkOptions: must be an iterable, not {type(wkOptions)}.')
@@ -419,15 +402,15 @@
 
         # If it errored, throw it as an exception.
         if process.returncode != 0:
             raise WKError(process.stderr.decode('utf-8'))
 
         return process.stdout
 
-    def getSaveRtfBody(self, **kwargs) -> bytes:
+    def getSaveRtfBody(self, **_) -> bytes:
         """
         Returns the RTF body that will be used in saving based on the arguments.
 
         :param kwargs: Used to allow kwargs expansion in the save function.
             Arguments absorbed by this are simply ignored.
         """
         # Inject the header into the data.
@@ -448,16 +431,14 @@
         Returns the HTML body from the MSG file (will check that it has one) with
         the HTML header injected into it.
 
         :param prepared: Determines whether to be using the standard HTML (False) or
             the prepared HTML (True) body (Default: False).
 
         :raises AttributeError: if the correct HTML body cannot be acquired.
-        :raises BadHtmlError: if :param preparedHtml: is False and the HTML fails to
-            validate.
         """
         if not self.htmlBody:
             raise AttributeError('Cannot inject the HTML header without an HTML body attribute.')
 
         body = None
 
         # We don't do this all at once because the prepared body is not cached.
@@ -468,26 +449,23 @@
             if not body:
                 raise AttributeError('Cannot find a prepared HTML body to inject into.')
         else:
             body = self.htmlBody
 
         # Validate the HTML.
         if not validateHtml(body):
-            # If we are not preparing the HTML body, then raise an
-            # exception.
-            if not prepared:
-                raise BadHtmlError('HTML body failed to pass validation.')
-
-            # If we are here, then we need to do what we can to fix the HTML body.
-            # Unfortunately this gets complicated because of the various ways the
-            # body could be wrong. If only the <body> tag is missing, then we just
-            # need to insert it at the end and be done. If both the <html> and
-            # <body> tag are missing, we determine where to put the body tag (around
-            # everything if there is no <head> tag, otherwise at the end) and then
-            # wrap it all in the <html> tag.
+            logger.warning('HTML body failed to validate. Code will attempt to correct it.')
+
+            # If we are here, then we need to do what we can to fix the HTML
+            # body. Unfortunately this gets complicated because of the various
+            # ways the body could be wrong. If only the <body> tag is missing,
+            # then we just need to insert it at the end and be done. If both
+            # the <html> and <body> tag are missing, we determine where to put
+            # the body tag (around everything if there is no <head> tag,
+            # otherwise at the end) and then wrap it all in the <html> tag.
             parser = bs4.BeautifulSoup(body, features = 'html.parser')
             if not parser.find('html') and not parser.find('body'):
                 if parser.find('head') or parser.find('footer'):
                     # Create the parser we will be using for the corrections.
                     correctedHtml = bs4.BeautifulSoup(b'<html></html>', features = 'html.parser')
                     htmlTag = correctedHtml.find('html')
 
@@ -554,15 +532,15 @@
             # how to get all of the properties we are formatting. They are all
             # processed in the same way, making everything neat. By defining them
             # in each class, any class can specify a completely different set to be
             # used.
             return bodyMarker.group() + self.htmlInjectableHeader.encode('utf-8')
 
         # Use the previously defined function to inject the HTML header.
-        return constants.RE_HTML_BODY_START.sub(replace, body, 1)
+        return constants.re.HTML_BODY_START.sub(replace, body, 1)
 
     def injectRtfHeader(self) -> bytes:
         """
         Returns the RTF body from this MSG file (will check that it has one)
         with the RTF header injected into it.
 
         :raises AttributeError: if the RTF body cannot be acquired.
@@ -583,26 +561,26 @@
             Internal function to replace the body tag with itself plus the header.
             """
             return bodyMarker.group() + injectableHeader
 
         # This first method only applies to documents with encapsulated HTML
         # that is formatted in a nice way.
         if isEncapsulatedRtf(self.rtfBody):
-            data = constants.RE_RTF_ENC_BODY_START.sub(replace, self.rtfBody, 1)
+            data = constants.re.RTF_ENC_BODY_START.sub(replace, self.rtfBody, 1)
             if data != self.rtfBody:
                 logger.debug('Successfully injected RTF header using encapsulation method.')
                 return data
             logger.debug('RTF has encapsulated HTML, but injection method failed. It is likely dirty. Will use normal RTF injection method.')
 
         # If the normal encapsulated HTML injection fails or it isn't
         # encapsulated, use the internal _rtf module.
         logger.debug('Using _rtf module to inject RTF text header.')
         return createDocument(injectStartRTF(self.rtfBody, injectableHeader))
 
-    def save(self, **kwargs) -> MessageBase:
+    def save(self, **kwargs) -> constants.SAVE_TYPE:
         """
         Saves the message body and attachments found in the message.
 
         The body and attachments are stored in a folder in the current running
         directory unless :param customPath: has been specified. The name of the
         folder will be determined by 3 factors.
            * If :param customFilename: has been set, the value provided for that
@@ -695,268 +673,265 @@
         # Track if we should skip the body if no valid body is found instead of
         # raising an exception.
         skipBodyNotFound = kwargs.get('skipBodyNotFound', False)
 
         if pdf:
             kwargs['preparedHtml'] = True
 
-        # ZipFile handling.
-        if _zip:
-            # `raw` and `zip` are incompatible.
-            if raw:
-                raise IncompatibleOptionsError('The options `raw` and `zip` are incompatible.')
-            # If we are doing a zip file, first check that we have been given a
-            # path.
-            if isinstance(_zip, (str, pathlib.Path)):
-                # If we have a path then we use the zip file.
-                _zip = zipfile.ZipFile(_zip, 'a', zipfile.ZIP_DEFLATED)
-                kwargs['zip'] = _zip
-                createdZip = True
-            else:
-                createdZip = False
-            # Path needs to be done in a special way if we are in a zip file.
-            path = pathlib.Path(kwargs.get('customPath', ''))
-            # Set the open command to be that of the zip file.
-            _open = createZipOpen(_zip.open)
-            # Zip files use w for writing in binary.
-            mode = 'w'
-        else:
-            path = pathlib.Path(kwargs.get('customPath', '.')).absolute()
-            mode = 'wb'
-            _open = open
-
-        # Reset this for sub save calls.
-        kwargs['customFilename'] = None
-
-        # Check if incompatible options have been provided in any way.
-        if _json + html + rtf + raw + attachOnly + pdf > 1:
-            raise IncompatibleOptionsError('Only one of the following options may be used at a time: json, raw, html, rtf, attachmentsOnly, pdf.')
-
-        # TODO: insert code here that will handle checking all of the msg files
-        # to see if the path with overflow.
-
-        if customFilename:
-            # First we need to validate it. If there are invalid characters,
-            # this will detect it.
-            if constants.RE_INVALID_FILENAME_CHARACTERS.search(customFilename):
-                raise ValueError('Invalid character found in customFilename. Must not contain any of the following characters: \\/:*?"<>|')
-            # Quick fix to remove spaces from the end of the filename, if any
-            # are there.
-            customFilename = customFilename.strip()
-            path /= customFilename[:maxNameLength]
-        elif useMsgFilename:
-            if not self.filename:
-                raise ValueError(':param useMsgFilename: is only available if you are using an msg file on the disk or have provided a filename.')
-            # Get the actual name of the file.
-            filename = os.path.split(self.filename)[1]
-            # Remove the extensions.
-            filename = os.path.splitext(filename)[0]
-            # Prepare the filename by removing any special characters.
-            filename = prepareFilename(filename)
-            # Shorted the filename.
-            filename = filename[:maxNameLength]
-            # Check to make sure we actually have a filename to use.
-            if not filename:
-                raise ValueError(f'Invalid filename found in self.filename: "{self.filename}"')
+        # Try to get the body, if needed, before messing with the path.
+        if not attachOnly:
+            # Check what to save the body with.
+            fext = 'json' if _json else 'txt'
+
+            fallbackToPlain = False
+            useHtml = False
+            usePdf = False
+            useRtf = False
+            if html:
+                if self.htmlBody:
+                    useHtml = True
+                    fext = 'html'
+                elif not allowFallback:
+                    if skipBodyNotFound:
+                        fext = None
+                    else:
+                        raise DataNotFoundError('Could not find the htmlBody.')
 
-            # Add the file name to the path.
-            path /= filename[:maxNameLength]
-        else:
-            path /= self.defaultFolderName[:maxNameLength]
+            if pdf:
+                if self.htmlBody:
+                    usePdf = True
+                    fext = 'pdf'
+                elif not allowFallback:
+                    if skipBodyNotFound:
+                        fext = None
+                    else:
+                        raise DataNotFoundError('Count not find the htmlBody to convert to pdf.')
 
-        # Create the folders.
-        if not _zip:
-            try:
-                os.makedirs(path)
-            except Exception:
-                newDirName = addNumToDir(path)
-                if newDirName:
-                    path = newDirName
-                else:
-                    raise Exception(f'Failed to create directory "{path}". Does it already exist?')
-        else:
-            # In my testing I ended up with multiple files in a zip at the same
-            # location so let's try to handle that.
-            pathCompare = str(path).replace('\\', '/').rstrip('/') + '/'
-            if any(x.startswith(pathCompare) for x in _zip.namelist()):
-                newDirName = addNumToZipDir(path, _zip)
-                if newDirName:
-                    path = newDirName
+            if rtf or (html and not useHtml) or (pdf and not usePdf):
+                if self.rtfBody:
+                    useRtf = True
+                    fext = 'rtf'
+                elif not allowFallback:
+                    if skipBodyNotFound:
+                        fext = None
+                    else:
+                        raise DataNotFoundError('Could not find the rtfBody.')
                 else:
-                    raise Exception(f'Failed to create directory "{path}". Does it already exist?')
+                    # This was the last resort before plain text, so fall
+                    # back to that.
+                    fallbackToPlain = True
+
+            # After all other options, try to go with plain text if
+            # possible.
+            if not (rtf or html or pdf) or fallbackToPlain:
+                # We need to check if the plain text body was found. If it
+                # was found but was empty that is considered valid, so we
+                # specifically check against None.
+                if self.body is None:
+                    if skipBodyNotFound:
+                        fext = None
+                    else:
+                        if allowFallback:
+                            raise DataNotFoundError('Could not find a valid body using current options.')
+                        else:
+                            raise DataNotFoundError('Plain text body could not be found.')
 
-        # Update the kwargs.
-        kwargs['customPath'] = path
+        createdZip = False
+        try:
+            # ZipFile handling.
+            if _zip:
+                # `raw` and `zip` are incompatible.
+                if raw:
+                    raise IncompatibleOptionsError('The options `raw` and `zip` are incompatible.')
+                # If we are doing a zip file, first check that we have been
+                # given a path.
+                if isinstance(_zip, (str, pathlib.Path)):
+                    # If we have a path then we use the zip file.
+                    _zip = zipfile.ZipFile(_zip, 'a', zipfile.ZIP_DEFLATED)
+                    kwargs['zip'] = _zip
+                    createdZip = True
+                # Path needs to be done in a special way if we are in a zip
+                # file.
+                path = pathlib.Path(kwargs.get('customPath', ''))
+                # Set the open command to be that of the zip file.
+                _open = createZipOpen(_zip.open)
+                # Zip files use w for writing in binary.
+                mode = 'w'
+            else:
+                path = pathlib.Path(kwargs.get('customPath', '.')).absolute()
+                mode = 'wb'
+                _open = open
+
+            # Reset this for sub save calls.
+            kwargs['customFilename'] = None
+
+            # Check if incompatible options have been provided in any way.
+            if _json + html + rtf + raw + attachOnly + pdf > 1:
+                raise IncompatibleOptionsError('Only one of the following options may be used at a time: json, raw, html, rtf, attachmentsOnly, pdf.')
+
+            # TODO: insert code here that will handle checking all of the msg
+            # files to see if the path with overflow.
+
+            if customFilename:
+                # First we need to validate it. If there are invalid characters,
+                # this will detect it.
+                if constants.re.INVALID_FILENAME_CHARS.search(customFilename):
+                    raise ValueError('Invalid character found in customFilename. Must not contain any of the following characters: \\/:*?"<>|')
+                # Quick fix to remove spaces from the end of the filename, if
+                # any are there.
+                customFilename = customFilename.strip()
+                path /= customFilename[:maxNameLength]
+            elif useMsgFilename:
+                if not self.filename:
+                    raise ValueError(':param useMsgFilename: is only available if you are using an msg file on the disk or have provided a filename.')
+                # Get the actual name of the file.
+                filename = os.path.split(self.filename)[1]
+                # Remove the extensions.
+                filename = os.path.splitext(filename)[0]
+                # Prepare the filename by removing any special characters.
+                filename = prepareFilename(filename)
+                # Shorted the filename.
+                filename = filename[:maxNameLength]
+                # Check to make sure we actually have a filename to use.
+                if not filename:
+                    raise ValueError(f'Invalid filename found in self.filename: "{self.filename}"')
 
-        if raw:
-            self.saveRaw(path)
-            return self
-
-        # If the user has requested the headers for this file, save it now.
-        if kwargs.get('saveHeader', False):
-            headerText = self.headerText
-            if not headerText:
-                headerText = constants.HEADER_FORMAT.format(subject = self.subject, **self.header)
+                # Add the file name to the path.
+                path /= filename[:maxNameLength]
+            else:
+                path /= self.defaultFolderName[:maxNameLength]
 
-            with _open(str(path / 'header.txt'), mode) as f:
-                f.write(headerText.encode('utf-8'))
+            # Create the folders.
+            if not _zip:
+                try:
+                    os.makedirs(path)
+                except Exception:
+                    newDirName = addNumToDir(path)
+                    if newDirName:
+                        path = newDirName
+                    else:
+                        raise OSError(f'Failed to create directory "{path}". Does it already exist?')
+            else:
+                # In my testing I ended up with multiple files in a zip at the
+                # same location so let's try to handle that.
+                pathCompare = str(path).replace('\\', '/').rstrip('/') + '/'
+                if any(x.startswith(pathCompare) for x in _zip.namelist()):
+                    newDirName = addNumToZipDir(path, _zip)
+                    if newDirName:
+                        path = newDirName
+                    else:
+                        raise Exception(f'Failed to create directory "{path}". Does it already exist?')
 
-        try:
-            if not attachOnly:
-                # Check what to save the body with.
-                fext = 'json' if _json else 'txt'
-
-                fallbackToPlain = False
-                useHtml = False
-                usePdf = False
-                useRtf = False
-                if html:
-                    if self.htmlBody:
-                        useHtml = True
-                        fext = 'html'
-                    elif not allowFallback:
-                        if skipBodyNotFound:
-                            fext = None
-                        else:
-                            raise DataNotFoundError('Could not find the htmlBody.')
+            # Update the kwargs.
+            kwargs['customPath'] = path
 
-                if pdf:
-                    if self.htmlBody:
-                        usePdf = True
-                        fext = 'pdf'
-                    elif not allowFallback:
-                        if skipBodyNotFound:
-                            fext = None
-                        else:
-                            raise DataNotFoundError('Count not find the htmlBody to convert to pdf.')
+            if raw:
+                self.saveRaw(path)
+                return (SaveType.FOLDER, str(path))
 
-                if rtf or (html and not useHtml) or (pdf and not usePdf):
-                    if self.rtfBody:
-                        useRtf = True
-                        fext = 'rtf'
-                    elif not allowFallback:
-                        if skipBodyNotFound:
-                            fext = None
-                        else:
-                            raise DataNotFoundError('Could not find the rtfBody.')
-                    else:
-                        # This was the last resort before plain text, so fall
-                        # back to that.
-                        fallbackToPlain = True
-
-                # After all other options, try to go with plain text if
-                # possible.
-                if not (rtf or html or pdf) or fallbackToPlain:
-                    # We need to check if the plain text body was found. If it
-                    # was found but was empty that is considered valid, so we
-                    # specifically check against None.
-                    if self.body is None:
-                        if skipBodyNotFound:
-                            fext = None
-                        else:
-                            if allowFallback:
-                                raise DataNotFoundError('Could not find a valid body using current options.')
-                            else:
-                                raise DataNotFoundError('Plain text body could not be found.')
+            # If the user has requested the headers for this file, save it now.
+            if kwargs.get('saveHeader', False):
+                headerText = self.headerText
+                if not headerText:
+                    headerText = constants.HEADER_FORMAT.format(subject = self.subject, **self.header)
+
+                with _open(str(path / 'header.txt'), mode) as f:
+                    f.write(headerText.encode('utf-8'))
 
 
             if not skipAttachments:
                 # Save the attachments.
-                attachmentNames = [attachment.save(**kwargs) for attachment in self.attachments if not (skipHidden and attachment.hidden)]
-                # Remove skipped attachments.
-                attachmentNames = [x for x in attachmentNames if x and isinstance(x, str)]
+                attachmentReturns = [attachment.save(**kwargs) for attachment in self.attachments if not (skipHidden and attachment.hidden)]
+                # Get the names from each.
+                attachmentNames = []
+                for x in attachmentReturns:
+                    if isinstance(x[1], str):
+                        attachmentNames.append(x[1])
+                    elif isinstance(x[1], list):
+                        attachmentNames.extend(x[1])
 
             if not attachOnly and fext:
                 with _open(str(path / ('message.' + fext)), mode) as f:
                     if _json:
                         emailObj = json.loads(self.getJson())
                         if not skipAttachments:
                             emailObj['attachments'] = attachmentNames
 
-                        f.write(inputToBytes(json.dumps(emailObj), 'utf-8'))
+                        f.write(json.dumps(emailObj).encode('utf-8'))
                     elif useHtml:
                         f.write(self.getSaveHtmlBody(**kwargs))
                     elif usePdf:
                         f.write(self.getSavePdfBody(**kwargs))
                     elif useRtf:
                         f.write(self.getSaveRtfBody(**kwargs))
                     else:
                         f.write(self.getSaveBody(**kwargs))
+
+            return (SaveType.FOLDER, str(path))
         finally:
             # Close the ZipFile if this function created it.
             if _zip and createdZip:
                 _zip.close()
 
-        # Return the instance so that functions can easily be chained.
-        return self
-
-    @property
+    @functools.cached_property
     def bcc(self) -> Optional[str]:
         """
         Returns the bcc field, if it exists.
         """
         return self._genRecipient('bcc', RecipientType.BCC)
 
-    @property
+    @functools.cached_property
     def body(self) -> Optional[str]:
         """
         Returns the message body, if it exists.
         """
-        try:
-            return self._body
-        except AttributeError:
-            if self._ensureSet('_body', '__substg1.0_1000'):
-                pass
-            else:
-                # If the body doesn't exist, see if we can get it from the RTF
-                # body.
-                if self.rtfBody:
-                    self._body = self.deencapsulateBody(self.rtfBody, DeencapType.PLAIN)
+        # If the body exists but is empty, that means it should be returned.
+        if (body := self._getStringStream('__substg1.0_1000')) is not None:
+            pass
+        elif self.rtfBody:
+            # If the body doesn't exist, see if we can get it from the RTF
+            # body.
+            body = self.deencapsulateBody(self.rtfBody, DeencapType.PLAIN)
+
+        if body:
+            body = inputToString(body, 'utf-8')
+            if re.search('\n', body) is not None:
+                if re.search('\r\n', body) is not None:
+                    self._crlf = '\r\n'
 
-            if self._body:
-                self._body = inputToString(self._body, 'utf-8')
-                a = re.search('\n', self._body)
-                if a is not None:
-                    if re.search('\r\n', self._body) is not None:
-                        self.__crlf = '\r\n'
-            return self._body
+        return body
 
-    @property
+    @functools.cached_property
     def cc(self) -> Optional[str]:
         """
         Returns the cc field, if it exists.
         """
         return self._genRecipient('cc', RecipientType.CC)
 
-    @property
+    @functools.cached_property
     def compressedRtf(self) -> Optional[bytes]:
         """
         Returns the compressed RTF stream, if it exists.
         """
-        return self._ensureSet('_compressedRtf', '__substg1.0_10090102', False)
+        return self._getStream('__substg1.0_10090102')
 
     @property
     def crlf(self) -> str:
         """
         Returns the value of self.__crlf, should you need it for whatever
         reason.
         """
-        self.body
-        return self.__crlf
+        return self._crlf
 
-    @property
-    def date(self) -> Optional[str]:
+    @functools.cached_property
+    def date(self) -> Optional[datetime.datetime]:
         """
         Returns the send date, if it exists.
         """
-        try:
-            return self._date
-        except AttributeError:
-            self._date = self._prop.date if self.isSent else None
-            return self._date
+        return self.props.date if self.isSent else None
 
     @property
     def deencapsulatedRtf(self) -> Optional[RTFDE.DeEncapsulator]:
         """
         Returns the instance of the deencapsulated RTF body. If there is no RTF
         body or the body is not encasulated, returns None.
         """
@@ -969,49 +944,28 @@
                 # Sometimes you get MSG files whose RTF body has stuff
                 # *after* the body, and RTFDE can't handle that. Here is
                 # how we compensate.
                 while body and body[-1] != 125:
                     body = body[:-1]
 
                 try:
-                    try:
-                        self._deencapsultor = RTFDE.DeEncapsulator(body)
-                    except UnicodeDecodeError:
-                        # There is a known issue that bytes are not well decoded
-                        # by RTFDE right now, so let's see if we can't manually
-                        # decode it and see if that will work.
-                        #
-                        # There is also the fact that it is decoded *at all*
-                        # before binary data is stripped out. This data should
-                        # almost certainly be stripped out, so let's log it and
-                        # then log if we removed any of them before trying this.
-                        logger.warning(f'RTFDE failed to decode rtfBody for message with subject "{self.subject}". Attempting to cut out unnecessary data and override decoding.')
-
-                        match = constants.RE_BIN.search(body)
-                        # Because we are going to be actively removing things,
-                        # we want to search the entire thing over again.
-                        while match:
-                            logger.info(f'Found match to bin data starting at location {match.start()}. Replacing with nothing.')
-                            length = int(match.group(1))
-                            # Extract the entire binary section and replace it.
-                            body = body.replace(body[match.start():match.end() + length], b'', 1)
-                            match = constants.RE_BIN.search(body)
-
-                        self._deencapsultor = RTFDE.DeEncapsulator(body.decode(chardet.detect(body)['encoding']))
+                    self._deencapsultor = RTFDE.DeEncapsulator(body)
                     self._deencapsultor.deencapsulate()
                 except RTFDE.exceptions.NotEncapsulatedRtf as e:
                     logger.debug('RTF body is not encapsulated.')
                     self._deencapsultor = None
                 except RTFDE.exceptions.MalformedEncapsulatedRtf as _e:
+                    if ErrorBehavior.RTFDE_MALFORMED not in self.errorBehavior:
+                        raise
                     logger.info('RTF body contains malformed encapsulated content.')
                     self._deencapsultor = None
                 except Exception:
                     # If we are just ignoring the errors, log it then set to
                     # None. Otherwise, continue the exception.
-                    if not self.__ignoreRtfDeErrors:
+                    if ErrorBehavior.RTFDE_UNKNOWN_ERROR not in self.errorBehavior:
                         raise
                     logger.exception('Unhandled error happened while using RTFDE. You have choosen to ignore these errors.')
                     self._deencapsultor = None
             else:
                 self._deencapsultor = None
             return self._deencapsultor
 
@@ -1043,41 +997,37 @@
         if self.exists('__substg1.0_10090102'):
             bodies |= BodyTypes.RTF
         if self.exists('__substg1.0_10130102'):
             bodies |= BodyTypes.HTML
 
         return bodies
 
-    @property
+    @functools.cached_property
     def header(self) -> email.message.Message:
         """
         Returns the message header, if it exists. Otherwise it will generate
         one.
         """
-        try:
-            return self._header
-        except AttributeError:
-            headerText = self.headerText
-            if headerText:
-                self._header = EmailParser().parsestr(headerText)
-                self._header['date'] = self.date
-            else:
-                logger.info('Header is empty or was not found. Header will be generated from other streams.')
-                header = EmailParser().parsestr('')
-                header.add_header('Date', self.date)
-                header.add_header('From', self.sender)
-                header.add_header('To', self.to)
-                header.add_header('Cc', self.cc)
-                header.add_header('Bcc', self.bcc)
-                header.add_header('Message-Id', self.messageId)
-                # TODO find authentication results outside of header
-                header.add_header('Authentication-Results', None)
-                self._header = header
+        headerText = self.headerText
+        if headerText:
+            header = EmailParser().parsestr(headerText)
+            header['date'] = self.date
+        else:
+            logger.info('Header is empty or was not found. Header will be generated from other streams.')
+            header = EmailParser().parsestr('')
+            header.add_header('Date', self.date)
+            header.add_header('From', self.sender)
+            header.add_header('To', self.to)
+            header.add_header('Cc', self.cc)
+            header.add_header('Bcc', self.bcc)
+            header.add_header('Message-Id', self.messageId)
+            # TODO find authentication results outside of header
+            header.add_header('Authentication-Results', None)
 
-            return self._header
+        return header
 
     @property
     def headerDict(self) -> dict:
         """
         Returns a dictionary of the entries in the header
         """
         try:
@@ -1135,42 +1085,38 @@
     @functools.cached_property
     def headerText(self) -> Optional[str]:
         """
         The raw text of the header stream, if it exists.
         """
         return self._getStringStream('__substg1.0_007D')
 
-    @property
+    @functools.cached_property
     def htmlBody(self) -> Optional[bytes]:
         """
         Returns the html body, if it exists.
         """
-        try:
-            return self._htmlBody
-        except AttributeError:
-            if self._ensureSet('_htmlBody', '__substg1.0_10130102', False):
-                # Reducing line repetition.
-                pass
-            elif self.rtfBody:
-                logger.info('HTML body was not found, attempting to generate from RTF.')
-                self._htmlBody = self.deencapsulateBody(self.rtfBody, DeencapType.HTML)
-            # This is it's own if statement so we can ensure it will generate
-            # even if there is an rtfBody, in the event it doesn't have HTML.
-            if not self._htmlBody and self.body:
-                # Convert the plain text body to html.
-                logger.info('HTML body was not found, attempting to generate from plain text body.')
-                correctedBody = html.escape(self.body).replace('\r', '').replace('\n', '<br />')
-                self._htmlBody = f'<html><body>{correctedBody}</body></head>'.encode('utf-8')
+        if (htmlBody := self._getStream('__substg1.0_10130102')) is not None:
+            pass
+        elif self.rtfBody:
+            logger.info('HTML body was not found, attempting to generate from RTF.')
+            htmlBody = self.deencapsulateBody(self.rtfBody, DeencapType.HTML)
+        # This is it's own if statement so we can ensure it will generate
+        # even if there is an rtfBody, in the event it doesn't have HTML.
+        if not htmlBody and self.body:
+            # Convert the plain text body to html.
+            logger.info('HTML body was not found, attempting to generate from plain text body.')
+            correctedBody = html.escape(self.body).replace('\r', '').replace('\n', '<br />')
+            htmlBody = f'<html><body>{correctedBody}</body></head>'.encode('utf-8')
 
-            if not self._htmlBody:
-                logger.info('HTML body could not be found nor generated.')
+        if not htmlBody:
+            logger.info('HTML body could not be found nor generated.')
 
-            return self._htmlBody
+        return htmlBody
 
-    @property
+    @functools.cached_property
     def htmlBodyPrepared(self) -> Optional[bytes]:
         """
         Returns the HTML body that has (where possible) the embedded attachments
         inserted into the body.
         """
         # If we can't get an HTML body then we have nothing to do.
         if not self.htmlBody:
@@ -1190,184 +1136,166 @@
             data = next((attachment.data for attachment in self.attachments if attachment.cid == cid), None)
             # If we found anything, inject it.
             if data:
                 tag['src'] = (b'data:image;base64,' + base64.b64encode(data)).decode('utf-8')
 
         return soup.prettify('utf-8')
 
-    @property
+    @functools.cached_property
     def htmlInjectableHeader(self) -> str:
         """
         The header that can be formatted and injected into the html body.
         """
         prefix = '<div id="injectedHeader"><div><p class="MsoNormal">'
         suffix = '<o:p></o:p></p></div></div>'
         joinStr = '<br/>'
         formatter = (lambda name, value : f'<b>{name}:</b>&nbsp;{inputToString(htmlSanitize(value), self.stringEncoding)}')
 
         return self.getInjectableHeader(prefix, joinStr, suffix, formatter)
 
-    @property
+    @functools.cached_property
     def inReplyTo(self) -> Optional[str]:
         """
         Returns the message id that this message is in reply to.
         """
-        return self._ensureSet('_in_reply_to', '__substg1.0_1042')
+        return self._getStringStream('__substg1.0_1042')
 
-    @property
+    @functools.cached_property
     def isRead(self) -> bool:
         """
         Returns if this email has been marked as read.
         """
-        return bool(self.props['0E070003'].value & 1)
+        try:
+            return bool(self.props['0E070003'].value & 1)
+        except (AttributeError, KeyError):
+            return False
 
-    @property
+    @functools.cached_property
     def isSent(self) -> bool:
         """
         Returns if this email has been marked as sent. Assumes True if no flags
         are found.
         """
         if not self.props.get('0E070003'):
             return True
         else:
             return not bool(self.props['0E070003'].value & 8)
 
-    @property
+    @functools.cached_property
     def messageId(self) -> Optional[str]:
-        try:
-            return self._messageId
-        except AttributeError:
-            headerResult = None
-            if self.headerInit():
-                headerResult = self.header['message-id']
-            if headerResult is not None:
-                self._messageId = headerResult
-            else:
-                if self.headerInit():
-                    logger.info('Header found, but "Message-Id" is not included. Will be generated from other streams.')
-                self._messageId = self._getStringStream('__substg1.0_1035')
-            return self._messageId
+        headerResult = None
+        if self.headerInit():
+            headerResult = self.header['message-id']
+        if headerResult is not None:
+            return headerResult
+
+        if self.headerInit():
+            logger.info('Header found, but "Message-Id" is not included. Will be generated from other streams.')
+        return self._getStringStream('__substg1.0_1035')
 
-    @property
+    @functools.cached_property
     def parsedDate(self):
         return email.utils.parsedate(self.date)
 
-    @property
+    @functools.cached_property
     def receivedTime(self) -> Optional[datetime.datetime]:
         """
         The date and time the message was received by the server.
         """
-        return self._ensureSetProperty('_receivedTime', '0E060040')
+        return self._getPropertyAs('0E060040')
 
     @property
     def recipientSeparator(self) -> str:
         return self.__recipientSeparator
 
-    @property
+    @functools.cached_property
     def recipients(self) -> List[Recipient]:
         """
         Returns a list of all recipients.
         """
-        try:
-            return self._recipients
-        except AttributeError:
-            # Get the recipients
-            recipientDirs = []
-            prefixLen = self.prefixLen
-            for dir_ in self.listDir():
-                if dir_[prefixLen].startswith('__recip') and\
-                        dir_[prefixLen] not in recipientDirs:
-                    recipientDirs.append(dir_[prefixLen])
+        recipientDirs = []
+        prefixLen = self.prefixLen
+        for dir_ in self.listDir():
+            if dir_[prefixLen].startswith('__recip') and\
+                    dir_[prefixLen] not in recipientDirs:
+                recipientDirs.append(dir_[prefixLen])
 
-            self._recipients = []
+        return [Recipient(recipientDir, self) for recipientDir in recipientDirs]
 
-            for recipientDir in recipientDirs:
-                self._recipients.append(Recipient(recipientDir, self))
-
-            return self._recipients
-
-    @property
+    @functools.cached_property
     def reportTag(self) -> Optional[ReportTag]:
         """
         Data that is used to correlate the report and the original message.
         """
-        return self._ensureSet('_reportTag', '__substg1.0_00310102', False, overrideClass = ReportTag)
+        return self._getStreamAs('__substg1.0_00310102', False, ReportTag)
 
-    @property
+    @functools.cached_property
     def rtfBody(self) -> Optional[bytes]:
         """
         Returns the decompressed Rtf body from the message.
         """
-        try:
-            return self._rtfBody
-        except AttributeError:
-            self._rtfBody = compressed_rtf.decompress(self.compressedRtf) if self.compressedRtf else None
-            return self._rtfBody
+        return compressed_rtf.decompress(self.compressedRtf) if self.compressedRtf else None
 
-    @property
+    @functools.cached_property
     def rtfEncapInjectableHeader(self) -> bytes:
         """
         The header that can be formatted and injected into the plain RTF body.
         """
         prefix = r'\htmlrtf {\htmlrtf0 {\*\htmltag96 <div>}{\*\htmltag96 <div>}{\*\htmltag64 <p class=MsoNormal>}'
         suffix = r'{\*\htmltag244 <o:p>}{\*\htmlrag252 </o:p>}\htmlrtf \par\par\htmlrtf0 {\*\htmltag72 </p>}{\*\htmltag104 </div>}{\*\htmltag104 </div>}\htmlrtf }\htmlrtf0 '
         joinStr = r'{\*\htmltag116 <br />}\htmlrtf \line\htmlrtf0 '
         formatter = (lambda name, value : fr'\htmlrtf {{\b\htmlrtf0{{\*\htmltag84 <b>}}{name}: {{\*\htmltag92 </b>}}\htmlrtf \b0\htmlrtf0 {inputToString(rtfSanitizeHtml(value), self.stringEncoding)}\htmlrtf }}\htmlrtf0')
 
         return self.getInjectableHeader(prefix, joinStr, suffix, formatter).encode('utf-8')
 
-    @property
+    @functools.cached_property
     def rtfPlainInjectableHeader(self) -> bytes:
         """
         The header that can be formatted and injected into the encapsulated RTF
         body.
         """
         prefix = '{'
-        suffix = r'\par\par}'
-        joinStr = r'\line'
+        suffix = '\\par\\par}'
+        joinStr = '\\line'
         formatter = (lambda name, value : fr'{{\b {name}: \b0 {inputToString(rtfSanitizePlain(value), self.stringEncoding)}}}')
 
         return self.getInjectableHeader(prefix, joinStr, suffix, formatter).encode('utf-8')
 
-    @property
+    @functools.cached_property
     def sender(self) -> Optional[str]:
         """
         Returns the message sender, if it exists.
         """
-        try:
-            return self._sender
-        except AttributeError:
-            # Check header first
-            if self.headerInit():
-                headerResult = self.header['from']
-                if headerResult is not None:
-                    self._sender = decodeRfc2047(headerResult)
-                    return headerResult
-                logger.info('Header found, but "sender" is not included. Will be generated from other streams.')
-            # Extract from other fields
-            text = self._getStringStream('__substg1.0_0C1A')
-            email = self._getStringStream('__substg1.0_5D01')
-            # Will not give an email address sometimes. Seems to exclude the email address if YOU are the sender.
-            result = None
-            if text is None:
-                result = email
-            else:
-                result = text
-                if email is not None:
-                    result += ' <' + email + '>'
+        # Check header first
+        if self.headerInit():
+            headerResult = self.header['from']
+            if headerResult is not None:
+                return decodeRfc2047(headerResult)
+            logger.info('Header found, but "sender" is not included. Will be generated from other streams.')
+        # Extract from other fields
+        text = self._getStringStream('__substg1.0_0C1A')
+        email = self._getStringStream('__substg1.0_5D01')
+        # Will not give an email address sometimes. Seems to exclude the email
+        # address if YOU are the sender.
+        result = None
+        if text is None:
+            result = email
+        else:
+            result = text
+            if email is not None:
+                result += ' <' + email + '>'
 
-            self._sender = result
-            return result
+        return result
 
-    @property
+    @functools.cached_property
     def subject(self) -> Optional[str]:
         """
         Returns the message subject, if it exists.
         """
-        return self._ensureSet('_subject', '__substg1.0_0037')
+        return self._getStringStream('__substg1.0_0037')
 
-    @property
+    @functools.cached_property
     def to(self) -> Optional[str]:
         """
         Returns the to field, if it exists.
         """
         return self._genRecipient('to', RecipientType.TO)
```

### Comparing `extract_msg-0.41.5/extract_msg/message_signed_base.py` & `extract_msg-0.42.0/extract_msg/properties/properties_store.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,189 +1,228 @@
 __all__ = [
-    'MessageSignedBase',
+    'PropertiesStore',
 ]
 
 
-import html
+import copy
+import datetime
 import logging
-import re
+import pprint
 
-from typing import List, Optional
+from typing import Any, Dict, Optional, Union
+from warnings import warn
 
-from .enums import ErrorBehavior
-from .exceptions import StandardViolationError
-from .message_base import MessageBase
-from .signed_attachment import SignedAttachment
-from .utils import inputToBytes, inputToString, unwrapMultipart
+from .. import constants
+from ..enums import Intelligence, PropertiesType
+from .prop import createProp, PropBase
+from ..utils import divide, properHex
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
-class MessageSignedBase(MessageBase):
+class PropertiesStore:
     """
-    Base class for Message like msg files.
+    Parser for msg properties files.
     """
 
-    def __init__(self, path, **kwargs):
-        """
-        :param path: path to the msg file in the system or is the raw msg file.
-        :param prefix: used for extracting embeded msg files
-            inside the main one. Do not set manually unless
-            you know what you are doing.
-        :param attachmentClass: optional, the class the Message object
-            will use for attachments. You probably should
-            not change this value unless you know what you
-            are doing.
-        :param signedAttachmentClass: optional, the class the object will use
-            for signed attachments.
-        :param filename: optional, the filename to be used by default when
-            saving.
-        :param delayAttachments: optional, delays the initialization of
-            attachments until the user attempts to retrieve them. Allows MSG
-            files with bad attachments to be initialized so the other data can
-            be retrieved.
-        :param overrideEncoding: optional, an encoding to use instead of the one
-            specified by the msg file. Do not report encoding errors caused by
-            this.
-        :param attachmentErrorBehavior: Optional, the behavior to use in the
-            event of an error when parsing the attachments.
-        :param recipientSeparator: Optional, Separator string to use between
-            recipients.
-        """
-        self.__recipientSeparator = kwargs.get('recipientSeparator', ';')
-        self.__signedAttachmentClass = kwargs.get('signedAttachmentClass', SignedAttachment)
-        super().__init__(path, **kwargs)
-        # Initialize properties in the order that is least likely to cause bugs.
-        # TODO have each function check for initialization of needed data so these
-        # lines will be unnecessary.
-        if not kwargs.get('delayAttachments', False):
-            self.attachments
+    def __init__(self, data : Optional[bytes], _type : Optional[PropertiesType] = None, skip : Optional[int] = None):
+        if not data:
+            # If data comes back false, make sure is is empty bytes.
+            data = b''
+        if not isinstance(data, bytes):
+            raise TypeError(':param data: MUST be bytes.')
+        self.__rawData = data
+        self.__len = len(data)
+        self.__props : Dict[PropBase] = {}
+        self.__naid = None
+        self.__nrid = None
+        self.__ac = None
+        self.__rc = None
+        # Handle an empty properties stream.
+        if self.__len == 0:
+            self.__intel = Intelligence.ERROR
+            skip = 0
+        elif _type is not None:
+                _type = PropertiesType(_type)
+                self.__intel = Intelligence.SMART
+                if _type == PropertiesType.MESSAGE:
+                    skip = 32
+                    self.__nrid, self.__naid, self.__rc, self.__ac = constants.st.ST1.unpack(self.__rawData[:24])
+                elif _type == PropertiesType.MESSAGE_EMBED:
+                    skip = 24
+                    self.__nrid, self.__naid, self.__rc, self.__ac = constants.st.ST1.unpack(self.__rawData[:24])
+                else:
+                    skip = 8
+        else:
+            self.__intel = Intelligence.DUMB
+            if skip is None:
+                # This section of the skip handling is not very good. While it
+                # does work, it is likely to create extra properties that are
+                # created from the properties file's header data. While that
+                # won't actually mess anything up, it is far from ideal.
+                # Basically, this is the dumb skip length calculation.
+                # Preferably, we want the type to have been specified so all of
+                # the additional fields will have been filled out.
+                #
+                # If the skip would end up at 0, set it to 32.
+                skip = (self.__len % 16) or 32
+        streams = divide(self.__rawData[skip:], 16)
+        for st in streams:
+            if len(st) == 16:
+                prop = createProp(st)
+                self.__props[prop.name] = prop
+            else:
+                logger.warning(f'Found stream from divide that was not 16 bytes: {st}. Ignoring.')
+        self.__pl = len(self.__props)
 
-    @property
-    def attachments(self) -> List:
+    def __contains__(self, key) -> bool:
+        return self.__props.__contains__(key)
+
+    def __getitem__(self, key) -> PropBase:
+        return self.__props.__getitem__(key)
+
+    def __iter__(self):
+        return self.__props.__iter__()
+
+    def __len__(self) -> int:
+        """
+        Returns the number of properties.
         """
-        Returns a list of all attachments.
+        return self.__pl
+
+    def __repr__(self) -> str:
+        return self.__props.__repr__()
 
-        :raises StandardViolationError: The standard for signed messages was
-            blatantly violated.
+    def get(self, name, default = None) -> Optional[Union[PropBase, Any]]:
+        """
+        Retrieve the property of :param name:. Returns the value of
+        :param default: if the property could not be found.
         """
         try:
-            return self._sAttachments
-        except AttributeError:
-            atts = super().attachments
+            return self.__props[name]
+        except KeyError:
+            # DEBUG
+            logger.debug('KeyError exception.')
+            logger.debug(properHex(self.__rawData))
+            logger.debug(self.__props)
+            return default
 
-            if len(atts) != 1:
-                if self.errorBehavior & ErrorBehavior.STANDARDS_VIOLATION:
-                    if len(atts) == 0:
-                        logger.error('Signed message has no attachments, a violation of the standard.')
-                        self._sAttachments = None
-                        self._signedBody = None
-                        self._signedHtmlBody = None
-                        return
-                    # If there is at least one attachment, just try to use the
-                    # first.
-                else:
-                    raise StandardViolationError('Signed messages without exactly 1 (regular) attachment constitue a violation of the standard.')
+    def has_key(self, key) -> bool:
+        """
+        Checks if :param key: is a key in the properties dictionary.
+        """
+        warn('`Properties.has_key` is deprecated. Use the `in` keyword instead.', DeprecationWarning)
+        return key in self.__props
+
+    def items(self):
+        return self.__props.items()
+
+    def keys(self):
+        return self.__props.keys()
 
-            # We need to unwrap the multipart stream.
-            unwrapped = unwrapMultipart(atts[0].data)
+    def pprintKeys(self) -> None:
+        """
+        Uses the pprint function on a sorted list of keys.
+        """
+        pprint.pprint(sorted(tuple(self.__props.keys())))
 
-            # Now store everything where it needs to be and make the
-            # attachments.
-            self._sAttachments = [self.__signedAttachmentClass(self, **att) for att in unwrapped['attachments']]
-            self._signedBody = unwrapped['plain_body']
-            self._signedHtmlBody = inputToBytes(unwrapped['html_body'], 'utf-8')
+    def values(self):
+        return self.__props.values()
 
-            return self._sAttachments
+    items.__doc__ = dict.items.__doc__
+    keys.__doc__ = dict.keys.__doc__
+    values.__doc__ = dict.values.__doc__
 
     @property
-    def body(self) -> Optional[str]:
+    def attachmentCount(self) -> int:
         """
-        Returns the message body, if it exists.
+        The number of Attachment objects for the MSGFile object.
+
+        :raises TypeError: The Properties instance is not for an MSGFile object.
         """
-        try:
-            return self._body
-        except AttributeError:
-            if self._ensureSet('_body', '__substg1.0_1000'):
-                pass
-            elif self.signedBody:
-                self._body = self.signedBody
-            else:
-                # If the body doesn't exist, see if we can get it from the RTF
-                # body.
-                if self.deencapsulatedRtf and self.deencapsulatedRtf.content_type == 'text':
-                    self._body = self.deencapsulatedRtf.text
-
-            if self._body:
-                self._body = inputToString(self._body, 'utf-8')
-                a = re.search('\n', self._body)
-                if a is not None:
-                    if re.search('\r\n', self._body) is not None:
-                        self.__crlf = '\r\n'
-            return self._body
+        if self.__ac is None:
+            raise TypeError('Properties instance must be intelligent and of type MESSAGE to get attachment count.')
+        return self.__ac
 
     @property
-    def htmlBody(self) -> Optional[bytes]:
+    def date(self) -> Optional[datetime.datetime]:
         """
-        Returns the html body, if it exists.
+        Returns the send date contained in the Properties file.
         """
         try:
-            return self._htmlBody
+            return self.__date
         except AttributeError:
-            if self._ensureSet('_htmlBody', '__substg1.0_10130102', False):
-                # Reducing line repetition.
-                pass
-            elif self.signedHtmlBody:
-                self._htmlBody = self.signedHtmlBody
-            elif self.rtfBody:
-                logger.info('HTML body was not found, attempting to generate from RTF.')
-                if self.deencapsulatedRtf and self.deencapsulatedRtf.content_type == 'html':
-                    self._htmlBody = self.deencapsulatedRtf.html.encode('utf-8')
-                else:
-                    logger.info('Could not deencapsulate HTML from RTF body.')
-            elif self.body:
-                # Convert the plain text body to html.
-                logger.info('HTML body was not found, attempting to generate from plain text body.')
-                correctedBody = html.escpae(self.body).replace('\r', '').replace('\n', '<br />')
-                self._htmlBody = f'<html><body>{correctedBody}</body></head>'.encode('utf-8')
-            else:
-                logger.info('HTML body could not be found nor generated.')
+            self.__date = None
+            if '00390040' in self:
+                dateValue = self.get('00390040').value
+                # A date can by bytes if it fails to initialize, so we check it
+                # first.
+                if isinstance(dateValue, datetime.datetime):
+                    self.__date = dateValue.__format__('%a, %d %b %Y %H:%M:%S %z')
+            return self.__date
 
-            return self._htmlBody
+    @property
+    def intelligence(self) -> Intelligence:
+        """
+        Returns the inteligence level of the Properties instance.
+        """
+        return self.__intel
 
     @property
-    def _rawAttachments(self) -> List:
+    def nextAttachmentId(self) -> int:
         """
-        A property to allow access to the non-signed attachments.
+        The ID to use for naming the next Attachment object storage if one is
+        created inside the .msg file.
+
+        :raises TypeError: The Properties instance is not for an MSGFile object.
         """
-        return super().attachments
+        if self.__naid is None:
+            raise TypeError('Properties instance must be intelligent and of type MESSAGE to get next attachment id.')
+        return self.__naid
 
     @property
-    def signedAttachmentClass(self):
+    def nextRecipientId(self) -> int:
         """
-        The attachment class used for signed attachments.
+        The ID to use for naming the next Recipient object storage if one is
+        created inside the .msg file.
+
+        :raises TypeError: The Properties instance is not for an MSGFile object.
         """
-        return self.__signedAttachmentClass
+        if self.__nrid is None:
+            raise TypeError('Properties instance must be intelligent and of type MESSAGE to get next recipient id.')
+        return self.__nrid
 
     @property
-    def signedBody(self) -> Optional[str]:
+    def props(self) -> Dict:
         """
-        Returns the body from the signed message if it exists.
+        Returns a copy of the internal properties dict.
         """
-        try:
-            return self._signedBody
-        except AttributeError:
-            self.attachments
-            return self._signedBody
+        return copy.deepcopy(self.__props)
 
     @property
-    def signedHtmlBody(self) -> Optional[bytes]:
+    def _propDict(self) -> Dict:
         """
-        Returns the HTML body from the signed message if it exists.
+        A direct reference to the underlying property dictionary. Used in one
+        place in the code, and not recommended to be used if you are not a
+        developer. Use `Properties.props` instead for a safe reference.
         """
-        try:
-            return self._signedHtmlBody
-        except AttributeError:
-            self.attachments
-            return self._signedHtmlBody
+        return self.__props
+
+    @property
+    def rawData(self) -> bytes:
+        """
+        The raw bytes used to create this object.
+        """
+        return self.__rawData
+
+    @property
+    def recipientCount(self) -> int:
+        """
+        The number of Recipient objects for the MSGFile object.
+
+        :raises TypeError: The Properties instance is not for an MSGFile object.
+        """
+        if self.__rc is None:
+            raise TypeError('Properties instance must be intelligent and of type MESSAGE to get recipient count.')
+        return self.__rc
```

### Comparing `extract_msg-0.41.5/extract_msg/msg.py` & `extract_msg-0.42.0/extract_msg/msg_classes/msg.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,49 @@
+from __future__ import annotations
+
+
 __all__ = [
     'MSGFile',
 ]
 
 
 import codecs
 import copy
 import datetime
+import functools
 import io
 import logging
 import os
 import pathlib
+import weakref
 import zipfile
 
 import olefile
 
-from typing import List, Optional, Set, Tuple, Union
+from typing import Any, Callable, cast, List, Optional, Set, Tuple, Union
 
-from . import constants
-from .attachment import Attachment, BrokenAttachment, UnsupportedAttachment
-from .enums import (
-        AttachErrorBehavior, ErrorBehavior, Importance, Priority,
-        PropertiesType, Sensitivity, SideEffect
+from .. import constants
+from ..attachments import (
+        AttachmentBase, initStandardAttachment, SignedAttachment
+    )
+from ..encoding import lookupCodePage
+from ..enums import (
+        AttachErrorBehavior, ErrorBehavior, InsecureFeatures, Importance,
+        Priority, PropertiesType, SaveType, Sensitivity, SideEffect
     )
-from .exceptions import (
-        InvalidFileFormatError, StandardViolationError, UnrecognizedMSGTypeError
+from ..exceptions import (
+        ConversionError, InvalidFileFormatError, PrefixError,
+        StandardViolationError
     )
-from .named import Named, NamedProperties
-from .prop import FixedLengthProp
-from .properties import Properties
-from .utils import  (
-        divide, getEncodingName, hasLen, inputToMsgPath, inputToString,
-        msgPathToString, parseType, properHex, verifyPropertyId, verifyType,
-        windowsUnicode
+from ..properties.named import Named, NamedProperties
+from ..properties.prop import FixedLengthProp
+from ..properties.properties_store import PropertiesStore
+from ..utils import  (
+        divide, hasLen, inputToMsgPath, makeWeakRef, msgPathToString,
+        parseType, properHex, verifyPropertyId, verifyType, windowsUnicode
     )
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
@@ -47,265 +55,187 @@
     def __init__(self, path, **kwargs):
         """
         :param path: path to the msg file in the system or is the raw msg file.
         :param prefix: Used for extracting embedded msg files inside the main
             one. Do not set manually unless you know what you are doing.
         :param parentMsg: Used for synchronizing named properties instances. Do
             not set this unless you know what you are doing.
-        :param attachmentClass: Optional, the class the MSGFile object will use
-            for attachments. You probably should not change this value unless
-            you know what you are doing.
+        :param initAttachment: Optional, the method used when creating an
+            attachment for an MSG file. MUST be a function that takes 2
+            arguments (the MSGFile instance and the directory in the MSG file
+            where the attachment is) and returns an instance of AttachmentBase.
         :param delayAttachments: Optional, delays the initialization of
             attachments until the user attempts to retrieve them. Allows MSG
             files with bad attachments to be initialized so the other data can
             be retrieved.
         :param filename: Optional, the filename to be used by default when
             saving.
-        :param errorBehavior: Optional, the behavior to use in the event of an
-            certain types of errors.
+        :param errorBehavior: Optional, the behavior to use in the event of
+            certain types of errors. Uses the ErrorBehavior enum.
         :param overrideEncoding: Optional, an encoding to use instead of the one
             specified by the msg file. Do not report encoding errors caused by
             this.
         :param treePath: Internal variable used for giving representation of the
             path, as a tuple of objects, of the MSGFile. When passing, this is
             the path to the parent object of this instance.
+        :param insecureFeatures: Optional, an enum value that specifies if
+            certain insecure features should be enabled. These features should
+            only be used on data that you trust. Uses the InsecureFeatures enum.
 
         :raises InvalidFileFormatError: If the file is not an OleFile or could
             not be parsed as an MSG file.
-        :raises StandardViolationError: If some part of the file badly violates 
+        :raises StandardViolationError: If some part of the file badly violates
             the standard.
         :raises IOError: If there is an issue opening the MSG file.
         :raises NameError: If the encoding provided is not supported.
-        :raises TypeError: If the prefix is not a supported type.
+        :raises PrefixError: If the prefix is not a supported type.
         :raises TypeError: If the parent is not an instance of MSGFile or a
             subclass.
         :raises ValueError: If the attachment error behavior is not valid.
 
         It's recommended to check the error message to ensure you know why a
         specific exceptions was raised.
         """
         # Retrieve all the kwargs that we need.
+        self.__inscFeat = kwargs.get('insecureFeatures', InsecureFeatures.NONE)
         prefix = kwargs.get('prefix', '')
-        self.__parentMsg = kwargs.get('parentMsg')
-        self.__treePath = kwargs.get('treePath', tuple()) + (self,)
+        self.__parentMsg = makeWeakRef(cast(MSGFile, kwargs.get('parentMsg')))
+        self.__treePath = kwargs.get('treePath', []) + [makeWeakRef(self)]
         # Verify it is a valid class.
-        if self.__parentMsg is not None and not isinstance(self.__parentMsg, MSGFile):
+        if self.__parentMsg and not isinstance(self.__parentMsg(), MSGFile):
             raise TypeError(':param parentMsg: must be an instance of MSGFile or a subclass.')
         filename = kwargs.get('filename', None)
         overrideEncoding = kwargs.get('overrideEncoding', None)
 
         # WARNING DO NOT MANUALLY MODIFY PREFIX. Let the program set it.
         self.__path = path
-        self.__attachmentClass = kwargs.get('attachmentClass', Attachment)
+        self.__initAttachmentFunc = kwargs.get('initAttachment', initStandardAttachment)
         self.__attachmentsDelayed = kwargs.get('delayAttachments', False)
         self.__attachmentsReady = False
         self.__errorBehavior = ErrorBehavior(kwargs.get('errorBehavior', ErrorBehavior.THROW))
         if self.__errorBehavior is None:
             if 'attachmentErrorBehavior' in kwargs:
                 import warnings
                 warnings.warn(':param attachmentErrorsBehavior: is deprecated. Use :param ErrorBehavior: instead.', DeprecationWarning)
 
                 # Get the error behavior and call the old class to convert it if
                 # necessary.
                 self.__errorBehavior = AttachErrorBehavior(kwargs['attachmentErrorBehavior'])
 
-        self.__waitingProperties = []
         if overrideEncoding is not None:
             codecs.lookup(overrideEncoding)
             logger.warning('You have chosen to override the string encoding. Do not report encoding errors caused by this.')
             self.__stringEncoding = overrideEncoding
         self.__overrideEncoding = overrideEncoding
 
         self.__listDirRes = {}
 
-        # This is a variable that tells whether we own the olefile. Used for
-        # closing.
-        self.__oleOwner = True
         if self.__parentMsg:
             # We should be able to directly access the private variables of
             # another instance with no issue.
-            self.__ole = self.__parentMsg.__ole
+            self.__ole = self.__parentMsg().__ole
             self.__oleOwner = False
         else:
+            # Verify the path at least evaluates to True, as not doing so can
+            # allow an OleFile to be created without a path.
+            if not path:
+                raise ValueError(':param path: must be set and must not be empty.')
             try:
-                self.__ole = olefile.OleFileIO(path)
+                if ErrorBehavior.OLE_DEFECT_INCORRECT in self.errorBehavior:
+                    defect = olefile.DEFECT_FATAL
+                else:
+                    defect = olefile.DEFECT_INCORRECT
+                self.__ole = olefile.OleFileIO(path, raise_defects = defect)
             except OSError as e:
                 logger.error(e)
                 if str(e) == 'not an OLE2 structured storage file':
                     raise InvalidFileFormatError(e)
                 else:
                     raise
+            # This is a variable that tells whether we own the olefile. Used for
+            # closing. We set it here for error handling.
+            self.__oleOwner = True
+
+        # The rest *must* be in a try-except block to ensure we close the file.
+        try:
+            kwargsCopy = copy.copy(kwargs)
+            if 'prefix' in kwargsCopy:
+                del kwargsCopy['prefix']
+            if 'parentMsg' in kwargsCopy:
+                del kwargsCopy['parentMsg']
+            if 'filename' in kwargsCopy:
+                del kwargsCopy['filename']
+            if 'treePath' in kwargsCopy:
+                del kwargsCopy['treePath']
+            self.__kwargs = kwargsCopy
 
-        kwargsCopy = copy.copy(kwargs)
-        if 'prefix' in kwargsCopy:
-            del kwargsCopy['prefix']
-        if 'parentMsg' in kwargsCopy:
-            del kwargsCopy['parentMsg']
-        if 'filename' in kwargsCopy:
-            del kwargsCopy['filename']
-        if 'treePath' in kwargsCopy:
-            del kwargsCopy['treePath']
-        self.__kwargs = kwargsCopy
-
-        prefixl = []
-        if prefix:
-            try:
-                prefix = inputToString(prefix, 'utf-8')
-            except Exception:
+            prefixl = []
+            if prefix:
                 try:
-                    prefix = '/'.join(prefix)
-                except Exception:
-                    raise TypeError(f'Invalid prefix type: {type(prefix)}\n' +
-                                    '(This was probably caused by you setting it manually).')
-            prefix = prefix.replace('\\', '/')
-            g = prefix.split('/')
-            if g[-1] == '':
-                g.pop()
-            prefixl = g
-            if prefix[-1] != '/':
-                prefix += '/'
-        self.__prefix = prefix
-        self.__prefixList = prefixl
-        self.__prefixLen = len(prefixl)
-        if prefix and not filename:
-            filename = self._getStringStream(prefixl[:-1] + ['__substg1.0_3001'], prefix = False)
-        if filename:
-            self.filename = filename
-        elif hasLen(path):
-            if len(path) < 1536:
+                    prefixl = inputToMsgPath(prefix)
+                    prefix = '/'.join(prefixl) + '/'
+                except ConversionError:
+                    raise PrefixError(f'The provided prefix could not be used: {prefix}')
+            self.__prefix = prefix
+            self.__prefixList = prefixl
+            self.__prefixLen = len(prefixl)
+            if prefix and not filename:
+                filename = self._getStringStream(prefixl[:-1] + ['__substg1.0_3001'], prefix = False)
+            if filename:
+                self.filename = filename
+            elif hasLen(path):
+                if len(path) < 1536:
+                    self.filename = str(path)
+                else:
+                    self.filename = None
+            elif isinstance(path, pathlib.Path):
                 self.filename = str(path)
             else:
                 self.filename = None
-        elif isinstance(path, pathlib.Path):
-            self.filename = str(path)
-        else:
-            self.filename = None
 
-        self.__open = True
+            self.__open = True
 
-        # Now, load the attachments if we are not delaying them.
-        if not self.__attachmentsDelayed:
-            self.attachments
+            # Now, load the attachments if we are not delaying them.
+            if not self.__attachmentsDelayed:
+                self.attachments
+        except:
+            # *Any* exception here requires that we close the file.
+            try:
+                self.close()
+            except:
+                pass
+            # Raise the exception after trying to close the file.
+            raise
 
-    def __enter__(self):
+    def __enter__(self) -> MSGFile:
         self.__ole.__enter__()
         return self
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *_) -> None:
         self.close()
 
-    def _ensureSet(self, variable : str, streamID, stringStream : bool = True, **kwargs):
+    def _getNamedAs(self, propertyName : str, guid : str, overrideClass = None, preserveNone : bool = True):
         """
-        Ensures that the variable exists, otherwise will set it using the
-        specified stream. After that, return said variable.
-
-        If the specified stream is not a string stream, make sure to set
-        :param stringStream: to False.
+        Returns the named property, setting the class if specified.
 
         :param overrideClass: Class/function to use to morph the data that was
             read. The data will be the first argument to the class's __init__
             function or the function itself, if that is what is provided. By
             default, this will be completely ignored if the value was not found.
         :param preserveNone: If true (default), causes the function to ignore
             :param overrideClass: when the value could not be found (is None).
             If this is changed to False, then the value will be used regardless.
         """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            if stringStream:
-                value = self._getStringStream(streamID)
-            else:
-                value = self._getStream(streamID)
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
+        value = self.namedProperties.get((propertyName, guid))
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if value is not None or not preserveNone:
+                value = overrideClass(value)
 
-    def _ensureSetNamed(self, variable : str, propertyName : str, guid : str, **kwargs):
-        """
-        Ensures that the variable exists, otherwise will set it using the named
-        property. After that, return said variable.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            value = self.namedProperties.get((propertyName, guid))
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
-
-    def _ensureSetProperty(self, variable : str, propertyName, **kwargs):
-        """
-        Ensures that the variable exists, otherwise will set it using the
-        property. After that, return said variable.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            try:
-                value = self.props[propertyName].value
-            except (KeyError, AttributeError):
-                value = None
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
-
-    def _ensureSetTyped(self, variable : str, _id, **kwargs):
-        """
-        Like the other ensure set functions, but designed for when something
-        could be multiple types (where only one will be present). This way you
-        have no need to set the type, it will be handled for you.
-
-        :param overrideClass: Class/function to use to morph the data that was
-            read. The data will be the first argument to the class's __init__
-            function or the function itself, if that is what is provided. By
-            default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
-            :param overrideClass: when the value could not be found (is None).
-            If this is changed to False, then the value will be used regardless.
-        """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            value = self._getTypedData(_id)
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
+        return value
 
     def _getOleEntry(self, filename, prefix : bool = True) -> olefile.olefile.OleDirectoryEntry:
         """
         Finds the directory entry from the olefile for the stream or storage
         specified. Use '/' to get the root entry.
         """
         sid = -1
@@ -315,14 +245,37 @@
             else:
                 return self.__ole.direntries[0]
         else:
             sid = self.__ole._find(self.fixPath(filename, prefix))
 
         return self.__ole.direntries[sid]
 
+    def _getPropertyAs(self, propertyName, overrideClass = None, preserveNone : bool = True):
+        """
+        Returns the property, setting the class if specified.
+
+        :param overrideClass: Class/function to use to morph the data that was
+            read. The data will be the first argument to the class's __init__
+            function or the function itself, if that is what is provided. By
+            default, this will be completely ignored if the value was not found.
+        :param preserveNone: If True (default), causes the function to ignore
+            :param overrideClass: when the value could not be found (is None).
+            If this is changed to False, then the value will be used regardless.
+        """
+        try:
+            value = self.props[propertyName].value
+        except (KeyError, AttributeError):
+            value = None
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if (value is not None or not preserveNone):
+                value = overrideClass(value)
+
+        return value
+
     def _getStream(self, filename, prefix : bool = True) -> Optional[bytes]:
         """
         Gets a binary representation of the requested filename.
 
         This should ALWAYS return a bytes object if it was found, otherwise
         returns None.
         """
@@ -330,14 +283,41 @@
         if self.exists(filename, False):
             with self.__ole.openstream(filename) as stream:
                 return stream.read() or b''
         else:
             logger.info(f'Stream "{filename}" was requested but could not be found. Returning `None`.')
             return None
 
+    def _getStreamAs(self, streamID, stringStream : bool = True, overrideClass = None, preserveNone : bool = True):
+        """
+        Returns the specified stream, modifying it to the class if specified.
+
+        If the specified stream is not a string stream, make sure to set
+        :param stringStream: to False.
+
+        :param overrideClass: Class/function to use to morph the data that was
+            read. The data will be the first argument to the class's __init__
+            function or the function itself, if that is what is provided. By
+            default, this will be completely ignored if the value was not found.
+        :param preserveNone: If true (default), causes the function to ignore
+            :param overrideClass: when the value could not be found (is None).
+            If this is changed to False, then the value will be used regardless.
+        """
+        if stringStream:
+            value = self._getStringStream(streamID)
+        else:
+            value = self._getStream(streamID)
+
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if value is not None or not preserveNone:
+                value = overrideClass(value)
+
+        return value
+
     def _getStringStream(self, filename, prefix : bool = True) -> Optional[str]:
         """
         Gets a string representation of the requested filename.
 
         Rather than the full filename, you should only feed this function the
         filename sans the type. So if the full name is "__substg1.0_001A001F",
         the filename this function should receive should be "__substg1.0_001A".
@@ -348,14 +328,36 @@
         filename = self.fixPath(filename, prefix)
         if self.areStringsUnicode:
             return windowsUnicode(self._getStream(filename + '001F', prefix = False))
         else:
             tmp = self._getStream(filename + '001E', prefix = False)
             return None if tmp is None else tmp.decode(self.stringEncoding)
 
+    def _getTypedAs(self, _id : str, overrideClass = None, preserveNone : bool = True):
+        """
+        Like the other get as functions, but designed for when something
+        could be multiple types (where only one will be present). This way you
+        have no need to set the type, it will be handled for you.
+
+        :param overrideClass: Class/function to use to morph the data that was
+            read. The data will be the first argument to the class's __init__
+            function or the function itself, if that is what is provided. By
+            default, this will be completely ignored if the value was not found.
+        :param preserveNone: If true (default), causes the function to ignore
+            :param overrideClass: when the value could not be found (is None).
+            If this is changed to False, then the value will be used regardless.
+        """
+        value = self._getTypedData(_id)
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if value is not None or not preserveNone:
+                value = overrideClass(value)
+
+        return value
+
     def _getTypedData(self, _id : str, _type = None, prefix : bool = True):
         """
         Gets the data for the specified id as the type that it is supposed to
         be. :param id: MUST be a 4 digit hexadecimal string.
 
         If you know for sure what type the data is before hand, you can specify
         it as being one of the strings in the constant FIXED_LENGTH_PROPS_STRING
@@ -366,15 +368,15 @@
         found, result = self._getTypedStream('__substg1.0_' + _id, prefix, _type)
         if found:
             return result
         else:
             found, result = self._getTypedProperty(_id, _type)
             return result if found else None
 
-    def _getTypedProperty(self, propertyID : str, _type = None):
+    def _getTypedProperty(self, propertyID : str, _type = None) -> Tuple[bool, Optional[object]]:
         """
         Gets the property with the specified id as the type that it is supposed
         to be. :param id: MUST be a 4 digit hexadecimal string.
 
         If you know for sure what type the property is before hand, you can
         specify it as being one of the strings in the constant
         FIXED_LENGTH_PROPS_STRING or VARIABLE_LENGTH_PROPS_STRING.
@@ -450,22 +452,19 @@
         Returns a list of the streams and or storages depending on the arguments
         given.
         """
         return self.__ole.listdir(streams, storages)
 
     def close(self) -> None:
         if self.__open:
-            try:
-                # If this throws an AttributeError then we have not loaded the attachments.
-                self._attachments
+            if self.attachmentsReady:
                 for attachment in self.attachments:
                     if attachment.type == 'msg':
                         attachment.data.close()
-            except AttributeError:
-                pass
+
             if self.__oleOwner:
                 self.__ole.close()
 
             self.__open = False
 
     def debug(self) -> None:
         for dir_ in self.listDir():
@@ -530,15 +529,15 @@
         the path given. If this is an embedded MSG file, the embedded streams
         and directories will be added to it as if they were at the root,
         allowing you to save it as it's own MSG file.
 
         :param path: An IO device with a write method which accepts bytes or a
             path-like object (including strings and pathlib.Path objects).
         """
-        from .ole_writer import OleWriter
+        from ..ole_writer import OleWriter
 
         # Create an instance of the class used for writing a new OLE file.
         writer = OleWriter()
         # Add all file and directory entries to it. If this
         writer.fromMsg(self)
         writer.write(path)
 
@@ -590,15 +589,18 @@
     def slistDir(self, streams : bool = True, storages : bool = False) -> List[str]:
         """
         Replacement for OleFileIO.listdir that runs at the current prefix
         directory. Returns a list of strings instead of lists.
         """
         return [msgPathToString(x) for x in self.listDir(streams, storages)]
 
-    def save(self, *args, **kwargs):
+    def save(self, **kwargs) -> constants.SAVE_TYPE:
+        if kwargs.get('skipNotImplemented', False):
+            return (SaveType.NONE, None)
+
         raise NotImplementedError(f'Saving is not yet supported for the {self.__class__.__name__} class.')
 
     def saveAttachments(self, **kwargs) -> None:
         """
         Saves only attachments in the same folder.
 
         :params skipHidden: If True, skips attachments marked as hidden.
@@ -637,80 +639,44 @@
                     data = self._getStream(dir_)
                     # Specifically check for None. If this is bytes we still want to do this line.
                     # There was actually this weird issue where for some reason data would be bytes
                     # but then also simultaneously register as None?
                     if data is not None:
                         f.write(data)
 
-    @property
+    @functools.cached_property
     def areStringsUnicode(self) -> bool:
         """
         Returns a boolean telling if the strings are unicode encoded.
         """
-        try:
-            return self.__bStringsUnicode
-        except AttributeError:
-            if '340D0003' in self.props:
-                if (self.props['340D0003'].value & 0x40000) != 0:
-                    self.__bStringsUnicode = True
-                    return self.__bStringsUnicode
-            self.__bStringsUnicode = False
-            return self.__bStringsUnicode
+        if '340D0003' in self.props:
+            if (self.props['340D0003'].value & 0x40000) != 0:
+                return True
 
-    @property
-    def attachments(self) -> List:
+        return False
+
+    @functools.cached_property
+    def attachments(self) -> Union[List[AttachmentBase], List[SignedAttachment]]:
         """
         Returns a list of all attachments.
         """
-        try:
-            return self._attachments
-        except AttributeError:
-            # Get the attachments.
-            attachmentDirs = []
-            prefixLen = self.prefixLen
-            for dir_ in self.listDir(False, True):
-                if dir_[prefixLen].startswith('__attach') and \
-                        dir_[prefixLen] not in attachmentDirs:
-                    attachmentDirs.append(dir_[prefixLen])
+        # Get the attachments.
+        attachmentDirs = []
+        for dir_ in self.listDir(False, True, False):
+            if dir_[0].startswith('__attach') and dir_[0] not in attachmentDirs:
+                attachmentDirs.append(dir_[0])
 
-            self._attachments = []
+        attachments = []
 
-            for attachmentDir in attachmentDirs:
-                try:
-                    self._attachments.append(self.attachmentClass(self, attachmentDir))
-                except (NotImplementedError, UnrecognizedMSGTypeError) as e:
-                    if self.errorBehavior & ErrorBehavior.ATTACH_NOT_IMPLEMENTED:
-                        logger.exception(f'Error processing attachment at {attachmentDir}')
-                        self._attachments.append(UnsupportedAttachment(self, attachmentDir))
-                    else:
-                        raise
-                except StandardViolationError as e:
-                    if self.errorBehavior & ErrorBehavior.STANDARDS_VIOLATION:
-                        logger.exception(f'Unresolvable standards violation in  {attachmentDir}')
-                        self._attachments.append(BrokenAttachment(self, attachmentDir))
-                    else:
-                        raise
-                except Exception as e:
-                    if self.errorBehavior & ErrorBehavior.ATTACH_BROKEN:
-                        logger.exception(f'Error processing attachment at {attachmentDir}')
-                        self._attachments.append(BrokenAttachment(self, attachmentDir))
-                    else:
-                        raise
+        for attachmentDir in attachmentDirs:
+            attachments.append(self.initAttachmentFunc(self, attachmentDir))
 
-            self.__attachmentsReady = True
+        self.__attachmentsReady = True
 
-            return self._attachments
-
-    @property
-    def attachmentClass(self):
-        """
-        Returns the Attachment class being used, should you need to use it
-        externally for whatever reason.
-        """
-        return self.__attachmentClass
+        return attachments
 
     @property
     def attachmentsDelayed(self) -> bool:
         """
         Returns True if the attachment initialization was delayed.
         """
         return self.__attachmentsDelayed
@@ -718,127 +684,136 @@
     @property
     def attachmentsReady(self) -> bool:
         """
         Returns True if the attachments are ready to be used.
         """
         return self.__attachmentsReady
 
-    @property
+    @functools.cached_property
     def classified(self) -> bool:
         """
         Indicates whether the contents of this message are regarded as
         classified information.
         """
-        return self._ensureSetNamed('_classified', '85B5', constants.PSETID_COMMON, overrideClass = bool, preserveNone = False)
+        return self._getNamedAs('85B5', constants.ps.PSETID_COMMON, overrideClass = bool, preserveNone = False)
 
-    @property
+    @functools.cached_property
     def classType(self) -> Optional[str]:
         """
         The class type of the MSG file.
         """
-        return self._ensureSet('_classType', '__substg1.0_001A')
+        return self._getStringStream('__substg1.0_001A')
 
-    @property
+    @functools.cached_property
     def commonEnd(self) -> Optional[datetime.datetime]:
         """
         The end time for the object.
         """
-        return self._ensureSetNamed('_commonEnd', '8517', constants.PSETID_COMMON)
+        return self._getNamedAs('8517', constants.ps.PSETID_COMMON)
 
-    @property
+    @functools.cached_property
     def commonStart(self) -> Optional[datetime.datetime]:
         """
         The start time for the object.
         """
-        return self._ensureSetNamed('_commonStart', '8516', constants.PSETID_COMMON)
+        return self._getNamedAs('8516', constants.ps.PSETID_COMMON)
 
-    @property
+    @functools.cached_property
     def currentVersion(self) -> Optional[int]:
         """
         Specifies the build number of the client application that sent the
         message.
         """
-        return self._ensureSetNamed('_currentVersion', '8552', constants.PSETID_COMMON)
+        return self._getNamedAs('8552', constants.ps.PSETID_COMMON)
 
-    @property
+    @functools.cached_property
     def currentVersionName(self) -> Optional[str]:
         """
         Specifies the name of the client application that sent the message.
         """
-        return self._ensureSetNamed('_currentVersionName', '8554', constants.PSETID_COMMON)
-    
+        return self._getNamedAs('8554', constants.ps.PSETID_COMMON)
+
     @property
     def errorBehavior(self) -> ErrorBehavior:
         """
-        The behavior to follow when an attachment raises an exception. Will be
-        a member of the ErrorBehavior enum.
+        The behavior to follow when certain errors occur. Will be an instance of
+        the ErrorBehavior enum.
         """
         return self.__errorBehavior
 
-    @property
+    @functools.cached_property
     def importance(self) -> Optional[Importance]:
         """
         The specified importance of the msg file.
         """
-        return self._ensureSetProperty('_importance', '00170003', overrideClass = Importance)
+        return self._getPropertyAs('00170003', Importance)
 
     @property
     def importanceString(self) -> Union[str, None]:
         """
         Returns the string to use for saving. If the importance is medium then
         it returns None. Mainly used for saving.
         """
         return {
             Importance.HIGH: 'High',
             Importance.MEDIUM: None,
-            Importance.LOW: 'low',
+            Importance.LOW: 'Low',
             None: None,
         }[self.importance]
 
     @property
+    def initAttachmentFunc(self) -> Callable[[MSGFile, Any], AttachmentBase]:
+        """
+        Returns the method for initializing attachments being used, should you
+        need to use it externally for whatever reason.
+        """
+        return self.__initAttachmentFunc
+
+    @property
+    def insecureFeatures(self) -> InsecureFeatures:
+        """
+        An enum specifying what insecure features have been enabled for this
+        file.
+        """
+        return self.__inscFeat
+
+    @property
     def kwargs(self) -> dict:
         """
         The kwargs used to initialize this message, excluding the prefix. This
         is used for initializing embedded msg files.
         """
         return self.__kwargs
 
-    @property
+    @functools.cached_property
     def named(self) -> Named:
         """
         The main named properties storage. This is not usable to access the data
         of the properties directly.
+
+        :raises ReferenceError: The parent MSGFile instance has been garbage
+            collected.
         """
-        try:
-            return self.__named
-        except AttributeError:
-            self.__named = None
-            # Handle the parent msg file existing.
-            if self.__parentMsg:
-                # Try to get the named properties and use that for our main
-                # instance.
-                try:
-                    self.__named = self.__parentMsg.named
-                except Exception:
-                    pass
-            if not self.__named:
-                self.__named = Named(self)
-            return self.__named
+        # Handle the parent msg file existing.
+        if self.__parentMsg:
+            # Try to get the named properties and use that for our main
+            # instance.
+            if (msg := self.__parentMsg()) is None:
+                raise ReferenceError('Parent MSGFile instance has been garbage collected.')
+            return msg.named
+        else:
+            return Named(self)
 
-    @property
+    @functools.cached_property
     def namedProperties(self) -> NamedProperties:
         """
         The NamedProperties instances usable to access the data for named
         properties.
         """
-        try:
-            return self.__namedProperties
-        except AttributeError:
-            self.__namedProperties = NamedProperties(self.named, self)
-            return self.__namedProperties
+        return NamedProperties(self.named, self)
 
     @property
     def overrideEncoding(self):
         """
         Returns None is the encoding has not been overriden, otherwise returns
         the encoding.
         """
@@ -863,61 +838,57 @@
     def prefixLen(self) -> int:
         """
         Returns the number of elements in the prefix.
         """
         return self.__prefixLen
 
     @property
-    def prefixList(self):
+    def prefixList(self) -> List[str]:
         """
         Returns the prefix list of the Message instance. Intended for developer
         use.
         """
         return copy.deepcopy(self.__prefixList)
 
-    @property
+    @functools.cached_property
     def priority(self) -> Optional[Priority]:
         """
         The specified priority of the msg file.
         """
-        return self._ensureSetProperty('_priority', '00260003', overrideClass = Priority)
+        return self._getPropertyAs('00260003', Priority)
 
-    @property
-    def props(self) -> Properties:
+    @functools.cached_property
+    def props(self) -> PropertiesStore:
         """
         Returns the Properties instance used by the MSGFile instance.
         """
-        try:
-            return self._prop
-        except AttributeError:
-            if not (stream := self._getStream('__properties_version1.0')):
-                if self.__errorBehavior & ErrorBehavior.STANDARDS_VIOLATION:
-                    logger.error('File does not contain a property stream.')
-                else:
-                    # Raise the exception from None so we don't get all the "during
-                    # the handling of the above exception" stuff.
-                    raise StandardViolationError('File does not contain a property stream.') from None
-            self._prop = Properties(stream,
-                                    PropertiesType.MESSAGE if self.prefix == '' else PropertiesType.MESSAGE_EMBED)
-            return self._prop
+        if not (stream := self._getStream('__properties_version1.0')):
+            if ErrorBehavior.STANDARDS_VIOLATION in self.__errorBehavior:
+                logger.error('File does not contain a property stream.')
+            else:
+                # Raise the exception from None so we don't get all the "during
+                # the handling of the above exception" stuff.
+                raise StandardViolationError('File does not contain a property stream.') from None
+        return PropertiesStore(stream,
+                               PropertiesType.MESSAGE if self.prefix == '' else PropertiesType.MESSAGE_EMBED)
 
-    @property
+    @functools.cached_property
     def sensitivity(self) -> Optional[Sensitivity]:
         """
         The specified sensitivity of the msg file.
         """
-        return self._ensureSetProperty('_sensitivity', '00360003', overrideClass = Sensitivity)
+        return self._getPropertyAs('00360003', Sensitivity)
 
-    @property
-    def sideEffects(self) -> Optional[Set[SideEffect]]:
+    @functools.cached_property
+    def sideEffects(self) -> Optional[SideEffect]:
         """
         Controls how a Message object is handled by the client in relation to
         certain user interface actions by the user, such as deleting a message.
         """
-        return self._ensureSetNamed('_sideEffects', '8510', constants.PSETID_COMMON, overrideClass = SideEffect.fromBits)
+        return self._getNamedAs('8510', constants.ps.PSETID_COMMON, SideEffect)
 
     @property
     def stringEncoding(self):
         try:
             return self.__stringEncoding
         except AttributeError:
             # We need to calculate the encoding.
@@ -931,17 +902,19 @@
                     # If this property is not set by the client, we SHOULD set
                     # it to ISO-8859-15, but MAY set it to ISO-8859-1.
                     logger.warning('Encoding property not found. Defaulting to ISO-8859-15.')
                     self.__stringEncoding = 'iso-8859-15'
                 else:
                     enc = self.props['3FFD0003'].value
                     # Now we just need to translate that value.
-                    self.__stringEncoding = getEncodingName(enc)
+                    self.__stringEncoding = lookupCodePage(enc)
                 return self.__stringEncoding
 
     @property
-    def treePath(self) -> Tuple:
+    def treePath(self) -> List[weakref.ReferenceType]:
         """
-        A path, as a tuple of instances, needed to get to this instance through
-        the MSGFile-Attachment tree.
+        A path, as a list of weak reference to the instances needed to get to
+        this instance through the MSGFile-Attachment tree. These are weak
+        references to ensure the garbage collector doesn't see the references
+        back to higher objects.
         """
         return self.__treePath
```

### Comparing `extract_msg-0.41.5/extract_msg/named.py` & `extract_msg-0.42.0/extract_msg/msg_classes/task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,363 +1,356 @@
-from __future__ import annotations
-
-
 __all__ = [
-    'Named',
-    'NamedProperties',
-    'NamedPropertyBase',
-    'NumericalNamedProperty',
-    'StringNamedProperty',
+    'Task',
 ]
 
 
-import copy
+import datetime
+import functools
 import logging
-import pprint
-
-from typing import Dict, Optional, TYPE_CHECKING
 
-from . import constants
-from .enums import NamedPropertyType
-from .utils import bytesToGuid, divide, properHex
-from compressed_rtf.crc32 import crc32
+from typing import Optional
 
+from .. import constants
+from ..enums import (
+        TaskAcceptance, TaskHistory, TaskMode, TaskMultipleRecipients,
+        TaskOwnership, TaskState, TaskStatus
+    )
+from .message_base import MessageBase
+from ..structures.recurrence_pattern import RecurrencePattern
+from ..utils import unsignedToSignedInt
 
-# Allow for nice type checking.
-if TYPE_CHECKING:
-    from .msg import MSGFile
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
-class Named:
-    __dir = '__nameid_version1.0'
-    def __init__(self, msg):
-        self.__msg = msg
-        # Get the basic streams. If all are emtpy, then nothing to do.
-        guidStream = self._getStream('__substg1.0_00020102') or self._getStream('__substg1.0_00020102', False)
-        entryStream = self._getStream('__substg1.0_00030102') or self._getStream('__substg1.0_00030102', False)
-        self.guidStream = guidStream
-        self.entryStream = entryStream
-        self.namesStream = self._getStream('__substg1.0_00040102') or self._getStream('__substg1.0_00040102', False)
-        # The if else stuff is for protection against None.
-        guidStreamLength = len(guidStream) if guidStream else 0
-        entryStreamLength = len(entryStream) if entryStream else 0
-
-        self.__propertiesDict = {}
-        self.__properties = []
-        self.__guids = tuple()
-        self.__names = {}
-
-        # Check that we even have any entries. If there are none, nothing to do.
-        if entryStream:
-            guids = tuple([None, constants.PS_MAPI, constants.PS_PUBLIC_STRINGS] + [bytesToGuid(x) for x in divide(guidStream, 16)])
-            entries = []
-            for rawStream in divide(entryStream, 8):
-                tmp = constants.STNP_ENT.unpack(rawStream)
-                entry = {
-                    'id': tmp[0],
-                    'pid': tmp[2],
-                    'guid_index': tmp[1] >> 1,
-                    'pkind': NamedPropertyType(tmp[1] & 1), # 0 if numerical, 1 if string.
-                    'rawStream': rawStream,
-                }
-                entry['guid'] = guids[entry['guid_index']]
-                entries.append(entry)
-
-            self.entries = entries
-            self.__guids = guids
-
-            for entry in entries:
-                self.__properties.append(StringNamedProperty(entry, self.__getName(entry['id'])) if entry['pkind'] == NamedPropertyType.STRING_NAMED else NumericalNamedProperty(entry))
-
-            for property in self.__properties:
-                name = property.name if isinstance(property, StringNamedProperty) else property.propertyID
-                self.__propertiesDict[(name, property.guid)] = property
-
-    def __contains__(self, key) -> bool:
-        return key in self.__propertiesDict
-
-    def __getitem__(self, key):
-        return self.__propertiesDict[key]
-
-    def __iter__(self):
-        return self.__propertiesDict.__iter__()
-
-    def __len__(self) -> int:
-        return self.__propertiesDict.__len__()
-
-    def __getName(self, offset : int) -> str:
-        """
-        Parses the offset into the named stream and returns the name found.
-        """
-        # We used to parse names by handing it as an array, as specified by the
-        # documentation, but this new method allows for a little bit more wiggle
-        # room in terms of what is accepted by the module.
-        if offset & 3 != 0:
-            # If the offset is not a multiple of 4, that is an error, but we are
-            # reducing it to a warning.
-            logger.warning(f'Malformed named properties detected due to bad offset ({offset}). Ignoring.')
-        # Check that offset is in string stream.
-        if offset > len(self.namesStream):
-            raise ValueError('Failed to parse named property: offset was not in string stream.')
-
-        # Get the length, in bytes, of the string.
-        length = constants.STNP_NAM.unpack(self.namesStream[offset:offset + 4])[0]
-        offset += 4
-
-        # Make sure the string can be read entirely. If it can't, something was
-        # corrupt.
-        if offset + length > len(self.namesStream):
-            raise ValueError(f'Failed to parse named property: length ({length}) of string overflows the string stream. This is probably due to a bad offset.')
-
-        return self.namesStream[offset:offset + length].decode('utf-16-le')
-
-    def _getStream(self, filename, prefix = True) -> Optional[bytes]:
-        return self.__msg._getStream([self.__dir, filename], prefix = prefix)
-
-    def _getStringStream(self, filename, prefix = True) -> Optional[str]:
-        """
-        Gets a string representation of the requested filename.
-        Checks for both ASCII and Unicode representations and returns
-        a value if possible.  If there are both ASCII and Unicode
-        versions, then :param prefer: specifies which will be
-        returned.
-        """
-        return self.__msg._getStringStream([self.__dir, filename], prefix = prefix)
-
-    def exists(self, filename) -> bool:
-        """
-        Checks if stream exists inside the named properties folder.
-        """
-        return self.__msg.exists([self.__dir, filename])
-
-    def sExists(self, filename) -> bool:
-        """
-        Checks if the string stream exists inside the named properties folder.
-        """
-        return self.__msg.sExists([self.__dir, filename])
-
-    def get(self, propertyName, default = None):
-        """
-        Tries to get a named property based on its key. Returns :param default:
-        if not found. Key is a tuple of the name and the property set GUID.
-        """
-        try:
-            return self.__propertiesDict[propertyName]
-        except KeyError:
-            propertyName = propertyName.upper()
-            for key in self.__propertiesDict.keys():
-                if propertyName == key.upper():
-                    return self.__propertiesDict[key]
-            return default
-
-    def keys(self):
-        return self.__propertiesDict.keys()
+class Task(MessageBase):
+    """
+    Class used for parsing task files.
+    """
 
-    def pprintKeys(self):
+    @property
+    def headerFormatProperties(self) -> constants.HEADER_FORMAT_TYPE:
         """
-        Uses the pprint function on a sorted list of keys.
+        Returns a dictionary of properties, in order, to be formatted into the
+        header. Keys are the names to use in the header while the values are one
+        of the following:
+        None: Signifies no data was found for the property and it should be
+            omitted from the header.
+        str: A string to be formatted into the header using the string encoding.
+        Tuple[Union[str, None], bool]: A string should be formatted into the
+            header. If the bool is True, then place an empty string if the value
+            is None, otherwise follow the same behavior as regular None.
+
+        Additional note: If the value is an empty string, it will be dropped as
+        well by default.
+
+        Additionally you can group members of a header together by placing them
+        in an embedded dictionary. Groups will be spaced out using a second
+        instance of the join string. If any member of a group is being printed,
+        it will be spaced apart from the next group/item.
+
+        If you class should not do *any* header injection, return None from this
+        property.
         """
-        pprint.pprint(sorted(self.__propertiesDict.keys()))
+        status = {
+            TaskStatus.NOT_STARTED: 'Not Started',
+            TaskStatus.IN_PROGRESS: 'In Progress',
+            TaskStatus.COMPLETE: 'Completed',
+            TaskStatus.WAITING_ON_OTHER: 'Waiting on someone else',
+            TaskStatus.DEFERRED: 'Deferred',
+            None: None,
+        }[self.taskStatus]
 
-    def values(self):
-        return self.__propertiesDict.values()
+        return {
+            '-basic info-': {
+                'Subject': self.subject,
+            },
+            '-status-': {
+                'Status': status,
+                'Percent Complete': f'{self.percentComplete*100:.0f}%',
+                'Date Completed': self.taskDateCompleted.__format__('%w, %B %d, %Y') if self.taskDateCompleted else None,
+            },
+            '-work-': {
+                'Total Work': f'{self.taskEstimatedEffort or 0} minutes',
+                'Actual Work': f'{self.taskActualEffort or 0} minutes',
+            },
+            '-owner-': {
+                'Owner': self.taskOwner,
+            },
+            '-importance-': {
+                'Importance': self.importanceString,
+            },
+        }
 
-    @property
-    def dir(self):
+    @functools.cached_property
+    def percentComplete(self) -> Optional[float]:
         """
-        Returns the directory inside the msg file where the named properties are located.
+        Indicates whether a time-flagged Message object is complete. Returns a
+        percentage in decimal form. 1.0 indicates it is complete.
         """
-        return self.__dir
+        return self._getNamedAs('8102', constants.ps.PSETID_TASK)
 
-    @property
-    def msg(self) -> MSGFile:
+    @functools.cached_property
+    def taskAcceptanceState(self) -> Optional[TaskAcceptance]:
         """
-        Returns the Message instance the attachment belongs to.
+        Indicates the acceptance state of the task.
         """
-        return self.__msg
+        return self._getNamedAs('812A', constants.ps.PSETID_TASK, TaskAcceptance)
 
-    @property
-    def namedProperties(self) -> Dict:
+    @functools.cached_property
+    def taskAccepted(self) -> bool:
         """
-        Returns a copy of the dictionary containing all the named properties.
+        Indicates whether a task assignee has replied to a tesk request for this
+        task object. Does not indicate if it was accepted or rejected.
         """
-        return copy.deepcopy(self.__propertiesDict)
+        return self._getNamedAs('8108', constants.ps.PSETID_TASK, bool, False)
 
+    @functools.cached_property
+    def taskActualEffort(self) -> Optional[int]:
+        """
+        Indicates the number of minutes that the user actually spent working on
+        a task.
+        """
+        return self._getNamedAs('8110', constants.ps.PSETID_TASK)
 
+    @functools.cached_property
+    def taskAssigner(self) -> Optional[str]:
+        """
+        Specifies the name of the user that last assigned the task.
+        """
+        return self._getNamedAs('8121', constants.ps.PSETID_TASK)
 
-class NamedProperties:
-    """
-    An instance that uses a Named instance and an extract-msg class to read the
-    data of named properties.
-    """
-    def __init__(self, named, streamSource):
+    @functools.cached_property
+    def taskAssigners(self) -> Optional[bytes]:
         """
-        :param named: The named instance to refer to for named properties
-            entries.
-        :param streamSource: The source to use for acquiring the data of a named
-            property.
+        A stack of entries, each representing a task assigner. The most recent
+        task assigner (that is, the top) appears at the bottom.
+
+        The documentation on this is weird, so I don't know how to parse it.
         """
-        self.__named = named
-        self.__streamSource = streamSource
+        return self._getNamedAs('8117', constants.ps.PSETID_TASK)
 
-    def __getitem__(self, item):
+    @functools.cached_property
+    def taskComplete(self) -> bool:
         """
-        Get a named property using the [] operator. Item must be a named
-        property instance or a tuple with 2 items: the name and the GUID string.
+        Indicates if the task is complete.
         """
-        if isinstance(item, NamedPropertyBase):
-            return self.__streamSource._getTypedData(item.propertyStreamID)
-        else:
-            return self.__streamSource._getTypedData(self.__named[item].propertyStreamID)
+        return self._getNamedAs('811C', constants.ps.PSETID_TASK, bool, False)
 
-    def get(self, item, default = None):
+    @functools.cached_property
+    def taskCustomFlags(self) -> Optional[int]:
         """
-        Get a named property, returning the value of :param default: if not
-        found. Item must be a tuple with 2 items: the name and the GUID string.
+        Custom flags set on the task.
         """
-        try:
-            return self[item]
-        except KeyError:
-            return default
+        return self._getNamedAs('8139', constants.ps.PSETID_TASK)
 
+    @functools.cached_property
+    def taskDateCompleted(self) -> Optional[datetime.datetime]:
+        """
+        The date when the user completed work on the task.
+        """
+        return self._getNamedAs('810F', constants.ps.PSETID_TASK)
 
+    @functools.cached_property
+    def taskDeadOccurrence(self) -> bool:
+        """
+        Indicates whether a new recurring task remains to be generated. Set to
+        False on a new Task object and True when the client generates the last
+        recurring task.
+        """
+        return self._getNamedAs('8109', constants.ps.PSETID_TASK, bool, False)
 
-class NamedPropertyBase:
-    def __init__(self, entry):
-        self.__entry = entry
-        self.__guidIndex = entry['guid_index']
-        self.__namedPropertyID = entry['pid']
-        self.__guid = entry['guid']
-        self.__propertyStreamID = f'{0x8000 + self.__namedPropertyID:04X}'
+    @functools.cached_property
+    def taskDueDate(self) -> Optional[datetime.datetime]:
+        """
+        Specifies the date by which the user expects work on the task to be
+        complete.
+        """
+        return self._getNamedAs('8105', constants.ps.PSETID_TASK)
 
-    @property
-    def guid(self) -> str:
+    @functools.cached_property
+    def taskEstimatedEffort(self) -> Optional[int]:
         """
-        The guid of the property's property set.
+        Indicates the number of minutes that the user expects to work on a task.
         """
-        return self.__guid
+        return self._getNamedAs('8111', constants.ps.PSETID_TASK)
 
-    @property
-    def guidIndex(self) -> int:
+    @functools.cached_property
+    def taskFCreator(self) -> bool:
         """
-        The guid index of the property's property set.
+        Indicates that the task object was originally created by the action of
+        the current user or user agent instead of by the processing of a task
+        request.
         """
-        return self.__guidIndex
+        return self._getNamedAs('811E', constants.ps.PSETID_TASK, bool, False)
 
-    @property
-    def namedPropertyID(self) -> int:
+    @functools.cached_property
+    def taskFFixOffline(self) -> bool:
         """
-        The named property id.
+        Indicates whether the value of the taskOwner property is correct.
         """
-        return self.__namedPropertyID
+        return self._getNamedAs('812C', constants.ps.PSETID_TASK, bool, False)
 
-    @property
-    def propertyStreamID(self) -> str:
+    @functools.cached_property
+    def taskFRecurring(self) -> bool:
         """
-        An ID usable for grabbing the value stream.
+        Indicates whether the task includes a recurrence pattern.
         """
-        return self.__propertyStreamID
+        return self._getNamedAs('8126', constants.ps.PSETID_TASK, bool, False)
 
-    @property
-    def rawEntry(self) -> dict:
-        return copy.deepcopy(self.__entry)
+    @functools.cached_property
+    def taskGlobalID(self) -> Optional[bytes]:
+        """
+        Specifies a unique GUID for this task, used to locate an existing task
+        upon receipt of a task response or task update.
+        """
+        return self._getNamedAs('8519', constants.ps.PSETID_COMMON)
 
-    @property
-    def rawEntryStream(self) -> bytes:
+    @functools.cached_property
+    def taskHistory(self) -> Optional[TaskHistory]:
         """
-        The raw data used for the entry.
+        Indicates the type of change that was last made to the Task object.
         """
-        return self.__entry['rawStream']
+        return self._getNamedAs('811A', constants.ps.PSETID_TASK, TaskHistory)
 
-    @property
-    def type(self) -> NamedPropertyType:
+    @functools.cached_property
+    def taskLastDelegate(self) -> Optional[str]:
+        """
+        Contains the name of the user who most recently assigned the task, or
+        the user to whom it was most recently assigned.
         """
-        The type of named property.
+        return self._getNamedAs('8125', constants.ps.PSETID_TASK)
+
+    @functools.cached_property
+    def taskLastUpdate(self) -> Optional[datetime.datetime]:
+        """
+        The date and time of the most recent change made to the task object.
         """
-        raise NotImplementedError('NamedPropertyBase cannot be used directly. Subclass it before using it.')
+        return self._getNamedAs('8115', constants.ps.PSETID_TASK)
 
+    @functools.cached_property
+    def taskLastUser(self) -> Optional[str]:
+        """
+        Contains the name of the most recent user to have been the owner of the
+        task.
+        """
+        return self._getNamedAs('8122', constants.ps.PSETID_TASK)
 
+    @functools.cached_property
+    def taskMode(self) -> Optional[TaskMode]:
+        """
+        Used in a task communication. Should be 0 (UNASSIGNED) on task objects.
+        """
+        return self._getNamedAs('8518', constants.ps.PSETID_COMMON, TaskMode)
 
-class StringNamedProperty(NamedPropertyBase):
-    def __init__(self, entry, name):
-        super().__init__(entry)
-        self.__name = name
-
-        # Finally got this to be correct after asking about it on a Microsoft
-        # forum. Apparently it uses the same CRC-32 as the Compressed RTF
-        # standard does, so we can just use the function defined in the
-        # compressed-rtf Python module.
-        #
-        # First thing to note is that the name should only ever be lowered if it
-        # is part of the PS_INTERNET_HEADERS property set **AND** it is
-        # generated by certain versions of Outlook. As such, a little bit of
-        # additional code will need to run to determine exactly what the stream
-        # ID should be if it is in that property set.
-        if self.guid == constants.PS_INTERNET_HEADERS:
-            # To be sure if it needs to be lower the most effective method would
-            # be to just get the Stream ID and then check if the entry is in
-            # there. If it isn't, then check the regular case and see. If it is
-            # not in either... well, we don't use it for anything so it will
-            # just be a warning, and the Stream ID will be set to 0.
-            #
-            # TODO: Unfortunately, doing this will need to be put off until a
-            # different version, preferably after Python 2 support is removed,
-            # as this will require restructuring a lot of internal code. For now
-            # we just assume that it is lowercase.
-            self.__streamID = 0x1000 + (crc32(name.lower().encode('utf-16-le')) ^ (self.guidIndex << 1 | 1)) % 0x1F
-
-        else:
-            # No special logic here to determine what to do.
-            self.__streamID = 0x1000 + (crc32(name.encode('utf-16-le')) ^ (self.guidIndex << 1 | 1)) % 0x1F
+    @functools.cached_property
+    def taskMultipleRecipients(self) -> Optional[TaskMultipleRecipients]:
+        """
+        Returns a union of flags that specify optimization hints about the
+        recipients of a Task object.
+        """
+        return self._getNamedAs('8120', constants.ps.PSETID_TASK, TaskMultipleRecipients)
 
-    @property
-    def name(self) -> str:
+    @functools.cached_property
+    def taskNoCompute(self) -> Optional[bool]:
         """
-        The name of the property.
+        This value is not used and has no impact on a Task, but is provided for
+        completeness.
         """
-        return self.__name
+        return self._getNamedAs('8124', constants.ps.PSETID_TASK)
 
-    @property
-    def streamID(self) -> int:
+    @functools.cached_property
+    def taskOrdinal(self) -> Optional[int]:
         """
-        Returns the streamID of the named property. This may not be accurate.
+        Specifies a number that aids custom sorting of Task objects.
         """
-        return self.__streamID
+        return self._getNamedAs('8123', constants.ps.PSETID_TASK, unsignedToSignedInt)
 
-    @property
-    def type(self) -> NamedPropertyType:
+    @functools.cached_property
+    def taskOwner(self) -> Optional[str]:
         """
-        Returns the type of the named property. This will either be NUMERICAL_NAMED or STRING_NAMED.
+        Contains the name of the owner of the task.
         """
-        return NamedPropertyType.STRING_NAMED
+        return self._getNamedAs('811F', constants.ps.PSETID_TASK)
 
+    @functools.cached_property
+    def taskOwnership(self) -> Optional[TaskOwnership]:
+        """
+        Contains the name of the owner of the task.
+        """
+        return self._getNamedAs('8129', constants.ps.PSETID_TASK, TaskOwnership)
 
+    @functools.cached_property
+    def taskRecurrence(self) -> Optional[RecurrencePattern]:
+        """
+        Contains a RecurrencePattern structure that provides information about
+        recurring tasks.
+        """
+        return self._getNamedAs('8116', constants.ps.PSETID_TASK, RecurrencePattern)
 
-class NumericalNamedProperty(NamedPropertyBase):
-    def __init__(self, entry):
-        super().__init__(entry)
-        self.__propertyID = properHex(entry['id'], 4).upper()
-        self.__streamID = 0x1000 + (entry['id'] ^ (self.guidIndex << 1)) % 0x1F
+    @functools.cached_property
+    def taskResetReminder(self) -> bool:
+        """
+        Indicates whether future recurring tasks need reminders.
+        """
+        return self._getNamedAs('8107', constants.ps.PSETID_TASK, bool, False)
 
-    @property
-    def propertyID(self) -> str:
+    @functools.cached_property
+    def taskRole(self) -> Optional[str]:
         """
-        The actualy property id of the named property.
+        This value is not used and has no impact on a Task, but is provided for
+        completeness.
         """
-        return self.__propertyID
+        return self._getNamedAs('8127', constants.ps.PSETID_TASK)
 
-    @property
-    def streamID(self) -> int:
+    @functools.cached_property
+    def taskStartDate(self) -> Optional[datetime.datetime]:
         """
-        Returns the streamID of the named property. This may not be accurate
+        Specifies the date on which the user expects work on the task to begin.
         """
-        return self.__streamID
+        return self._getNamedAs('8104', constants.ps.PSETID_TASK)
 
-    @property
-    def type(self) -> NamedPropertyType:
+    @functools.cached_property
+    def taskState(self) -> Optional[TaskState]:
+        """
+        Indicates the current assignment state of the Task object.
+        """
+        return self._getNamedAs('8113', constants.ps.PSETID_TASK, TaskState)
+
+    @functools.cached_property
+    def taskStatus(self) -> Optional[TaskStatus]:
+        """
+        The completion status of a task.
+        """
+        return self._getNamedAs('8101', constants.ps.PSETID_TASK, TaskStatus)
+
+    @functools.cached_property
+    def taskStatusOnComplete(self) -> bool:
+        """
+        Indicates whether the task assignee has been requested to send an email
+        message upon completion of the assigned task.
+        """
+        return self._getNamedAs('8119', constants.ps.PSETID_TASK, bool, False)
+
+    @functools.cached_property
+    def taskUpdates(self) -> bool:
+        """
+        Indicates whether the task assignee has been requested to send a task
+        update when the assigned Task object changes.
+        """
+        return self._getNamedAs('811B', constants.ps.PSETID_TASK, bool, False)
+
+    @functools.cached_property
+    def taskVersion(self) -> Optional[int]:
+        """
+        Indicates which copy is the latest update of a Task object.
+        """
+        return self._getNamedAs('8112', constants.ps.PSETID_TASK)
+
+    @functools.cached_property
+    def teamTask(self) -> Optional[bool]:
         """
-        Returns the type of the named property. This will either be NUMERICAL_NAMED or STRING_NAMED.
+        This value is not used and has no impact on a Task, but is provided for
+        completeness.
         """
-        return NamedPropertyType.NUMERICAL_NAMED
+        return self._getNamedAs('8103', constants.ps.PSETID_TASK)
```

### Comparing `extract_msg-0.41.5/extract_msg/ole_writer.py` & `extract_msg-0.42.0/extract_msg/ole_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from .utils import ceilDiv, dictGetCasedKey, inputToMsgPath
 from olefile.olefile import OleDirectoryEntry, OleFileIO
 from red_black_dict_mod import RedBlackTree
 
 
 # Allow for nice type checking.
 if TYPE_CHECKING:
-    from .msg import MSGFile
-
+    from .msg_classes import MSGFile
 
 
 class DirectoryEntry:
     """
     An internal representation of a stream or storage in the OleWriter.
     Originals should be inaccessible outside of the class.
     """
@@ -66,15 +65,15 @@
         if len(self.name) < 1:
             raise ValueError('Directory entry must have a name.')
         if re.search('/\\\\:!', self.name):
             raise ValueError('Directory entry name contains an illegal character.')
 
         nameBytes = self.name.encode('utf-16-le')
 
-        return constants.ST_CF_DIR_ENTRY.pack(
+        return constants.st.ST_CF_DIR_ENTRY.pack(
                                               nameBytes,
                                               len(nameBytes) + 2,
                                               self.type,
                                               self.color,
                                               self.leftSiblingID,
                                               self.rightSiblingID,
                                               self.childID,
@@ -432,46 +431,46 @@
         # Sector shift.
         f.write(b'\x09\x00')
         # Mini sector shift.
         f.write(b'\x06\x00')
         # Reserved.
         f.write(b'\x00\x00\x00\x00\x00\x00')
         # Number of directory sectors. Version 3 says this *must* be 0.
-        f.write(constants.ST_LE_UI32.pack(0))
+        f.write(constants.st.ST_LE_UI32.pack(0))
         # Number of FAT sectors.
-        f.write(constants.ST_LE_UI32.pack(numFat))
+        f.write(constants.st.ST_LE_UI32.pack(numFat))
         # First directory sector location (Sector for the directory stream).
         # We place that right after the DIFAT and FAT.
-        f.write(constants.ST_LE_UI32.pack(numFat + numDifat))
+        f.write(constants.st.ST_LE_UI32.pack(numFat + numDifat))
         # Transation signature number.
         f.write(b'\x00\x00\x00\x00')
         # Mini stream cutoff size.
         f.write(b'\x00\x10\x00\x00')
         # First mini FAT sector location.
-        f.write(constants.ST_LE_UI32.pack((numFat + numDifat + ceilDiv(self.__dirEntryCount, 4)) if self.__numMinifat > 0 else 0xFFFFFFFE))
+        f.write(constants.st.ST_LE_UI32.pack((numFat + numDifat + ceilDiv(self.__dirEntryCount, 4)) if self.__numMinifat > 0 else 0xFFFFFFFE))
         # Number of mini FAT sectors.
-        f.write(constants.ST_LE_UI32.pack(ceilDiv(self.__numMinifatSectors, 128)))
+        f.write(constants.st.ST_LE_UI32.pack(ceilDiv(self.__numMinifatSectors, 128)))
         # First DIFAT sector location. If there are none, set to 0xFFFFFFFE (End
         # of chain).
-        f.write(constants.ST_LE_UI32.pack(0 if numDifat else 0xFFFFFFFE))
+        f.write(constants.st.ST_LE_UI32.pack(0 if numDifat else 0xFFFFFFFE))
         # Number of DIFAT sectors.
-        f.write(constants.ST_LE_UI32.pack(numDifat))
+        f.write(constants.st.ST_LE_UI32.pack(numDifat))
 
         # To make life easier on me, I'm having the code start with the DIFAT
         # followed by the FAT sectors, as I can write them all at once before
         # writing the actual contents of the file.
 
         # Write the DIFAT sectors.
         for x in range(numFat):
             # This kind of sucks to code, ngl.
             if x > 109 and (x - 109) % 127 == 0:
                 # If we are at the end of a DIFAT sector, write the jump.
-                f.write(constants.ST_LE_UI32.pack((x - 109) // 127))
+                f.write(constants.st.ST_LE_UI32.pack((x - 109) // 127))
             # Write the next FAT sector location.
-            f.write(constants.ST_LE_UI32.pack(x + numDifat))
+            f.write(constants.st.ST_LE_UI32.pack(x + numDifat))
 
         # Finally, fill out the last DIFAT sector with null entries.
         if numFat > 109:
             f.write(b'\xFF\xFF\xFF\xFF' * (127 - ((numFat - 109) % 127)))
             # Finally, make sure to write the end of chain marker for the DIFAT.
             f.write(b'\xFE\xFF\xFF\xFF')
         else:
@@ -485,50 +484,50 @@
         # Second write that the next x sectors are all FAT sectors.
         f.write(b'\xFD\xFF\xFF\xFF' * numFat)
 
         offset = numDifat + numFat
 
         # Fill in the values for the directory stream.
         for x in range(offset + 1, offset + ceilDiv(self.__dirEntryCount, 4)):
-            f.write(constants.ST_LE_UI32.pack(x))
+            f.write(constants.st.ST_LE_UI32.pack(x))
 
         # Write the end of chain marker.
         f.write(b'\xFE\xFF\xFF\xFF')
 
         offset += ceilDiv(self.__dirEntryCount, 4)
 
         # Check if we have minifat *at all* first.
         if self.__numMinifatSectors > 0:
             # Mini FAT chain.
             for x in range(offset + 1, offset + ceilDiv(self.__numMinifat, 16)):
-                f.write(constants.ST_LE_UI32.pack(x))
+                f.write(constants.st.ST_LE_UI32.pack(x))
 
             # Write the end of chain marker.
             f.write(b'\xFE\xFF\xFF\xFF')
 
             offset += ceilDiv(self.__numMinifat, 16)
 
             # The mini stream sectors.
             for x in range(offset + 1, offset + self.__numMinifat):
-                f.write(constants.ST_LE_UI32.pack(x))
+                f.write(constants.st.ST_LE_UI32.pack(x))
 
             # Write the end of chain marker.
             f.write(b'\xFE\xFF\xFF\xFF')
 
             offset += self.__numMinifat
 
         # Regular stream chains. These are the most complex to handle. We handle
         # them by checking a list that was make of entries which were only added
         # to that list if the size was more than 4096. The order in the list is
         # how they will eventually be stored into the file correctly.
         for entry in self.__largeEntries:
             size = ceilDiv(len(entry.data), 512)
             entry.startingSectorLocation = offset
             for x in range(offset + 1, offset + size):
-                f.write(constants.ST_LE_UI32.pack(x))
+                f.write(constants.st.ST_LE_UI32.pack(x))
 
             # Write the end of chain marker.
             f.write(b'\xFE\xFF\xFF\xFF')
 
             offset += size
 
         # Finally, fill fat with markers to specify no block exists.
@@ -573,15 +572,15 @@
         """
         # For each of the entires that are streams and less than 4096.
         currentSector = 0
         for x in entries:
             if x.type == DirectoryEntryType.STREAM and len(x.data) < 4096:
                 size = ceilDiv(len(x.data), 64)
                 for x in range(currentSector + 1, currentSector + size):
-                    f.write(constants.ST_LE_UI32.pack(x))
+                    f.write(constants.st.ST_LE_UI32.pack(x))
                 if size > 0:
                     f.write(b'\xFE\xFF\xFF\xFF')
                 currentSector += size
 
         # Finally, write the remaining slots.
         if currentSector & 127:
             f.write(b'\xFF\xFF\xFF\xFF' * (128 - (currentSector & 127)))
@@ -875,15 +874,15 @@
             name already exists,
         :raises ValueError: If access to an internal item is attempted or the
             new name provided is invalid.
         """
         # First, validate the new name.
         if not isinstance(newName, str):
             raise ValueError('New name must be a string.')
-        if constants.RE_INVALID_OLE_PATH.search(newName):
+        if constants.re.INVALID_OLE_PATH.search(newName):
             raise ValueError('Invalid character(s) in new name. Must not contain the following characters: \\//!:')
         if len(newName) > 31:
             raise ValueError('New name must be less than 32 characters.')
 
         # Get the storage for our entry. Entry *must* exist.
         _dir = self.__getContainingStorage(inputToMsgPath(path))
```

### Comparing `extract_msg-0.41.5/extract_msg/post.py` & `extract_msg-0.42.0/extract_msg/msg_classes/post.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 __all__ = [
     'Post',
 ]
 
 
+import functools
 import json
 
 from typing import Optional
 
-from . import constants
+from .. import constants
 from .message_base import MessageBase
-from .utils import inputToString
+from ..utils import inputToString
 
 from imapclient.imapclient import decode_utf7
 
 
 class Post(MessageBase):
     """
     Class for parsing Post messages.
@@ -27,20 +28,20 @@
             'from': inputToString(self.sender, self.stringEncoding),
             'subject': inputToString(self.subject, self.stringEncoding),
             'date': inputToString(self.date, self.stringEncoding),
             'conversation': inputToString(self.conversation, self.stringEncoding),
             'body': decode_utf7(self.body),
         })
 
-    @property
+    @functools.cached_property
     def conversation(self) -> Optional[str]:
         """
         The name of the conversation being posted to.
         """
-        return self._ensureSet('_convo', '__substg1.0_0070')
+        return self._getStringStream('__substg1.0_0070')
 
     @property
     def headerFormatProperties(self) -> constants.HEADER_FORMAT_TYPE:
         """
         Returns a dictionary of properties, in order, to be formatted into the
         header. Keys are the names to use in the header while the values are one
         of the following:
```

### Comparing `extract_msg-0.41.5/extract_msg/prop.py` & `extract_msg-0.42.0/extract_msg/properties/prop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,55 @@
+from __future__ import annotations
+
+
 __all__ = [
-    # Classes.
+    # Classes:
     'FixedLengthProp'
     'PropBase',
     'VariableLengthProp',
 
-    # Functions.
+    # Functions:
     'createProp',
 ]
 
 
 import datetime
 import logging
 
 from typing import Any
 
-from . import constants
-from .enums import ErrorCode, ErrorCodeType
-from .utils import filetimeToDatetime, properHex
+from .. import constants
+from ..enums import ErrorCode, ErrorCodeType
+from ..utils import filetimeToDatetime, properHex
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
-def createProp(data : bytes) -> 'PropBase':
-    temp = constants.ST2.unpack(data)[0]
+def createProp(data : bytes) -> PropBase:
+    temp = constants.st.ST2.unpack(data)[0]
     if temp in constants.FIXED_LENGTH_PROPS:
         return FixedLengthProp(data)
     else:
         if temp not in constants.VARIABLE_LENGTH_PROPS:
-            # DEBUG
+            # DEBUG.
             logger.warning(f'Unknown property type: {properHex(temp)}')
         return VariableLengthProp(data)
 
 
 class PropBase:
     """
     Base class for Prop instances.
     """
 
     def __init__(self, data : bytes):
         self.__rawData = data
         self.__name = properHex(data[3::-1]).upper()
-        self.__type, self.__flags = constants.ST2.unpack(data)
+        self.__type, self.__flags = constants.st.ST2.unpack(data)
         self.__fm = self.__flags & 1 == 1
         self.__fr = self.__flags & 2 == 2
         self.__fw = self.__flags & 4 == 4
 
     @property
     def flagMandatory(self) -> bool:
         """
@@ -93,24 +96,25 @@
     def type(self) -> int:
         """
         The type of property.
         """
         return self.__type
 
 
+
 class FixedLengthProp(PropBase):
     """
     Class to contain the data for a single fixed length property.
 
     Currently a work in progress.
     """
 
     def __init__(self, data : bytes):
         super().__init__(data)
-        self.__value = self.parseType(self.type, constants.STFIX.unpack(data)[0])
+        self.__value = self.parseType(self.type, constants.st.STFIX.unpack(data)[0])
 
     def parseType(self, _type : int, stream : bytes) -> Any:
         """
         Converts the data in :param stream: to a much more accurate type,
         specified by :param _type:, if possible.
         :param stream: The data that the value is extracted from.
 
@@ -122,45 +126,45 @@
             pass
         elif _type == 0x0001: # PtypNull
             if value != b'\x00\x00\x00\x00\x00\x00\x00\x00':
                 # DEBUG.
                 logger.warning('Property type is PtypNull, but is not equal to 0.')
             value = None
         elif _type == 0x0002: # PtypInteger16
-            value = constants.STI16.unpack(value)[0]
+            value = constants.st.STI16.unpack(value)[0]
         elif _type == 0x0003: # PtypInteger32
-            value = constants.STI32.unpack(value)[0]
+            value = constants.st.STI32.unpack(value)[0]
         elif _type == 0x0004: # PtypFloating32
-            value = constants.STF32.unpack(value)[0]
+            value = constants.st.STF32.unpack(value)[0]
         elif _type == 0x0005: # PtypFloating64
-            value = constants.STF64.unpack(value)[0]
+            value = constants.st.STF64.unpack(value)[0]
         elif _type == 0x0006: # PtypCurrency
-            value = (constants.STI64.unpack(value))[0] / 10000.0
+            value = (constants.st.STI64.unpack(value))[0] / 10000.0
         elif _type == 0x0007: # PtypFloatingTime
-            value = constants.STF64.unpack(value)[0]
+            value = constants.st.STF64.unpack(value)[0]
             return constants.PYTPFLOATINGTIME_START + datetime.timedelta(days = value)
         elif _type == 0x000A: # PtypErrorCode
-            value = constants.STI32.unpack(value)[0]
+            value = constants.st.STI32.unpack(value)[0]
             try:
                 value = ErrorCodeType(value)
             except ValueError:
                 logger.warning(f'Error type found that was not from Additional Error Codes. Value was {value}. You should report this to the developers.')
                 # So here, the value should be from Additional Error Codes, but
                 # it wasn't. So we are just returning the int. However, we want
                 # to see if it is a normal error code.
                 try:
                     logger.warning(f'REPORT TO DEVELOPERS: Error type of {ErrorCode(value)} was found.')
                 except ValueError:
                     pass
         elif _type == 0x000B:  # PtypBoolean
-            value = constants.ST3.unpack(value)[0] == 1
+            value = constants.st.ST3.unpack(value)[0] == 1
         elif _type == 0x0014:  # PtypInteger64
-            value = constants.STI64.unpack(value)[0]
+            value = constants.st.STI64.unpack(value)[0]
         elif _type == 0x0040:  # PtypTime
-            rawTime = constants.ST3.unpack(value)[0]
+            rawTime = constants.st.ST3.unpack(value)[0]
             try:
                 value = filetimeToDatetime(rawTime)
             except ValueError as e:
                 logger.exception(e)
                 logger.error(self.rawData)
         elif _type == 0x0048:  # PtypGuid
             # TODO parsing for this
@@ -171,22 +175,23 @@
     def value(self) -> Any:
         """
         Property value.
         """
         return self.__value
 
 
+
 class VariableLengthProp(PropBase):
     """
     Class to contain the data for a single variable length property.
     """
 
     def __init__(self, data : bytes):
         super().__init__(data)
-        self.__length, self.__reserved = constants.STVAR.unpack(data)
+        self.__length, self.__reserved = constants.st.STVAR.unpack(data)
         if self.type == 0x001E:
             self.__realLength = self.__length - 1
         elif self.type == 0x001F:
             self.__realLength = self.__length - 2
         elif self.type in constants.MULTIPLE_2_BYTES_HEX:
             self.__realLength = self.__length // 2
         elif self.type in constants.MULTIPLE_4_BYTES_HEX:
```

### Comparing `extract_msg-0.41.5/extract_msg/recipient.py` & `extract_msg-0.42.0/extract_msg/recipient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,181 @@
 __all__ = [
     'Recipient',
 ]
 
 
+import functools
 import logging
 
-from typing import Optional, Union
+from typing import Optional, Tuple, Union
 
 from .enums import ErrorBehavior, MeetingRecipientType, PropertiesType, RecipientType
 from .exceptions import StandardViolationError
-from .prop import FixedLengthProp
-from .properties import Properties
+from .properties.prop import FixedLengthProp
+from .properties.properties_store import PropertiesStore
 from .structures.entry_id import PermanentEntryID
-from .utils import verifyPropertyId, verifyType
+from .utils import makeWeakRef, verifyPropertyId, verifyType
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class Recipient:
     """
-    Contains the data of one of the recipients in an msg file.
+    Contains the data of one of the recipients in an MSG file.
     """
 
     def __init__(self, _dir, msg):
-        self.__msg = msg # Allows calls to original msg file.
+        self.__msg = makeWeakRef(msg) # Allows calls to original msg file.
         self.__dir = _dir
         if not self.exists('__properties_version1.0'):
-            if msg.errorBehavior & ErrorBehavior.STANDARDS_VIOLATION:
+            if ErrorBehavior.STANDARDS_VIOLATION in msg.errorBehavior:
                 logger.error('Recipients MUST have a property stream.')
             else:
                 raise StandardViolationError('Recipients MUST have a property stream.') from None
-        self.__props = Properties(self._getStream('__properties_version1.0'), PropertiesType.RECIPIENT)
+        self.__props = PropertiesStore(self._getStream('__properties_version1.0'), PropertiesType.RECIPIENT)
         self.__email = self._getStringStream('__substg1.0_39FE')
         if not self.__email:
             self.__email = self._getStringStream('__substg1.0_3003')
         self.__name = self._getStringStream('__substg1.0_3001')
         self.__typeFlags = self.__props.get('0C150003').value or 0
-        from .calendar_base import CalendarBase
+        from .msg_classes.calendar_base import CalendarBase
         if isinstance(msg, CalendarBase):
             self.__type = MeetingRecipientType(0xF & self.__typeFlags)
         else:
             self.__type = RecipientType(0xF & self.__typeFlags)
         self.__formatted = f'{self.__name} <{self.__email}>'
 
-    def _ensureSet(self, variable, streamID, stringStream : bool = True, **kwargs):
+    def _getPropertyAs(self, propertyName, overrideClass = None, preserveNone : bool = True):
         """
-        Ensures that the variable exists, otherwise will set it using the
-        specified stream. After that, return said variable.
-
-        If the specified stream is not a string stream, make sure to set
-        :param string stream: to False.
+        Returns the property, setting the class if specified.
 
         :param overrideClass: Class/function to use to morph the data that was
             read. The data will be the first argument to the class's __init__
             function or the function itself, if that is what is provided. By
             default, this will be completely ignored if the value was not found.
-        :param preserveNone: If true (default), causes the function to ignore
+        :param preserveNone: If True (default), causes the function to ignore
             :param overrideClass: when the value could not be found (is None).
             If this is changed to False, then the value will be used regardless.
         """
         try:
-            return getattr(self, variable)
-        except AttributeError:
-            if stringStream:
-                value = self._getStringStream(streamID)
-            else:
-                value = self._getStream(streamID)
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
+            value = self.props[propertyName].value
+        except (KeyError, AttributeError):
+            value = None
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if (value is not None or not preserveNone):
+                value = overrideClass(value)
+
+        return value
+
+    def _getStream(self, filename) -> Optional[bytes]:
+        """
+        Gets a binary representation of the requested filename.
+
+        This should ALWAYS return a bytes object if it was found, otherwise
+        returns None.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
+        """
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Recipient instance has been garbage collected.')
+        return msg._getStream([self.__dir, filename])
 
-    def _ensureSetProperty(self, variable : str, propertyName : str, **kwargs):
+    def _getStreamAs(self, streamID, stringStream : bool = True, overrideClass = None, preserveNone : bool = True):
         """
-        Ensures that the variable exists, otherwise will set it using the
-        property. After that, return said variable.
+        Returns the specified stream, modifying it to the class if specified.
+
+        If the specified stream is not a string stream, make sure to set
+        :param stringStream: to False.
 
         :param overrideClass: Class/function to use to morph the data that was
             read. The data will be the first argument to the class's __init__
             function or the function itself, if that is what is provided. By
             default, this will be completely ignored if the value was not found.
         :param preserveNone: If true (default), causes the function to ignore
             :param overrideClass: when the value could not be found (is None).
             If this is changed to False, then the value will be used regardless.
         """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            try:
-                value = self.props[propertyName].value
-            except (KeyError, AttributeError):
-                value = None
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
+        if stringStream:
+            value = self._getStringStream(streamID)
+        else:
+            value = self._getStream(streamID)
+
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if value is not None or not preserveNone:
+                value = overrideClass(value)
+
+        return value
+
+    def _getStringStream(self, filename) -> Optional[str]:
+        """
+        Gets a string representation of the requested filename.
+
+        Rather than the full filename, you should only feed this function the
+        filename sans the type. So if the full name is "__substg1.0_001A001F",
+        the filename this function should receive should be "__substg1.0_001A".
 
-    def _ensureSetTyped(self, variable : str, _id, **kwargs):
+        This should ALWAYS return a string if it was found, otherwise returns
+        None.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
+        """
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Recipient instance has been garbage collected.')
+        return msg._getStringStream([self.__dir, filename])
+
+    def _getTypedAs(self, _id : str, overrideClass = None, preserveNone : bool = True):
         """
-        Like the other ensure set functions, but designed for when something
+        Like the other get as functions, but designed for when something
         could be multiple types (where only one will be present). This way you
         have no need to set the type, it will be handled for you.
 
         :param overrideClass: Class/function to use to morph the data that was
             read. The data will be the first argument to the class's __init__
             function or the function itself, if that is what is provided. By
             default, this will be completely ignored if the value was not found.
         :param preserveNone: If true (default), causes the function to ignore
             :param overrideClass: when the value could not be found (is None).
             If this is changed to False, then the value will be used regardless.
         """
-        try:
-            return getattr(self, variable)
-        except AttributeError:
-            value = self._getTypedData(_id)
-            # Check if we should be overriding the data type for this instance.
-            if kwargs:
-                overrideClass = kwargs.get('overrideClass')
-                if overrideClass is not None and (value is not None or not kwargs.get('preserveNone', True)):
-                    value = overrideClass(value)
-            setattr(self, variable, value)
-            return value
-
-    def _getStream(self, filename) -> Optional[bytes]:
-        """
-        Gets a binary representation of the requested filename.
+        value = self._getTypedData(_id)
+        # Check if we should be overriding the data type for this instance.
+        if overrideClass is not None:
+            if value is not None or not preserveNone:
+                value = overrideClass(value)
 
-        This should ALWAYS return a bytes object if it was found, otherwise
-        returns None.
-        """
-        return self.__msg._getStream([self.__dir, filename])
-
-    def _getStringStream(self, filename) -> Optional[str]:
-        """
-        Gets a string representation of the requested filename. Checks for both
-        Unicode and Non-Unicode representations and returns a value if possible.
-        If there are both Unicode and Non-Unicode versions, then :param prefer:
-        specifies which will be returned.
-        """
-        return self.__msg._getStringStream([self.__dir, filename])
+        return value
 
     def _getTypedData(self, _id, _type = None):
         """
         Gets the data for the specified id as the type that it is supposed to
         be. :param id: MUST be a 4 digit hexadecimal string.
 
         If you know for sure what type the data is before hand, you can specify
         it as being one of the strings in the constant FIXED_LENGTH_PROPS_STRING
         or VARIABLE_LENGTH_PROPS_STRING.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
         verifyPropertyId(id)
         _id = _id.upper()
         found, result = self._getTypedStream('__substg1.0_' + _id, _type)
         if found:
             return result
         else:
             found, result = self._getTypedProperty(_id, _type)
             return result if found else None
 
-    def _getTypedProperty(self, propertyID : str, _type = None):
+    def _getTypedProperty(self, propertyID : str, _type = None) -> Tuple[bool, Optional[object]]:
         """
         Gets the property with the specified id as the type that it is supposed
         to be. :param id: MUST be a 4 digit hexadecimal string.
 
         If you know for sure what type the property is before hand, you can
         specify it as being one of the strings in the constant
         FIXED_LENGTH_PROPS_STRING or VARIABLE_LENGTH_PROPS_STRING.
@@ -197,113 +202,133 @@
         specify it as being one of the strings in the constant
         FIXED_LENGTH_PROPS_STRING or VARIABLE_LENGTH_PROPS_STRING.
 
         If you have not specified the type, the type this function returns in
         many cases cannot be predicted. As such, when using this function it is
         best for you to check the type that it returns. If the function returns
         None, that means it could not find the stream specified.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        self.__msg._getTypedStream(self, [self.__dir, filename], True, _type)
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Recipient instance has been garbage collected.')
+        return msg._getTypedStream(self, [self.__dir, filename], True, _type)
 
     def exists(self, filename) -> bool:
         """
         Checks if stream exists inside the recipient folder.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self.__msg.exists([self.__dir, filename])
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Recipient instance has been garbage collected.')
+        return msg.exists([self.__dir, filename])
 
     def sExists(self, filename) -> bool:
         """
         Checks if the string stream exists inside the recipient folder.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self.__msg.sExists([self.__dir, filename])
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Recipient instance has been garbage collected.')
+        return msg.sExists([self.__dir, filename])
 
     def existsTypedProperty(self, id, _type = None) -> bool:
         """
         Determines if the stream with the provided id exists. The return of this
         function is 2 values, the first being a boolean for if anything was
         found, and the second being how many were found.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self.__msg.existsTypedProperty(id, self.__dir, _type, True, self.__props)
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Recipient instance has been garbage collected.')
+        return msg.existsTypedProperty(id, self.__dir, _type, True, self.__props)
 
-    @property
+    @functools.cached_property
     def account(self) -> Optional[str]:
         """
         Returns the account of this recipient.
         """
-        return self._ensureSet('_account', '__substg1.0_3A00')
+        return self._getStringStream('__substg1.0_3A00')
 
     @property
     def email(self) -> Optional[str]:
         """
         Returns the recipient's email.
         """
         return self.__email
 
-    @property
+    @functools.cached_property
     def entryID(self) -> Optional[PermanentEntryID]:
         """
         Returns the recipient's Entry ID.
         """
-        return self._ensureSet('_entryID', '__substg1.0_0FFF0102', False, overrideClass = PermanentEntryID)
+        return self._getStreamAs('__substg1.0_0FFF0102', False, PermanentEntryID)
 
     @property
     def formatted(self) -> str:
         """
         Returns the formatted recipient string.
         """
         return self.__formatted
 
-    @property
+    @functools.cached_property
     def instanceKey(self) -> Optional[bytes]:
         """
         Returns the instance key of this recipient.
         """
-        return self._ensureSet('_instanceKey', '__substg1.0_0FF60102', False)
+        return self._getStream('__substg1.0_0FF60102')
 
     @property
     def name(self) -> Optional[str]:
         """
         Returns the recipient's name.
         """
         return self.__name
 
     @property
-    def props(self) -> Properties:
+    def props(self) -> PropertiesStore:
         """
         Returns the Properties instance of the recipient.
         """
         return self.__props
 
-    @property
+    @functools.cached_property
     def recordKey(self) -> Optional[bytes]:
         """
         Returns the instance key of this recipient.
         """
-        return self._ensureSet('_recordKey', '__substg1.0_0FF90102', False)
+        return self._getStream('__substg1.0_0FF90102')
 
-    @property
+    @functools.cached_property
     def searchKey(self) -> Optional[bytes]:
         """
         Returns the search key of this recipient.
         """
-        return self._ensureSet('_searchKey', '__substg1.0_300B0102', False)
+        return self._getStream('__substg1.0_300B0102')
 
-    @property
+    @functools.cached_property
     def smtpAddress(self) -> Optional[str]:
         """
         Returns the SMTP address of this recipient.
         """
-        return self._ensureSet('_smtpAddress', '__substg1.0_39FE')
+        return self._getStringStream('__substg1.0_39FE')
 
-    @property
+    @functools.cached_property
     def transmittableDisplayName(self) -> Optional[str]:
         """
         Returns the transmittable display name of this recipient.
         """
-        return self._ensureSet('_transmittableDisplayName', '__substg1.0_3A20')
+        return self._getStringStream('__substg1.0_3A20')
 
     @property
     def type(self) -> Union[RecipientType, MeetingRecipientType]:
         """
         Returns the recipient type. Type is:
             * Sender if `type & 0xf == 0`
             * To if `type & 0xf == 1`
```

### Comparing `extract_msg-0.41.5/extract_msg/signed_attachment.py` & `extract_msg-0.42.0/extract_msg/attachments/signed_att.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 ]
 
 
 import email
 import logging
 import os
 import pathlib
+import weakref
 import zipfile
 
-from typing import Tuple, TYPE_CHECKING, Union
+from typing import List, Optional, Type, TYPE_CHECKING, Union
 
-from .enums import AttachmentType
-from .utils import createZipOpen, inputToString, openMsg, prepareFilename
+from .. import constants
+from ..enums import AttachmentType, SaveType
+from ..open_msg import openMsg
+from ..utils import createZipOpen, inputToString, makeWeakRef, prepareFilename
 
 
 # Allow for nice type checking.
 if TYPE_CHECKING:
-    from .msg import MSGFile
+    from ..msg_classes.msg import MSGFile
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class SignedAttachment:
     def __init__(self, msg, data : bytes, name : str, mimetype : str, node : email.message.Message):
@@ -34,17 +37,17 @@
         :param name: The reported name of the attachment.
         :param mimetype: The reported mimetype of the attachment.
         :param node: The email Message instance for this node.
         """
         self.__asBytes = data
         self.__name = name
         self.__mimetype = mimetype
-        self.__msg = msg
+        self.__msg = makeWeakRef(msg)
         self.__node = node
-        self.__treePath = msg.treePath + (self,)
+        self.__treePath = msg.treePath + [makeWeakRef(self)]
 
         self.__data = None
         # To add support for embedded MSG files, we are going to completely
         # ignore the mimetype and just do a few simple checks to see if we can
         # use the bytes as am embedded file.
         if data[:8] == b'\xD0\xCF\x11\xE0\xA1\xB1\x1A\xE1':
             try:
@@ -55,15 +58,15 @@
                 self.__data = openMsg(data, treePath = self.__treePath, **msg.kwargs)
             except Exception:
                 logger.exception('Signed message was an OLE file, but could not be read as an MSG file due to an exception.')
 
         if self.__data is None:
             self.__data = data
 
-    def save(self, **kwargs):
+    def save(self, **kwargs) -> constants.SAVE_TYPE:
         """
         Saves the attachment data.
 
         The name of the file is determined by several factors. The first
         thing that is checked is if you have provided :param customFilename:
         to this function. If you have, that is the name that will be used.
         If no custom name has been provided and :param contentId: is True,
@@ -79,19 +82,28 @@
         of :param customPath: when calling this function. The default save
         directory is the working directory.
 
         If you want to save the contents into a ZipFile or similar object,
         either pass a path to where you want to create one or pass an instance
         to :param zip:. If :param zip: is an instance, :param customPath: will
         refer to a location inside the zip file.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
         # First check if we are skipping embedded messages and stop
         # *immediately* if we are.
         if self.type is AttachmentType.SIGNED_EMBEDDED and kwargs.get('skipEmbedded'):
-            return None
+            return (SaveType.NONE, None)
+
+        # If we are running the save function for the MSG file, just let it
+        # handle everything.
+        if (self.type is AttachmentType.SIGNED_EMBEDDED and
+            not kwargs.get('extractEmbedded', False)):
+            return self.saveEmbededMessage(**kwargs)
 
         # Check if the user has specified a custom filename
         filename = self.name
 
         # Someone managed to have a null character here, so let's get rid of that
         filename = prepareFilename(inputToString(filename, self.msg.stringEncoding))
 
@@ -102,105 +114,90 @@
         if len(filename) > maxNameLength:
             name, ext = os.path.splitext(filename)
             filename = name[:maxNameLength - len(ext)] + ext
 
         # Check if we are doing a zip file.
         _zip = kwargs.get('zip')
 
-        # ZipFile handling.
-        if _zip:
-            # If we are doing a zip file, first check that we have been given a path.
-            if isinstance(_zip, (str, pathlib.Path)):
-                # If we have a path then we use the zip file.
-                _zip = zipfile.ZipFile(_zip, 'a', zipfile.ZIP_DEFLATED)
-                kwargs['zip'] = _zip
-                createdZip = True
-            else:
-                createdZip = False
-            # Path needs to be done in a special way if we are in a zip file.
-            customPath = pathlib.Path(kwargs.get('customPath', ''))
-            # Set the open command to be that of the zip file.
-            _open = createZipOpen(_zip.open)
-            # Zip files use w for writing in binary.
-            mode = 'w'
-        else:
-            customPath = pathlib.Path(kwargs.get('customPath', '.')).absolute()
-            mode = 'wb'
-            _open = open
-
-        fullFilename = customPath / filename
-
-        if self.type is AttachmentType.DATA:
+        createdZip = True
+        try:
+            # ZipFile handling.
             if _zip:
-                name, ext = os.path.splitext(filename)
-                nameList = _zip.namelist()
-                if fullFilename in nameList:
-                    for i in range(2, 100):
-                        testName = customPath / f'{name} ({i}){ext}'
-                        if testName not in nameList:
-                            fullFilename = testName
-                            break
-                    else:
-                        # If we couldn't find one that didn't exist.
-                        raise FileExistsError(f'Could not create the specified file because it already exists ("{fullFilename}").')
+                # If we are doing a zip file, first check that we have been
+                # given a path.
+                if isinstance(_zip, (str, pathlib.Path)):
+                    # If we have a path then we use the zip file.
+                    _zip = zipfile.ZipFile(_zip, 'a', zipfile.ZIP_DEFLATED)
+                    kwargs['zip'] = _zip
+                    createdZip = True
+                else:
+                    createdZip = False
+                # Path needs to be done in a special way if we are in a zip
+                # file.
+                customPath = pathlib.Path(kwargs.get('customPath', ''))
+                # Set the open command to be that of the zip file.
+                _open = createZipOpen(_zip.open)
+                # Zip files use w for writing in binary.
+                mode = 'w'
             else:
-                if fullFilename.exists():
-                    # Try to split the filename into a name and extention.
-                    name, ext = os.path.splitext(filename)
-                    # Try to add a number to it so that we can save without overwriting.
-                    for i in range(2, 100):
-                        testName = customPath / f'{name} ({i}){ext}'
-                        if not testName.exists():
-                            fullFilename = testName
-                            break
-                    else:
-                        # If we couldn't find one that didn't exist.
-                        raise FileExistsError(f'Could not create the specified file because it already exists ("{fullFilename}").')
+                customPath = pathlib.Path(kwargs.get('customPath', '.')).absolute()
+                mode = 'wb'
+                _open = open
 
-            with _open(str(fullFilename), mode) as f:
-                f.write(self.__data)
+            fullFilename = self._handleFnc(_zip, filename, customPath, kwargs)
 
-            # Close the ZipFile if this function created it.
-            if _zip and createdZip:
-                _zip.close()
+            if self.type is AttachmentType.DATA:
+                with _open(str(fullFilename), mode) as f:
+                    f.write(self.__data)
 
-            return str(fullFilename)
-        else:
-            if kwargs.get('extractEmbedded', False):
+                return (SaveType.FILE, str(fullFilename))
+            else:
                 with _open(str(fullFilename), mode) as f:
                     # We just use the data we were given for this one.
                     f.write(self.__asBytes)
-            else:
-                self.saveEmbededMessage(**kwargs)
-
+                return (SaveType.FILE, str(fullFilename))
+        finally:
             # Close the ZipFile if this function created it.
             if _zip and createdZip:
                 _zip.close()
 
-            return self.msg
-
-    def saveEmbededMessage(self, **kwargs) -> None:
+    def saveEmbededMessage(self, **kwargs) -> constants.SAVE_TYPE:
         """
         Seperate function from save to allow it to easily be overridden by a
         subclass.
         """
-        self.data.save(**kwargs)
+        return self.data.save(**kwargs)
 
     @property
     def asBytes(self) -> bytes:
         return self.__asBytes
 
     @property
     def data(self) -> Union[bytes, MSGFile]:
         """
         The bytes that compose this attachment.
         """
         return self.__data
 
     @property
+    def dataType(self) -> Optional[Type[type]]:
+        """
+        The class that the data type will use, if it can be retrieved.
+
+        This is a safe way to do type checking on data before knowing if it will
+        raise an exception. Returns None if no data will be returns or if an
+        exception will be raised.
+        """
+        try:
+            return None if self.data is None else self.data.__class__
+        except Exception:
+            # All exceptions that accessing data would cause should be silenced.
+            return None
+
+    @property
     def emailMessage(self) -> email.message.Message:
         """
         The email Message instance that is the source for this attachment.
         """
         return self.__node
 
     @property
@@ -210,34 +207,39 @@
         """
         return self.__mimetype
 
     @property
     def msg(self) -> MSGFile:
         """
         The MSGFile instance this attachment belongs to.
+
+        :raises ReferenceError: The associated MSGFile instance has been garbage
+            collected.
         """
-        return self.__msg
+        if (msg := self.__msg()) is None:
+            raise ReferenceError('The msg file for this Attachment instance has been garbage collected.')
+        return msg
 
     @property
     def name(self) -> str:
         """
         The reported name of this attachment.
         """
         return self.__name
 
     longFilename = name
     shortFilename = name
 
     @property
-    def treePath(self) -> Tuple:
+    def treePath(self) -> List[weakref.ReferenceType]:
         """
         A path, as a tuple of instances, needed to get to this instance through
         the MSGFile-Attachment tree.
         """
         return self.__treePath
 
     @property
     def type(self) -> AttachmentType:
         """
-        The AttachmentType.
+        Returns an enum value that identifies the type of attachment.
         """
         return AttachmentType.SIGNED if isinstance(self.__data, bytes) else AttachmentType.SIGNED_EMBEDDED
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/_helpers.py` & `extract_msg-0.42.0/extract_msg/structures/_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,35 +21,35 @@
     stream.
     """
 
     def __init__(self, *args, littleEndian = True, **kwargs):
         super().__init__(*args, **kwargs)
         self.__le = bool(littleEndian)
         if self.__le:
-            self.__int8_t = constants.ST_LE_I8
-            self.__int16_t = constants.ST_LE_I16
-            self.__int32_t = constants.ST_LE_I32
-            self.__int64_t = constants.ST_LE_I64
-            self.__uint8_t = constants.ST_LE_UI8
-            self.__uint16_t = constants.ST_LE_UI16
-            self.__uint32_t = constants.ST_LE_UI32
-            self.__uint64_t = constants.ST_LE_UI64
-            self.__float_t = constants.ST_LE_F32
-            self.__double_t = constants.ST_LE_F64
+            self.__int8_t = constants.st.ST_LE_I8
+            self.__int16_t = constants.st.ST_LE_I16
+            self.__int32_t = constants.st.ST_LE_I32
+            self.__int64_t = constants.st.ST_LE_I64
+            self.__uint8_t = constants.st.ST_LE_UI8
+            self.__uint16_t = constants.st.ST_LE_UI16
+            self.__uint32_t = constants.st.ST_LE_UI32
+            self.__uint64_t = constants.st.ST_LE_UI64
+            self.__float_t = constants.st.ST_LE_F32
+            self.__double_t = constants.st.ST_LE_F64
         else:
-            self.__int8_t = constants.ST_BE_I8
-            self.__int16_t = constants.ST_BE_I16
-            self.__int32_t = constants.ST_BE_I32
-            self.__int64_t = constants.ST_BE_I64
-            self.__uint8_t = constants.ST_BE_UI8
-            self.__uint16_t = constants.ST_BE_UI16
-            self.__uint32_t = constants.ST_BE_UI32
-            self.__uint64_t = constants.ST_BE_UI64
-            self.__float_t = constants.ST_BE_F32
-            self.__double_t = constants.ST_BE_F64
+            self.__int8_t = constants.st.ST_BE_I8
+            self.__int16_t = constants.st.ST_BE_I16
+            self.__int32_t = constants.st.ST_BE_I32
+            self.__int64_t = constants.st.ST_BE_I64
+            self.__uint8_t = constants.st.ST_BE_UI8
+            self.__uint16_t = constants.st.ST_BE_UI16
+            self.__uint32_t = constants.st.ST_BE_UI32
+            self.__uint64_t = constants.st.ST_BE_UI64
+            self.__float_t = constants.st.ST_BE_F32
+            self.__double_t = constants.st.ST_BE_F64
 
     def _readDecodedString(self, encoding, width : int = 1) -> str:
         """
         Reads a null terminated string with the specified character width
         decoded using the specified encoding. If it cannot be read or cannot be
         decoded then the position of the read pointer will not be changed.
         """
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/business_card.py` & `extract_msg-0.42.0/extract_msg/structures/business_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Data structure for PidLidBusinessCardDisplayDefinition. Contains information
     used to contruct a business card for a contact.
     """
 
     def __init__(self, data : bytes):
         self.__rawData = data
         reader = BytesReader(data)
-        unpacked = constants.ST_BC_HEAD.unpack(reader.read(13))
+        unpacked = constants.st.ST_BC_HEAD.unpack(reader.read(13))
         # Because doc says it must be ignored, we don't check the reserved here.
         reader.read(4)
         self.__majorVersion = unpacked[0]
         self.__minorVersion = unpacked[1]
         self.__templateID = BCTemplateID(unpacked[2])
         self.__countOfFields = unpacked[3]
         self.__fieldInfoSize = unpacked[4] # Must be 16.
@@ -135,15 +135,15 @@
         return self.__templateID
 
 
 
 class FieldInfo:
     def __init__(self, data : bytes, extraInfo : bytes):
         self.__raw = data
-        unpacked = constants.ST_BC_FIELD_INFO.unpack(data)
+        unpacked = constants.st.ST_BC_FIELD_INFO.unpack(data)
         self.__textPropertyID = unpacked[0]
         self.__textFormat = BCTextFormat(unpacked[1])
         self.__labelFormat = BCLabelFormat(unpacked[2])
         self.__fontSize = unpacked[3]
         self.__labelOffset = unpacked[4]
         self.__labelText = None if unpacked[4] == 0xFFFE else BytesReader(extraInfo[unpacked[4]:]).readUtf16String()
         self.__valueFontColor = (bitwiseAdjustedAnd(unpacked[5], 0xFF),
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/entry_id.py` & `extract_msg-0.42.0/extract_msg/structures/entry_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
     def __init__(self, data : bytes):
         super().__init__(data)
         reader = BytesReader(data[20:])
         self.__folderType = MessageType(reader.readUnsignedShort())
         self.__databaseGuid = bytesToGuid(reader.read(16))
         # This entry is 6 bytes, so we pull some shenanigans to unpack it.
-        self.__globalCounter = constants.ST_LE_UI64.unpack(reader.read(6) + b'\x00\x00')
+        self.__globalCounter = constants.st.ST_LE_UI64.unpack(reader.read(6) + b'\x00\x00')
         reader.assertNull(2, 'Pad bytes were not 0.')
 
     @property
     def databaseGuid(self) -> str:
         """
         A GUID associated with the Store Object and corresponding to the
         ReplicaID field of the FID structure.
@@ -258,19 +258,19 @@
 
     def __init__(self, data : bytes):
         super().__init__(data)
         reader = BytesReader(data[20:])
         self.__messageType = MessageType(reader.readUnsignedShort())
         self.__folderDatabaseGuid = bytesToGuid(reader.read(16))
         # This entry is 6 bytes, so we pull some shenanigans to unpack it.
-        self.__folderGlobalCounter = constants.ST_LE_UI64.unpack(reader.read(6) + b'\x00\x00')
+        self.__folderGlobalCounter = constants.st.ST_LE_UI64.unpack(reader.read(6) + b'\x00\x00')
         reader.assertNull(2, 'Pad bytes were not 0.')
         self.__messageDatabaseGuid = bytesToGuid(reader.read(16))
         # This entry is 6 bytes, so we pull some shenanigans to unpack it.
-        self.__messageGlobalCounter = constants.ST_LE_UI64.unpack(reader.read(6) + b'\x00\x00')
+        self.__messageGlobalCounter = constants.st.ST_LE_UI64.unpack(reader.read(6) + b'\x00\x00')
         reader.assertNull(2, 'Pad bytes were not 0.')
         # Not sure why Microsoft decided to say "yes, let's do 2 6-byte integers
         # followed by 2 pad bits each" instead of just 2 8-byte integers with a
         # maximum value, but here we are.
 
     @property
     def folderDatabaseGuid(self) -> str:
@@ -449,15 +449,15 @@
 class PermanentEntryID(EntryID):
     """
     A Permanent EntryID structure, as defined in [MS-OXNSPI].
     """
 
     def __init__(self, data : bytes):
         super().__init__(data)
-        unpacked = constants.STPEID.unpack(data[:28])
+        unpacked = constants.st.STPEID.unpack(data[:28])
         if unpacked[0] != 0:
             raise TypeError(f'Not a PermanentEntryID (expected 0, got {unpacked[0]}).')
         self.__displayTypeString = DisplayType(unpacked[2])
         self.__distinguishedName = data[28:-1].decode('ascii') # Cut off the null character at the end and decode the data as ascii
 
     @property
     def displayTypeString(self) -> DisplayType:
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/misc_id.py` & `extract_msg-0.42.0/extract_msg/structures/misc_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     A Folder ID structure specified in [MS-OXCDATA].
     """
 
     __SIZE__ : int = 16
 
     def __init__(self, data : bytes):
         self.__rawData = data
-        self.__replicaID = constants.STUI16.unpack(data[:2])
+        self.__replicaID = constants.st.STUI16.unpack(data[:2])
         # This entry is 6 bytes, so we pull some shenanigans to unpack it.
-        self.__globalCounter = constants.STUI64.unpack(data[2:8] + b'\x00\x00')
+        self.__globalCounter = constants.st.STUI64.unpack(data[2:8] + b'\x00\x00')
 
     @property
     def globalCounter(self) -> int:
         """
         An unsigned integer identifying the folder within its Store object.
         """
         return self.__globalCounter
@@ -64,15 +64,15 @@
         self.__rawData = data
         reader = BytesReader(data)
         expectedBytes = b'\x04\x00\x00\x00\x82\x00\xE0\x00\x74\xC5\xB7\x10\x1A\x82\xE0\x08'
         errorMsg = 'Byte Array ID did not match for GlobalObjectID (got {actual}).'
         self.__byteArrayID = reader.assertRead(expectedBytes, errorMsg)
         self.__yh = reader.read(1)
         self.__yl = reader.read(1)
-        self.__year = constants.ST_BE_UI16.unpack(self.__yh + self.__yl)[0]
+        self.__year = constants.st.ST_BE_UI16.unpack(self.__yh + self.__yl)[0]
         self.__month = reader.readUnsignedByte()
         self.__day = reader.readUnsignedByte()
         self.__creationTime = filetimeToDatetime(reader.readUnsignedLong())
         reader.assertNull(8, 'Reserved was not set to null.')
         size = reader.readUnsignedInt()
         self.__data = reader.read(size)
 
@@ -137,17 +137,17 @@
     A Message ID structure, as defined in [MS-OXCDATA].
     """
 
     __SIZE__ : int = 8
 
     def __init__(self, data : bytes):
         self.__rawData = data
-        self.__replicaID = constants.STUI16.unpack(data[:2])
+        self.__replicaID = constants.st.STUI16.unpack(data[:2])
         # This entry is 6 bytes, so we pull some shenanigans to unpack it.
-        self.__globalCounter = constants.STUI64.unpack(data[2:8] + b'\x00\x00')
+        self.__globalCounter = constants.st.STUI64.unpack(data[2:8] + b'\x00\x00')
 
     @property
     def globalCounter(self) -> int:
         """
         An unsigned integer identifying the folder within its Store object.
         """
         return self.__globalCounter
@@ -188,15 +188,15 @@
         # According to the docs, the first byte being a 1 means it follows this
         # structure. A value of 0 means it does not.
         if data[0] != 1:
             raise TypeError('Not a standard ServerID.')
         self.__rawData = data
         self.__folderID = FolderID(data[1:9])
         self.__messageID = MessageID(data[9:17])
-        self.__instance = constants.STUI32.unpack(data[17:21])
+        self.__instance = constants.st.STUI32.unpack(data[17:21])
 
     @property
     def folderID(self) -> FolderID:
         """
         The folder the message will be in.
         """
         return self.__folderID
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/recurrence_pattern.py` & `extract_msg-0.42.0/extract_msg/structures/recurrence_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
         self.__slidingFlag = reader.readUnsignedInt()
         # This is just here to help shorten lines.
         RPTSW = RecurPatternTypeSpecificWeekday
         # This field changes depending on the recurrence type.
         if self.__patternType == RecurPatternType.DAY:
             self.__patternTypeSpecific = None
         elif self.__patternType == RecurPatternType.WEEK:
-            self.__patternTypeSpecific = RPTSW.fromBits(reader.readUnsignedInt())
+            self.__patternTypeSpecific = RPTSW(reader.readUnsignedInt())
         elif self.__patternType in (RecurPatternType.MONTH_NTH, RecurPatternType.HJ_MONTH_NTH):
             self.__patternTypeSpecific = reader.readUnsignedInt()
         else:
-            self.__patternTypeSpecific = (RPTSW.fromBits(reader.readUnsignedInt()),
+            self.__patternTypeSpecific = (RPTSW(reader.readUnsignedInt()),
                                           RecurMonthNthWeek(reader.readUnsignedInt()))
 
         self.__endType = RecurEndType.fromInt(reader.readUnsignedInt())
         self.__occurrenceCount = reader.readUnsignedInt()
         self.__firstDOW = RecurDOW(reader.readUnsignedInt())
         deletedInstanceCount = reader.readUnsignedInt()
         self.__deletedInstanceDates = tuple(reader.readUnsignedInt() for x in range(deletedInstanceCount))
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/report_tag.py` & `extract_msg-0.42.0/extract_msg/structures/report_tag.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/structures/system_time.py` & `extract_msg-0.42.0/extract_msg/structures/system_time.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def pack(self) -> bytes:
         """
         Packs the current data into bytes.
         """
-        return constants.ST_SYSTEMTIME.pack(self.year, self.month,
+        return constants.st.ST_SYSTEMTIME.pack(self.year, self.month,
                                             self.dayOfWeek, self.day, self.hour,
                                             self.minute, self.second,
                                             self.milliseconds)
 
     def unpack(self, data : bytes) -> None:
         """
         Fills out the fields of this instance by unpacking the bytes.
         """
-        unpacked = constants.ST_SYSTEMTIME.unpack(data)
+        unpacked = constants.st.ST_SYSTEMTIME.unpack(data)
         self.year = unpacked[0]
         self.month = unpacked[1]
         self.dayOfWeek = unpacked[2]
         self.day = unpacked[3]
         self.hour = unpacked[4]
         self.minute = unpacked[5]
         self.second = unpacked[6]
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/time_zone_definition.py` & `extract_msg-0.42.0/extract_msg/structures/time_zone_definition.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.5/extract_msg/structures/time_zone_struct.py` & `extract_msg-0.42.0/extract_msg/structures/time_zone_struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class TimeZoneStruct:
     """
     A TimeZoneStruct, as specified in [MS-OXOCAL].
     """
 
     def __init__(self, data : bytes):
         self.__rawData = data
-        unpacked = constants.ST_TZ.unpack(data)
+        unpacked = constants.st.ST_TZ.unpack(data)
         self.__bias = unpacked[0]
         self.__standardBias = unpacked[1]
         self.__daylightBias = unpacked[2]
         self.__standardYear = unpacked[3]
         self.__standardDate = SystemTime(unpacked[4])
         self.__daylightYear = unpacked[5]
         self.__daylightDate = SystemTime(unpacked[6])
```

### Comparing `extract_msg-0.41.5/extract_msg/structures/tz_rule.py` & `extract_msg-0.42.0/extract_msg/structures/tz_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def __init__(self, data : bytes):
         self.__rawData = data
         reader = BytesReader(data)
         self.__majorVersion = reader.readByte()
         self.__minorVersion = reader.readByte()
         reader.assertRead(b'\x3E\x00')
-        self.__flags = TZFlag.fromBits(reader.readUnsignedShort())
+        self.__flags = TZFlag(reader.readUnsignedShort())
         self.__year = reader.readShort()
         # We *should* be doing this, but Outlook is violating the standard so...
         #reader.assertNull(14)
         self.__bias = reader.readInt()
         self.__standardBias = reader.readInt()
         self.__daylightBias = reader.readInt()
         self.__standardDate = SystemTime(reader.read(16))
```

### Comparing `extract_msg-0.41.5/extract_msg/task_request.py` & `extract_msg-0.42.0/extract_msg/msg_classes/task_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 __all__ = [
     'TaskRequest',
 ]
 
 
+import functools
 import logging
 
 from typing import Optional
 
-from . import constants
-from .enums import ErrorBehavior, TaskMode, TaskRequestType
-from .exceptions import StandardViolationError
+from .. import constants
+from ..enums import ErrorBehavior, TaskMode, TaskRequestType
+from ..exceptions import StandardViolationError
 from .message_base import MessageBase
 from .task import Task
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
@@ -49,63 +50,61 @@
         property.
         """
         # So this is rather weird. Looks like TaskRequest does not rely on
         # headers at all, simply using the body itself for all the data to
         # print. So I guess we just return None and handle that.
         return None
 
-    @property
+    @functools.cached_property
     def processed(self) -> bool:
         """
         Indicates whether a client has already processed a received task
         communication.
         """
-        return self._ensureSetProperty('_processed', '7D01000B', overrideClass = bool, preserveNone = False)
+        return self._getPropertyAs('7D01000B', bool, False)
 
-    @property
+    @functools.cached_property
     def taskMode(self) -> Optional[TaskMode]:
         """
         The assignment status of the embedded Task object.
         """
-        return self._ensureSetNamed('_taskMode', '8518', constants.PSETID_COMMON, overrideClass = TaskMode)
+        return self._getNamedAs('8518', constants.ps.PSETID_COMMON, TaskMode)
 
-    @property
-    def taskObject(self) -> Task:
+    @functools.cached_property
+    def taskObject(self) -> Optional[Task]:
         """
         The task object embedded in this Task Request object.
 
         This function does all of the most basic validation, and so will log
         most issues or throw exceptions if there are too many problems.
 
         :raises StandardViolationError: A standard was blatently violated in a
             way that program does not tolerate.
         """
-        try:
-            return self._taskObject
-        except AttributeError:
-            # Get the task object.
-            #
-            # The task object MUST be the first attachment, but we will be
-            # lenient and allow it to be in any position. It not existing,
-            # however, will not be tolerated.
-            task = next(((index, att) for index, att in self.attachments if isinstance(att.data, Task)), None)
-            if task is None:
-                if self.errorBehavior & ErrorBehavior.STANDARDS_VIOLATION:
-                    logger.error('Task object not found on TaskRequest object.')
-                    return
-                raise StandardViolationError('Task object not found on TaskRequest object.')
-
-            # We know we have the task, let's make sure it's at index 0. If not,
-            # log it.
-            if task[0] != 0:
-                logger.warning('Embedded task object was not located at index 0.')
+        # Get the task object.
+        #
+        # The task object MUST be the first attachment, but we will be
+        # lenient and allow it to be in any position. It not existing,
+        # however, will not be tolerated.
+        task = next(((index, att) for index, att in self.attachments if isinstance(att.data, Task)), None)
+
+        if task is None:
+            if ErrorBehavior.STANDARDS_VIOLATION in self.errorBehavior:
+                logger.error('Task object not found on TaskRequest object.')
+                return
+            raise StandardViolationError('Task object not found on TaskRequest object.')
+
+        # We know we have the task, let's make sure it's at index 0. If not,
+        # log it.
+        if task[0] != 0:
+            logger.warning('Embedded task object was not located at index 0.')
 
-            self._taskObject = task[1]
+        self._taskObject = task[1]
 
-            return self._taskObject
+        return self._taskObject
 
-    @property
+    @functools.cached_property
     def taskRequestType(self) -> TaskRequestType:
         """
         The type of task request.
         """
-        return self._ensureSet('_taskRequestType', '__substg1.0_001A', TaskRequestType.fromClassType)
+        return self._getStreamAs('__substg1.0_001A', TaskRequestType.fromClassType)
```

### Comparing `extract_msg-0.41.5/extract_msg/utils.py` & `extract_msg-0.42.0/extract_msg/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,101 @@
 from __future__ import annotations
 
+
 """
 Utility functions of extract_msg.
 """
 
 
 __all__ = [
-    'addNumToDir', 'addNumToZipDir', 'bitwiseAdjust', 'bitwiseAdjustedAnd',
-    'bytesToGuid', 'ceilDiv', 'cloneOleFile', 'createZipOpen',
-    'dictGetCasedKey', 'divide', 'filetimeToDatetime', 'findWk',
-    'fromTimeStamp', 'getCommandArgs', 'getEncodingName', 'getFullClassName',
-    'hasLen', 'htmlSanitize', 'inputToBytes', 'inputToMsgPath', 'inputToString',
-    'isEncapsulatedRtf', 'isEmptyString', 'knownMsgClass', 'filetimeToUtc',
-    'msgPathToString', 'openMsg', 'openMsgBulk', 'parseType', 'prepareFilename',
-    'properHex', 'roundUp', 'rtfSanitizeHtml', 'rtfSanitizePlain',
-    'setupLogging', 'tryGetMimetype', 'unsignedToSignedInt', 'unwrapMsg',
-    'unwrapMultipart', 'validateHtml', 'verifyPropertyId', 'verifyType',
+    'addNumToDir',
+    'addNumToZipDir',
+    'bitwiseAdjust',
+    'bitwiseAdjustedAnd',
+    'bytesToGuid',
+    'ceilDiv',
+    'cloneOleFile',
+    'createZipOpen',
+    'dictGetCasedKey',
+    'divide',
+    'filetimeToDatetime',
+    'filetimeToUtc',
+    'findWk',
+    'fromTimeStamp',
+    'getCommandArgs',
+    'hasLen',
+    'htmlSanitize',
+    'inputToBytes',
+    'inputToMsgPath',
+    'inputToString',
+    'isEncapsulatedRtf',
+    'isEmptyString',
+    'makeWeakRef',
+    'msgPathToString',
+    'parseType',
+    'prepareFilename',
+    'properHex',
+    'roundUp',
+    'rtfSanitizeHtml',
+    'rtfSanitizePlain',
+    'setupLogging',
+    'tryGetMimetype',
+    'unsignedToSignedInt',
+    'unwrapMsg',
+    'unwrapMultipart',
+    'validateHtml',
+    'verifyPropertyId',
+    'verifyType',
     'windowsUnicode',
 ]
 
 
 import argparse
-import codecs
 import collections
 import copy
 import datetime
 import email.header
 import email.message
 import email.policy
 import glob
 import json
 import logging
 import logging.config
 import os
 import pathlib
 import shutil
 import struct
-# Not actually sure if this needs to be here for the logging, so just in case.
-import sys
+import weakref
 import zipfile
 
 import bs4
 import olefile
 import tzlocal
 
 from html import escape as htmlEscape
-from typing import Any, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import Any, Dict, List, Optional, TypeVar, TYPE_CHECKING, Union
 
 from . import constants
 from .enums import AttachmentType
 from .exceptions import (
         ConversionError, ExecutableNotFound, IncompatibleOptionsError,
-        InvalidFileFormatError, InvaildPropertyIdError, TZError,
-        UnknownCodepageError, UnknownTypeError, UnrecognizedMSGTypeError,
-        UnsupportedEncodingError, UnsupportedMSGTypeError
+        InvaildPropertyIdError, TZError, UnknownTypeError
     )
 
 
 # Allow for nice type checking.
 if TYPE_CHECKING:
-    from .msg import MSGFile
+    from .msg_classes.msg import MSGFile
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 logging.addLevelName(5, 'DEVELOPER')
 
+_T = TypeVar("_T")
+
 
 def addNumToDir(dirName : pathlib.Path) -> Optional[pathlib.Path]:
     """
     Attempt to create the directory with a '(n)' appended.
     """
     for i in range(2, 100):
         try:
@@ -123,15 +150,15 @@
     return (inp & mask) >> bin(mask)[::-1].index('1')
 
 
 def bytesToGuid(bytesInput : bytes) -> str:
     """
     Converts a bytes instance to a GUID.
     """
-    guidVals = constants.ST_GUID.unpack(bytesInput)
+    guidVals = constants.st.ST_GUID.unpack(bytesInput)
     return f'{{{guidVals[0]:08X}-{guidVals[1]:04X}-{guidVals[2]:04X}-{guidVals[3][:2].hex().upper()}-{guidVals[3][2:].hex().upper()}}}'
 
 
 def ceilDiv(n : int, d : int) -> int:
     """
     Returns the int from the ceil division of n / d.
     ONLY use ints as inputs to this function.
@@ -375,14 +402,17 @@
                         help='Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with --out-name.')
     # --skip-embedded
     parser.add_argument('--skip-embedded', dest='skipEmbedded', action='store_true',
                         help='Skips all embedded MSG files when saving attachments.')
     # --extract-embedded
     parser.add_argument('--extract-embedded', dest='extractEmbedded', action='store_true',
                         help='Extracts the embedded MSG files as MSG files instead of running their save functions.')
+    # --overwrite-existing
+    parser.add_argument('--overwrite-existing', dest='overwriteExisting', action='store_true',
+                        help='Disables filename conflict resolution code for attachments when saving a file, causing files to be overwriten if two attachments with the same filename are on an MSG file.')
     # --skip-not-implemented
     parser.add_argument('--skip-not-implemented', '--skip-ni', dest='skipNotImplemented', action='store_true',
                         help='Skips any attachments that are not implemented, allowing saving of the rest of the message.')
     # --out-name NAME
     inputFormat.add_argument('--out-name', dest='outName',
                         help='Name to be used with saving the file output. Cannot be used if you are saving more than one file.')
     # --glob
@@ -465,35 +495,14 @@
 
     # If --no-folders is turned on but --attachments-only is not, error.
     if options.noFolders and not options.attachmentsOnly:
         raise ValueError('--no-folders requires the --attachments-only option.')
 
     return options
 
-
-def getEncodingName(codepage : int) -> str:
-    """
-    Returns the name of the encoding with the specified codepage.
-
-    :raises UnknownCodepageError: if the codepage is unrecognized.
-    :raises UnsupportedEncodingError: if the codepage is not supported.
-    """
-    if codepage not in constants.CODE_PAGES:
-        raise UnknownCodepageError(str(codepage))
-    try:
-        codecs.lookup(constants.CODE_PAGES[codepage])
-        return constants.CODE_PAGES[codepage]
-    except LookupError:
-        raise UnsupportedEncodingError(f'The codepage {codepage} ({constants.CODE_PAGES[codepage]}) is not currently supported by your version of Python.')
-
-
-def getFullClassName(inp) -> str:
-    return inp.__class__.__module__ + '.' + inp.__class__.__name__
-
-
 def hasLen(obj) -> bool:
     """
     Checks if :param obj: has a __len__ attribute.
     """
     return hasattr(obj, '__len__')
 
 
@@ -505,15 +514,15 @@
     # First step, do a basic escape of the HTML.
     inp = htmlEscape(inp)
 
     # Change newlines to <br/> to they won't be ignored.
     inp = inp.replace('\r\n', '\n').replace('\n', '<br/>')
 
     # Escape long sections of spaces to ensure they won't be ignored.
-    inp = constants.RE_HTML_SAN_SPACE.sub((lambda spaces : '&nbsp;' * len(spaces.group(0))),inp)
+    inp = constants.re.HTML_SAN_SPACE.sub((lambda spaces : '&nbsp;' * len(spaces.group(0))),inp)
 
     return inp
 
 
 def inputToBytes(stringInputVar, encoding) -> bytes:
     """
     Converts the input into bytes.
@@ -584,35 +593,30 @@
 def isEmptyString(inp : str) -> bool:
     """
     Returns true if the input is None or is an Empty string.
     """
     return (inp == '' or inp is None)
 
 
-def knownMsgClass(classType : str) -> bool:
+def filetimeToUtc(inp : int) -> float:
     """
-    Checks if the specified class type is recognized by the module. Usually used
-    for checking if a type is simply unsupported rather than unknown.
+    Converts a FILETIME into a unix timestamp.
     """
-    classType = classType.lower()
-    if classType == 'ipm':
-        return True
-
-    for item in constants.KNOWN_CLASS_TYPES:
-        if classType.startswith(item):
-            return True
-
-    return False
+    return (inp - 116444736000000000) / 10000000.0
 
 
-def filetimeToUtc(inp : int) -> float:
+def makeWeakRef(obj : Optional[_T]) -> Optional[weakref.ReferenceType[_T]]:
     """
-    Converts a FILETIME into a unix timestamp.
+    Attempts to return a weak reference to the object, returning None if not
+    possible.
     """
-    return (inp - 116444736000000000) / 10000000.0
+    try:
+        return weakref.ref(obj)
+    except TypeError:
+        return None
 
 
 def msgPathToString(inp) -> str:
     """
     Converts an MSG path (one of the internal paths inside an MSG file) into a
     string.
     """
@@ -620,173 +624,14 @@
         return None
     if isinstance(inp, (list, tuple)):
         inp = '/'.join(inp)
     inp.replace('\\', '/')
     return inp
 
 
-def openMsg(path, **kwargs) -> MSGFile:
-    """
-    Function to automatically open an MSG file and detect what type it is.
-
-    :param path: Path to the msg file in the system or is the raw msg file.
-    :param prefix: Used for extracting embeded msg files inside the main one.
-        Do not set manually unless you know what you are doing.
-    :param parentMsg: Used for syncronizing named properties instances. Do not
-        set this unless you know what you are doing.
-    :param attachmentClass: Optional, the class the Message object will use for
-        attachments. You probably should not change this value unless you know
-        what you are doing.
-    :param signedAttachmentClass: Optional, the class the object will use for
-        signed attachments.
-    :param filename: Optional, the filename to be used by default when saving.
-    :param delayAttachments: Optional, delays the initialization of attachments
-        until the user attempts to retrieve them. Allows MSG files with bad
-        attachments to be initialized so the other data can be retrieved.
-    :param overrideEncoding: Optional, overrides the specified encoding of the
-        MSG file.
-    :param attachmentErrorBehavior: Optional, the behaviour to use in the event
-        of an error when parsing the attachments.
-    :param recipientSeparator: Optional, Separator string to use between
-        recipients.
-    :param ignoreRtfDeErrors: Optional, specifies that any errors that occur
-        from the usage of RTFDE should be ignored (default: False).
-
-    If :param strict: is set to `True`, this function will raise an exception
-    when it cannot identify what MSGFile derivitive to use. Otherwise, it will
-    log the error and return a basic MSGFile instance.
-
-    :raises UnsupportedMSGTypeError: if the type is recognized but not suppoted.
-    :raises UnrecognizedMSGTypeError: if the type is not recognized.
-    """
-    from .appointment import AppointmentMeeting
-    from .contact import Contact
-    from .meeting_cancellation import MeetingCancellation
-    from .meeting_exception import MeetingException
-    from .meeting_forward import MeetingForwardNotification
-    from .meeting_request import MeetingRequest
-    from .meeting_response import MeetingResponse
-    from .message import Message
-    from .msg import MSGFile
-    from .message_signed import MessageSigned
-    from .post import Post
-    from .task import Task
-    from .task_request import TaskRequest
-
-    # When the initial MSG file is opened, it should *always* delay attachments
-    # so it can get the main class type. We only need to load them after that
-    # if we are directly returning the MSGFile instance *and* delayAttachments
-    # is False.
-    #
-    # So first let's store the original value.
-    delayAttachments = kwargs.get('delayAttachments', False)
-    kwargs['delayAttachments'] = True
-
-    msg = MSGFile(path, **kwargs)
-
-    # Restore the option in the kwargs so we don't have to worry about it.
-    kwargs['delayAttachments'] = delayAttachments
-
-    # After rechecking the docs, all comparisons should be case-insensitive, not
-    # case-sensitive. My reading ability is great.
-    #
-    # Also after consideration, I realized we need to be very careful here, as
-    # other file types (like doc, ppt, etc.) might open but not return a class
-    # type. If the stream is not found, classType returns None, which has no
-    # lower function. So let's make sure we got a good return first.
-    if not msg.classType:
-        if kwargs.get('strict', True):
-            raise InvalidFileFormatError('File was confirmed to be an olefile, but was not an MSG file.')
-        else:
-            # If strict mode is off, we'll just return an MSGFile anyways.
-            logging.critical('Received file that was an olefile but was not an MSG file. Returning MSGFile anyways because strict mode is off.')
-            return msg
-    classType = msg.classType.lower()
-    # Put the message class first as it is most common.
-    if classType.startswith('ipm.note') or classType.startswith('report'):
-        msg.close()
-        if classType.endswith('smime.multipartsigned') or classType.endswith('smime'):
-            return MessageSigned(path, **kwargs)
-        else:
-            return Message(path, **kwargs)
-    elif classType.startswith('ipm.appointment'):
-        msg.close()
-        return AppointmentMeeting(path, **kwargs)
-    elif classType.startswith('ipm.contact') or classType.startswith('ipm.distlist'):
-        msg.close()
-        return Contact(path, **kwargs)
-    elif classType.startswith('ipm.post'):
-        msg.close()
-        return Post(path, **kwargs)
-    elif classType.startswith('ipm.schedule.meeting.request'):
-        msg.close()
-        return MeetingRequest(path, **kwargs)
-    elif classType.startswith('ipm.schedule.meeting.canceled'):
-        msg.close()
-        return MeetingCancellation(path, **kwargs)
-    elif classType.startswith('ipm.schedule.meeting.notification.forward'):
-        msg.close()
-        return MeetingForwardNotification(path, **kwargs)
-    elif classType.startswith('ipm.schedule.meeting.resp'):
-        msg.close()
-        return MeetingResponse(path, **kwargs)
-    elif classType.startswith('ipm.taskrequest'):
-        msg.close()
-        return TaskRequest(path, **kwargs)
-    elif classType.startswith('ipm.task'):
-        msg.close()
-        return Task(path, **kwargs)
-    elif classType.startswith('ipm.ole.class.{00061055-0000-0000-c000-000000000046}'):
-        # Exception objects have a weird class type.
-        msg.close()
-        return MeetingException(path, **kwargs)
-    elif classType == 'ipm':
-        # Unspecified format. It should be equal to this and not just start with
-        # it.
-        if not delayAttachments:
-            msg.attachments
-        return msg
-    elif kwargs.get('strict', True):
-        # Because we are closing it, we need to store it in a variable first.
-        ct = msg.classType
-        msg.close()
-        if knownMsgClass(classType):
-            raise UnsupportedMSGTypeError(f'MSG type "{ct}" currently is not supported by the module. If you would like support, please make a feature request.')
-        raise UnrecognizedMSGTypeError(f'Could not recognize msg class type "{ct}".')
-    else:
-        logger.error(f'Could not recognize msg class type "{msg.classType}". This most likely means it hasn\'t been implemented yet, and you should ask the developers to add support for it.')
-        if not delayAttachments:
-            msg.attachments
-        return msg
-
-
-def openMsgBulk(path, **kwargs) -> Union[List[MSGFile], Tuple[Exception, Union[str, bytes]]]:
-    """
-    Takes the same arguments as openMsg, but opens a collection of msg files
-    based on a wild card. Returns a list if successful, otherwise returns a
-    tuple.
-
-    :param ignoreFailures: If this is True, will return a list of all successful
-        files, ignoring any failures. Otherwise, will close all that
-        successfully opened, and return a tuple of the exception and the path of
-        the file that failed.
-    """
-    files = []
-    for x in glob.glob(str(path)):
-        try:
-            files.append(openMsg(x, **kwargs))
-        except Exception as e:
-            if not kwargs.get('ignoreFailures', False):
-                for msg in files:
-                    msg.close()
-                return (e, x)
-
-    return files
-
-
 def parseType(_type : int, stream, encoding, extras):
     """
     Converts the data in :param stream: to a much more accurate type, specified
     by :param _type:.
     :param _type: the data's type.
     :param stream: is the data to be converted.
     :param encoding: is the encoding to be used for regular strings.
@@ -804,62 +649,62 @@
         pass
     elif _type == 0x0001:  # PtypNull
         if value != b'\x00\x00\x00\x00\x00\x00\x00\x00':
             # DEBUG
             logger.warning('Property type is PtypNull, but is not equal to 0.')
         return None
     elif _type == 0x0002:  # PtypInteger16
-        return constants.STI16.unpack(value)[0]
+        return constants.st.STI16.unpack(value)[0]
     elif _type == 0x0003:  # PtypInteger32
-        return constants.STI32.unpack(value)[0]
+        return constants.st.STI32.unpack(value)[0]
     elif _type == 0x0004:  # PtypFloating32
-        return constants.STF32.unpack(value)[0]
+        return constants.st.STF32.unpack(value)[0]
     elif _type == 0x0005:  # PtypFloating64
-        return constants.STF64.unpack(value)[0]
+        return constants.st.STF64.unpack(value)[0]
     elif _type == 0x0006:  # PtypCurrency
-        return (constants.STI64.unpack(value)[0]) / 10000.0
+        return (constants.st.STI64.unpack(value)[0]) / 10000.0
     elif _type == 0x0007:  # PtypFloatingTime
-        value = constants.STF64.unpack(value)[0]
+        value = constants.st.STF64.unpack(value)[0]
         return constants.PYTPFLOATINGTIME_START + datetime.timedelta(days = value)
     elif _type == 0x000A:  # PtypErrorCode
         from .enums import ErrorCode, ErrorCodeType
-        value = constants.STUI32.unpack(value)[0]
+        value = constants.st.STUI32.unpack(value)[0]
         try:
             value = ErrorCodeType(value)
         except ValueError:
             logger.warning(f'Error type found that was not from Additional Error Codes. Value was {value}. You should report this to the developers.')
             # So here, the value should be from Additional Error Codes, but it
             # wasn't. So we are just returning the int. However, we want to see
             # if it is a normal error code.
             try:
                 logger.warning(f'REPORT TO DEVELOPERS: Error type of {ErrorCode(value)} was found.')
             except ValueError:
                 pass
         return value
     elif _type == 0x000B:  # PtypBoolean
-        return constants.ST3.unpack(value)[0] == 1
+        return constants.st.ST3.unpack(value)[0] == 1
     elif _type == 0x000D:  # PtypObject/PtypEmbeddedTable
         # TODO parsing for this.
         # Wait, that's the extension for an attachment folder, so parsing this
         # might not be as easy as we would hope. The function may be released
         # without support for this.
         raise NotImplementedError('Current version of extract-msg does not support the parsing of PtypObject/PtypEmbeddedTable in this function.')
     elif _type == 0x0014:  # PtypInteger64
-        return constants.STI64.unpack(value)[0]
+        return constants.st.STI64.unpack(value)[0]
     elif _type == 0x001E:  # PtypString8
         return value.decode(encoding)
     elif _type == 0x001F:  # PtypString
         return value.decode('utf-16-le')
     elif _type == 0x0040:  # PtypTime
-        rawTime = constants.ST3.unpack(value)[0]
+        rawTime = constants.st.ST3.unpack(value)[0]
         return filetimeToDatetime(rawTime)
     elif _type == 0x0048:  # PtypGuid
         return bytesToGuid(value)
     elif _type == 0x00FB:  # PtypServerId
-        count = constants.STUI16.unpack(value[:2])
+        count = constants.st.STUI16.unpack(value[:2])
         # If the first byte is a 1 then it uses the ServerID structure.
         if value[3] == 1:
             from .structures.misc_id import ServerID
             return ServerID(value)
         else:
             return (count, value[2:count + 2])
     elif _type == 0x00FD:  # PtypRestriction
@@ -880,40 +725,40 @@
                 logger.warning(f'Error while parsing multiple type. Expected {lengthLengths} stream{"s" if lengthLengths != 1 else ""}, got {lengthExtras}. Ignoring.')
             for x, y in enumerate(extras):
                 if lengths[x] != len(y):
                     logger.warning(f'Error while parsing multiple type. Expected length {lengths[x]}, got {len(y)}. Ignoring.')
             return ret
         elif _type == 0x1102: # PtypMultipleBinary
             ret = copy.deepcopy(extras)
-            lengths = tuple(constants.STUI32.unpack(stream[pos*8:(pos+1)*8])[0] for pos in range(len(stream) // 8))
+            lengths = tuple(constants.st.STUI32.unpack(stream[pos*8:(pos+1)*8])[0] for pos in range(len(stream) // 8))
             lengthLengths = len(lengths)
             if lengthLengths > lengthExtras:
                 logger.warning(f'Error while parsing multiple type. Expected {lengthLengths} stream{"s" if lengthLengths != 1 else ""}, got {lengthExtras}. Ignoring.')
             for x, y in enumerate(extras):
                 if lengths[x] != len(y):
                     logger.warning(f'Error while parsing multiple type. Expected length {lengths[x]}, got {len(y)}. Ignoring.')
             return ret
         elif _type in (0x1002, 0x1003, 0x1004, 0x1005, 0x1007, 0x1014, 0x1040, 0x1048):
             if stream != len(extras):
                 logger.warning(f'Error while parsing multiple type. Expected {stream} entr{"y" if stream == 1 else "ies"}, got {len(extras)}. Ignoring.')
             if _type == 0x1002: # PtypMultipleInteger16
-                return tuple(constants.STMI16.unpack(x)[0] for x in extras)
+                return tuple(constants.st.STMI16.unpack(x)[0] for x in extras)
             if _type == 0x1003: # PtypMultipleInteger32
-                return tuple(constants.STMI32.unpack(x)[0] for x in extras)
+                return tuple(constants.st.STMI32.unpack(x)[0] for x in extras)
             if _type == 0x1004: # PtypMultipleFloating32
-                return tuple(constants.STMF32.unpack(x)[0] for x in extras)
+                return tuple(constants.st.STMF32.unpack(x)[0] for x in extras)
             if _type == 0x1005: # PtypMultipleFloating64
-                return tuple(constants.STMF64.unpack(x)[0] for x in extras)
+                return tuple(constants.st.STMF64.unpack(x)[0] for x in extras)
             if _type == 0x1007: # PtypMultipleFloatingTime
-                values = tuple(constants.STMF64.unpack(x)[0] for x in extras)
+                values = tuple(constants.st.STMF64.unpack(x)[0] for x in extras)
                 return tuple(constants.PYTPFLOATINGTIME_START + datetime.timedelta(days = amount) for amount in values)
             if _type == 0x1014: # PtypMultipleInteger64
-                return tuple(constants.STMI64.unpack(x)[0] for x in extras)
+                return tuple(constants.st.STMI64.unpack(x)[0] for x in extras)
             if _type == 0x1040: # PtypMultipleTime
-                return tuple(filetimeToUtc(constants.ST3.unpack(x)[0]) for x in extras)
+                return tuple(filetimeToUtc(constants.st.ST3.unpack(x)[0]) for x in extras)
             if _type == 0x1048: # PtypMultipleGuid
                 return tuple(bytesToGuid(x) for x in extras)
         else:
             raise NotImplementedError(f'Parsing for type {_type} has not yet been implmented. If you need this type, please create a new issue labeled "NotImplementedError: parseType {_type}".')
     return value
 
 
@@ -1018,15 +863,15 @@
     :param env_key: Environment variable name to search for, for setting logfile
         path.
     :param enableFileLogging: Whether to use a file to log or not.
 
     Returns:
         bool: True if the configuration file was found and applied, False otherwise
     """
-    shippedConfig = pathlib.Path(__file__).parent / 'logging-config'
+    shippedConfig = pathlib.Path(__file__).parent / 'data' / 'logging-config'
     if os.name == 'nt':
         null = 'NUL'
         shippedConfig /= 'logging-nt.json'
     elif os.name == 'posix':
         null = '/dev/null'
         shippedConfig /= 'logging-posix.json'
     # Find logging.json if not provided
@@ -1123,27 +968,27 @@
 
     :raises ValueError: The number was not valid.
     """
     if uInt > 0xFFFFFFFF:
         raise ValueError('Value is too large.')
     if uInt < 0:
         raise ValueError('Value is already signed.')
-    return constants.STI32.unpack(constants.STUI32.pack(uInt))[0]
+    return constants.st.STI32.unpack(constants.st.STUI32.pack(uInt))[0]
 
 
 def unwrapMsg(msg : MSGFile) -> Dict:
     """
     Takes a recursive message-attachment structure and unwraps it into a linear
     dictionary for easy iteration. Dictionary contains 4 keys: "attachments" for
     main message attachments, not including embedded MSG files, "embedded" for
     attachments representing embedded MSG files, "msg" for all MSG files
     (including the original in the first index), and "raw_attachments" for raw
     attachments from signed messages.
     """
-    from .message_signed_base import MessageSignedBase
+    from .msg_classes import MessageSignedBase
 
     # Here is where we store main attachments.
     attachments = []
     # Here is where we are going to store embedded msg files.
     msgFiles = [msg]
     # Here is where we store embedded attachments.
     embedded = []
@@ -1163,17 +1008,17 @@
         # Remove the last item from the list of things to process, and store it
         # in `currentItem`. We will be processing it in the for loop.
         currentItem = toProcess.popleft()
         # iterate through the attachments and
         for att in currentItem.attachments:
             # If it is a regular attachment, add it to the list. Otherwise, add
             # it to be processed
-            if att.type in (AttachmentType.DATA, AttachmentType.SIGNED):
+            if att.type not in (AttachmentType.MSG, AttachmentType.SIGNED_EMBEDDED):
                 attachments.append(att)
-            elif att.type is AttachmentType.MSG:
+            else:
                 # Here we do two things. The first is we store it to the output
                 # so we can return it. The second is we add it to the processing
                 # list. The reason this is two steps is because we need to be
                 # able to remove items from the processing list, but can't
                 # do that from the output.
                 embedded.append(att)
                 msgFiles.append(att.data)
@@ -1311,14 +1156,15 @@
 
     return {
         'attachments': attachments,
         'plain_body': plainBody,
         'html_body': htmlBody,
     }
 
+
 def validateHtml(html : bytes) -> bool:
     """
     Checks whether the HTML is considered valid. To be valid, the HTML must, at
     minimum, contain an <html> tag, a <body> tag, and closing tags for each.
     """
     bs = bs4.BeautifulSoup(html, 'html.parser')
     if not bs.find('html') or not bs.find('body'):
@@ -1355,7 +1201,8 @@
     if _type is not None:
         if (_type not in constants.VARIABLE_LENGTH_PROPS_STRING) and (_type not in constants.FIXED_LENGTH_PROPS_STRING):
             raise UnknownTypeError(f'Unknown type {_type}.')
 
 
 def windowsUnicode(string) -> Optional[str]:
     return str(string, 'utf-16-le') if string is not None else None
+
```

### Comparing `extract_msg-0.41.5/extract_msg.egg-info/PKG-INFO` & `extract_msg-0.42.0/extract_msg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: extract-msg
-Version: 0.41.5
+Version: 0.42.0
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: mime
+Provides-Extra: image
 License-File: LICENSE.txt
 
 |License: GPL v3| |PyPI3| |PyPI2|
 
 extract-msg
 =============
 
@@ -70,70 +71,62 @@
 
 
 #########REWRITE COMMAND LINE USAGE#############
 Currently, the README is in the process of being redone. For now, please
 refer to the usage information provided from the program's help dialog:
 ::
 
-    usage: extract_msg [-h] [--use-content-id] [--validate] [--json] [--file-logging] [-v] [--log LOG] [--config CONFIGPATH]
-                       [--out OUTPATH] [--use-filename] [--dump-stdout] [--html] [--pdf] [--wk-path WKPATH]
-                       [--wk-options [WKOPTIONS ...]] [--prepared-html] [--charset CHARSET] [--raw] [--rtf] [--allow-fallback]
-                       [--skip-body-not-found] [--zip ZIP] [--save-header] [--attachments-only] [--skip-hidden] [--no-folders]
-                       [--skip-embedded] [--extract-embedded] [--skip-not-implemented] [--out-name OUTNAME | --glob] [--ignore-rtfde]
-                       [--progress]
-                       msg [msg ...]
-
-    extract_msg: Extracts emails and attachments saved in Microsoft Outlook's .msg files. https://github.com/TeamMsgExtractor/msg-
-    extractor
-
-    positional arguments:
-      msg                   An MSG file to be parsed.
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      --use-content-id, --cid
-                            Save attachments by their Content ID, if they have one. Useful when working with the HTML body.
-      --validate            Turns on file validation mode. Turns off regular file output.
-      --json                Changes to write output files as json.
-      --file-logging        Enables file logging. Implies --verbose level 1.
-      -v, --verbose         Turns on console logging. Specify more than once for higher verbosity.
-      --log LOG             Set the path to write the file log to.
-      --config CONFIGPATH   Set the path to load the logging config from.
-      --out OUTPATH         Set the folder to use for the program output. (Default: Current directory)
-      --use-filename        Sets whether the name of each output is based on the msg filename.
-      --dump-stdout         Tells the program to dump the message body (plain text) to stdout. Overrides saving arguments.
-      --html                Sets whether the output should be HTML. If this is not possible, will error.
-      --pdf                 Saves the body as a PDF. If this is not possible, will error.
-      --wk-path WKPATH      Overrides the path for finding wkhtmltopdf.
-      --wk-options [WKOPTIONS ...]
-                            Sets additional options to be used in wkhtmltopdf. Should be a series of options and values, replacing the -
-                            or -- in the beginning with + or ++, respectively. For example: --wk-options "+O Landscape"
-      --prepared-html       When used in conjunction with --html, sets whether the HTML output should be prepared for embedded
-                            attachments.
-      --charset CHARSET     Character set to use for the prepared HTML in the added tag. (Default: utf-8)
-      --raw                 Sets whether the output should be raw. If this is not possible, will error.
-      --rtf                 Sets whether the output should be RTF. If this is not possible, will error.
-      --allow-fallback      Tells the program to fallback to a different save type if the selected one is not possible.
-      --skip-body-not-found
-                            Skips saving the body if the body cannot be found, rather than throwing an error.
-      --zip ZIP             Path to use for saving to a zip file.
-      --save-header         Store the header in a separate file.
-      --attachments-only    Specify to only save attachments from an msg file.
-      --skip-hidden         Skips any attachment marked as hidden (usually ones embedded in the body).
-      --no-folders          Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with
-                            --out-name.
-      --skip-embedded       Skips all embedded MSG files when saving attachments.
-      --extract-embedded    Extracts the embedded MSG files as MSG files instead of running their save functions.
-      --skip-not-implemented, --skip-ni
-                            Skips any attachments that are not implemented, allowing saving of the rest of the message.
-      --out-name OUTNAME    Name to be used with saving the file output. Cannot be used if you are saving more than one file.
-      --glob, --wildcard    Interpret all paths as having wildcards. Incompatible with --out-name.
-      --ignore-rtfde        Ignores all errors thrown from RTFDE when trying to save. Useful for allowing fallback to continue when an
-                            exception happens.
-      --progress            Shows what file the program is currently working on during it's progress.
+     usage: extract_msg [-h] [--use-content-id] [--json] [--file-logging] [-v] [--log LOG] [--config CONFIGPATH] [--out OUTPATH] [--use-filename] [--dump-stdout] [--html] [--pdf] [--wk-path WKPATH] [--wk-options [WKOPTIONS ...]]
+                        [--prepared-html] [--charset CHARSET] [--raw] [--rtf] [--allow-fallback] [--skip-body-not-found] [--zip ZIP] [--save-header] [--attachments-only] [--skip-hidden] [--no-folders] [--skip-embedded] [--extract-embedded]
+                        [--overwrite-existing] [--skip-not-implemented] [--out-name OUTNAME | --glob] [--ignore-rtfde] [--progress]
+                        msg [msg ...]
+
+     extract_msg: Extracts emails and attachments saved in Microsoft Outlook's .msg files. https://github.com/TeamMsgExtractor/msg-extractor
+
+     positional arguments:
+       msg                   An MSG file to be parsed.
+
+     options:
+       -h, --help            show this help message and exit
+       --use-content-id, --cid
+                             Save attachments by their Content ID, if they have one. Useful when working with the HTML body.
+       --json                Changes to write output files as json.
+       --file-logging        Enables file logging. Implies --verbose level 1.
+       -v, --verbose         Turns on console logging. Specify more than once for higher verbosity.
+       --log LOG             Set the path to write the file log to.
+       --config CONFIGPATH   Set the path to load the logging config from.
+       --out OUTPATH         Set the folder to use for the program output. (Default: Current directory)
+       --use-filename        Sets whether the name of each output is based on the msg filename.
+       --dump-stdout         Tells the program to dump the message body (plain text) to stdout. Overrides saving arguments.
+       --html                Sets whether the output should be HTML. If this is not possible, will error.
+       --pdf                 Saves the body as a PDF. If this is not possible, will error.
+       --wk-path WKPATH      Overrides the path for finding wkhtmltopdf.
+       --wk-options [WKOPTIONS ...]
+                             Sets additional options to be used in wkhtmltopdf. Should be a series of options and values, replacing the - or -- in the beginning with + or ++, respectively. For example: --wk-options "+O Landscape"
+       --prepared-html       When used in conjunction with --html, sets whether the HTML output should be prepared for embedded attachments.
+       --charset CHARSET     Character set to use for the prepared HTML in the added tag. (Default: utf-8)
+       --raw                 Sets whether the output should be raw. If this is not possible, will error.
+       --rtf                 Sets whether the output should be RTF. If this is not possible, will error.
+       --allow-fallback      Tells the program to fallback to a different save type if the selected one is not possible.
+       --skip-body-not-found
+                             Skips saving the body if the body cannot be found, rather than throwing an error.
+       --zip ZIP             Path to use for saving to a zip file.
+       --save-header         Store the header in a separate file.
+       --attachments-only    Specify to only save attachments from an msg file.
+       --skip-hidden         Skips any attachment marked as hidden (usually ones embedded in the body).
+       --no-folders          Stores everything in the location specified by --out. Requires --attachments-only and is incompatible with --out-name.
+       --skip-embedded       Skips all embedded MSG files when saving attachments.
+       --extract-embedded    Extracts the embedded MSG files as MSG files instead of running their save functions.
+       --overwrite-existing  Disables filename conflict resolution code for attachments when saving a file, causing files to be overwriten if two attachments with the same filename are on an MSG file.
+       --skip-not-implemented, --skip-ni
+                             Skips any attachments that are not implemented, allowing saving of the rest of the message.
+       --out-name OUTNAME    Name to be used with saving the file output. Cannot be used if you are saving more than one file.
+       --glob, --wildcard    Interpret all paths as having wildcards. Incompatible with --out-name.
+       --ignore-rtfde        Ignores all errors thrown from RTFDE when trying to save. Useful for allowing fallback to continue when an exception happens.
+       --progress            Shows what file the program is currently working on during it's progress.
 
 **To use this in your own script**, start by using:
 
 ::
 
      import extract_msg
 
@@ -261,16 +254,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.5-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.5/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.0-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.42.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.5/setup.py` & `extract_msg-0.42.0/setup.py`

 * *Files identical despite different names*

