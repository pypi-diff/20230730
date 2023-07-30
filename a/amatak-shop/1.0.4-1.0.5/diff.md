# Comparing `tmp/amatak-shop-1.0.4.tar.gz` & `tmp/amatak-shop-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amatak-shop-1.0.4.tar", last modified: Sun Jul 30 00:54:24 2023, max compression
+gzip compressed data, was "amatak-shop-1.0.5.tar", last modified: Sun Jul 30 02:04:03 2023, max compression
```

## Comparing `amatak-shop-1.0.4.tar` & `amatak-shop-1.0.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.572194 amatak-shop-1.0.4/
--rw-rw-rw-   0        0        0     3001 2023-07-30 00:54:24.572194 amatak-shop-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2484 2023-07-30 00:52:06.000000 amatak-shop-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.396122 amatak-shop-1.0.4/amatak_shop/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.433894 amatak-shop-1.0.4/amatak_shop/forms/
--rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.4/amatak_shop/forms/__init__.py
--rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.4/amatak_shop/forms/checkout.py
--rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.4/amatak_shop/forms/coupon.py
--rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.4/amatak_shop/forms/payment.py
--rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.4/amatak_shop/forms/payment_choices.py
--rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.4/amatak_shop/forms/refund.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.396122 amatak-shop-1.0.4/amatak_shop/management/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.449554 amatak-shop-1.0.4/amatak_shop/management/commands/
--rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.4/amatak_shop/management/commands/rename.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.449554 amatak-shop-1.0.4/amatak_shop/migrations/
--rw-rw-rw-   0        0        0     7382 2023-07-29 03:02:06.000000 amatak-shop-1.0.4/amatak_shop/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.4/amatak_shop/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.471906 amatak-shop-1.0.4/amatak_shop/models/
--rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.4/amatak_shop/models/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.4/amatak_shop/models/address.py
--rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.4/amatak_shop/models/category.py
--rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.4/amatak_shop/models/coupon.py
--rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.4/amatak_shop/models/item.py
--rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.4/amatak_shop/models/mixins.py
--rw-rw-rw-   0        0        0     2691 2023-07-27 12:36:01.000000 amatak-shop-1.0.4/amatak_shop/models/order.py
--rw-rw-rw-   0        0        0     1648 2023-07-27 12:36:18.000000 amatak-shop-1.0.4/amatak_shop/models/order_item.py
--rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.4/amatak_shop/models/payment.py
--rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.4/amatak_shop/models/refund.py
--rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.4/amatak_shop/models/user_profile.py
--rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.4/amatak_shop/models/user_receiver_profile.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.471906 amatak-shop-1.0.4/amatak_shop/settings/
--rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.4/amatak_shop/settings/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.4/amatak_shop/settings/base.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.487525 amatak-shop-1.0.4/amatak_shop/templatetags/
--rw-rw-rw-   0        0        0      249 2023-07-27 12:27:28.000000 amatak-shop-1.0.4/amatak_shop/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2316 2023-07-28 23:36:12.000000 amatak-shop-1.0.4/amatak_shop/templatetags/amatak_shop.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.487525 amatak-shop-1.0.4/amatak_shop/tests/
--rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.4/amatak_shop/tests/__init__.py
--rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.4/amatak_shop/tests/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.520775 amatak-shop-1.0.4/amatak_shop/urls/
--rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.4/amatak_shop/urls/__init__.py
--rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.4/amatak_shop/urls/add_coupon.py
--rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.4/amatak_shop/urls/add_to_cart.py
--rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.4/amatak_shop/urls/checkout.py
--rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.4/amatak_shop/urls/home.py
--rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.4/amatak_shop/urls/order_summary.py
--rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.4/amatak_shop/urls/payment.py
--rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.4/amatak_shop/urls/policy.py
--rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.4/amatak_shop/urls/products.py
--rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.4/amatak_shop/urls/remove_from_cart.py
--rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.4/amatak_shop/urls/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.4/amatak_shop/urls/request_refund.py
--rw-rw-rw-   0        0        0      419 2023-07-27 11:58:31.000000 amatak-shop-1.0.4/amatak_shop/urls/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.556573 amatak-shop-1.0.4/amatak_shop/views/
--rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.4/amatak_shop/views/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.4/amatak_shop/views/add_coupon.py
--rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.4/amatak_shop/views/add_to_cart.py
--rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.4/amatak_shop/views/checkout.py
--rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.4/amatak_shop/views/create_ref_code.py
--rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.4/amatak_shop/views/get_coupon.py
--rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.4/amatak_shop/views/home.py
--rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.4/amatak_shop/views/is_valid_form.py
--rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.4/amatak_shop/views/items_detail_views.py
--rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.4/amatak_shop/views/login.py
--rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.4/amatak_shop/views/logout.py
--rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.4/amatak_shop/views/order_summary.py
--rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.4/amatak_shop/views/payment.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.4/amatak_shop/views/policy.py
--rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.4/amatak_shop/views/products.py
--rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.4/amatak_shop/views/remove_from_cart.py
--rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.4/amatak_shop/views/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.4/amatak_shop/views/request_refund.py
--rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.4/amatak_shop/views/sign_up.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.4/amatak_shop/views/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.433894 amatak-shop-1.0.4/amatak_shop.egg-info/
--rw-rw-rw-   0        0        0     3001 2023-07-30 00:54:24.000000 amatak-shop-1.0.4/amatak_shop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2023-07-30 00:54:24.000000 amatak-shop-1.0.4/amatak_shop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 00:54:24.000000 amatak-shop-1.0.4/amatak_shop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-30 00:54:24.000000 amatak-shop-1.0.4/amatak_shop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.396122 amatak-shop-1.0.4/eCommerce/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:54:24.572194 amatak-shop-1.0.4/eCommerce/settings/
--rw-rw-rw-   0        0        0     1537 2023-07-27 00:30:50.000000 amatak-shop-1.0.4/eCommerce/settings/AmatakShopDev.py
--rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.4/eCommerce/settings/__init__.py
--rw-rw-rw-   0        0        0     2534 2023-07-29 06:54:45.000000 amatak-shop-1.0.4/eCommerce/settings/base.py
--rw-rw-rw-   0        0        0     1173 2023-07-26 22:52:25.000000 amatak-shop-1.0.4/eCommerce/settings/production.py
--rw-rw-rw-   0        0        0      564 2023-07-30 00:52:58.000000 amatak-shop-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 00:54:24.572194 amatak-shop-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.853702 amatak-shop-1.0.5/
+-rw-rw-rw-   0        0        0     3213 2023-07-30 02:04:03.853702 amatak-shop-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2023-07-30 02:01:47.000000 amatak-shop-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.144834 amatak-shop-1.0.5/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.249372 amatak-shop-1.0.5/amatak_shop/forms/
+-rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.5/amatak_shop/forms/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.5/amatak_shop/forms/checkout.py
+-rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.5/amatak_shop/forms/coupon.py
+-rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.5/amatak_shop/forms/payment.py
+-rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.5/amatak_shop/forms/payment_choices.py
+-rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.5/amatak_shop/forms/refund.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.144834 amatak-shop-1.0.5/amatak_shop/management/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.249372 amatak-shop-1.0.5/amatak_shop/management/commands/
+-rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.5/amatak_shop/management/commands/rename.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.270826 amatak-shop-1.0.5/amatak_shop/migrations/
+-rw-rw-rw-   0        0        0     7382 2023-07-29 03:02:06.000000 amatak-shop-1.0.5/amatak_shop/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.5/amatak_shop/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.402025 amatak-shop-1.0.5/amatak_shop/models/
+-rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.5/amatak_shop/models/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.5/amatak_shop/models/address.py
+-rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.5/amatak_shop/models/category.py
+-rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.5/amatak_shop/models/coupon.py
+-rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.5/amatak_shop/models/item.py
+-rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.5/amatak_shop/models/mixins.py
+-rw-rw-rw-   0        0        0     2691 2023-07-27 12:36:01.000000 amatak-shop-1.0.5/amatak_shop/models/order.py
+-rw-rw-rw-   0        0        0     1648 2023-07-27 12:36:18.000000 amatak-shop-1.0.5/amatak_shop/models/order_item.py
+-rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.5/amatak_shop/models/payment.py
+-rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.5/amatak_shop/models/refund.py
+-rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.5/amatak_shop/models/user_profile.py
+-rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.5/amatak_shop/models/user_receiver_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.433304 amatak-shop-1.0.5/amatak_shop/settings/
+-rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.5/amatak_shop/settings/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.5/amatak_shop/settings/base.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.448889 amatak-shop-1.0.5/amatak_shop/templatetags/
+-rw-rw-rw-   0        0        0      499 2023-07-30 01:57:57.000000 amatak-shop-1.0.5/amatak_shop/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2316 2023-07-28 23:36:12.000000 amatak-shop-1.0.5/amatak_shop/templatetags/amatak_shop.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.480133 amatak-shop-1.0.5/amatak_shop/tests/
+-rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.5/amatak_shop/tests/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.5/amatak_shop/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.564401 amatak-shop-1.0.5/amatak_shop/urls/
+-rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.5/amatak_shop/urls/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.5/amatak_shop/urls/add_coupon.py
+-rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.5/amatak_shop/urls/add_to_cart.py
+-rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.5/amatak_shop/urls/checkout.py
+-rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.5/amatak_shop/urls/home.py
+-rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.5/amatak_shop/urls/order_summary.py
+-rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.5/amatak_shop/urls/payment.py
+-rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.5/amatak_shop/urls/policy.py
+-rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.5/amatak_shop/urls/products.py
+-rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.5/amatak_shop/urls/remove_from_cart.py
+-rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.5/amatak_shop/urls/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.5/amatak_shop/urls/request_refund.py
+-rw-rw-rw-   0        0        0      419 2023-07-27 11:58:31.000000 amatak-shop-1.0.5/amatak_shop/urls/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.785076 amatak-shop-1.0.5/amatak_shop/views/
+-rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.5/amatak_shop/views/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.5/amatak_shop/views/add_coupon.py
+-rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.5/amatak_shop/views/add_to_cart.py
+-rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.5/amatak_shop/views/checkout.py
+-rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.5/amatak_shop/views/create_ref_code.py
+-rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.5/amatak_shop/views/get_coupon.py
+-rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.5/amatak_shop/views/home.py
+-rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.5/amatak_shop/views/is_valid_form.py
+-rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.5/amatak_shop/views/items_detail_views.py
+-rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.5/amatak_shop/views/login.py
+-rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.5/amatak_shop/views/logout.py
+-rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.5/amatak_shop/views/order_summary.py
+-rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.5/amatak_shop/views/payment.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.5/amatak_shop/views/policy.py
+-rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.5/amatak_shop/views/products.py
+-rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.5/amatak_shop/views/remove_from_cart.py
+-rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.5/amatak_shop/views/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.5/amatak_shop/views/request_refund.py
+-rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.5/amatak_shop/views/sign_up.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.5/amatak_shop/views/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.171238 amatak-shop-1.0.5/amatak_shop.egg-info/
+-rw-rw-rw-   0        0        0     3213 2023-07-30 02:04:03.000000 amatak-shop-1.0.5/amatak_shop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2233 2023-07-30 02:04:03.000000 amatak-shop-1.0.5/amatak_shop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 02:04:03.000000 amatak-shop-1.0.5/amatak_shop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-30 02:04:03.000000 amatak-shop-1.0.5/amatak_shop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.144834 amatak-shop-1.0.5/eCommerce/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:04:03.853702 amatak-shop-1.0.5/eCommerce/settings/
+-rw-rw-rw-   0        0        0     1537 2023-07-27 00:30:50.000000 amatak-shop-1.0.5/eCommerce/settings/AmatakShopDev.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.5/eCommerce/settings/__init__.py
+-rw-rw-rw-   0        0        0     2534 2023-07-29 06:54:45.000000 amatak-shop-1.0.5/eCommerce/settings/base.py
+-rw-rw-rw-   0        0        0     1173 2023-07-26 22:52:25.000000 amatak-shop-1.0.5/eCommerce/settings/production.py
+-rw-rw-rw-   0        0        0      564 2023-07-30 02:02:56.000000 amatak-shop-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 02:04:03.853702 amatak-shop-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.5/setup.py
```

### Comparing `amatak-shop-1.0.4/PKG-INFO` & `amatak-shop-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.4
+Version: 1.0.5
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,19 +43,27 @@
 
 ### Install from py library:
 
 ````
 pip install amatak-shop
 ````
 
-### add amatak to django app installed:
-# in Django App setting.
+### Installed App:
+# add (amatak_shop) in Django App setting.
 
 ````
-pip install Django
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'amatak_shop',
+]
 ````
 
 
 ### Current Contents.
 # Current Version 1.0.4
 # features:
 ## Categories:
```

### Comparing `amatak-shop-1.0.4/README.md` & `amatak-shop-1.0.5/amatak_shop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: amatak-shop
+Version: 1.0.5
+Summary: Amatak OpenSource Online Shop 
+Author-email: Rony MAN <amatak.io@outlook.com>
+Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
+Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 __Amatak Online Shop__ was created and is currently maintained and developed by Amatak the full documentation can be found in
 [amatak.org](https://amatak.org/docs/projects/AmatakOnlineShop)
 
 ### Join our  [Stack Overflow](https://stackoverflow.com/users/22269946/amatak)
 
 To clone this project from 
 [GitHub](https://github.com/amatak-org/AmatakOnlineShop).
@@ -30,19 +43,27 @@
 
 ### Install from py library:
 
 ````
 pip install amatak-shop
 ````
 
-### add amatak to django app installed:
-# in Django App setting.
+### Installed App:
+# add (amatak_shop) in Django App setting.
 
 ````
-pip install Django
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'amatak_shop',
+]
 ````
 
 
 ### Current Contents.
 # Current Version 1.0.4
 # features:
 ## Categories:
@@ -94,8 +115,8 @@
 # Homepage Screen
 ![Home Screen](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot.png)
 
 # Client Checkout With Coupon
 ![Check Out cart](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot_checkout_with_coupon.png)
 
 # Client Checkout Views
-![Check Out cart](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot_checkout.png)
+![Check Out cart](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot_checkout.png)
```

### Comparing `amatak-shop-1.0.4/amatak_shop/forms/checkout.py` & `amatak-shop-1.0.5/amatak_shop/forms/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/forms/coupon.py` & `amatak-shop-1.0.5/amatak_shop/forms/coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/forms/payment.py` & `amatak-shop-1.0.5/amatak_shop/forms/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/forms/refund.py` & `amatak-shop-1.0.5/amatak_shop/forms/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/management/commands/rename.py` & `amatak-shop-1.0.5/amatak_shop/management/commands/rename.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/migrations/0001_initial.py` & `amatak-shop-1.0.5/amatak_shop/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/__init__.py` & `amatak-shop-1.0.5/amatak_shop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/address.py` & `amatak-shop-1.0.5/amatak_shop/models/address.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/category.py` & `amatak-shop-1.0.5/amatak_shop/models/category.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/item.py` & `amatak-shop-1.0.5/amatak_shop/models/item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/mixins.py` & `amatak-shop-1.0.5/amatak_shop/models/mixins.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/order.py` & `amatak-shop-1.0.5/amatak_shop/models/order.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/order_item.py` & `amatak-shop-1.0.5/amatak_shop/models/order_item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/payment.py` & `amatak-shop-1.0.5/amatak_shop/models/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/refund.py` & `amatak-shop-1.0.5/amatak_shop/models/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/models/user_receiver_profile.py` & `amatak-shop-1.0.5/amatak_shop/models/user_receiver_profile.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/settings/base.py` & `amatak-shop-1.0.5/amatak_shop/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/templatetags/amatak_shop.py` & `amatak-shop-1.0.5/amatak_shop/templatetags/amatak_shop.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/tests/__init__.py` & `amatak-shop-1.0.5/amatak_shop/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/urls/__init__.py` & `amatak-shop-1.0.5/amatak_shop/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/urls/home.py` & `amatak-shop-1.0.5/amatak_shop/urls/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/__init__.py` & `amatak-shop-1.0.5/amatak_shop/views/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/add_coupon.py` & `amatak-shop-1.0.5/amatak_shop/views/add_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/add_to_cart.py` & `amatak-shop-1.0.5/amatak_shop/views/add_to_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/checkout.py` & `amatak-shop-1.0.5/amatak_shop/views/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/get_coupon.py` & `amatak-shop-1.0.5/amatak_shop/views/get_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/home.py` & `amatak-shop-1.0.5/amatak_shop/views/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/is_valid_form.py` & `amatak-shop-1.0.5/amatak_shop/views/is_valid_form.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/login.py` & `amatak-shop-1.0.5/amatak_shop/views/login.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/logout.py` & `amatak-shop-1.0.5/amatak_shop/views/logout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/order_summary.py` & `amatak-shop-1.0.5/amatak_shop/views/order_summary.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/payment.py` & `amatak-shop-1.0.5/amatak_shop/views/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/policy.py` & `amatak-shop-1.0.5/amatak_shop/views/policy.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/products.py` & `amatak-shop-1.0.5/amatak_shop/views/products.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/remove_from_cart.py` & `amatak-shop-1.0.5/amatak_shop/views/remove_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/remove_single_item_from_cart.py` & `amatak-shop-1.0.5/amatak_shop/views/remove_single_item_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/request_refund.py` & `amatak-shop-1.0.5/amatak_shop/views/request_refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/sign_up.py` & `amatak-shop-1.0.5/amatak_shop/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop/views/terms.py` & `amatak-shop-1.0.5/amatak_shop/views/terms.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/amatak_shop.egg-info/PKG-INFO` & `amatak-shop-1.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: amatak-shop
-Version: 1.0.4
-Summary: Amatak OpenSource Online Shop 
-Author-email: Rony MAN <amatak.io@outlook.com>
-Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
-Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 __Amatak Online Shop__ was created and is currently maintained and developed by Amatak the full documentation can be found in
 [amatak.org](https://amatak.org/docs/projects/AmatakOnlineShop)
 
 ### Join our  [Stack Overflow](https://stackoverflow.com/users/22269946/amatak)
 
 To clone this project from 
 [GitHub](https://github.com/amatak-org/AmatakOnlineShop).
@@ -43,19 +30,27 @@
 
 ### Install from py library:
 
 ````
 pip install amatak-shop
 ````
 
-### add amatak to django app installed:
-# in Django App setting.
+### Installed App:
+# add (amatak_shop) in Django App setting.
 
 ````
-pip install Django
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'amatak_shop',
+]
 ````
 
 
 ### Current Contents.
 # Current Version 1.0.4
 # features:
 ## Categories:
@@ -107,8 +102,8 @@
 # Homepage Screen
 ![Home Screen](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot.png)
 
 # Client Checkout With Coupon
 ![Check Out cart](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot_checkout_with_coupon.png)
 
 # Client Checkout Views
-![Check Out cart](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot_checkout.png)
+![Check Out cart](https://pub-3f83785b7aa64195b0afb81d8ef9ca5c.r2.dev/Images/cdn.amatak.org/screenshot_checkout.png)
```

### Comparing `amatak-shop-1.0.4/amatak_shop.egg-info/SOURCES.txt` & `amatak-shop-1.0.5/amatak_shop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/eCommerce/settings/AmatakShopDev.py` & `amatak-shop-1.0.5/eCommerce/settings/AmatakShopDev.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/eCommerce/settings/base.py` & `amatak-shop-1.0.5/eCommerce/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/eCommerce/settings/production.py` & `amatak-shop-1.0.5/eCommerce/settings/production.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.4/pyproject.toml` & `amatak-shop-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amatak-shop"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Rony MAN", email="amatak.io@outlook.com" },
 ]
 description = "Amatak OpenSource Online Shop "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

