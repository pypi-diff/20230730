# Comparing `tmp/amatak-shop-1.0.7.tar.gz` & `tmp/amatak-shop-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amatak-shop-1.0.7.tar", last modified: Sun Jul 30 06:44:56 2023, max compression
+gzip compressed data, was "amatak-shop-1.0.8.tar", last modified: Sun Jul 30 07:39:11 2023, max compression
```

## Comparing `amatak-shop-1.0.7.tar` & `amatak-shop-1.0.8.tar`

### file list

```diff
@@ -1,88 +1,389 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/
--rw-rw-rw-   0        0        0     3188 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2671 2023-07-30 02:05:48.000000 amatak-shop-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.052040 amatak-shop-1.0.7/amatak_shop/
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.095329 amatak-shop-1.0.7/amatak_shop/forms/
--rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.7/amatak_shop/forms/__init__.py
--rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.7/amatak_shop/forms/checkout.py
--rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.7/amatak_shop/forms/coupon.py
--rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.7/amatak_shop/forms/payment.py
--rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.7/amatak_shop/forms/payment_choices.py
--rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.7/amatak_shop/forms/refund.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.052040 amatak-shop-1.0.7/amatak_shop/management/
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.099335 amatak-shop-1.0.7/amatak_shop/management/commands/
--rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.7/amatak_shop/management/commands/rename.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.099335 amatak-shop-1.0.7/amatak_shop/migrations/
--rw-rw-rw-   0        0        0     7375 2023-07-30 06:40:44.000000 amatak-shop-1.0.7/amatak_shop/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.7/amatak_shop/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.114962 amatak-shop-1.0.7/amatak_shop/models/
--rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.7/amatak_shop/models/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.7/amatak_shop/models/address.py
--rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.7/amatak_shop/models/category.py
--rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.7/amatak_shop/models/coupon.py
--rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.7/amatak_shop/models/item.py
--rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.7/amatak_shop/models/mixins.py
--rw-rw-rw-   0        0        0     2255 2023-07-30 06:32:21.000000 amatak-shop-1.0.7/amatak_shop/models/order.py
--rw-rw-rw-   0        0        0     1308 2023-07-30 06:28:38.000000 amatak-shop-1.0.7/amatak_shop/models/order_item.py
--rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.7/amatak_shop/models/payment.py
--rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.7/amatak_shop/models/refund.py
--rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.7/amatak_shop/models/user_profile.py
--rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.7/amatak_shop/models/user_receiver_profile.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.130584 amatak-shop-1.0.7/amatak_shop/settings/
--rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.7/amatak_shop/settings/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.7/amatak_shop/settings/base.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.130584 amatak-shop-1.0.7/amatak_shop/templatetags/
--rw-rw-rw-   0        0        0      499 2023-07-30 06:43:41.000000 amatak-shop-1.0.7/amatak_shop/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-07-30 03:29:14.000000 amatak-shop-1.0.7/amatak_shop/templatetags/amatak_shop.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.130584 amatak-shop-1.0.7/amatak_shop/tests/
--rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.7/amatak_shop/tests/__init__.py
--rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.7/amatak_shop/tests/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.167933 amatak-shop-1.0.7/amatak_shop/urls/
--rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.7/amatak_shop/urls/__init__.py
--rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.7/amatak_shop/urls/add_coupon.py
--rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.7/amatak_shop/urls/add_to_cart.py
--rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.7/amatak_shop/urls/checkout.py
--rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.7/amatak_shop/urls/home.py
--rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.7/amatak_shop/urls/order_summary.py
--rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.7/amatak_shop/urls/payment.py
--rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.7/amatak_shop/urls/policy.py
--rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.7/amatak_shop/urls/products.py
--rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.7/amatak_shop/urls/remove_from_cart.py
--rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.7/amatak_shop/urls/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.7/amatak_shop/urls/request_refund.py
--rw-rw-rw-   0        0        0      419 2023-07-27 11:58:31.000000 amatak-shop-1.0.7/amatak_shop/urls/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.199603 amatak-shop-1.0.7/amatak_shop/views/
--rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.7/amatak_shop/views/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.7/amatak_shop/views/add_coupon.py
--rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.7/amatak_shop/views/add_to_cart.py
--rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.7/amatak_shop/views/checkout.py
--rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.7/amatak_shop/views/create_ref_code.py
--rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.7/amatak_shop/views/get_coupon.py
--rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.7/amatak_shop/views/home.py
--rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.7/amatak_shop/views/is_valid_form.py
--rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.7/amatak_shop/views/items_detail_views.py
--rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.7/amatak_shop/views/login.py
--rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.7/amatak_shop/views/logout.py
--rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.7/amatak_shop/views/order_summary.py
--rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.7/amatak_shop/views/payment.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.7/amatak_shop/views/policy.py
--rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.7/amatak_shop/views/products.py
--rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.7/amatak_shop/views/remove_from_cart.py
--rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.7/amatak_shop/views/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.7/amatak_shop/views/request_refund.py
--rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.7/amatak_shop/views/sign_up.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.7/amatak_shop/views/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.067703 amatak-shop-1.0.7/amatak_shop.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-07-30 06:44:55.000000 amatak-shop-1.0.7/amatak_shop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2023-07-30 06:44:56.000000 amatak-shop-1.0.7/amatak_shop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 06:44:55.000000 amatak-shop-1.0.7/amatak_shop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-30 06:44:55.000000 amatak-shop-1.0.7/amatak_shop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.052040 amatak-shop-1.0.7/eCommerce/
-drwxrwxrwx   0        0        0        0 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/eCommerce/settings/
--rw-rw-rw-   0        0        0     1487 2023-07-30 03:32:50.000000 amatak-shop-1.0.7/eCommerce/settings/AmatakShopDev.py
--rw-rw-rw-   0        0        0      256 2023-07-30 02:54:02.000000 amatak-shop-1.0.7/eCommerce/settings/__init__.py
--rw-rw-rw-   0        0        0     2588 2023-07-30 03:15:58.000000 amatak-shop-1.0.7/eCommerce/settings/base.py
--rw-rw-rw-   0        0        0     1096 2023-07-30 02:56:09.000000 amatak-shop-1.0.7/eCommerce/settings/production.py
--rw-rw-rw-   0        0        0      564 2023-07-30 06:42:33.000000 amatak-shop-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 06:44:56.215232 amatak-shop-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:11.019781 amatak-shop-1.0.8/
+-rw-rw-rw-   0        0        0       86 2023-07-30 07:37:14.000000 amatak-shop-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3188 2023-07-30 07:39:11.019781 amatak-shop-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2671 2023-07-30 02:05:48.000000 amatak-shop-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.680952 amatak-shop-1.0.8/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.828806 amatak-shop-1.0.8/amatak_shop/forms/
+-rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.8/amatak_shop/forms/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.8/amatak_shop/forms/checkout.py
+-rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.8/amatak_shop/forms/coupon.py
+-rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.8/amatak_shop/forms/payment.py
+-rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.8/amatak_shop/forms/payment_choices.py
+-rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.8/amatak_shop/forms/refund.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.640060 amatak-shop-1.0.8/amatak_shop/management/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.844424 amatak-shop-1.0.8/amatak_shop/management/commands/
+-rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.8/amatak_shop/management/commands/rename.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.844424 amatak-shop-1.0.8/amatak_shop/migrations/
+-rw-rw-rw-   0        0        0     7375 2023-07-30 06:40:44.000000 amatak-shop-1.0.8/amatak_shop/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.8/amatak_shop/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.012486 amatak-shop-1.0.8/amatak_shop/models/
+-rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.8/amatak_shop/models/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.8/amatak_shop/models/address.py
+-rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.8/amatak_shop/models/category.py
+-rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.8/amatak_shop/models/coupon.py
+-rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.8/amatak_shop/models/item.py
+-rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.8/amatak_shop/models/mixins.py
+-rw-rw-rw-   0        0        0     2255 2023-07-30 06:32:21.000000 amatak-shop-1.0.8/amatak_shop/models/order.py
+-rw-rw-rw-   0        0        0     1308 2023-07-30 06:28:38.000000 amatak-shop-1.0.8/amatak_shop/models/order_item.py
+-rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.8/amatak_shop/models/payment.py
+-rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.8/amatak_shop/models/refund.py
+-rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.8/amatak_shop/models/user_profile.py
+-rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.8/amatak_shop/models/user_receiver_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.043732 amatak-shop-1.0.8/amatak_shop/settings/
+-rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.8/amatak_shop/settings/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.8/amatak_shop/settings/base.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.644048 amatak-shop-1.0.8/amatak_shop/static/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.665992 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.129372 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/
+-rw-rw-rw-   0        0        0     1080 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/LICENSE
+-rw-rw-rw-   0        0        0    12459 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/README.md
+-rw-rw-rw-   0        0        0      300 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/bulma.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.242764 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/
+-rw-rw-rw-   0        0        0   245633 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css
+-rw-rw-rw-   0        0        0    98598 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css.map
+-rw-rw-rw-   0        0        0   207445 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.min.css
+-rw-rw-rw-   0        0        0   245486 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/bulma.css
+-rw-rw-rw-   0        0        0    98583 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/bulma.css.map
+-rw-rw-rw-   0        0        0   207302 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/css/bulma.min.css
+-rw-rw-rw-   0        0        0     1761 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/package.json
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.655022 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.342687 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/base/
+-rw-rw-rw-   0        0        0       94 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/base/_all.sass
+-rw-rw-rw-   0        0        0       92 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/base/animations.sass
+-rw-rw-rw-   0        0        0     2640 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/base/generic.sass
+-rw-rw-rw-   0        0        0      129 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/base/helpers.sass
+-rw-rw-rw-   0        0        0      709 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/base/minireset.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.628389 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/
+-rw-rw-rw-   0        0        0      246 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/_all.sass
+-rw-rw-rw-   0        0        0     1786 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/breadcrumb.sass
+-rw-rw-rw-   0        0        0     2489 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/card.sass
+-rw-rw-rw-   0        0        0     2191 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/dropdown.sass
+-rw-rw-rw-   0        0        0     1487 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/level.sass
+-rw-rw-rw-   0        0        0     1439 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/media.sass
+-rw-rw-rw-   0        0        0     1714 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/menu.sass
+-rw-rw-rw-   0        0        0     3025 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/message.sass
+-rw-rw-rw-   0        0        0     3000 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/modal.sass
+-rw-rw-rw-   0        0        0    12197 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/navbar.sass
+-rw-rw-rw-   0        0        0     4133 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/pagination.sass
+-rw-rw-rw-   0        0        0     3288 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/panel.sass
+-rw-rw-rw-   0        0        0     5717 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/components/tabs.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:05.907538 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/
+-rw-rw-rw-   0        0        0      244 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/_all.sass
+-rw-rw-rw-   0        0        0      690 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/box.sass
+-rw-rw-rw-   0        0        0    10853 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/button.sass
+-rw-rw-rw-   0        0        0      886 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/container.sass
+-rw-rw-rw-   0        0        0     3913 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/content.sass
+-rw-rw-rw-   0        0        0      120 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/form.sass
+-rw-rw-rw-   0        0        0     1054 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/icon.sass
+-rw-rw-rw-   0        0        0     1263 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/image.sass
+-rw-rw-rw-   0        0        0     1445 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/notification.sass
+-rw-rw-rw-   0        0        0      521 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/other.sass
+-rw-rw-rw-   0        0        0     2050 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/progress.sass
+-rw-rw-rw-   0        0        0     3475 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/table.sass
+-rw-rw-rw-   0        0        0     3491 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/tag.sass
+-rw-rw-rw-   0        0        0     1743 2023-07-28 13:03:46.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/elements/title.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.023102 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/
+-rw-rw-rw-   0        0        0      150 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/_all.sass
+-rw-rw-rw-   0        0        0      407 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/checkbox-radio.sass
+-rw-rw-rw-   0        0        0     4263 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/file.sass
+-rw-rw-rw-   0        0        0     1453 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/input-textarea.sass
+-rw-rw-rw-   0        0        0     1999 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/select.sass
+-rw-rw-rw-   0        0        0     1792 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/shared.sass
+-rw-rw-rw-   0        0        0     4674 2023-07-28 13:03:44.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/form/tools.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.085652 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/grid/
+-rw-rw-rw-   0        0        0       69 2023-07-28 13:03:48.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/grid/_all.sass
+-rw-rw-rw-   0        0        0    14019 2023-07-28 13:03:48.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/grid/columns.sass
+-rw-rw-rw-   0        0        0      815 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/grid/tiles.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.250898 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/
+-rw-rw-rw-   0        0        0      202 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/_all.sass
+-rw-rw-rw-   0        0        0     1096 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/color.sass
+-rw-rw-rw-   0        0        0     1317 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/flexbox.sass
+-rw-rw-rw-   0        0        0      142 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/float.sass
+-rw-rw-rw-   0        0        0      241 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/other.sass
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/overflow.sass
+-rw-rw-rw-   0        0        0      108 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/position.sass
+-rw-rw-rw-   0        0        0     1164 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/spacing.sass
+-rw-rw-rw-   0        0        0     2474 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/typography.sass
+-rw-rw-rw-   0        0        0     2448 2023-07-28 13:03:47.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/helpers/visibility.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.344671 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/layout/
+-rw-rw-rw-   0        0        0       87 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/layout/_all.sass
+-rw-rw-rw-   0        0        0      293 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/layout/footer.sass
+-rw-rw-rw-   0        0        0     3651 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/layout/hero.sass
+-rw-rw-rw-   0        0        0      433 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/layout/section.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.518258 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/
+-rw-rw-rw-   0        0        0      170 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/_all.sass
+-rw-rw-rw-   0        0        0      119 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/animations.sass
+-rw-rw-rw-   0        0        0     1296 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/controls.sass
+-rw-rw-rw-   0        0        0     4005 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/derived-variables.sass
+-rw-rw-rw-   0        0        0      179 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/extends.sass
+-rw-rw-rw-   0        0        0     4896 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/functions.sass
+-rw-rw-rw-   0        0        0     2691 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/initial-variables.sass
+-rw-rw-rw-   0        0        0     6291 2023-07-28 13:03:45.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/bulma/sass/utilities/mixins.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.677194 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.792688 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/
+-rw-rw-rw-   0        0        0     5364 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/datatables-select.css
+-rw-rw-rw-   0        0        0     3962 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/datatables-select.min.css
+-rw-rw-rw-   0        0        0     5289 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/datatables.css
+-rw-rw-rw-   0        0        0     3767 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/datatables.min.css
+-rw-rw-rw-   0        0        0    10673 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/directives.css
+-rw-rw-rw-   0        0        0     8362 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/addons/directives.min.css
+-rw-rw-rw-   0        0        0   192348 2023-06-26 09:22:18.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/bootstrap.css
+-rw-rw-rw-   0        0        0   155758 2023-06-26 09:22:18.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   314326 2023-06-26 09:22:18.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/mdb.css
+-rw-rw-rw-   0        0        0   243602 2023-06-26 09:22:18.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/mdb.lite.css
+-rw-rw-rw-   0        0        0   199949 2023-06-26 09:22:18.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/mdb.lite.min.css
+-rw-rw-rw-   0        0        0   255261 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/mdb.min.css
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:06.829021 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/modules/
+-rw-rw-rw-   0        0        0    70879 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/modules/animations-extended.css
+-rw-rw-rw-   0        0        0    55325 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/modules/animations-extended.min.css
+-rw-rw-rw-   0        0        0      556 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/style.css
+-rw-rw-rw-   0        0        0      248 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/css/style.min.css
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.659009 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:07.231749 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/
+-rw-rw-rw-   0        0        0    20966 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.eot
+-rw-rw-rw-   0        0        0   127744 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0    62876 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff
+-rw-rw-rw-   0        0        0    49976 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff2
+-rw-rw-rw-   0        0        0    20940 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.eot
+-rw-rw-rw-   0        0        0   126792 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0    62316 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff
+-rw-rw-rw-   0        0        0    49380 2023-06-26 09:22:19.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff2
+-rw-rw-rw-   0        0        0    21364 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.eot
+-rw-rw-rw-   0        0        0   127488 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0    62980 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff
+-rw-rw-rw-   0        0        0    50224 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff2
+-rw-rw-rw-   0        0        0    21320 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.eot
+-rw-rw-rw-   0        0        0   126072 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0    61736 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff
+-rw-rw-rw-   0        0        0    49236 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff2
+-rw-rw-rw-   0        0        0    21659 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.eot
+-rw-rw-rw-   0        0        0   127584 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0    61628 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff
+-rw-rw-rw-   0        0        0    48524 2023-06-26 09:22:20.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff2
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:07.247370 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:07.283777 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/lightbox/
+-rw-rw-rw-   0        0        0      547 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/lightbox/default-skin.png
+-rw-rw-rw-   0        0        0     1554 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/lightbox/default-skin.svg
+-rw-rw-rw-   0        0        0      866 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/lightbox/preloader.gif
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:07.414855 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/
+-rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/01.png
+-rw-rw-rw-   0        0        0      213 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/02.png
+-rw-rw-rw-   0        0        0      209 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/03.png
+-rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/04.png
+-rw-rw-rw-   0        0        0      213 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/05.png
+-rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/06.png
+-rw-rw-rw-   0        0        0      215 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/07.png
+-rw-rw-rw-   0        0        0      146 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/08.png
+-rw-rw-rw-   0        0        0      137 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/overlays/09.png
+-rw-rw-rw-   0        0        0   204946 2023-06-26 09:22:21.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/sample.jpg
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:07.446094 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/svg/
+-rw-rw-rw-   0        0        0      218 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/svg/arrow_left.svg
+-rw-rw-rw-   0        0        0      217 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/img/svg/arrow_right.svg
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:07.925856 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:08.155759 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/addons/
+-rw-rw-rw-   0        0        0    32005 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/addons/datatables-select.js
+-rw-rw-rw-   0        0        0    11741 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/addons/datatables-select.min.js
+-rw-rw-rw-   0        0        0   452723 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/addons/datatables.js
+-rw-rw-rw-   0        0        0    84932 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/addons/datatables.min.js
+-rw-rw-rw-   0        0        0     1637 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/addons/rating.js
+-rw-rw-rw-   0        0        0   131637 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/bootstrap.js
+-rw-rw-rw-   0        0        0    58072 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    86927 2023-06-26 09:22:22.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0   478685 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/mdb.js
+-rw-rw-rw-   0        0        0   209696 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/mdb.min.js
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:08.593013 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/
+-rw-rw-rw-   0        0        0   402487 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/chart.js
+-rw-rw-rw-   0        0        0      570 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/default-file-input.js
+-rw-rw-rw-   0        0        0      685 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/enhanced-modals.js
+-rw-rw-rw-   0        0        0     5373 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/forms-free.js
+-rw-rw-rw-   0        0        0     8661 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/jquery.easing.js
+-rw-rw-rw-   0        0        0      409 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/scrolling-navbar.js
+-rw-rw-rw-   0        0        0      290 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/treeview.js
+-rw-rw-rw-   0        0        0    35106 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/velocity.js
+-rw-rw-rw-   0        0        0    35106 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/velocity.min.js
+-rw-rw-rw-   0        0        0    18936 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/waves.js
+-rw-rw-rw-   0        0        0     5324 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/modules/wow.js
+-rw-rw-rw-   0        0        0    20537 2023-06-26 09:22:23.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/js/popper.min.js
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:08.719719 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/
+-rw-rw-rw-   0        0        0      734 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/_custom-skin.scss
+-rw-rw-rw-   0        0        0       21 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/_custom-styles.scss
+-rw-rw-rw-   0        0        0       24 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/_custom-variables.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:08.772734 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/addons/
+-rw-rw-rw-   0        0        0     4573 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/addons/_datatables-select.scss
+-rw-rw-rw-   0        0        0     4203 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/addons/_datatables.scss
+-rw-rw-rw-   0        0        0     1477 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/addons/_directives.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:08.950801 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/
+-rw-rw-rw-   0        0        0    28149 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_colors.scss
+-rw-rw-rw-   0        0        0     2549 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_global.scss
+-rw-rw-rw-   0        0        0     1074 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_helpers.scss
+-rw-rw-rw-   0        0        0     1199 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_masks.scss
+-rw-rw-rw-   0        0        0    13073 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_mixins.scss
+-rw-rw-rw-   0        0        0     3665 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_typography.scss
+-rw-rw-rw-   0        0        0    17282 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_variables.scss
+-rw-rw-rw-   0        0        0     3967 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/_waves.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.020401 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/bootstrap/
+-rw-rw-rw-   0        0        0     2719 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/bootstrap/_functions.scss
+-rw-rw-rw-   0        0        0     6474 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/bootstrap/_rfs.scss
+-rw-rw-rw-   0        0        0    47781 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/core/bootstrap/_variables.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.437050 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/
+-rw-rw-rw-   0        0        0     2603 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_animations-basic.scss
+-rw-rw-rw-   0        0        0      335 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_badges.scss
+-rw-rw-rw-   0        0        0     3273 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_buttons.scss
+-rw-rw-rw-   0        0        0      580 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_cards.scss
+-rw-rw-rw-   0        0        0     1205 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_carousels.scss
+-rw-rw-rw-   0        0        0       47 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_depreciated.scss
+-rw-rw-rw-   0        0        0      144 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_dropdowns.scss
+-rw-rw-rw-   0        0        0      314 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_footers.scss
+-rw-rw-rw-   0        0        0    12170 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_forms.scss
+-rw-rw-rw-   0        0        0     1738 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_input-group.scss
+-rw-rw-rw-   0        0        0      557 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_list-group.scss
+-rw-rw-rw-   0        0        0      177 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_loader.scss
+-rw-rw-rw-   0        0        0     6505 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_modals.scss
+-rw-rw-rw-   0        0        0     3243 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_msc.scss
+-rw-rw-rw-   0        0        0     2540 2023-06-26 09:22:26.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_navbars.scss
+-rw-rw-rw-   0        0        0     1960 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_pagination.scss
+-rw-rw-rw-   0        0        0     3888 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_steppers.scss
+-rw-rw-rw-   0        0        0      894 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_switch.scss
+-rw-rw-rw-   0        0        0     1340 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_tables.scss
+-rw-rw-rw-   0        0        0      418 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/_treeview.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.671973 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/modules/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.470324 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/
+-rw-rw-rw-   0        0        0    22617 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/_module.scss
+-rw-rw-rw-   0        0        0      175 2023-06-26 09:22:27.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/animations-extended.scss
+-rw-rw-rw-   0        0        0     1555 2023-06-26 09:22:24.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/mdb.lite.scss
+-rw-rw-rw-   0        0        0     1724 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/mdb.scss
+-rw-rw-rw-   0        0        0      604 2023-06-26 09:22:25.000000 amatak-shop-1.0.8/amatak_shop/static/amatak_shop/scss/style.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.672970 amatak-shop-1.0.8/amatak_shop/templates/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.680952 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.779619 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/
+-rw-rw-rw-   0        0        0      277 2023-07-27 13:33:19.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/account_inactive.html
+-rw-rw-rw-   0        0        0      848 2023-07-28 06:39:08.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/account_update.html
+-rw-rw-rw-   0        0        0     2038 2023-07-28 15:41:18.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/base.html
+-rw-rw-rw-   0        0        0     2503 2023-07-27 02:28:31.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/email.html
+-rw-rw-rw-   0        0        0      955 2023-07-27 02:28:37.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/email_confirm.html
+-rw-rw-rw-   0        0        0     2144 2023-07-28 15:32:57.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/login.html
+-rw-rw-rw-   0        0        0      925 2023-07-28 15:59:50.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/logout.html
+-rw-rw-rw-   0        0        0      464 2023-07-27 02:28:45.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/password_change.html
+-rw-rw-rw-   0        0        0      833 2023-07-27 02:28:49.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/password_reset.html
+-rw-rw-rw-   0        0        0      502 2023-07-27 02:28:54.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/password_reset_done.html
+-rw-rw-rw-   0        0        0      971 2023-07-27 02:28:59.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/password_reset_from_key.html
+-rw-rw-rw-   0        0        0      280 2023-07-27 02:29:04.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/password_reset_from_key_done.html
+-rw-rw-rw-   0        0        0      448 2023-07-27 02:29:08.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/password_set.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.826481 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/profile/
+-rw-rw-rw-   0        0        0      482 2023-05-24 11:09:56.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/profile/form.html
+-rw-rw-rw-   0        0        0     3695 2023-07-26 14:40:33.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/profile/view.html
+-rw-rw-rw-   0        0        0     1294 2023-07-28 15:37:43.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/signup.html
+-rw-rw-rw-   0        0        0      292 2023-07-27 02:29:13.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/signup_closed.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.842102 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/snippets/
+-rw-rw-rw-   0        0        0      186 2023-07-28 15:44:32.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/snippets/already_logged_in.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.842102 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/tags/
+-rw-rw-rw-   0        0        0        0 2023-07-28 05:59:38.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/tags/account_txs_table.html
+-rw-rw-rw-   0        0        0        0 2023-07-28 05:59:44.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/tags/accounts_table.html
+-rw-rw-rw-   0        0        0      465 2023-07-27 02:29:16.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/verification_sent.html
+-rw-rw-rw-   0        0        0      825 2023-07-27 02:29:20.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/account/verified_email_required.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.878435 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/
+-rw-rw-rw-   0        0        0     1340 2023-07-28 06:23:43.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/customer_create.html
+-rw-rw-rw-   0        0        0      691 2023-07-28 06:24:43.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/customer_list.html
+-rw-rw-rw-   0        0        0     1365 2023-07-28 06:25:42.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/customer_update.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.878435 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/includes/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:07:55.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/includes/card_customer.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.894079 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/tags/
+-rw-rw-rw-   0        0        0     1331 2023-07-28 06:22:05.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/customer/tags/customer_table.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.925325 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/legal/
+-rw-rw-rw-   0        0        0      878 2023-07-27 13:25:10.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/legal/policy.html
+-rw-rw-rw-   0        0        0     1008 2023-07-27 13:25:24.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/legal/terms.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:09.956568 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/openid/
+-rw-rw-rw-   0        0        0       52 2023-07-27 13:34:26.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/openid/base.html
+-rw-rw-rw-   0        0        0      369 2023-07-27 13:34:31.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/openid/login.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.039820 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/
+-rw-rw-rw-   0        0        0      337 2023-07-27 12:24:13.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/authentication_error.html
+-rw-rw-rw-   0        0        0       46 2023-07-27 12:22:35.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/base.html
+-rw-rw-rw-   0        0        0     1434 2023-07-26 13:51:34.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/connections.html
+-rw-rw-rw-   0        0        0      454 2023-07-26 13:51:39.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/login_cancelled.html
+-rw-rw-rw-   0        0        0      783 2023-07-27 12:22:58.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/signup.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.072735 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/snippets/
+-rw-rw-rw-   0        0        0       51 2023-06-26 09:22:30.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/snippets/login_extra.html
+-rw-rw-rw-   0        0        0      663 2023-06-26 09:22:30.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/socialaccount/snippets/provider_list.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.680952 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/static/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.126591 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/static/tags/
+-rw-rw-rw-   0        0        0    12761 2023-07-28 23:51:28.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/static/tags/brand.html
+-rw-rw-rw-   0        0        0      743 2023-07-28 22:56:20.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/static/tags/scripts.html
+-rw-rw-rw-   0        0        0      205 2023-07-28 22:56:25.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/static/tags/styles.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.375505 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/
+-rw-rw-rw-   0        0        0     1834 2023-07-28 22:32:41.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/base.html
+-rw-rw-rw-   0        0        0     6790 2023-07-29 01:13:33.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/checkout.html
+-rw-rw-rw-   0        0        0     1703 2023-07-28 23:27:38.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/footer.html
+-rw-rw-rw-   0        0        0     5118 2023-07-29 00:57:35.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/home.html
+-rw-rw-rw-   0        0        0     3631 2023-07-28 23:44:10.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/navbar.html
+-rw-rw-rw-   0        0        0     1620 2023-07-29 01:14:11.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/order_snippet.html
+-rw-rw-rw-   0        0        0     2571 2023-07-29 00:46:52.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/order_summary.html
+-rw-rw-rw-   0        0        0     8738 2023-07-29 04:39:57.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/payment.html
+-rw-rw-rw-   0        0        0     2972 2023-07-29 04:29:32.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/product.html
+-rw-rw-rw-   0        0        0      366 2023-07-27 12:21:37.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/request_refund.html
+-rw-rw-rw-   0        0        0      601 2023-07-27 12:22:11.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/scripts.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.406785 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/tags/
+-rw-rw-rw-   0        0        0      277 2023-07-28 14:20:28.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/tags/sidebar_left.html
+-rw-rw-rw-   0        0        0      489 2023-07-28 14:06:24.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/store/tags/store_advertise_red.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.445217 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.445217 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/includes/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:26:37.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/includes/card_vendor.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.445217 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/tags/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:06:22.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/tags/vendor_table.html
+-rw-rw-rw-   0        0        0     1326 2023-07-28 06:29:13.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/vendor_create.html
+-rw-rw-rw-   0        0        0      673 2023-07-28 06:30:11.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/vendor_list.html
+-rw-rw-rw-   0        0        0     1363 2023-07-28 06:30:58.000000 amatak-shop-1.0.8/amatak_shop/templates/amatak_shop/vendor/vendor_update.html
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.460834 amatak-shop-1.0.8/amatak_shop/templatetags/
+-rw-rw-rw-   0        0        0      499 2023-07-30 07:11:29.000000 amatak-shop-1.0.8/amatak_shop/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2269 2023-07-30 03:29:14.000000 amatak-shop-1.0.8/amatak_shop/templatetags/amatak_shop.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.507702 amatak-shop-1.0.8/amatak_shop/tests/
+-rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.8/amatak_shop/tests/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.8/amatak_shop/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.678371 amatak-shop-1.0.8/amatak_shop/urls/
+-rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.8/amatak_shop/urls/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.8/amatak_shop/urls/add_coupon.py
+-rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.8/amatak_shop/urls/add_to_cart.py
+-rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.8/amatak_shop/urls/checkout.py
+-rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.8/amatak_shop/urls/home.py
+-rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.8/amatak_shop/urls/order_summary.py
+-rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.8/amatak_shop/urls/payment.py
+-rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.8/amatak_shop/urls/policy.py
+-rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.8/amatak_shop/urls/products.py
+-rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.8/amatak_shop/urls/remove_from_cart.py
+-rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.8/amatak_shop/urls/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.8/amatak_shop/urls/request_refund.py
+-rw-rw-rw-   0        0        0      419 2023-07-27 11:58:31.000000 amatak-shop-1.0.8/amatak_shop/urls/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:10.934798 amatak-shop-1.0.8/amatak_shop/views/
+-rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.8/amatak_shop/views/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.8/amatak_shop/views/add_coupon.py
+-rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.8/amatak_shop/views/add_to_cart.py
+-rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.8/amatak_shop/views/checkout.py
+-rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.8/amatak_shop/views/create_ref_code.py
+-rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.8/amatak_shop/views/get_coupon.py
+-rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.8/amatak_shop/views/home.py
+-rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.8/amatak_shop/views/is_valid_form.py
+-rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.8/amatak_shop/views/items_detail_views.py
+-rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.8/amatak_shop/views/login.py
+-rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.8/amatak_shop/views/logout.py
+-rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.8/amatak_shop/views/order_summary.py
+-rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.8/amatak_shop/views/payment.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.8/amatak_shop/views/policy.py
+-rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.8/amatak_shop/views/products.py
+-rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.8/amatak_shop/views/remove_from_cart.py
+-rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.8/amatak_shop/views/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.8/amatak_shop/views/request_refund.py
+-rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.8/amatak_shop/views/sign_up.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.8/amatak_shop/views/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.727865 amatak-shop-1.0.8/amatak_shop.egg-info/
+-rw-rw-rw-   0        0        0     3188 2023-07-30 07:39:04.000000 amatak-shop-1.0.8/amatak_shop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16932 2023-07-30 07:39:04.000000 amatak-shop-1.0.8/amatak_shop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 07:39:04.000000 amatak-shop-1.0.8/amatak_shop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-30 07:39:04.000000 amatak-shop-1.0.8/amatak_shop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:04.680952 amatak-shop-1.0.8/eCommerce/
+drwxrwxrwx   0        0        0        0 2023-07-30 07:39:11.004155 amatak-shop-1.0.8/eCommerce/settings/
+-rw-rw-rw-   0        0        0     1487 2023-07-30 03:32:50.000000 amatak-shop-1.0.8/eCommerce/settings/AmatakShopDev.py
+-rw-rw-rw-   0        0        0      256 2023-07-30 02:54:02.000000 amatak-shop-1.0.8/eCommerce/settings/__init__.py
+-rw-rw-rw-   0        0        0     2588 2023-07-30 03:15:58.000000 amatak-shop-1.0.8/eCommerce/settings/base.py
+-rw-rw-rw-   0        0        0     1096 2023-07-30 02:56:09.000000 amatak-shop-1.0.8/eCommerce/settings/production.py
+-rw-rw-rw-   0        0        0      564 2023-07-30 07:17:22.000000 amatak-shop-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 07:39:11.019781 amatak-shop-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.8/setup.py
```

### Comparing `amatak-shop-1.0.7/PKG-INFO` & `amatak-shop-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.7
+Version: 1.0.8
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `amatak-shop-1.0.7/README.md` & `amatak-shop-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/forms/checkout.py` & `amatak-shop-1.0.8/amatak_shop/forms/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/forms/coupon.py` & `amatak-shop-1.0.8/amatak_shop/forms/coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/forms/payment.py` & `amatak-shop-1.0.8/amatak_shop/forms/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/forms/refund.py` & `amatak-shop-1.0.8/amatak_shop/forms/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/management/commands/rename.py` & `amatak-shop-1.0.8/amatak_shop/management/commands/rename.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/migrations/0001_initial.py` & `amatak-shop-1.0.8/amatak_shop/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/__init__.py` & `amatak-shop-1.0.8/amatak_shop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/address.py` & `amatak-shop-1.0.8/amatak_shop/models/address.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/category.py` & `amatak-shop-1.0.8/amatak_shop/models/category.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/item.py` & `amatak-shop-1.0.8/amatak_shop/models/item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/mixins.py` & `amatak-shop-1.0.8/amatak_shop/models/mixins.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/order.py` & `amatak-shop-1.0.8/amatak_shop/models/order.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/order_item.py` & `amatak-shop-1.0.8/amatak_shop/models/order_item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/payment.py` & `amatak-shop-1.0.8/amatak_shop/models/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/refund.py` & `amatak-shop-1.0.8/amatak_shop/models/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/models/user_receiver_profile.py` & `amatak-shop-1.0.8/amatak_shop/models/user_receiver_profile.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/settings/base.py` & `amatak-shop-1.0.8/amatak_shop/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/templatetags/amatak_shop.py` & `amatak-shop-1.0.8/amatak_shop/templatetags/amatak_shop.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/tests/__init__.py` & `amatak-shop-1.0.8/amatak_shop/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/urls/__init__.py` & `amatak-shop-1.0.8/amatak_shop/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/urls/home.py` & `amatak-shop-1.0.8/amatak_shop/urls/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/__init__.py` & `amatak-shop-1.0.8/amatak_shop/views/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/add_coupon.py` & `amatak-shop-1.0.8/amatak_shop/views/add_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/add_to_cart.py` & `amatak-shop-1.0.8/amatak_shop/views/add_to_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/checkout.py` & `amatak-shop-1.0.8/amatak_shop/views/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/get_coupon.py` & `amatak-shop-1.0.8/amatak_shop/views/get_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/home.py` & `amatak-shop-1.0.8/amatak_shop/views/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/is_valid_form.py` & `amatak-shop-1.0.8/amatak_shop/views/is_valid_form.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/login.py` & `amatak-shop-1.0.8/amatak_shop/views/login.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/logout.py` & `amatak-shop-1.0.8/amatak_shop/views/logout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/order_summary.py` & `amatak-shop-1.0.8/amatak_shop/views/order_summary.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/payment.py` & `amatak-shop-1.0.8/amatak_shop/views/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/policy.py` & `amatak-shop-1.0.8/amatak_shop/views/policy.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/products.py` & `amatak-shop-1.0.8/amatak_shop/views/products.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/remove_from_cart.py` & `amatak-shop-1.0.8/amatak_shop/views/remove_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/remove_single_item_from_cart.py` & `amatak-shop-1.0.8/amatak_shop/views/remove_single_item_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/request_refund.py` & `amatak-shop-1.0.8/amatak_shop/views/request_refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/sign_up.py` & `amatak-shop-1.0.8/amatak_shop/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop/views/terms.py` & `amatak-shop-1.0.8/amatak_shop/views/terms.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/amatak_shop.egg-info/PKG-INFO` & `amatak-shop-1.0.8/amatak_shop.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.7
+Version: 1.0.8
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `amatak-shop-1.0.7/eCommerce/settings/AmatakShopDev.py` & `amatak-shop-1.0.8/eCommerce/settings/AmatakShopDev.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/eCommerce/settings/base.py` & `amatak-shop-1.0.8/eCommerce/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/eCommerce/settings/production.py` & `amatak-shop-1.0.8/eCommerce/settings/production.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.7/pyproject.toml` & `amatak-shop-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amatak-shop"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Rony MAN", email="amatak.io@outlook.com" },
 ]
 description = "Amatak OpenSource Online Shop "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

