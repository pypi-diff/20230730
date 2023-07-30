# Comparing `tmp/kingsoftcloud-sdk-python-1.1.6.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.1.6.tar", last modified: Tue Jul 25 11:59:15 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.7.tar", last modified: Sun Jul 30 15:28:32 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.1.6.tar` & `kingsoftcloud-sdk-python-1.1.7.tar`

### file list

```diff
@@ -1,179 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51841 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45896 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85663 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   126047 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-30 15:28:32.000000 kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-30 15:28:32.000000 kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:28:32.000000 kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 15:28:32.000000 kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 15:28:32.000000 kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.236311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51841 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45896 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.240311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85663 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126047 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20100525/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20100525/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20100525/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20100525/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20181114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20181114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20181114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20181114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20220101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20220101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20220101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20220101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.244311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.248311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 15:28:32.252311 kingsoftcloud-sdk-python-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-30 15:28:20.000000 kingsoftcloud-sdk-python-1.1.7/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.6/LICENSE` & `kingsoftcloud-sdk-python-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.6/README.rst` & `kingsoftcloud-sdk-python-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.7/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 ksyun/client/mongodb/v20170101/__init__.py
 ksyun/client/mongodb/v20170101/client.py
 ksyun/client/mongodb/v20170101/models.py
 ksyun/client/monitor/__init__.py
 ksyun/client/monitor/v20100525/__init__.py
 ksyun/client/monitor/v20100525/client.py
 ksyun/client/monitor/v20100525/models.py
+ksyun/client/monitor/v20181114/__init__.py
+ksyun/client/monitor/v20181114/client.py
+ksyun/client/monitor/v20181114/models.py
 ksyun/client/monitor/v20210101/__init__.py
 ksyun/client/monitor/v20210101/client.py
 ksyun/client/monitor/v20210101/models.py
 ksyun/client/monitor/v20220101/__init__.py
 ksyun/client/monitor/v20220101/client.py
 ksyun/client/monitor/v20220101/models.py
 ksyun/client/resourcemanager/__init__.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.1.6'
+__version__ = '1.1.7'
```

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kec/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/kls/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20100525/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20100525/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20210101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20210101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20220101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/monitor/v20220101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20171210/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/slb/v20171210/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.7/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.6/setup.py` & `kingsoftcloud-sdk-python-1.1.7/setup.py`

 * *Files identical despite different names*

