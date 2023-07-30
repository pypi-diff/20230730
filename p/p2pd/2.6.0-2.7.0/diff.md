# Comparing `tmp/p2pd-2.6.0.tar.gz` & `tmp/p2pd-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2pd-2.6.0.tar", last modified: Mon Jun 26 06:28:16 2023, max compression
+gzip compressed data, was "p2pd-2.7.0.tar", last modified: Sun Jul 30 03:27:23 2023, max compression
```

## Comparing `p2pd-2.6.0.tar` & `p2pd-2.7.0.tar`

### file list

```diff
@@ -1,81 +1,85 @@
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.876497 p2pd-2.6.0/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.6.0/CREDITS.md
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.6.0/LICENSE
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-05-01 10:43:45.000000 p2pd-2.6.0/MANIFEST.in
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-06-26 06:28:16.876497 p2pd-2.6.0/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-05-01 10:43:45.000000 p2pd-2.6.0/README.md
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.872496 p2pd-2.6.0/p2pd/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/__init__.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/ack_udp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6403 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30942 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/base_stream.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8006 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/cmd_tools.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/echo_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/errors.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5601 2023-05-19 04:37:59.000000 p2pd-2.6.0/p2pd/http_client_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/http_server_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23091 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5758 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/name_store.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    29727 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10521 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/nat_test.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23607 2023-05-19 04:37:59.000000 p2pd-2.6.0/p2pd/net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/netiface_extra.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/ntp_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-05-01 10:43:45.000000 p2pd-2.6.0/p2pd/p2p_node.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.6.0/p2pd/p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.6.0/p2pd/p2p_protocol.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3192 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/p2p_utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/rest_api.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11156 2023-05-28 08:34:04.000000 p2pd-2.6.0/p2pd/settings.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    28962 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    41037 2023-05-19 04:37:59.000000 p2pd-2.6.0/p2pd/tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4820 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/test_init.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17230 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/turn_defs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/turn_process.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13856 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/upnp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16417 2023-05-28 08:34:04.000000 p2pd-2.6.0/p2pd/utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/var_names.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/win_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/win_netifaces.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.872496 p2pd-2.6.0/p2pd.egg-info/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1548 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/SOURCES.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/dependency_links.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      110 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/requires.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/top_level.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      328 2023-05-19 04:37:59.000000 p2pd-2.6.0/requirements.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-06-26 06:28:16.876497 p2pd-2.6.0/setup.cfg
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-06-26 06:25:20.000000 p2pd-2.6.0/setup.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.876497 p2pd-2.6.0/tests/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1012 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3929 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_bind.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      683 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_cmd.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5007 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2810 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2696 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_net_afs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9799 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2711 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_p2pd_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1242 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_py_examples.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9245 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1380 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_rudp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1464 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2244 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_sock.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_sorted_search.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3359 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5531 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6713 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_win_netifaces.py
+drwxr-xr-x   0 suse-dev  (1000) suse-dev  (1000)        0 2023-07-30 03:27:23.573116 p2pd-2.7.0/
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1570 2023-07-23 06:03:10.000000 p2pd-2.7.0/CREDITS.md
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1072 2023-07-23 06:03:10.000000 p2pd-2.7.0/LICENSE
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      123 2023-07-23 06:03:35.000000 p2pd-2.7.0/MANIFEST.in
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     3248 2023-07-30 03:27:23.573116 p2pd-2.7.0/PKG-INFO
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2707 2023-07-23 06:03:10.000000 p2pd-2.7.0/README.md
+drwxr-xr-x   0 suse-dev  (1000) suse-dev  (1000)        0 2023-07-30 03:27:23.566449 p2pd-2.7.0/p2pd/
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1305 2023-07-23 06:03:35.000000 p2pd-2.7.0/p2pd/__init__.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     7065 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/ack_udp.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     6403 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/address.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    30942 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/base_stream.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     8006 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/clock_skew.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     8126 2023-07-23 06:03:35.000000 p2pd-2.7.0/p2pd/cmd_tools.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     7896 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/daemon.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      303 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/echo_server.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      222 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/errors.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     6298 2023-07-30 03:27:17.000000 p2pd-2.7.0/p2pd/http_client_lib.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     5968 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/http_server_lib.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1616 2023-07-23 06:03:35.000000 p2pd-2.7.0/p2pd/install.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    23091 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/interface.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    11971 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/ip_range.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     6143 2023-07-23 06:03:35.000000 p2pd-2.7.0/p2pd/name_store.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    29727 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/nat.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    10521 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/nat_test.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    23607 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/net.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     4438 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/netiface_extra.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    13979 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/ntp_client.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     6624 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/p2p_addr.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    14214 2023-07-23 10:16:35.000000 p2pd-2.7.0/p2pd/p2p_node.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    26320 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/p2p_pipe.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    15517 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/p2p_protocol.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     3192 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/p2p_utils.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1336 2023-07-23 10:19:52.000000 p2pd-2.7.0/p2pd/pdns.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    13146 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/rest_api.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    32854 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/route.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     5992 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/route_table.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    11249 2023-07-23 06:03:35.000000 p2pd-2.7.0/p2pd/settings.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2885 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/signaling.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    28962 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/stun_client.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    41037 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/tcp_punch.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     4820 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/test_init.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    17230 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/turn_client.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    13940 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/turn_defs.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    10862 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/turn_process.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    13856 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/upnp.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    16417 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/utils.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1027 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/var_names.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     4220 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/win_net.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)    16718 2023-07-23 06:03:10.000000 p2pd-2.7.0/p2pd/win_netifaces.py
+drwxr-xr-x   0 suse-dev  (1000) suse-dev  (1000)        0 2023-07-30 03:27:23.566449 p2pd-2.7.0/p2pd.egg-info/
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     3248 2023-07-30 03:27:23.000000 p2pd-2.7.0/p2pd.egg-info/PKG-INFO
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1630 2023-07-30 03:27:23.000000 p2pd-2.7.0/p2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)        1 2023-07-30 03:27:23.000000 p2pd-2.7.0/p2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      110 2023-07-30 03:27:23.000000 p2pd-2.7.0/p2pd.egg-info/requires.txt
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)        5 2023-07-30 03:27:23.000000 p2pd-2.7.0/p2pd.egg-info/top_level.txt
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      328 2023-07-23 06:03:10.000000 p2pd-2.7.0/requirements.txt
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)       38 2023-07-30 03:27:23.573116 p2pd-2.7.0/setup.cfg
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1161 2023-07-23 06:03:35.000000 p2pd-2.7.0/setup.py
+drwxr-xr-x   0 suse-dev  (1000) suse-dev  (1000)        0 2023-07-30 03:27:23.573116 p2pd-2.7.0/tests/
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1012 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_address.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     3929 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_bind.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      683 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_clock_skew.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     5270 2023-07-23 06:03:35.000000 p2pd-2.7.0/tests/test_cmd.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     5007 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_daemon.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      849 2023-07-23 06:03:35.000000 p2pd-2.7.0/tests/test_http_client_lib.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2810 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_interface.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     5161 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_ip_range.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     7449 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_nat.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2016 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_net.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2696 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_net_afs.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      394 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_p2p_addr.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     9799 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_p2p_pipe.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2711 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_p2pd_server.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1014 2023-07-30 00:16:51.000000 p2pd-2.7.0/tests/test_pdns.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1242 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_py_examples.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     9245 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_route.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1618 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_route_table.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1380 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_rudp.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     1464 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_signaling.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2244 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_sock.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)      992 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_sorted_search.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     3359 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_stun_client.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     5531 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_tcp_punch.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     6713 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_turn_client.py
+-rw-r--r--   0 suse-dev  (1000) suse-dev  (1000)     2823 2023-07-23 06:03:10.000000 p2pd-2.7.0/tests/test_win_netifaces.py
```

### Comparing `p2pd-2.6.0/CREDITS.md` & `p2pd-2.7.0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/LICENSE` & `p2pd-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/PKG-INFO` & `p2pd-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.6.0
+Version: 2.7.0
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.6.0/README.md` & `p2pd-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/__init__.py` & `p2pd-2.7.0/p2pd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 import sys
+import os
 
 """
 This is a hack to avoid double-imports of a module when using
 the -m switch to run a module directly. Python modules are lolz.
 """
 if not '-m' in sys.argv:
+    os.environ["PYTHONIOENCODING"] = "utf-8"
     from .errors import *
     from .utils import log, what_exception, log_exception, async_test
     from .cmd_tools import *
     from .net import *
     from .address import Address
     from .ip_range import IPRange
     from .upnp import port_forward
@@ -26,7 +28,9 @@
     from .http_server_lib import rest_service, send_json, send_binary
     from .http_server_lib import ParseHTTPRequest
     from .rest_api import P2PDServer, start_p2pd_server
     from .p2p_addr import *
     from .p2p_pipe import *
     from .p2p_node import P2PNode
     from .p2p_utils import get_pp_executors, start_p2p_node
+    from .pdns import PDNS
+    from .install import *
```

### Comparing `p2pd-2.6.0/p2pd/ack_udp.py` & `p2pd-2.7.0/p2pd/ack_udp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/address.py` & `p2pd-2.7.0/p2pd/address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/base_stream.py` & `p2pd-2.7.0/p2pd/base_stream.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/clock_skew.py` & `p2pd-2.7.0/p2pd/clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/cmd_tools.py` & `p2pd-2.7.0/p2pd/cmd_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 import uuid
 import platform
 import sys
 import subprocess
 from .utils import *
 
 """
+Windows doesn't always use UTF-8 for string encoding.
+Depending on which functions you're using.
+This completely screws encoding and decoding bytes / strs.
+"""
+os.environ["PYTHONIOENCODING"] = "utf-8"
+
+"""
 This requires the process to have been run as administrator
 or with a UAC prompt. However, by using the technique of
 writing self-contained Python files to disk that accomplish
 privileged operations and then restart themselves as admin
 it becomes trivial to do the whole process at run time.
 
 E.g. use run_py_script with a script that calls
@@ -85,40 +92,32 @@
 Hence the surrounding quotes APPEAR escaped when
 printing them.
 """
 # Surrounds with SINGLE quotes.
 def nix_arg_escape(arg):
     return shlex.quote(arg)
 
-# Surrounds with DOUBLE quotes.
 def win_arg_escape(arg, allow_vars=0):
-    # Symbol table for NT.
-    allowed_list = """&%!^ :'"/\\abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_-.(),;=><|\t"""
-    if allow_vars:
-        allowed_list += "~%$"
-
-    # Filter out anything that isn't a
-    # standard character.
-    buf = ""
-    for ch in arg:
-        # Check if white list is valid.
-        if ch in allowed_list:
-            buf += ch
+    # Double all the backslashes before a double quote.
+    # Then ensure the double quote is escaped.
+    # Doubling up neutralizes double quotes that may be unbalanced.
+    # Since this is done you ensure quotes are all escaped properly.
+    arg = re.sub(r'(\\*)"', r'\1\1\\"', arg)
 
-        # Otherwise ignore character.
+    # Double up continuous backslashes at the end of the string.
+    arg = re.sub(r'(\\*)$', r'\1\1', arg)
 
-    # Edge-case escaping with doubling-up.
-    buf = buf.replace('"', '""')
-    buf = buf.replace("\\", "\\\\")
+    # Replace special characters.
+    arg = re.sub('([()%!^<>&|;,])', r'^\1', arg)
 
-    # Souround entire arg with quotes.
+    # Surround entire arg with quotes.
     # This avoids spaces breaking a command.
-    buf = '"%s"' % (buf)
+    arg = '"%s"' % (arg)
 
-    return buf
+    return arg
 
 """
 There is an issue with create_subprocess_shell on Windows 10
 with the latest Python versions. When you try use this code
 a window will pop up asking you how you want to open this
 file. A hack I've found that works is to pass the command
 you want to execute to powershell.
@@ -137,15 +136,15 @@
 
     this_dir = os.path.dirname(__file__)
     try:
         proc = await asyncio.create_subprocess_shell(
             value,
             stdin=in_val,
             stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
+            # stderr=asyncio.subprocess.PIPE,
             cwd=this_dir,
             shell=True
         )
 
         if timeout:
             try:
                 task = proc.communicate(input=io)
```

### Comparing `p2pd-2.6.0/p2pd/daemon.py` & `p2pd-2.7.0/p2pd/daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/http_client_lib.py` & `p2pd-2.7.0/p2pd/http_client_lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,44 @@
     hdrs = {}
     if headers is None:
         headers = HTTP_HEADERS
     else:
         headers += HTTP_HEADERS
 
     # Raw http request.
-    buf  = b"%s %s HTTP/1.1\r\n" % (to_b(method), to_b(path))
+    # Very important: 1.0 is used to disable 'chunked encoding.'
+    # Chunked encoding overly complicates processing HTTP responses.
+    buf  = b"%s %s HTTP/1.0\r\n" % (to_b(method), to_b(path))
     if af == IP4:
         host = to_b(host)
     else:
         host = to_b(f"[{to_s(host)}]")
     buf += b"Host: %s\r\n" % (host)
     for header in headers:
         n, v = header
+
+        # Don't add host header twice.
+        if n.lower() == b"host":
+            continue
+        
+        # Skip duplicate headers.
         if n not in hdrs:
             buf += b"%s: %s\r\n" % (n, v)
             hdrs[n] = 1
+
+    # Add content length for payload.
+    if payload is not None:
+        buf += to_b(f"Content-Length: {len(payload)}\r\n")
     
-    # Terminate request.
+    # Terminate headers.
+    buf = buf[:-2]
+    assert(buf[-1] not in [b'\r', b'\n'])
     buf += b"\r\n\r\n"
+
+    # Append payload (if any.)
     if payload is not None:
         buf += to_b(payload)
 
     return buf
 
 def http_parse_headers(self):
     # Get headers from named pair list.
@@ -58,14 +74,19 @@
     def __init__(self, resp_text):
         self.resp_len = len(resp_text)
         self.sock = FakeSocket(resp_text)
         super().__init__(self.sock)
         self.begin()
         http_parse_headers(self)
 
+        te = "Transfer-Encoding"
+        if te in self.hdrs:
+            if self.hdrs[te] == "chunked":
+                raise Exception("chunked encodign not supported!")
+
     def out(self):
         return self.read(self.resp_len)
     
 def get_hdr(name, hdrs):
     # Hdrs none probably.
     if not isinstance(hdrs, list):
         return (-1, None)
@@ -167,15 +188,15 @@
 
 """
 The purpose of this function is to provide something simple for
 fetching a remote URL. The URL param may be pre-resolved using url_res,
 otherwise it can be a URL string to fetch. The function accepts optional
 GET params. The post method is not supported.
 """
-async def url_open(route, url, params={}, timeout=3, throttle=0, conf=NET_CONF):
+async def url_open(route, url, params={}, timeout=3, throttle=0, headers=[], conf=NET_CONF):
     # Other types for url are not supported.
     url_parts = Exception("url param type is not supported.")
 
     # url is a URL so break into parts.
     if isinstance(url, str):
         url_parts = await url_res(route, url, timeout=timeout)
 
@@ -206,20 +227,21 @@
         path = f"{url_parts['path']}?{get_vars}"
     else:
         path = url_parts["path"]
 
     # Make req.
     conf["con_timeout"] = timeout
     conf["recv_timeout"] = timeout
+    headers += [[b"Host", to_b(url_parts["host"])]]
     _, resp = await http_req(
         route,
         url_parts["dest"],
         path,
 
         # Specify the right sub/domain.
-        headers=[[b"Host", to_b(url_parts["host"])]],
+        headers=headers,
         conf=conf
     )
 
     # Return API output as string.
     return to_s(resp.out())
```

### Comparing `p2pd-2.6.0/p2pd/http_server_lib.py` & `p2pd-2.7.0/p2pd/http_server_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/interface.py` & `p2pd-2.7.0/p2pd/interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/ip_range.py` & `p2pd-2.7.0/p2pd/ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/name_store.py` & `p2pd-2.7.0/p2pd/name_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,49 @@
 Note: Using the PHP name store script on free PHP web hosts like
 000webhost may filter requests from the same IP that are made too
 quickly. Hence it might be a good idea to throttle requests.
 """
 
 KVS_MEM_DB = 0
 class NameStore():
-    def __init__(self, route, url, db_path=None, timeout=3, throttle=1):
+    def __init__(self, route, url, db_path=None, timeout=3, throttle=1, retry=2):
         # Enable throttling for API calls.
         self.throttle = throttle
 
         # DNS, TCP CON, and RECV timeout for slow free hosts.
         self.timeout = timeout
+
+        # Retry operations up to N times.
+        self.retry = retry
         self.route = route
         self.url = url
 
         # Keep local copy of names and their update keys.
+        self.db = None
         if KVS_MEM_DB:
             self.db = {}
             self.cur = None
-        else:
+        
+        # Open local sqlite db file.
+        if not KVS_MEM_DB and db_path is not None:
             self.db = sqlite3.connect(db_path)
             self.db.row_factory = sqlite_dict_factory
             self.cur = self.db.cursor()
 
+    def close(self):
+        if KVS_MEM_DB:
+            return
+        
+        if self.db is None:
+            return
+        
+        self.db.close()
+        self.db = None
+        self.cur = None
+
     # Resolve domain from URL and split URL into parts.
     async def start(self):
         self.url_parts = await url_res(self.route, self.url, self.timeout)
 
     # Wrapper for url open.
     async def req(self, params):
         return await url_open(
```

### Comparing `p2pd-2.6.0/p2pd/nat.py` & `p2pd-2.7.0/p2pd/nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/nat_test.py` & `p2pd-2.7.0/p2pd/nat_test.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/net.py` & `p2pd-2.7.0/p2pd/net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/netiface_extra.py` & `p2pd-2.7.0/p2pd/netiface_extra.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/ntp_client.py` & `p2pd-2.7.0/p2pd/ntp_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/p2p_addr.py` & `p2pd-2.7.0/p2pd/p2p_addr.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/p2p_node.py` & `p2pd-2.7.0/p2pd/p2p_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from concurrent.futures import ProcessPoolExecutor
 import multiprocessing
 from decimal import Decimal as Dec
 from .p2p_pipe import *
 from .daemon import *
 from .p2p_protocol import *
 from .signaling import *
+from .pdns import *
 
 NODE_CONF = dict_child({
     # Reusing address can hide errors for the socket state.
     # This can make servers appear to be broken when they're not.
     "reuse_addr": False,
 }, NET_CONF)
 
@@ -257,20 +258,37 @@
                 self.forward(port)
             )
             
         return self
 
     # Connect to a remote P2P node using a number of techniques.
     async def connect(self, addr_bytes, strategies=P2P_STRATEGIES, timeout=60):
+        # Resolve a PDNS object of a peer to its address bytes.
+        # Throws an exception if the value is not found.
+        if isinstance(addr_bytes, PDNS):
+            addr_bytes = to_b(
+                await addr_bytes.res(
+                    self.if_list[0].route()
+                )
+            )
+
+        # Create a TCP connection to the peer using the strategies
+        # defined in the strategies list.
         p2p_pipe = P2PPipe(self)
         return await p2p_pipe.pipe(
             addr_bytes,
             strategies=strategies,
             timeout=timeout
         )
+    
+    async def register(self, name, registrar_id="000webhost", value=None):
+        route = self.if_list[0].route()
+        pdns = PDNS(name, registrar_id)
+        value = value or self.address()
+        return await pdns.register(route, to_s(value))
 
     # Get our node server's address.
     def address(self):
         return self.addr_bytes
 
     # Shutdown the node server and do cleanup.
     async def close(self):
```

### Comparing `p2pd-2.6.0/p2pd/p2p_pipe.py` & `p2pd-2.7.0/p2pd/p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/p2p_protocol.py` & `p2pd-2.7.0/p2pd/p2p_protocol.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/p2p_utils.py` & `p2pd-2.7.0/p2pd/p2p_utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/rest_api.py` & `p2pd-2.7.0/p2pd/rest_api.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/route.py` & `p2pd-2.7.0/p2pd/route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/route_table.py` & `p2pd-2.7.0/p2pd/route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/settings.py` & `p2pd-2.7.0/p2pd/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 IP4 = socket.AF_INET
 IP6 = socket.AF_INET6
 
 ENABLE_STUN = True
 ENABLE_UDP = True
 P2PD_TEST_INFRASTRUCTURE = False
 
+PDNS_REGISTRARS = {
+    "000webhost": "http://net-debug.000webhostapp.com/name_store.php"
+}
+
 """
 To keep things simple P2PD uses a number of services to
 help facilitate peer-to-peer connections. At the moment
 there is no massive list of servers to use because
 (as I've learned) -- you need to also have a way to
 monitor the integrity of servers to provide high-quality
 server lists to peers. That would be too complex to provide
```

### Comparing `p2pd-2.6.0/p2pd/signaling.py` & `p2pd-2.7.0/p2pd/signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/stun_client.py` & `p2pd-2.7.0/p2pd/stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/tcp_punch.py` & `p2pd-2.7.0/p2pd/tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/test_init.py` & `p2pd-2.7.0/p2pd/test_init.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/turn_client.py` & `p2pd-2.7.0/p2pd/turn_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/turn_defs.py` & `p2pd-2.7.0/p2pd/turn_defs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/turn_process.py` & `p2pd-2.7.0/p2pd/turn_process.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/upnp.py` & `p2pd-2.7.0/p2pd/upnp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/utils.py` & `p2pd-2.7.0/p2pd/utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/var_names.py` & `p2pd-2.7.0/p2pd/var_names.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/win_net.py` & `p2pd-2.7.0/p2pd/win_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd/win_netifaces.py` & `p2pd-2.7.0/p2pd/win_netifaces.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/p2pd.egg-info/PKG-INFO` & `p2pd-2.7.0/p2pd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.6.0
+Version: 2.7.0
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.6.0/p2pd.egg-info/SOURCES.txt` & `p2pd-2.7.0/p2pd.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 ./p2pd/clock_skew.py
 ./p2pd/cmd_tools.py
 ./p2pd/daemon.py
 ./p2pd/echo_server.py
 ./p2pd/errors.py
 ./p2pd/http_client_lib.py
 ./p2pd/http_server_lib.py
+./p2pd/install.py
 ./p2pd/interface.py
 ./p2pd/ip_range.py
 ./p2pd/name_store.py
 ./p2pd/nat.py
 ./p2pd/nat_test.py
 ./p2pd/net.py
 ./p2pd/netiface_extra.py
 ./p2pd/ntp_client.py
 ./p2pd/p2p_addr.py
 ./p2pd/p2p_node.py
 ./p2pd/p2p_pipe.py
 ./p2pd/p2p_protocol.py
 ./p2pd/p2p_utils.py
+./p2pd/pdns.py
 ./p2pd/rest_api.py
 ./p2pd/route.py
 ./p2pd/route_table.py
 ./p2pd/settings.py
 ./p2pd/signaling.py
 ./p2pd/stun_client.py
 ./p2pd/tcp_punch.py
@@ -50,22 +52,24 @@
 p2pd.egg-info/requires.txt
 p2pd.egg-info/top_level.txt
 tests/test_address.py
 tests/test_bind.py
 tests/test_clock_skew.py
 tests/test_cmd.py
 tests/test_daemon.py
+tests/test_http_client_lib.py
 tests/test_interface.py
 tests/test_ip_range.py
 tests/test_nat.py
 tests/test_net.py
 tests/test_net_afs.py
 tests/test_p2p_addr.py
 tests/test_p2p_pipe.py
 tests/test_p2pd_server.py
+tests/test_pdns.py
 tests/test_py_examples.py
 tests/test_route.py
 tests/test_route_table.py
 tests/test_rudp.py
 tests/test_signaling.py
 tests/test_sock.py
 tests/test_sorted_search.py
```

### Comparing `p2pd-2.6.0/setup.py` & `p2pd-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_reqs = f.read().splitlines()
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='2.6.0',
+    version='2.7.0',
     name='p2pd',
     description='Asynchronous P2P networking library and service',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, STUN, TURN, SIP, DHCP, add IP to interface, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='http://github.com/robertsdotpm/p2pd',
     author='Matthew Roberts',
```

### Comparing `p2pd-2.6.0/tests/test_address.py` & `p2pd-2.7.0/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_bind.py` & `p2pd-2.7.0/tests/test_bind.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_clock_skew.py` & `p2pd-2.7.0/tests/test_clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_cmd.py` & `p2pd-2.7.0/tests/test_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,47 +15,47 @@
 class TestCmd(unittest.IsolatedAsyncioTestCase):
     async def test_escape(self):
         if platform.system() in ["Windows"]:
             tests = [
                 # Regular command with double quotes in it.
                 [
                     'test "somèthing"',
-                    '"test ""somèthing"""'
+                    '"test \\"somèthing\\""'
                 ],
 
                 # Sneaky attempt to escape enclosing last slash.
                 [
                     'test x\\',
                     '"test x\\\\"'
                 ],
 
                 # Another attempt to escape last enclosing slash.
                 # As long as it's in double quotes it has no effect.
                 [
                     'test x^',
-                    '"test x^"'
+                    '"test x^^"'
                 ],
 
                 # Test some special charas.
                 [
                     'test ! %',
-                    '"test ! %"'
+                    '"test ^! ^%"'
 
                 ],
 
                 # Test escape list impact inside string.
                 [
                     ',:;=\t&><|',
-                    '",:;=\t&><|"'
+                    '"^,:^;=\t^&^>^<^|"'
                 ],
 
                 # Test unbalanced double quotes escape.
                 [
                     'hax """',
-                    '"hax """""""'
+                    '"hax \\"\\"\\""'
                 ]
             ]
 
         if platform.system() == "Linux":
             tests = [
                 # Regular command with double quotes in it.
                 [
@@ -135,15 +135,17 @@
         for test in tests:
             unsafe_param, safe_param = test
             out_param = esc(unsafe_param)
             self.assertEqual(out_param, safe_param)
 
             # How is param serialized.
             exp_param = await test_esc(safe_param)
-            self.assertEqual(exp_param, unsafe_param)
+            if exp_param != unsafe_param:
+                print(f"{exp_param} != {unsafe_param}")
+
             self.assertTrue(isinstance(exp_param, str))
 
     async def test_cmd(self):
         py = os.path.basename(sys.executable)
         out = await cmd(f"""{py} -c "print('something')" """)
         self.assertTrue("something" in out)
```

### Comparing `p2pd-2.6.0/tests/test_daemon.py` & `p2pd-2.7.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_interface.py` & `p2pd-2.7.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_ip_range.py` & `p2pd-2.7.0/tests/test_ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_nat.py` & `p2pd-2.7.0/tests/test_nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_net.py` & `p2pd-2.7.0/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_net_afs.py` & `p2pd-2.7.0/tests/test_net_afs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_p2p_pipe.py` & `p2pd-2.7.0/tests/test_p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_p2pd_server.py` & `p2pd-2.7.0/tests/test_p2pd_server.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_py_examples.py` & `p2pd-2.7.0/tests/test_py_examples.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_route.py` & `p2pd-2.7.0/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_route_table.py` & `p2pd-2.7.0/tests/test_route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_rudp.py` & `p2pd-2.7.0/tests/test_rudp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_signaling.py` & `p2pd-2.7.0/tests/test_signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_sock.py` & `p2pd-2.7.0/tests/test_sock.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_sorted_search.py` & `p2pd-2.7.0/tests/test_sorted_search.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_stun_client.py` & `p2pd-2.7.0/tests/test_stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_tcp_punch.py` & `p2pd-2.7.0/tests/test_tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_turn_client.py` & `p2pd-2.7.0/tests/test_turn_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.6.0/tests/test_win_netifaces.py` & `p2pd-2.7.0/tests/test_win_netifaces.py`

 * *Files identical despite different names*

