# Comparing `tmp/amatak-shop-1.0.6.tar.gz` & `tmp/amatak-shop-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amatak-shop-1.0.6.tar", last modified: Sun Jul 30 03:36:45 2023, max compression
+gzip compressed data, was "amatak-shop-1.0.7.tar", last modified: Sun Jul 30 06:44:56 2023, max compression
```

## Comparing `amatak-shop-1.0.6.tar` & `amatak-shop-1.0.7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.825978 amatak-shop-1.0.6/
--rw-rw-rw-   0        0        0     3188 2023-07-30 03:36:45.808935 amatak-shop-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2671 2023-07-30 02:05:48.000000 amatak-shop-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:44.957822 amatak-shop-1.0.6/amatak_shop/
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.073690 amatak-shop-1.0.6/amatak_shop/forms/
--rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.6/amatak_shop/forms/__init__.py
--rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.6/amatak_shop/forms/checkout.py
--rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.6/amatak_shop/forms/coupon.py
--rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.6/amatak_shop/forms/payment.py
--rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.6/amatak_shop/forms/payment_choices.py
--rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.6/amatak_shop/forms/refund.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:44.942205 amatak-shop-1.0.6/amatak_shop/management/
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.089314 amatak-shop-1.0.6/amatak_shop/management/commands/
--rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.6/amatak_shop/management/commands/rename.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.104934 amatak-shop-1.0.6/amatak_shop/migrations/
--rw-rw-rw-   0        0        0     7382 2023-07-29 03:02:06.000000 amatak-shop-1.0.6/amatak_shop/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.6/amatak_shop/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.251983 amatak-shop-1.0.6/amatak_shop/models/
--rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.6/amatak_shop/models/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.6/amatak_shop/models/address.py
--rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.6/amatak_shop/models/category.py
--rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.6/amatak_shop/models/coupon.py
--rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.6/amatak_shop/models/item.py
--rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.6/amatak_shop/models/mixins.py
--rw-rw-rw-   0        0        0     2691 2023-07-27 12:36:01.000000 amatak-shop-1.0.6/amatak_shop/models/order.py
--rw-rw-rw-   0        0        0     1648 2023-07-27 12:36:18.000000 amatak-shop-1.0.6/amatak_shop/models/order_item.py
--rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.6/amatak_shop/models/payment.py
--rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.6/amatak_shop/models/refund.py
--rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.6/amatak_shop/models/user_profile.py
--rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.6/amatak_shop/models/user_receiver_profile.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.289146 amatak-shop-1.0.6/amatak_shop/settings/
--rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.6/amatak_shop/settings/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.6/amatak_shop/settings/base.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.289146 amatak-shop-1.0.6/amatak_shop/templatetags/
--rw-rw-rw-   0        0        0      499 2023-07-30 03:34:40.000000 amatak-shop-1.0.6/amatak_shop/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-07-30 03:29:14.000000 amatak-shop-1.0.6/amatak_shop/templatetags/amatak_shop.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.320350 amatak-shop-1.0.6/amatak_shop/tests/
--rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.6/amatak_shop/tests/__init__.py
--rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.6/amatak_shop/tests/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.493894 amatak-shop-1.0.6/amatak_shop/urls/
--rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.6/amatak_shop/urls/__init__.py
--rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.6/amatak_shop/urls/add_coupon.py
--rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.6/amatak_shop/urls/add_to_cart.py
--rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.6/amatak_shop/urls/checkout.py
--rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.6/amatak_shop/urls/home.py
--rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.6/amatak_shop/urls/order_summary.py
--rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.6/amatak_shop/urls/payment.py
--rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.6/amatak_shop/urls/policy.py
--rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.6/amatak_shop/urls/products.py
--rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.6/amatak_shop/urls/remove_from_cart.py
--rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.6/amatak_shop/urls/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.6/amatak_shop/urls/request_refund.py
--rw-rw-rw-   0        0        0      419 2023-07-27 11:58:31.000000 amatak-shop-1.0.6/amatak_shop/urls/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.746449 amatak-shop-1.0.6/amatak_shop/views/
--rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.6/amatak_shop/views/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.6/amatak_shop/views/add_coupon.py
--rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.6/amatak_shop/views/add_to_cart.py
--rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.6/amatak_shop/views/checkout.py
--rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.6/amatak_shop/views/create_ref_code.py
--rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.6/amatak_shop/views/get_coupon.py
--rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.6/amatak_shop/views/home.py
--rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.6/amatak_shop/views/is_valid_form.py
--rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.6/amatak_shop/views/items_detail_views.py
--rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.6/amatak_shop/views/login.py
--rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.6/amatak_shop/views/logout.py
--rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.6/amatak_shop/views/order_summary.py
--rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.6/amatak_shop/views/payment.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.6/amatak_shop/views/policy.py
--rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.6/amatak_shop/views/products.py
--rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.6/amatak_shop/views/remove_from_cart.py
--rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.6/amatak_shop/views/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.6/amatak_shop/views/request_refund.py
--rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.6/amatak_shop/views/sign_up.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.6/amatak_shop/views/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:44.989064 amatak-shop-1.0.6/amatak_shop.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-07-30 03:36:44.000000 amatak-shop-1.0.6/amatak_shop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2023-07-30 03:36:44.000000 amatak-shop-1.0.6/amatak_shop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 03:36:44.000000 amatak-shop-1.0.6/amatak_shop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-30 03:36:44.000000 amatak-shop-1.0.6/amatak_shop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:44.957822 amatak-shop-1.0.6/eCommerce/
-drwxrwxrwx   0        0        0        0 2023-07-30 03:36:45.808935 amatak-shop-1.0.6/eCommerce/settings/
--rw-rw-rw-   0        0        0     1487 2023-07-30 03:32:50.000000 amatak-shop-1.0.6/eCommerce/settings/AmatakShopDev.py
--rw-rw-rw-   0        0        0      256 2023-07-30 02:54:02.000000 amatak-shop-1.0.6/eCommerce/settings/__init__.py
--rw-rw-rw-   0        0        0     2588 2023-07-30 03:15:58.000000 amatak-shop-1.0.6/eCommerce/settings/base.py
--rw-rw-rw-   0        0        0     1096 2023-07-30 02:56:09.000000 amatak-shop-1.0.6/eCommerce/settings/production.py
--rw-rw-rw-   0        0        0      564 2023-07-30 03:35:09.000000 amatak-shop-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 03:36:45.825978 amatak-shop-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/
+-rw-rw-rw-   0        0        0     3188 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2671 2023-07-30 02:05:48.000000 amatak-shop-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.052040 amatak-shop-1.0.7/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.095329 amatak-shop-1.0.7/amatak_shop/forms/
+-rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.7/amatak_shop/forms/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.7/amatak_shop/forms/checkout.py
+-rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.7/amatak_shop/forms/coupon.py
+-rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.7/amatak_shop/forms/payment.py
+-rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.7/amatak_shop/forms/payment_choices.py
+-rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.7/amatak_shop/forms/refund.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.052040 amatak-shop-1.0.7/amatak_shop/management/
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.099335 amatak-shop-1.0.7/amatak_shop/management/commands/
+-rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.7/amatak_shop/management/commands/rename.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.099335 amatak-shop-1.0.7/amatak_shop/migrations/
+-rw-rw-rw-   0        0        0     7375 2023-07-30 06:40:44.000000 amatak-shop-1.0.7/amatak_shop/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.7/amatak_shop/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.114962 amatak-shop-1.0.7/amatak_shop/models/
+-rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.7/amatak_shop/models/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.7/amatak_shop/models/address.py
+-rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.7/amatak_shop/models/category.py
+-rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.7/amatak_shop/models/coupon.py
+-rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.7/amatak_shop/models/item.py
+-rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.7/amatak_shop/models/mixins.py
+-rw-rw-rw-   0        0        0     2255 2023-07-30 06:32:21.000000 amatak-shop-1.0.7/amatak_shop/models/order.py
+-rw-rw-rw-   0        0        0     1308 2023-07-30 06:28:38.000000 amatak-shop-1.0.7/amatak_shop/models/order_item.py
+-rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.7/amatak_shop/models/payment.py
+-rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.7/amatak_shop/models/refund.py
+-rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.7/amatak_shop/models/user_profile.py
+-rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.7/amatak_shop/models/user_receiver_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.130584 amatak-shop-1.0.7/amatak_shop/settings/
+-rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.7/amatak_shop/settings/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.7/amatak_shop/settings/base.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.130584 amatak-shop-1.0.7/amatak_shop/templatetags/
+-rw-rw-rw-   0        0        0      499 2023-07-30 06:43:41.000000 amatak-shop-1.0.7/amatak_shop/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2269 2023-07-30 03:29:14.000000 amatak-shop-1.0.7/amatak_shop/templatetags/amatak_shop.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.130584 amatak-shop-1.0.7/amatak_shop/tests/
+-rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.7/amatak_shop/tests/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.7/amatak_shop/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.167933 amatak-shop-1.0.7/amatak_shop/urls/
+-rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.7/amatak_shop/urls/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.7/amatak_shop/urls/add_coupon.py
+-rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.7/amatak_shop/urls/add_to_cart.py
+-rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.7/amatak_shop/urls/checkout.py
+-rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.7/amatak_shop/urls/home.py
+-rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.7/amatak_shop/urls/order_summary.py
+-rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.7/amatak_shop/urls/payment.py
+-rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.7/amatak_shop/urls/policy.py
+-rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.7/amatak_shop/urls/products.py
+-rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.7/amatak_shop/urls/remove_from_cart.py
+-rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.7/amatak_shop/urls/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.7/amatak_shop/urls/request_refund.py
+-rw-rw-rw-   0        0        0      419 2023-07-27 11:58:31.000000 amatak-shop-1.0.7/amatak_shop/urls/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.199603 amatak-shop-1.0.7/amatak_shop/views/
+-rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.7/amatak_shop/views/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.7/amatak_shop/views/add_coupon.py
+-rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.7/amatak_shop/views/add_to_cart.py
+-rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.7/amatak_shop/views/checkout.py
+-rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.7/amatak_shop/views/create_ref_code.py
+-rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.7/amatak_shop/views/get_coupon.py
+-rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.7/amatak_shop/views/home.py
+-rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.7/amatak_shop/views/is_valid_form.py
+-rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.7/amatak_shop/views/items_detail_views.py
+-rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.7/amatak_shop/views/login.py
+-rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.7/amatak_shop/views/logout.py
+-rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.7/amatak_shop/views/order_summary.py
+-rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.7/amatak_shop/views/payment.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.7/amatak_shop/views/policy.py
+-rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.7/amatak_shop/views/products.py
+-rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.7/amatak_shop/views/remove_from_cart.py
+-rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.7/amatak_shop/views/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.7/amatak_shop/views/request_refund.py
+-rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.7/amatak_shop/views/sign_up.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.7/amatak_shop/views/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.067703 amatak-shop-1.0.7/amatak_shop.egg-info/
+-rw-rw-rw-   0        0        0     3188 2023-07-30 06:44:55.000000 amatak-shop-1.0.7/amatak_shop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2233 2023-07-30 06:44:56.000000 amatak-shop-1.0.7/amatak_shop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 06:44:55.000000 amatak-shop-1.0.7/amatak_shop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-30 06:44:55.000000 amatak-shop-1.0.7/amatak_shop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.052040 amatak-shop-1.0.7/eCommerce/
+drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/eCommerce/settings/
+-rw-rw-rw-   0        0        0     1487 2023-07-30 03:32:50.000000 amatak-shop-1.0.7/eCommerce/settings/AmatakShopDev.py
+-rw-rw-rw-   0        0        0      256 2023-07-30 02:54:02.000000 amatak-shop-1.0.7/eCommerce/settings/__init__.py
+-rw-rw-rw-   0        0        0     2588 2023-07-30 03:15:58.000000 amatak-shop-1.0.7/eCommerce/settings/base.py
+-rw-rw-rw-   0        0        0     1096 2023-07-30 02:56:09.000000 amatak-shop-1.0.7/eCommerce/settings/production.py
+-rw-rw-rw-   0        0        0      564 2023-07-30 06:42:33.000000 amatak-shop-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.7/setup.py
```

### Comparing `amatak-shop-1.0.6/PKG-INFO` & `amatak-shop-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.6
+Version: 1.0.7
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `amatak-shop-1.0.6/README.md` & `amatak-shop-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/forms/checkout.py` & `amatak-shop-1.0.7/amatak_shop/forms/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/forms/coupon.py` & `amatak-shop-1.0.7/amatak_shop/forms/coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/forms/payment.py` & `amatak-shop-1.0.7/amatak_shop/forms/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/forms/refund.py` & `amatak-shop-1.0.7/amatak_shop/forms/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/management/commands/rename.py` & `amatak-shop-1.0.7/amatak_shop/management/commands/rename.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/migrations/0001_initial.py` & `amatak-shop-1.0.7/amatak_shop/migrations/0001_initial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.2 on 2023-07-29 03:02
+# Generated by Django 4.2.2 on 2023-07-30 06:40
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django_countries.fields
 
 
@@ -62,16 +62,16 @@
                 ('start_date', models.DateTimeField(auto_now_add=True)),
                 ('ordered_date', models.DateTimeField()),
                 ('ordered', models.BooleanField(default=False)),
                 ('being_delivered', models.BooleanField(default=False)),
                 ('received', models.BooleanField(default=False)),
                 ('refund_requested', models.BooleanField(default=False)),
                 ('refund_granted', models.BooleanField(default=False)),
-                ('billing_address', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='billing_address', to='Aamatak_shop.address')),
-                ('coupon', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='Aamatak_shop.coupon')),
+                ('billing_address', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='billing_address', to='amatak_shop.address')),
+                ('coupon', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='amatak_shop.coupon')),
             ],
         ),
         migrations.CreateModel(
             name='UserProfile',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('stripe_customer_id', models.CharField(blank=True, max_length=50, null=True)),
@@ -82,15 +82,15 @@
         migrations.CreateModel(
             name='Refund',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('reason', models.TextField()),
                 ('accepted', models.BooleanField(default=False)),
                 ('email', models.EmailField(max_length=254)),
-                ('order', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='Aamatak_shop.order')),
+                ('order', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='amatak_shop.order')),
             ],
         ),
         migrations.CreateModel(
             name='Payment',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('stripe_charge_id', models.CharField(max_length=50)),
@@ -101,32 +101,32 @@
         ),
         migrations.CreateModel(
             name='OrderItem',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('ordered', models.BooleanField(default=False)),
                 ('quantity', models.IntegerField(default=1)),
-                ('item', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='Aamatak_shop.item')),
+                ('item', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='amatak_shop.item')),
                 ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
             ],
         ),
         migrations.AddField(
             model_name='order',
             name='items',
-            field=models.ManyToManyField(to='Aamatak_shop.orderitem'),
+            field=models.ManyToManyField(to='amatak_shop.orderitem'),
         ),
         migrations.AddField(
             model_name='order',
             name='payment',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='Aamatak_shop.payment'),
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='amatak_shop.payment'),
         ),
         migrations.AddField(
             model_name='order',
             name='shipping_address',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='shipping_address', to='Aamatak_shop.address'),
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='shipping_address', to='amatak_shop.address'),
         ),
         migrations.AddField(
             model_name='order',
             name='user',
             field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL),
         ),
     ]
```

### Comparing `amatak-shop-1.0.6/amatak_shop/models/__init__.py` & `amatak-shop-1.0.7/amatak_shop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/address.py` & `amatak-shop-1.0.7/amatak_shop/models/address.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/category.py` & `amatak-shop-1.0.7/amatak_shop/models/category.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/item.py` & `amatak-shop-1.0.7/amatak_shop/models/item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/mixins.py` & `amatak-shop-1.0.7/amatak_shop/models/mixins.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/order.py` & `amatak-shop-1.0.7/amatak_shop/models/order.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,40 +14,20 @@
 from django.db.models.signals import post_save
 from django.conf import settings
 from django.db import models
 from django.db.models import Sum
 from django.shortcuts import reverse
 from django_countries.fields import CountryField
 from amatak_shop.models.order_item import OrderItem
+from amatak_shop.models.category import CATEGORY_CHOICES,LABEL_CHOICES, ADDRESS_CHOICES, COLOR_CHOICES
 
 stripe.api_key = settings.STRIPE_SECRET_KEY
 
 
 
-CATEGORY_CHOICES = (
-    ('S', 'Shirt'),
-    ('SW', 'Sport wear'),
-    ('OW', 'Outwear'),
-    ('AU', 'Automotive'),
-    ('HD', 'Honda')
-
-)
-
-LABEL_CHOICES = (
-    ('P', 'primary'),
-    ('S', 'secondary'),
-    ('D', 'danger')
-)
-
-ADDRESS_CHOICES = (
-    ('B', 'Billing'),
-    ('S', 'Shipping'),
-)
-
-
 class Order(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL,
                              on_delete=models.CASCADE)
     ref_code = models.CharField(max_length=20, blank=True, null=True)
     items = models.ManyToManyField(OrderItem)
     start_date = models.DateTimeField(auto_now_add=True)
     ordered_date = models.DateTimeField()
@@ -61,24 +41,14 @@
     coupon = models.ForeignKey(
         'Coupon', on_delete=models.SET_NULL, blank=True, null=True)
     being_delivered = models.BooleanField(default=False)
     received = models.BooleanField(default=False)
     refund_requested = models.BooleanField(default=False)
     refund_granted = models.BooleanField(default=False)
 
-    '''
-    1. Item added to cart
-    2. Adding a billing address
-    (Failed checkout)
-    3. Payment
-    (Preprocessing, processing, packaging etc.)
-    4. Being delivered
-    5. Received
-    6. Refunds
-    '''
 
     def __str__(self):
         return self.user.username
 
     def get_total(self):
         total = 0
         for order_item in self.items.all():
```

### Comparing `amatak-shop-1.0.6/amatak_shop/models/order_item.py` & `amatak-shop-1.0.7/amatak_shop/models/order_item.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,34 +7,14 @@
 for business <www.amatak.io>
 OpenSource <www.amatak.org>
 """
 from django.conf import settings
 from django.db import models
 from amatak_shop.models.item import Item
 
-CATEGORY_CHOICES = (
-    ('M', 'Makes'),
-    ('B', 'Body'),
-    ('AE', 'Auto Electrical'),
-    ('L', 'Lighting'),
-    ('ME', 'Mechanical'),
-    ('C', 'Cooling')
-
-)
-
-LABEL_CHOICES = (
-    ('M', 'primary'),
-    ('B', 'secondary'),
-    ('AE', 'danger')
-)
-
-ADDRESS_CHOICES = (
-    ('B', 'Billing'),
-    ('S', 'Shipping'),
-)
 
 class OrderItem(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL,
                              on_delete=models.CASCADE)
     ordered = models.BooleanField(default=False)
     item = models.ForeignKey(Item, on_delete=models.CASCADE)
     quantity = models.IntegerField(default=1)
```

### Comparing `amatak-shop-1.0.6/amatak_shop/models/payment.py` & `amatak-shop-1.0.7/amatak_shop/models/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/refund.py` & `amatak-shop-1.0.7/amatak_shop/models/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/models/user_receiver_profile.py` & `amatak-shop-1.0.7/amatak_shop/models/user_receiver_profile.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/settings/base.py` & `amatak-shop-1.0.7/amatak_shop/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/templatetags/amatak_shop.py` & `amatak-shop-1.0.7/amatak_shop/templatetags/amatak_shop.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/tests/__init__.py` & `amatak-shop-1.0.7/amatak_shop/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/urls/__init__.py` & `amatak-shop-1.0.7/amatak_shop/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/urls/home.py` & `amatak-shop-1.0.7/amatak_shop/urls/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/__init__.py` & `amatak-shop-1.0.7/amatak_shop/views/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/add_coupon.py` & `amatak-shop-1.0.7/amatak_shop/views/add_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/add_to_cart.py` & `amatak-shop-1.0.7/amatak_shop/views/add_to_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/checkout.py` & `amatak-shop-1.0.7/amatak_shop/views/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/get_coupon.py` & `amatak-shop-1.0.7/amatak_shop/views/get_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/home.py` & `amatak-shop-1.0.7/amatak_shop/views/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/is_valid_form.py` & `amatak-shop-1.0.7/amatak_shop/views/is_valid_form.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/login.py` & `amatak-shop-1.0.7/amatak_shop/views/login.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/logout.py` & `amatak-shop-1.0.7/amatak_shop/views/logout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/order_summary.py` & `amatak-shop-1.0.7/amatak_shop/views/order_summary.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/payment.py` & `amatak-shop-1.0.7/amatak_shop/views/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/policy.py` & `amatak-shop-1.0.7/amatak_shop/views/policy.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/products.py` & `amatak-shop-1.0.7/amatak_shop/views/products.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/remove_from_cart.py` & `amatak-shop-1.0.7/amatak_shop/views/remove_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/remove_single_item_from_cart.py` & `amatak-shop-1.0.7/amatak_shop/views/remove_single_item_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/request_refund.py` & `amatak-shop-1.0.7/amatak_shop/views/request_refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/sign_up.py` & `amatak-shop-1.0.7/amatak_shop/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop/views/terms.py` & `amatak-shop-1.0.7/amatak_shop/views/terms.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/amatak_shop.egg-info/PKG-INFO` & `amatak-shop-1.0.7/amatak_shop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.6
+Version: 1.0.7
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `amatak-shop-1.0.6/amatak_shop.egg-info/SOURCES.txt` & `amatak-shop-1.0.7/amatak_shop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/eCommerce/settings/AmatakShopDev.py` & `amatak-shop-1.0.7/eCommerce/settings/AmatakShopDev.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/eCommerce/settings/base.py` & `amatak-shop-1.0.7/eCommerce/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/eCommerce/settings/production.py` & `amatak-shop-1.0.7/eCommerce/settings/production.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.6/pyproject.toml` & `amatak-shop-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amatak-shop"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Rony MAN", email="amatak.io@outlook.com" },
 ]
 description = "Amatak OpenSource Online Shop "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

