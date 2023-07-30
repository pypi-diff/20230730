# Comparing `tmp/amatak-shop-1.0.9.tar.gz` & `tmp/amatak-shop-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amatak-shop-1.0.9.tar", last modified: Sun Jul 30 08:31:03 2023, max compression
+gzip compressed data, was "amatak-shop-1.1.0.tar", last modified: Sun Jul 30 11:13:52 2023, max compression
```

## Comparing `amatak-shop-1.0.9.tar` & `amatak-shop-1.1.0.tar`

### file list

```diff
@@ -1,411 +1,414 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.799527 amatak-shop-1.0.9/
--rw-rw-rw-   0        0        0       81 2023-07-30 08:23:59.000000 amatak-shop-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3188 2023-07-30 08:31:03.799527 amatak-shop-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2671 2023-07-30 02:05:48.000000 amatak-shop-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.868518 amatak-shop-1.0.9/amatak_shop/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.967354 amatak-shop-1.0.9/amatak_shop/forms/
--rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.0.9/amatak_shop/forms/__init__.py
--rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.0.9/amatak_shop/forms/checkout.py
--rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.0.9/amatak_shop/forms/coupon.py
--rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.0.9/amatak_shop/forms/payment.py
--rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.0.9/amatak_shop/forms/payment_choices.py
--rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.0.9/amatak_shop/forms/refund.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.822764 amatak-shop-1.0.9/amatak_shop/management/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.982976 amatak-shop-1.0.9/amatak_shop/management/commands/
--rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.0.9/amatak_shop/management/commands/rename.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.998641 amatak-shop-1.0.9/amatak_shop/migrations/
--rw-rw-rw-   0        0        0     7375 2023-07-30 06:40:44.000000 amatak-shop-1.0.9/amatak_shop/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.0.9/amatak_shop/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.147455 amatak-shop-1.0.9/amatak_shop/models/
--rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.0.9/amatak_shop/models/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.0.9/amatak_shop/models/address.py
--rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.0.9/amatak_shop/models/category.py
--rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.0.9/amatak_shop/models/coupon.py
--rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.0.9/amatak_shop/models/item.py
--rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.0.9/amatak_shop/models/mixins.py
--rw-rw-rw-   0        0        0     2255 2023-07-30 06:32:21.000000 amatak-shop-1.0.9/amatak_shop/models/order.py
--rw-rw-rw-   0        0        0     1308 2023-07-30 06:28:38.000000 amatak-shop-1.0.9/amatak_shop/models/order_item.py
--rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.0.9/amatak_shop/models/payment.py
--rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.0.9/amatak_shop/models/refund.py
--rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.0.9/amatak_shop/models/user_profile.py
--rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.0.9/amatak_shop/models/user_receiver_profile.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.167176 amatak-shop-1.0.9/amatak_shop/settings/
--rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.0.9/amatak_shop/settings/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.0.9/amatak_shop/settings/base.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.822764 amatak-shop-1.0.9/amatak_shop/static/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.837269 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.238555 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/
--rw-rw-rw-   0        0        0     1080 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/LICENSE
--rw-rw-rw-   0        0        0    12459 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/README.md
--rw-rw-rw-   0        0        0      300 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/bulma.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.305418 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/
--rw-rw-rw-   0        0        0   245633 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css
--rw-rw-rw-   0        0        0    98598 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css.map
--rw-rw-rw-   0        0        0   207445 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.min.css
--rw-rw-rw-   0        0        0   245486 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma.css
--rw-rw-rw-   0        0        0    98583 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma.css.map
--rw-rw-rw-   0        0        0   207302 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma.min.css
--rw-rw-rw-   0        0        0     1761 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/package.json
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.837269 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.380021 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/
--rw-rw-rw-   0        0        0       94 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/_all.sass
--rw-rw-rw-   0        0        0       92 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/animations.sass
--rw-rw-rw-   0        0        0     2640 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/generic.sass
--rw-rw-rw-   0        0        0      129 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/helpers.sass
--rw-rw-rw-   0        0        0      709 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/minireset.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.625968 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/
--rw-rw-rw-   0        0        0      246 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/_all.sass
--rw-rw-rw-   0        0        0     1786 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/breadcrumb.sass
--rw-rw-rw-   0        0        0     2489 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/card.sass
--rw-rw-rw-   0        0        0     2191 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/dropdown.sass
--rw-rw-rw-   0        0        0     1487 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/level.sass
--rw-rw-rw-   0        0        0     1439 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/media.sass
--rw-rw-rw-   0        0        0     1714 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/menu.sass
--rw-rw-rw-   0        0        0     3025 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/message.sass
--rw-rw-rw-   0        0        0     3000 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/modal.sass
--rw-rw-rw-   0        0        0    12197 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/navbar.sass
--rw-rw-rw-   0        0        0     4133 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/pagination.sass
--rw-rw-rw-   0        0        0     3288 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/panel.sass
--rw-rw-rw-   0        0        0     5717 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/tabs.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.881474 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/
--rw-rw-rw-   0        0        0      244 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/_all.sass
--rw-rw-rw-   0        0        0      690 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/box.sass
--rw-rw-rw-   0        0        0    10853 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/button.sass
--rw-rw-rw-   0        0        0      886 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/container.sass
--rw-rw-rw-   0        0        0     3913 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/content.sass
--rw-rw-rw-   0        0        0      120 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/form.sass
--rw-rw-rw-   0        0        0     1054 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/icon.sass
--rw-rw-rw-   0        0        0     1263 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/image.sass
--rw-rw-rw-   0        0        0     1445 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/notification.sass
--rw-rw-rw-   0        0        0      521 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/other.sass
--rw-rw-rw-   0        0        0     2050 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/progress.sass
--rw-rw-rw-   0        0        0     3475 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/table.sass
--rw-rw-rw-   0        0        0     3491 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/tag.sass
--rw-rw-rw-   0        0        0     1743 2023-07-28 13:03:46.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/title.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:59.997455 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/
--rw-rw-rw-   0        0        0      150 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/_all.sass
--rw-rw-rw-   0        0        0      407 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/checkbox-radio.sass
--rw-rw-rw-   0        0        0     4263 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/file.sass
--rw-rw-rw-   0        0        0     1453 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/input-textarea.sass
--rw-rw-rw-   0        0        0     1999 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/select.sass
--rw-rw-rw-   0        0        0     1792 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/shared.sass
--rw-rw-rw-   0        0        0     4674 2023-07-28 13:03:44.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/tools.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.049443 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/grid/
--rw-rw-rw-   0        0        0       69 2023-07-28 13:03:48.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/grid/_all.sass
--rw-rw-rw-   0        0        0    14019 2023-07-28 13:03:48.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/grid/columns.sass
--rw-rw-rw-   0        0        0      815 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/grid/tiles.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.211901 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/
--rw-rw-rw-   0        0        0      202 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/_all.sass
--rw-rw-rw-   0        0        0     1096 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/color.sass
--rw-rw-rw-   0        0        0     1317 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/flexbox.sass
--rw-rw-rw-   0        0        0      142 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/float.sass
--rw-rw-rw-   0        0        0      241 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/other.sass
--rw-rw-rw-   0        0        0       42 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/overflow.sass
--rw-rw-rw-   0        0        0      108 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/position.sass
--rw-rw-rw-   0        0        0     1164 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/spacing.sass
--rw-rw-rw-   0        0        0     2474 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/typography.sass
--rw-rw-rw-   0        0        0     2448 2023-07-28 13:03:47.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/visibility.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.283459 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/layout/
--rw-rw-rw-   0        0        0       87 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/layout/_all.sass
--rw-rw-rw-   0        0        0      293 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/layout/footer.sass
--rw-rw-rw-   0        0        0     3651 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/layout/hero.sass
--rw-rw-rw-   0        0        0      433 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/layout/section.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.404637 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/
--rw-rw-rw-   0        0        0      170 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/_all.sass
--rw-rw-rw-   0        0        0      119 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/animations.sass
--rw-rw-rw-   0        0        0     1296 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/controls.sass
--rw-rw-rw-   0        0        0     4005 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/derived-variables.sass
--rw-rw-rw-   0        0        0      179 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/extends.sass
--rw-rw-rw-   0        0        0     4896 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/functions.sass
--rw-rw-rw-   0        0        0     2691 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/initial-variables.sass
--rw-rw-rw-   0        0        0     6291 2023-07-28 13:03:45.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/mixins.sass
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.550367 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.634524 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/
--rw-rw-rw-   0        0        0     5364 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables-select.css
--rw-rw-rw-   0        0        0     3962 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables-select.min.css
--rw-rw-rw-   0        0        0     5289 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables.css
--rw-rw-rw-   0        0        0     3767 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables.min.css
--rw-rw-rw-   0        0        0    10673 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/directives.css
--rw-rw-rw-   0        0        0     8362 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/directives.min.css
--rw-rw-rw-   0        0        0   192348 2023-06-26 09:22:18.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/bootstrap.css
--rw-rw-rw-   0        0        0   155758 2023-06-26 09:22:18.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   314326 2023-06-26 09:22:18.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.css
--rw-rw-rw-   0        0        0   243602 2023-06-26 09:22:18.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.lite.css
--rw-rw-rw-   0        0        0   199949 2023-06-26 09:22:18.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.lite.min.css
--rw-rw-rw-   0        0        0   255261 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.min.css
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.665771 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/modules/
--rw-rw-rw-   0        0        0    70879 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/modules/animations-extended.css
--rw-rw-rw-   0        0        0    55325 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/modules/animations-extended.min.css
--rw-rw-rw-   0        0        0      556 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/style.css
--rw-rw-rw-   0        0        0      248 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/style.min.css
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.837269 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:00.999106 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/
--rw-rw-rw-   0        0        0    20966 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.eot
--rw-rw-rw-   0        0        0   127744 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0    62876 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff
--rw-rw-rw-   0        0        0    49976 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff2
--rw-rw-rw-   0        0        0    20940 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.eot
--rw-rw-rw-   0        0        0   126792 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.ttf
--rw-rw-rw-   0        0        0    62316 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff
--rw-rw-rw-   0        0        0    49380 2023-06-26 09:22:19.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff2
--rw-rw-rw-   0        0        0    21364 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.eot
--rw-rw-rw-   0        0        0   127488 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0    62980 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff
--rw-rw-rw-   0        0        0    50224 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff2
--rw-rw-rw-   0        0        0    21320 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.eot
--rw-rw-rw-   0        0        0   126072 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0    61736 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff
--rw-rw-rw-   0        0        0    49236 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff2
--rw-rw-rw-   0        0        0    21659 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.eot
--rw-rw-rw-   0        0        0   127584 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0    61628 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff
--rw-rw-rw-   0        0        0    48524 2023-06-26 09:22:20.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff2
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:01.014726 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:01.045966 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/
--rw-rw-rw-   0        0        0      547 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/default-skin.png
--rw-rw-rw-   0        0        0     1554 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/default-skin.svg
--rw-rw-rw-   0        0        0      866 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/preloader.gif
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:01.145886 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/
--rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/01.png
--rw-rw-rw-   0        0        0      213 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/02.png
--rw-rw-rw-   0        0        0      209 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/03.png
--rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/04.png
--rw-rw-rw-   0        0        0      213 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/05.png
--rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/06.png
--rw-rw-rw-   0        0        0      215 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/07.png
--rw-rw-rw-   0        0        0      146 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/08.png
--rw-rw-rw-   0        0        0      137 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/overlays/09.png
--rw-rw-rw-   0        0        0   204946 2023-06-26 09:22:21.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/sample.jpg
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:01.182215 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/svg/
--rw-rw-rw-   0        0        0      218 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/svg/arrow_left.svg
--rw-rw-rw-   0        0        0      217 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/svg/arrow_right.svg
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:01.558446 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:01.763470 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/
--rw-rw-rw-   0        0        0    32005 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables-select.js
--rw-rw-rw-   0        0        0    11741 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables-select.min.js
--rw-rw-rw-   0        0        0   452723 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables.js
--rw-rw-rw-   0        0        0    84932 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables.min.js
--rw-rw-rw-   0        0        0     1637 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/rating.js
--rw-rw-rw-   0        0        0   131637 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/bootstrap.js
--rw-rw-rw-   0        0        0    58072 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    86927 2023-06-26 09:22:22.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0   478685 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/mdb.js
--rw-rw-rw-   0        0        0   209696 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/mdb.min.js
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.128389 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/
--rw-rw-rw-   0        0        0   402487 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/chart.js
--rw-rw-rw-   0        0        0      570 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/default-file-input.js
--rw-rw-rw-   0        0        0      685 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/enhanced-modals.js
--rw-rw-rw-   0        0        0     5373 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/forms-free.js
--rw-rw-rw-   0        0        0     8661 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/jquery.easing.js
--rw-rw-rw-   0        0        0      409 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/scrolling-navbar.js
--rw-rw-rw-   0        0        0      290 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/treeview.js
--rw-rw-rw-   0        0        0    35106 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/velocity.js
--rw-rw-rw-   0        0        0    35106 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/velocity.min.js
--rw-rw-rw-   0        0        0    18936 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/waves.js
--rw-rw-rw-   0        0        0     5324 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/wow.js
--rw-rw-rw-   0        0        0    20537 2023-06-26 09:22:23.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/popper.min.js
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.143977 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/
--rw-rw-rw-   0        0        0      734 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/_custom-skin.scss
--rw-rw-rw-   0        0        0       21 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/_custom-styles.scss
--rw-rw-rw-   0        0        0       24 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/_custom-variables.scss
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.143977 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/
--rw-rw-rw-   0        0        0     4573 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/_datatables-select.scss
--rw-rw-rw-   0        0        0     4203 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/_datatables.scss
--rw-rw-rw-   0        0        0     1477 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/_directives.scss
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.175221 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/
--rw-rw-rw-   0        0        0    28149 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_colors.scss
--rw-rw-rw-   0        0        0     2549 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_global.scss
--rw-rw-rw-   0        0        0     1074 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_helpers.scss
--rw-rw-rw-   0        0        0     1199 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_masks.scss
--rw-rw-rw-   0        0        0    13073 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_mixins.scss
--rw-rw-rw-   0        0        0     3665 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_typography.scss
--rw-rw-rw-   0        0        0    17282 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_variables.scss
--rw-rw-rw-   0        0        0     3967 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_waves.scss
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.175221 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/
--rw-rw-rw-   0        0        0     2719 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/_functions.scss
--rw-rw-rw-   0        0        0     6474 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/_rfs.scss
--rw-rw-rw-   0        0        0    47781 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/_variables.scss
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.227162 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/
--rw-rw-rw-   0        0        0     2603 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_animations-basic.scss
--rw-rw-rw-   0        0        0      335 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_badges.scss
--rw-rw-rw-   0        0        0     3273 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_buttons.scss
--rw-rw-rw-   0        0        0      580 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_cards.scss
--rw-rw-rw-   0        0        0     1205 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_carousels.scss
--rw-rw-rw-   0        0        0       47 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_depreciated.scss
--rw-rw-rw-   0        0        0      144 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_dropdowns.scss
--rw-rw-rw-   0        0        0      314 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_footers.scss
--rw-rw-rw-   0        0        0    12170 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_forms.scss
--rw-rw-rw-   0        0        0     1738 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_input-group.scss
--rw-rw-rw-   0        0        0      557 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_list-group.scss
--rw-rw-rw-   0        0        0      177 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_loader.scss
--rw-rw-rw-   0        0        0     6505 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_modals.scss
--rw-rw-rw-   0        0        0     3243 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_msc.scss
--rw-rw-rw-   0        0        0     2540 2023-06-26 09:22:26.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_navbars.scss
--rw-rw-rw-   0        0        0     1960 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_pagination.scss
--rw-rw-rw-   0        0        0     3888 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_steppers.scss
--rw-rw-rw-   0        0        0      894 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_switch.scss
--rw-rw-rw-   0        0        0     1340 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_tables.scss
--rw-rw-rw-   0        0        0      418 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_treeview.scss
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.837269 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/modules/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.227162 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/
--rw-rw-rw-   0        0        0    22617 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/_module.scss
--rw-rw-rw-   0        0        0      175 2023-06-26 09:22:27.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/animations-extended.scss
--rw-rw-rw-   0        0        0     1555 2023-06-26 09:22:24.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/mdb.lite.scss
--rw-rw-rw-   0        0        0     1724 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/mdb.scss
--rw-rw-rw-   0        0        0      604 2023-06-26 09:22:25.000000 amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/style.scss
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.852897 amatak-shop-1.0.9/amatak_shop/templates/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.852897 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.468143 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/
--rw-rw-rw-   0        0        0      277 2023-07-27 13:33:19.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/account_inactive.html
--rw-rw-rw-   0        0        0      848 2023-07-28 06:39:08.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/account_update.html
--rw-rw-rw-   0        0        0     2038 2023-07-28 15:41:18.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/base.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.552361 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/
--rw-rw-rw-   0        0        0      569 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/email_confirmation_message.txt
--rw-rw-rw-   0        0        0       61 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/email_confirmation_signup_message.txt
--rw-rw-rw-   0        0        0       61 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/email_confirmation_signup_subject.txt
--rw-rw-rw-   0        0        0      127 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/email_confirmation_subject.txt
--rw-rw-rw-   0        0        0      659 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/password_reset_key_message.txt
--rw-rw-rw-   0        0        0      114 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/password_reset_key_subject.txt
--rw-rw-rw-   0        0        0     2503 2023-07-27 02:28:31.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email.html
--rw-rw-rw-   0        0        0      955 2023-07-27 02:28:37.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email_confirm.html
--rw-rw-rw-   0        0        0     2144 2023-07-28 15:32:57.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/login.html
--rw-rw-rw-   0        0        0      925 2023-07-28 15:59:50.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/logout.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.698422 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/
--rw-rw-rw-   0        0        0      110 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/cannot_delete_primary_email.txt
--rw-rw-rw-   0        0        0       90 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/email_confirmation_sent.txt
--rw-rw-rw-   0        0        0       81 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/email_confirmed.txt
--rw-rw-rw-   0        0        0       85 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/email_deleted.txt
--rw-rw-rw-   0        0        0      138 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/logged_in.txt
--rw-rw-rw-   0        0        0       72 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/logged_out.txt
--rw-rw-rw-   0        0        0       82 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/password_changed.txt
--rw-rw-rw-   0        0        0       78 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/password_set.txt
--rw-rw-rw-   0        0        0       79 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/primary_email_set.txt
--rw-rw-rw-   0        0        0       97 2023-06-26 09:22:29.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/messages/unverified_primary_email.txt
--rw-rw-rw-   0        0        0      464 2023-07-27 02:28:45.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_change.html
--rw-rw-rw-   0        0        0      833 2023-07-27 02:28:49.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_reset.html
--rw-rw-rw-   0        0        0      502 2023-07-27 02:28:54.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_reset_done.html
--rw-rw-rw-   0        0        0      971 2023-07-27 02:28:59.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_reset_from_key.html
--rw-rw-rw-   0        0        0      280 2023-07-27 02:29:04.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_reset_from_key_done.html
--rw-rw-rw-   0        0        0      448 2023-07-27 02:29:08.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_set.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.751338 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/profile/
--rw-rw-rw-   0        0        0      482 2023-05-24 11:09:56.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/profile/form.html
--rw-rw-rw-   0        0        0     3695 2023-07-26 14:40:33.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/profile/view.html
--rw-rw-rw-   0        0        0     1294 2023-07-28 15:37:43.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/signup.html
--rw-rw-rw-   0        0        0      292 2023-07-27 02:29:13.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/signup_closed.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.766996 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/snippets/
--rw-rw-rw-   0        0        0      186 2023-07-28 15:44:32.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/snippets/already_logged_in.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.766996 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/tags/
--rw-rw-rw-   0        0        0        0 2023-07-28 05:59:38.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/tags/account_txs_table.html
--rw-rw-rw-   0        0        0        0 2023-07-28 05:59:44.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/tags/accounts_table.html
--rw-rw-rw-   0        0        0      465 2023-07-27 02:29:16.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/verification_sent.html
--rw-rw-rw-   0        0        0      825 2023-07-27 02:29:20.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/verified_email_required.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.807870 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/
--rw-rw-rw-   0        0        0     1340 2023-07-28 06:23:43.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/customer_create.html
--rw-rw-rw-   0        0        0      691 2023-07-28 06:24:43.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/customer_list.html
--rw-rw-rw-   0        0        0     1365 2023-07-28 06:25:42.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/customer_update.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.807870 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/includes/
--rw-rw-rw-   0        0        0        0 2023-07-28 06:07:55.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/includes/card_customer.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.807870 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/tags/
--rw-rw-rw-   0        0        0     1331 2023-07-28 06:22:05.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/tags/customer_table.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.839111 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/legal/
--rw-rw-rw-   0        0        0      878 2023-07-27 13:25:10.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/legal/policy.html
--rw-rw-rw-   0        0        0     1008 2023-07-27 13:25:24.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/legal/terms.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.871215 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/openid/
--rw-rw-rw-   0        0        0       52 2023-07-27 13:34:26.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/openid/base.html
--rw-rw-rw-   0        0        0      369 2023-07-27 13:34:31.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/openid/login.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.941025 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/
--rw-rw-rw-   0        0        0      337 2023-07-27 12:24:13.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/authentication_error.html
--rw-rw-rw-   0        0        0       46 2023-07-27 12:22:35.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/base.html
--rw-rw-rw-   0        0        0     1434 2023-07-26 13:51:34.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/connections.html
--rw-rw-rw-   0        0        0      454 2023-07-26 13:51:39.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/login_cancelled.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:02.985941 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/messages/
--rw-rw-rw-   0        0        0       90 2023-06-26 09:22:30.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/messages/account_connected.txt
--rw-rw-rw-   0        0        0      115 2023-06-26 09:22:30.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/messages/account_connected_other.txt
--rw-rw-rw-   0        0        0       93 2023-06-26 09:22:30.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/messages/account_disconnected.txt
--rw-rw-rw-   0        0        0      783 2023-07-27 12:22:58.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/signup.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.011839 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/snippets/
--rw-rw-rw-   0        0        0       51 2023-06-26 09:22:30.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/snippets/login_extra.html
--rw-rw-rw-   0        0        0      663 2023-06-26 09:22:30.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/snippets/provider_list.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.852897 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.053757 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/tags/
--rw-rw-rw-   0        0        0    12761 2023-07-28 23:51:28.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/tags/brand.html
--rw-rw-rw-   0        0        0      743 2023-07-28 22:56:20.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/tags/scripts.html
--rw-rw-rw-   0        0        0      205 2023-07-28 22:56:25.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/tags/styles.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.260437 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/
--rw-rw-rw-   0        0        0     1834 2023-07-28 22:32:41.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/base.html
--rw-rw-rw-   0        0        0     6790 2023-07-29 01:13:33.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/checkout.html
--rw-rw-rw-   0        0        0     1703 2023-07-28 23:27:38.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/footer.html
--rw-rw-rw-   0        0        0     5118 2023-07-29 00:57:35.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/home.html
--rw-rw-rw-   0        0        0     3631 2023-07-28 23:44:10.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/navbar.html
--rw-rw-rw-   0        0        0     1620 2023-07-29 01:14:11.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/order_snippet.html
--rw-rw-rw-   0        0        0     2571 2023-07-29 00:46:52.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/order_summary.html
--rw-rw-rw-   0        0        0     8738 2023-07-29 04:39:57.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/payment.html
--rw-rw-rw-   0        0        0     2972 2023-07-29 04:29:32.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/product.html
--rw-rw-rw-   0        0        0      366 2023-07-27 12:21:37.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/request_refund.html
--rw-rw-rw-   0        0        0      601 2023-07-27 12:22:11.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/scripts.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.276023 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/tags/
--rw-rw-rw-   0        0        0      277 2023-07-28 14:20:28.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/tags/sidebar_left.html
--rw-rw-rw-   0        0        0      489 2023-07-28 14:06:24.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/tags/store_advertise_red.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.313728 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.313728 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/includes/
--rw-rw-rw-   0        0        0        0 2023-07-28 06:26:37.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/includes/card_vendor.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.313728 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/tags/
--rw-rw-rw-   0        0        0        0 2023-07-28 06:06:22.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/tags/vendor_table.html
--rw-rw-rw-   0        0        0     1326 2023-07-28 06:29:13.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/vendor_create.html
--rw-rw-rw-   0        0        0      673 2023-07-28 06:30:11.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/vendor_list.html
--rw-rw-rw-   0        0        0     1363 2023-07-28 06:30:58.000000 amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/vendor_update.html
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.329346 amatak-shop-1.0.9/amatak_shop/templatetags/
--rw-rw-rw-   0        0        0      499 2023-07-30 08:25:53.000000 amatak-shop-1.0.9/amatak_shop/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-07-30 03:29:14.000000 amatak-shop-1.0.9/amatak_shop/templatetags/amatak_shop.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.360589 amatak-shop-1.0.9/amatak_shop/tests/
--rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.0.9/amatak_shop/tests/__init__.py
--rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.0.9/amatak_shop/tests/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.481064 amatak-shop-1.0.9/amatak_shop/urls/
--rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.0.9/amatak_shop/urls/__init__.py
--rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.0.9/amatak_shop/urls/add_coupon.py
--rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.0.9/amatak_shop/urls/add_to_cart.py
--rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.0.9/amatak_shop/urls/checkout.py
--rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.0.9/amatak_shop/urls/home.py
--rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.0.9/amatak_shop/urls/order_summary.py
--rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.0.9/amatak_shop/urls/payment.py
--rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.0.9/amatak_shop/urls/policy.py
--rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.0.9/amatak_shop/urls/products.py
--rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.0.9/amatak_shop/urls/remove_from_cart.py
--rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.0.9/amatak_shop/urls/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.0.9/amatak_shop/urls/request_refund.py
--rw-rw-rw-   0        0        0      419 2023-07-30 08:29:35.000000 amatak-shop-1.0.9/amatak_shop/urls/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.726968 amatak-shop-1.0.9/amatak_shop/views/
--rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.0.9/amatak_shop/views/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.0.9/amatak_shop/views/add_coupon.py
--rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.0.9/amatak_shop/views/add_to_cart.py
--rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.0.9/amatak_shop/views/checkout.py
--rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.0.9/amatak_shop/views/create_ref_code.py
--rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.0.9/amatak_shop/views/get_coupon.py
--rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.0.9/amatak_shop/views/home.py
--rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.0.9/amatak_shop/views/is_valid_form.py
--rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.0.9/amatak_shop/views/items_detail_views.py
--rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.0.9/amatak_shop/views/login.py
--rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.0.9/amatak_shop/views/logout.py
--rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.0.9/amatak_shop/views/order_summary.py
--rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.0.9/amatak_shop/views/payment.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.0.9/amatak_shop/views/policy.py
--rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.0.9/amatak_shop/views/products.py
--rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.0.9/amatak_shop/views/remove_from_cart.py
--rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.0.9/amatak_shop/views/remove_single_item_from_cart.py
--rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.0.9/amatak_shop/views/request_refund.py
--rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.0.9/amatak_shop/views/sign_up.py
--rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.0.9/amatak_shop/views/terms.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.899764 amatak-shop-1.0.9/amatak_shop.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-07-30 08:30:58.000000 amatak-shop-1.0.9/amatak_shop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18392 2023-07-30 08:30:58.000000 amatak-shop-1.0.9/amatak_shop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 08:30:58.000000 amatak-shop-1.0.9/amatak_shop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-30 08:30:58.000000 amatak-shop-1.0.9/amatak_shop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 08:30:58.868518 amatak-shop-1.0.9/eCommerce/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:31:03.799527 amatak-shop-1.0.9/eCommerce/settings/
--rw-rw-rw-   0        0        0     1487 2023-07-30 03:32:50.000000 amatak-shop-1.0.9/eCommerce/settings/AmatakShopDev.py
--rw-rw-rw-   0        0        0      256 2023-07-30 02:54:02.000000 amatak-shop-1.0.9/eCommerce/settings/__init__.py
--rw-rw-rw-   0        0        0     2588 2023-07-30 03:15:58.000000 amatak-shop-1.0.9/eCommerce/settings/base.py
--rw-rw-rw-   0        0        0     1096 2023-07-30 02:56:09.000000 amatak-shop-1.0.9/eCommerce/settings/production.py
--rw-rw-rw-   0        0        0      564 2023-07-30 08:25:27.000000 amatak-shop-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 08:31:03.799527 amatak-shop-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.553714 amatak-shop-1.1.0/
+-rw-rw-rw-   0        0        0      117 2023-07-30 11:12:42.000000 amatak-shop-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3188 2023-07-30 11:13:52.552717 amatak-shop-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2671 2023-07-30 02:05:48.000000 amatak-shop-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.153278 amatak-shop-1.1.0/amatak_shop/
+-rw-rw-rw-   0        0        0      258 2023-07-30 03:30:45.000000 amatak-shop-1.1.0/amatak_shop/__init__.py
+-rw-rw-rw-   0        0        0     2445 2023-07-28 23:07:30.000000 amatak-shop-1.1.0/amatak_shop/admin.py
+-rw-rw-rw-   0        0        0      413 2023-07-30 06:40:19.000000 amatak-shop-1.1.0/amatak_shop/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.267745 amatak-shop-1.1.0/amatak_shop/forms/
+-rw-rw-rw-   0        0        0      386 2023-07-27 11:41:56.000000 amatak-shop-1.1.0/amatak_shop/forms/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-07-27 11:42:05.000000 amatak-shop-1.1.0/amatak_shop/forms/checkout.py
+-rw-rw-rw-   0        0        0      726 2023-07-27 11:42:19.000000 amatak-shop-1.1.0/amatak_shop/forms/coupon.py
+-rw-rw-rw-   0        0        0      643 2023-07-27 11:42:33.000000 amatak-shop-1.1.0/amatak_shop/forms/payment.py
+-rw-rw-rw-   0        0        0      461 2023-07-27 11:42:47.000000 amatak-shop-1.1.0/amatak_shop/forms/payment_choices.py
+-rw-rw-rw-   0        0        0      647 2023-07-27 11:42:57.000000 amatak-shop-1.1.0/amatak_shop/forms/refund.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.044419 amatak-shop-1.1.0/amatak_shop/management/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.283365 amatak-shop-1.1.0/amatak_shop/management/commands/
+-rw-rw-rw-   0        0        0     1512 2023-07-26 22:57:22.000000 amatak-shop-1.1.0/amatak_shop/management/commands/rename.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.315062 amatak-shop-1.1.0/amatak_shop/migrations/
+-rw-rw-rw-   0        0        0     7375 2023-07-30 06:40:44.000000 amatak-shop-1.1.0/amatak_shop/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 09:22:18.000000 amatak-shop-1.1.0/amatak_shop/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.522411 amatak-shop-1.1.0/amatak_shop/models/
+-rw-rw-rw-   0        0        0      593 2023-07-27 11:44:33.000000 amatak-shop-1.1.0/amatak_shop/models/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-07-29 01:41:51.000000 amatak-shop-1.1.0/amatak_shop/models/address.py
+-rw-rw-rw-   0        0        0     1465 2023-07-27 13:18:17.000000 amatak-shop-1.1.0/amatak_shop/models/category.py
+-rw-rw-rw-   0        0        0      447 2023-07-27 11:45:31.000000 amatak-shop-1.1.0/amatak_shop/models/coupon.py
+-rw-rw-rw-   0        0        0     1630 2023-07-27 12:57:51.000000 amatak-shop-1.1.0/amatak_shop/models/item.py
+-rw-rw-rw-   0        0        0     9892 2023-07-26 22:58:12.000000 amatak-shop-1.1.0/amatak_shop/models/mixins.py
+-rw-rw-rw-   0        0        0     2255 2023-07-30 06:32:21.000000 amatak-shop-1.1.0/amatak_shop/models/order.py
+-rw-rw-rw-   0        0        0     1308 2023-07-30 06:28:38.000000 amatak-shop-1.1.0/amatak_shop/models/order_item.py
+-rw-rw-rw-   0        0        0     1431 2023-07-29 02:58:37.000000 amatak-shop-1.1.0/amatak_shop/models/payment.py
+-rw-rw-rw-   0        0        0      883 2023-07-27 12:36:35.000000 amatak-shop-1.1.0/amatak_shop/models/refund.py
+-rw-rw-rw-   0        0        0      442 2023-07-27 12:37:01.000000 amatak-shop-1.1.0/amatak_shop/models/user_profile.py
+-rw-rw-rw-   0        0        0      862 2023-07-29 02:11:51.000000 amatak-shop-1.1.0/amatak_shop/models/user_receiver_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.545099 amatak-shop-1.1.0/amatak_shop/settings/
+-rw-rw-rw-   0        0        0      260 2023-07-27 11:47:13.000000 amatak-shop-1.1.0/amatak_shop/settings/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-07-30 00:06:13.000000 amatak-shop-1.1.0/amatak_shop/settings/base.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.054424 amatak-shop-1.1.0/amatak_shop/static/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.070055 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.623205 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/
+-rw-rw-rw-   0        0        0     1080 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/LICENSE
+-rw-rw-rw-   0        0        0    12459 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/README.md
+-rw-rw-rw-   0        0        0      300 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/bulma.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.707895 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/
+-rw-rw-rw-   0        0        0   245633 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css
+-rw-rw-rw-   0        0        0    98598 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css.map
+-rw-rw-rw-   0        0        0   207445 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.min.css
+-rw-rw-rw-   0        0        0   245486 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma.css
+-rw-rw-rw-   0        0        0    98583 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma.css.map
+-rw-rw-rw-   0        0        0   207302 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma.min.css
+-rw-rw-rw-   0        0        0     1761 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/package.json
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.054424 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.791177 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/
+-rw-rw-rw-   0        0        0       94 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/_all.sass
+-rw-rw-rw-   0        0        0       92 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/animations.sass
+-rw-rw-rw-   0        0        0     2640 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/generic.sass
+-rw-rw-rw-   0        0        0      129 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/helpers.sass
+-rw-rw-rw-   0        0        0      709 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/minireset.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.050081 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/
+-rw-rw-rw-   0        0        0      246 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/_all.sass
+-rw-rw-rw-   0        0        0     1786 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/breadcrumb.sass
+-rw-rw-rw-   0        0        0     2489 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/card.sass
+-rw-rw-rw-   0        0        0     2191 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/dropdown.sass
+-rw-rw-rw-   0        0        0     1487 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/level.sass
+-rw-rw-rw-   0        0        0     1439 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/media.sass
+-rw-rw-rw-   0        0        0     1714 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/menu.sass
+-rw-rw-rw-   0        0        0     3025 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/message.sass
+-rw-rw-rw-   0        0        0     3000 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/modal.sass
+-rw-rw-rw-   0        0        0    12197 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/navbar.sass
+-rw-rw-rw-   0        0        0     4133 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/pagination.sass
+-rw-rw-rw-   0        0        0     3288 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/panel.sass
+-rw-rw-rw-   0        0        0     5717 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/tabs.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.280055 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/
+-rw-rw-rw-   0        0        0      244 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/_all.sass
+-rw-rw-rw-   0        0        0      690 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/box.sass
+-rw-rw-rw-   0        0        0    10853 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/button.sass
+-rw-rw-rw-   0        0        0      886 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/container.sass
+-rw-rw-rw-   0        0        0     3913 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/content.sass
+-rw-rw-rw-   0        0        0      120 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/form.sass
+-rw-rw-rw-   0        0        0     1054 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/icon.sass
+-rw-rw-rw-   0        0        0     1263 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/image.sass
+-rw-rw-rw-   0        0        0     1445 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/notification.sass
+-rw-rw-rw-   0        0        0      521 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/other.sass
+-rw-rw-rw-   0        0        0     2050 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/progress.sass
+-rw-rw-rw-   0        0        0     3475 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/table.sass
+-rw-rw-rw-   0        0        0     3491 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/tag.sass
+-rw-rw-rw-   0        0        0     1743 2023-07-28 13:03:46.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/title.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.394623 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/
+-rw-rw-rw-   0        0        0      150 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/_all.sass
+-rw-rw-rw-   0        0        0      407 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/checkbox-radio.sass
+-rw-rw-rw-   0        0        0     4263 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/file.sass
+-rw-rw-rw-   0        0        0     1453 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/input-textarea.sass
+-rw-rw-rw-   0        0        0     1999 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/select.sass
+-rw-rw-rw-   0        0        0     1792 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/shared.sass
+-rw-rw-rw-   0        0        0     4674 2023-07-28 13:03:44.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/tools.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.441489 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/grid/
+-rw-rw-rw-   0        0        0       69 2023-07-28 13:03:48.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/grid/_all.sass
+-rw-rw-rw-   0        0        0    14019 2023-07-28 13:03:48.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/grid/columns.sass
+-rw-rw-rw-   0        0        0      815 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/grid/tiles.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.654339 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/
+-rw-rw-rw-   0        0        0      202 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/_all.sass
+-rw-rw-rw-   0        0        0     1096 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/color.sass
+-rw-rw-rw-   0        0        0     1317 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/flexbox.sass
+-rw-rw-rw-   0        0        0      142 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/float.sass
+-rw-rw-rw-   0        0        0      241 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/other.sass
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/overflow.sass
+-rw-rw-rw-   0        0        0      108 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/position.sass
+-rw-rw-rw-   0        0        0     1164 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/spacing.sass
+-rw-rw-rw-   0        0        0     2474 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/typography.sass
+-rw-rw-rw-   0        0        0     2448 2023-07-28 13:03:47.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/visibility.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.722960 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/layout/
+-rw-rw-rw-   0        0        0       87 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/layout/_all.sass
+-rw-rw-rw-   0        0        0      293 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/layout/footer.sass
+-rw-rw-rw-   0        0        0     3651 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/layout/hero.sass
+-rw-rw-rw-   0        0        0      433 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/layout/section.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:48.885278 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/
+-rw-rw-rw-   0        0        0      170 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/_all.sass
+-rw-rw-rw-   0        0        0      119 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/animations.sass
+-rw-rw-rw-   0        0        0     1296 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/controls.sass
+-rw-rw-rw-   0        0        0     4005 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/derived-variables.sass
+-rw-rw-rw-   0        0        0      179 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/extends.sass
+-rw-rw-rw-   0        0        0     4896 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/functions.sass
+-rw-rw-rw-   0        0        0     2691 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/initial-variables.sass
+-rw-rw-rw-   0        0        0     6291 2023-07-28 13:03:45.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/mixins.sass
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.021467 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.168966 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/
+-rw-rw-rw-   0        0        0     5364 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables-select.css
+-rw-rw-rw-   0        0        0     3962 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables-select.min.css
+-rw-rw-rw-   0        0        0     5289 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables.css
+-rw-rw-rw-   0        0        0     3767 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables.min.css
+-rw-rw-rw-   0        0        0    10673 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/directives.css
+-rw-rw-rw-   0        0        0     8362 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/directives.min.css
+-rw-rw-rw-   0        0        0   192348 2023-06-26 09:22:18.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/bootstrap.css
+-rw-rw-rw-   0        0        0   155758 2023-06-26 09:22:18.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   314326 2023-06-26 09:22:18.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.css
+-rw-rw-rw-   0        0        0   243602 2023-06-26 09:22:18.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.lite.css
+-rw-rw-rw-   0        0        0   199949 2023-06-26 09:22:18.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.lite.min.css
+-rw-rw-rw-   0        0        0   255261 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.min.css
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.200203 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/modules/
+-rw-rw-rw-   0        0        0    70879 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/modules/animations-extended.css
+-rw-rw-rw-   0        0        0    55325 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/modules/animations-extended.min.css
+-rw-rw-rw-   0        0        0      556 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/style.css
+-rw-rw-rw-   0        0        0      248 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/style.min.css
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.054424 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.575533 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/
+-rw-rw-rw-   0        0        0    20966 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.eot
+-rw-rw-rw-   0        0        0   127744 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0    62876 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff
+-rw-rw-rw-   0        0        0    49976 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff2
+-rw-rw-rw-   0        0        0    20940 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.eot
+-rw-rw-rw-   0        0        0   126792 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0    62316 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff
+-rw-rw-rw-   0        0        0    49380 2023-06-26 09:22:19.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff2
+-rw-rw-rw-   0        0        0    21364 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.eot
+-rw-rw-rw-   0        0        0   127488 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0    62980 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff
+-rw-rw-rw-   0        0        0    50224 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff2
+-rw-rw-rw-   0        0        0    21320 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.eot
+-rw-rw-rw-   0        0        0   126072 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0    61736 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff
+-rw-rw-rw-   0        0        0    49236 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff2
+-rw-rw-rw-   0        0        0    21659 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.eot
+-rw-rw-rw-   0        0        0   127584 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0    61628 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff
+-rw-rw-rw-   0        0        0    48524 2023-06-26 09:22:20.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff2
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.588620 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.619864 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/
+-rw-rw-rw-   0        0        0      547 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/default-skin.png
+-rw-rw-rw-   0        0        0     1554 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/default-skin.svg
+-rw-rw-rw-   0        0        0      866 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/preloader.gif
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.767126 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/
+-rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/01.png
+-rw-rw-rw-   0        0        0      213 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/02.png
+-rw-rw-rw-   0        0        0      209 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/03.png
+-rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/04.png
+-rw-rw-rw-   0        0        0      213 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/05.png
+-rw-rw-rw-   0        0        0      211 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/06.png
+-rw-rw-rw-   0        0        0      215 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/07.png
+-rw-rw-rw-   0        0        0      146 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/08.png
+-rw-rw-rw-   0        0        0      137 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/overlays/09.png
+-rw-rw-rw-   0        0        0   204946 2023-06-26 09:22:21.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/sample.jpg
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:49.782746 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/svg/
+-rw-rw-rw-   0        0        0      218 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/svg/arrow_left.svg
+-rw-rw-rw-   0        0        0      217 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/svg/arrow_right.svg
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.217315 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.431678 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/
+-rw-rw-rw-   0        0        0    32005 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables-select.js
+-rw-rw-rw-   0        0        0    11741 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables-select.min.js
+-rw-rw-rw-   0        0        0   452723 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables.js
+-rw-rw-rw-   0        0        0    84932 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables.min.js
+-rw-rw-rw-   0        0        0     1637 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/rating.js
+-rw-rw-rw-   0        0        0   131637 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/bootstrap.js
+-rw-rw-rw-   0        0        0    58072 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    86927 2023-06-26 09:22:22.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0   478685 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/mdb.js
+-rw-rw-rw-   0        0        0   209696 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/mdb.min.js
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.849548 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/
+-rw-rw-rw-   0        0        0   402487 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/chart.js
+-rw-rw-rw-   0        0        0      570 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/default-file-input.js
+-rw-rw-rw-   0        0        0      685 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/enhanced-modals.js
+-rw-rw-rw-   0        0        0     5373 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/forms-free.js
+-rw-rw-rw-   0        0        0     8661 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/jquery.easing.js
+-rw-rw-rw-   0        0        0      409 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/scrolling-navbar.js
+-rw-rw-rw-   0        0        0      290 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/treeview.js
+-rw-rw-rw-   0        0        0    35106 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/velocity.js
+-rw-rw-rw-   0        0        0    35106 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/velocity.min.js
+-rw-rw-rw-   0        0        0    18936 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/waves.js
+-rw-rw-rw-   0        0        0     5324 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/wow.js
+-rw-rw-rw-   0        0        0    20537 2023-06-26 09:22:23.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/popper.min.js
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.865172 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/
+-rw-rw-rw-   0        0        0      734 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/_custom-skin.scss
+-rw-rw-rw-   0        0        0       21 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/_custom-styles.scss
+-rw-rw-rw-   0        0        0       24 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/_custom-variables.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.865172 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/
+-rw-rw-rw-   0        0        0     4573 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/_datatables-select.scss
+-rw-rw-rw-   0        0        0     4203 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/_datatables.scss
+-rw-rw-rw-   0        0        0     1477 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/_directives.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.880793 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/
+-rw-rw-rw-   0        0        0    28149 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_colors.scss
+-rw-rw-rw-   0        0        0     2549 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_global.scss
+-rw-rw-rw-   0        0        0     1074 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_helpers.scss
+-rw-rw-rw-   0        0        0     1199 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_masks.scss
+-rw-rw-rw-   0        0        0    13073 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_mixins.scss
+-rw-rw-rw-   0        0        0     3665 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_typography.scss
+-rw-rw-rw-   0        0        0    17282 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_variables.scss
+-rw-rw-rw-   0        0        0     3967 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_waves.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.896413 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/
+-rw-rw-rw-   0        0        0     2719 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/_functions.scss
+-rw-rw-rw-   0        0        0     6474 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/_rfs.scss
+-rw-rw-rw-   0        0        0    47781 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/_variables.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.945313 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/
+-rw-rw-rw-   0        0        0     2603 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_animations-basic.scss
+-rw-rw-rw-   0        0        0      335 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_badges.scss
+-rw-rw-rw-   0        0        0     3273 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_buttons.scss
+-rw-rw-rw-   0        0        0      580 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_cards.scss
+-rw-rw-rw-   0        0        0     1205 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_carousels.scss
+-rw-rw-rw-   0        0        0       47 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_depreciated.scss
+-rw-rw-rw-   0        0        0      144 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_dropdowns.scss
+-rw-rw-rw-   0        0        0      314 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_footers.scss
+-rw-rw-rw-   0        0        0    12170 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_forms.scss
+-rw-rw-rw-   0        0        0     1738 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_input-group.scss
+-rw-rw-rw-   0        0        0      557 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_list-group.scss
+-rw-rw-rw-   0        0        0      177 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_loader.scss
+-rw-rw-rw-   0        0        0     6505 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_modals.scss
+-rw-rw-rw-   0        0        0     3243 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_msc.scss
+-rw-rw-rw-   0        0        0     2540 2023-06-26 09:22:26.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_navbars.scss
+-rw-rw-rw-   0        0        0     1960 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_pagination.scss
+-rw-rw-rw-   0        0        0     3888 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_steppers.scss
+-rw-rw-rw-   0        0        0      894 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_switch.scss
+-rw-rw-rw-   0        0        0     1340 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_tables.scss
+-rw-rw-rw-   0        0        0      418 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_treeview.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.070055 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/modules/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:50.949559 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/
+-rw-rw-rw-   0        0        0    22617 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/_module.scss
+-rw-rw-rw-   0        0        0      175 2023-06-26 09:22:27.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/animations-extended.scss
+-rw-rw-rw-   0        0        0     1555 2023-06-26 09:22:24.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/mdb.lite.scss
+-rw-rw-rw-   0        0        0     1724 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/mdb.scss
+-rw-rw-rw-   0        0        0      604 2023-06-26 09:22:25.000000 amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/style.scss
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.070055 amatak-shop-1.1.0/amatak_shop/templates/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.090760 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.232570 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/
+-rw-rw-rw-   0        0        0      277 2023-07-27 13:33:19.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/account_inactive.html
+-rw-rw-rw-   0        0        0      848 2023-07-28 06:39:08.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/account_update.html
+-rw-rw-rw-   0        0        0     2038 2023-07-28 15:41:18.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/base.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.319038 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/
+-rw-rw-rw-   0        0        0      569 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/email_confirmation_message.txt
+-rw-rw-rw-   0        0        0       61 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/email_confirmation_signup_message.txt
+-rw-rw-rw-   0        0        0       61 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/email_confirmation_signup_subject.txt
+-rw-rw-rw-   0        0        0      127 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/email_confirmation_subject.txt
+-rw-rw-rw-   0        0        0      659 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/password_reset_key_message.txt
+-rw-rw-rw-   0        0        0      114 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/password_reset_key_subject.txt
+-rw-rw-rw-   0        0        0     2503 2023-07-27 02:28:31.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email.html
+-rw-rw-rw-   0        0        0      955 2023-07-27 02:28:37.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email_confirm.html
+-rw-rw-rw-   0        0        0     2144 2023-07-28 15:32:57.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/login.html
+-rw-rw-rw-   0        0        0      925 2023-07-28 15:59:50.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/logout.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.449162 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/
+-rw-rw-rw-   0        0        0      110 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/cannot_delete_primary_email.txt
+-rw-rw-rw-   0        0        0       90 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/email_confirmation_sent.txt
+-rw-rw-rw-   0        0        0       81 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/email_confirmed.txt
+-rw-rw-rw-   0        0        0       85 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/email_deleted.txt
+-rw-rw-rw-   0        0        0      138 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/logged_in.txt
+-rw-rw-rw-   0        0        0       72 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/logged_out.txt
+-rw-rw-rw-   0        0        0       82 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/password_changed.txt
+-rw-rw-rw-   0        0        0       78 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/password_set.txt
+-rw-rw-rw-   0        0        0       79 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/primary_email_set.txt
+-rw-rw-rw-   0        0        0       97 2023-06-26 09:22:29.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/messages/unverified_primary_email.txt
+-rw-rw-rw-   0        0        0      464 2023-07-27 02:28:45.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_change.html
+-rw-rw-rw-   0        0        0      833 2023-07-27 02:28:49.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_reset.html
+-rw-rw-rw-   0        0        0      502 2023-07-27 02:28:54.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_reset_done.html
+-rw-rw-rw-   0        0        0      971 2023-07-27 02:28:59.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_reset_from_key.html
+-rw-rw-rw-   0        0        0      280 2023-07-27 02:29:04.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_reset_from_key_done.html
+-rw-rw-rw-   0        0        0      448 2023-07-27 02:29:08.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_set.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.500080 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/profile/
+-rw-rw-rw-   0        0        0      482 2023-05-24 11:09:56.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/profile/form.html
+-rw-rw-rw-   0        0        0     3695 2023-07-26 14:40:33.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/profile/view.html
+-rw-rw-rw-   0        0        0     1294 2023-07-28 15:37:43.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/signup.html
+-rw-rw-rw-   0        0        0      292 2023-07-27 02:29:13.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/signup_closed.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.513044 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/snippets/
+-rw-rw-rw-   0        0        0      186 2023-07-28 15:44:32.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/snippets/already_logged_in.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.517036 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/tags/
+-rw-rw-rw-   0        0        0        0 2023-07-28 05:59:38.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/tags/account_txs_table.html
+-rw-rw-rw-   0        0        0        0 2023-07-28 05:59:44.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/tags/accounts_table.html
+-rw-rw-rw-   0        0        0      465 2023-07-27 02:29:16.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/verification_sent.html
+-rw-rw-rw-   0        0        0      825 2023-07-27 02:29:20.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/verified_email_required.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.549948 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/
+-rw-rw-rw-   0        0        0     1340 2023-07-28 06:23:43.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/customer_create.html
+-rw-rw-rw-   0        0        0      691 2023-07-28 06:24:43.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/customer_list.html
+-rw-rw-rw-   0        0        0     1365 2023-07-28 06:25:42.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/customer_update.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.551941 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/includes/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:07:55.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/includes/card_customer.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.561914 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/tags/
+-rw-rw-rw-   0        0        0     1331 2023-07-28 06:22:05.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/tags/customer_table.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.581862 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/legal/
+-rw-rw-rw-   0        0        0      878 2023-07-27 13:25:10.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/legal/policy.html
+-rw-rw-rw-   0        0        0     1008 2023-07-27 13:25:24.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/legal/terms.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.605865 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/openid/
+-rw-rw-rw-   0        0        0       52 2023-07-27 13:34:26.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/openid/base.html
+-rw-rw-rw-   0        0        0      369 2023-07-27 13:34:31.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/openid/login.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.668351 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/
+-rw-rw-rw-   0        0        0      337 2023-07-27 12:24:13.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/authentication_error.html
+-rw-rw-rw-   0        0        0       46 2023-07-27 12:22:35.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/base.html
+-rw-rw-rw-   0        0        0     1434 2023-07-26 13:51:34.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/connections.html
+-rw-rw-rw-   0        0        0      454 2023-07-26 13:51:39.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/login_cancelled.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.719334 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/messages/
+-rw-rw-rw-   0        0        0       90 2023-06-26 09:22:30.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/messages/account_connected.txt
+-rw-rw-rw-   0        0        0      115 2023-06-26 09:22:30.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/messages/account_connected_other.txt
+-rw-rw-rw-   0        0        0       93 2023-06-26 09:22:30.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/messages/account_disconnected.txt
+-rw-rw-rw-   0        0        0      783 2023-07-27 12:22:58.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/signup.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.737033 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/snippets/
+-rw-rw-rw-   0        0        0       51 2023-06-26 09:22:30.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/snippets/login_extra.html
+-rw-rw-rw-   0        0        0      663 2023-06-26 09:22:30.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/snippets/provider_list.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.090760 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.783898 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/tags/
+-rw-rw-rw-   0        0        0    12761 2023-07-28 23:51:28.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/tags/brand.html
+-rw-rw-rw-   0        0        0      743 2023-07-28 22:56:20.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/tags/scripts.html
+-rw-rw-rw-   0        0        0      205 2023-07-28 22:56:25.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/tags/styles.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:51.998331 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/
+-rw-rw-rw-   0        0        0     1834 2023-07-28 22:32:41.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/base.html
+-rw-rw-rw-   0        0        0     6790 2023-07-29 01:13:33.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/checkout.html
+-rw-rw-rw-   0        0        0     1703 2023-07-28 23:27:38.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/footer.html
+-rw-rw-rw-   0        0        0     5118 2023-07-29 00:57:35.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/home.html
+-rw-rw-rw-   0        0        0     3631 2023-07-28 23:44:10.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/navbar.html
+-rw-rw-rw-   0        0        0     1620 2023-07-29 01:14:11.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/order_snippet.html
+-rw-rw-rw-   0        0        0     2571 2023-07-29 00:46:52.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/order_summary.html
+-rw-rw-rw-   0        0        0     8738 2023-07-29 04:39:57.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/payment.html
+-rw-rw-rw-   0        0        0     2972 2023-07-29 04:29:32.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/product.html
+-rw-rw-rw-   0        0        0      366 2023-07-27 12:21:37.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/request_refund.html
+-rw-rw-rw-   0        0        0      601 2023-07-27 12:22:11.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/scripts.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.013952 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/tags/
+-rw-rw-rw-   0        0        0      277 2023-07-28 14:20:28.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/tags/sidebar_left.html
+-rw-rw-rw-   0        0        0      489 2023-07-28 14:06:24.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/tags/store_advertise_red.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.045194 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.045194 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/includes/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:26:37.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/includes/card_vendor.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.060987 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/tags/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:06:22.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/tags/vendor_table.html
+-rw-rw-rw-   0        0        0     1326 2023-07-28 06:29:13.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/vendor_create.html
+-rw-rw-rw-   0        0        0      673 2023-07-28 06:30:11.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/vendor_list.html
+-rw-rw-rw-   0        0        0     1363 2023-07-28 06:30:58.000000 amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/vendor_update.html
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.067224 amatak-shop-1.1.0/amatak_shop/templatetags/
+-rw-rw-rw-   0        0        0      499 2023-07-30 11:06:46.000000 amatak-shop-1.1.0/amatak_shop/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2269 2023-07-30 03:29:14.000000 amatak-shop-1.1.0/amatak_shop/templatetags/amatak_shop.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.095036 amatak-shop-1.1.0/amatak_shop/tests/
+-rw-rw-rw-   0        0        0      530 2023-07-27 14:14:21.000000 amatak-shop-1.1.0/amatak_shop/tests/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-07-27 14:13:22.000000 amatak-shop-1.1.0/amatak_shop/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.240798 amatak-shop-1.1.0/amatak_shop/urls/
+-rw-rw-rw-   0        0        0      786 2023-07-27 11:50:04.000000 amatak-shop-1.1.0/amatak_shop/urls/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-07-27 11:50:25.000000 amatak-shop-1.1.0/amatak_shop/urls/add_coupon.py
+-rw-rw-rw-   0        0        0      192 2023-07-27 11:50:49.000000 amatak-shop-1.1.0/amatak_shop/urls/add_to_cart.py
+-rw-rw-rw-   0        0        0      187 2023-07-27 11:51:11.000000 amatak-shop-1.1.0/amatak_shop/urls/checkout.py
+-rw-rw-rw-   0        0        0     1955 2023-07-29 02:35:17.000000 amatak-shop-1.1.0/amatak_shop/urls/home.py
+-rw-rw-rw-   0        0        0      206 2023-07-27 11:55:00.000000 amatak-shop-1.1.0/amatak_shop/urls/order_summary.py
+-rw-rw-rw-   0        0        0      259 2023-07-29 02:33:41.000000 amatak-shop-1.1.0/amatak_shop/urls/payment.py
+-rw-rw-rw-   0        0        0      164 2023-07-27 11:55:58.000000 amatak-shop-1.1.0/amatak_shop/urls/policy.py
+-rw-rw-rw-   0        0        0      264 2023-07-27 11:56:23.000000 amatak-shop-1.1.0/amatak_shop/urls/products.py
+-rw-rw-rw-   0        0        0      212 2023-07-27 11:56:47.000000 amatak-shop-1.1.0/amatak_shop/urls/remove_from_cart.py
+-rw-rw-rw-   0        0        0      263 2023-07-27 11:57:06.000000 amatak-shop-1.1.0/amatak_shop/urls/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0      468 2023-07-27 11:58:25.000000 amatak-shop-1.1.0/amatak_shop/urls/request_refund.py
+-rw-rw-rw-   0        0        0      419 2023-07-30 08:29:35.000000 amatak-shop-1.1.0/amatak_shop/urls/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.469795 amatak-shop-1.1.0/amatak_shop/views/
+-rw-rw-rw-   0        0        0     1066 2023-07-27 12:00:52.000000 amatak-shop-1.1.0/amatak_shop/views/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-07-29 01:36:29.000000 amatak-shop-1.1.0/amatak_shop/views/add_coupon.py
+-rw-rw-rw-   0        0        0     1989 2023-07-29 00:45:48.000000 amatak-shop-1.1.0/amatak_shop/views/add_to_cart.py
+-rw-rw-rw-   0        0        0     8972 2023-07-29 01:58:06.000000 amatak-shop-1.1.0/amatak_shop/views/checkout.py
+-rw-rw-rw-   0        0        0      396 2023-07-27 12:03:04.000000 amatak-shop-1.1.0/amatak_shop/views/create_ref_code.py
+-rw-rw-rw-   0        0        0      693 2023-07-29 04:32:48.000000 amatak-shop-1.1.0/amatak_shop/views/get_coupon.py
+-rw-rw-rw-   0        0        0     1110 2023-07-27 12:11:56.000000 amatak-shop-1.1.0/amatak_shop/views/home.py
+-rw-rw-rw-   0        0        0     1132 2023-07-29 01:39:28.000000 amatak-shop-1.1.0/amatak_shop/views/is_valid_form.py
+-rw-rw-rw-   0        0        0      471 2023-07-27 12:12:39.000000 amatak-shop-1.1.0/amatak_shop/views/items_detail_views.py
+-rw-rw-rw-   0        0        0      689 2023-07-29 04:09:03.000000 amatak-shop-1.1.0/amatak_shop/views/login.py
+-rw-rw-rw-   0        0        0      708 2023-07-29 04:09:12.000000 amatak-shop-1.1.0/amatak_shop/views/logout.py
+-rw-rw-rw-   0        0        0     1482 2023-07-27 12:13:42.000000 amatak-shop-1.1.0/amatak_shop/views/order_summary.py
+-rw-rw-rw-   0        0        0     6935 2023-07-29 04:42:13.000000 amatak-shop-1.1.0/amatak_shop/views/payment.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:14:56.000000 amatak-shop-1.1.0/amatak_shop/views/policy.py
+-rw-rw-rw-   0        0        0     1024 2023-07-27 12:15:28.000000 amatak-shop-1.1.0/amatak_shop/views/products.py
+-rw-rw-rw-   0        0        0     2040 2023-07-29 04:49:57.000000 amatak-shop-1.1.0/amatak_shop/views/remove_from_cart.py
+-rw-rw-rw-   0        0        0     2152 2023-07-29 00:51:11.000000 amatak-shop-1.1.0/amatak_shop/views/remove_single_item_from_cart.py
+-rw-rw-rw-   0        0        0     2119 2023-07-27 12:17:13.000000 amatak-shop-1.1.0/amatak_shop/views/request_refund.py
+-rw-rw-rw-   0        0        0      691 2023-07-29 04:08:52.000000 amatak-shop-1.1.0/amatak_shop/views/sign_up.py
+-rw-rw-rw-   0        0        0      610 2023-07-27 12:17:44.000000 amatak-shop-1.1.0/amatak_shop/views/terms.py
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.184527 amatak-shop-1.1.0/amatak_shop.egg-info/
+-rw-rw-rw-   0        0        0     3188 2023-07-30 11:13:46.000000 amatak-shop-1.1.0/amatak_shop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18457 2023-07-30 11:13:47.000000 amatak-shop-1.1.0/amatak_shop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 11:13:46.000000 amatak-shop-1.1.0/amatak_shop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-30 11:13:46.000000 amatak-shop-1.1.0/amatak_shop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:47.090760 amatak-shop-1.1.0/eCommerce/
+drwxrwxrwx   0        0        0        0 2023-07-30 11:13:52.550722 amatak-shop-1.1.0/eCommerce/settings/
+-rw-rw-rw-   0        0        0     1487 2023-07-30 03:32:50.000000 amatak-shop-1.1.0/eCommerce/settings/AmatakShopDev.py
+-rw-rw-rw-   0        0        0      256 2023-07-30 02:54:02.000000 amatak-shop-1.1.0/eCommerce/settings/__init__.py
+-rw-rw-rw-   0        0        0     2588 2023-07-30 03:15:58.000000 amatak-shop-1.1.0/eCommerce/settings/base.py
+-rw-rw-rw-   0        0        0     1096 2023-07-30 02:56:09.000000 amatak-shop-1.1.0/eCommerce/settings/production.py
+-rw-rw-rw-   0        0        0      564 2023-07-30 11:07:03.000000 amatak-shop-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 11:13:52.554712 amatak-shop-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-07-30 00:24:33.000000 amatak-shop-1.1.0/setup.py
```

### Comparing `amatak-shop-1.0.9/PKG-INFO` & `amatak-shop-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.9
+Version: 1.1.0
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `amatak-shop-1.0.9/README.md` & `amatak-shop-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/forms/checkout.py` & `amatak-shop-1.1.0/amatak_shop/forms/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/forms/coupon.py` & `amatak-shop-1.1.0/amatak_shop/forms/coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/forms/payment.py` & `amatak-shop-1.1.0/amatak_shop/forms/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/forms/refund.py` & `amatak-shop-1.1.0/amatak_shop/forms/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/management/commands/rename.py` & `amatak-shop-1.1.0/amatak_shop/management/commands/rename.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/migrations/0001_initial.py` & `amatak-shop-1.1.0/amatak_shop/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/__init__.py` & `amatak-shop-1.1.0/amatak_shop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/address.py` & `amatak-shop-1.1.0/amatak_shop/models/address.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/category.py` & `amatak-shop-1.1.0/amatak_shop/models/category.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/item.py` & `amatak-shop-1.1.0/amatak_shop/models/item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/mixins.py` & `amatak-shop-1.1.0/amatak_shop/models/mixins.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/order.py` & `amatak-shop-1.1.0/amatak_shop/models/order.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/order_item.py` & `amatak-shop-1.1.0/amatak_shop/models/order_item.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/payment.py` & `amatak-shop-1.1.0/amatak_shop/models/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/refund.py` & `amatak-shop-1.1.0/amatak_shop/models/refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/models/user_receiver_profile.py` & `amatak-shop-1.1.0/amatak_shop/models/user_receiver_profile.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/settings/base.py` & `amatak-shop-1.1.0/amatak_shop/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/LICENSE` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/LICENSE`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/README.md` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/README.md`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css.map` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.css.map`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma-rtl.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma.css.map` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma.css.map`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/css/bulma.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/css/bulma.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/package.json` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/package.json`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/generic.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/generic.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/base/minireset.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/base/minireset.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/breadcrumb.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/breadcrumb.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/card.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/card.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/dropdown.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/dropdown.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/level.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/level.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/media.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/media.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/menu.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/menu.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/message.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/message.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/modal.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/modal.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/navbar.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/navbar.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/pagination.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/pagination.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/panel.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/panel.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/components/tabs.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/components/tabs.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/box.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/box.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/button.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/button.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/container.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/container.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/content.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/content.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/icon.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/icon.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/image.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/image.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/notification.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/notification.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/other.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/other.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/progress.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/progress.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/table.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/table.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/tag.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/tag.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/elements/title.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/elements/title.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/file.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/file.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/input-textarea.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/input-textarea.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/select.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/select.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/shared.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/shared.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/form/tools.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/form/tools.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/grid/columns.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/grid/columns.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/grid/tiles.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/grid/tiles.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/color.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/color.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/flexbox.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/flexbox.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/spacing.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/spacing.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/typography.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/typography.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/helpers/visibility.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/helpers/visibility.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/layout/hero.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/layout/hero.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/controls.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/controls.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/derived-variables.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/derived-variables.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/functions.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/functions.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/initial-variables.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/initial-variables.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/bulma/sass/utilities/mixins.sass` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/bulma/sass/utilities/mixins.sass`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables-select.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables-select.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables-select.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables-select.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/datatables.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/datatables.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/directives.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/directives.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/addons/directives.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/addons/directives.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/bootstrap.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/bootstrap.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.lite.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.lite.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.lite.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.lite.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/mdb.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/mdb.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/modules/animations-extended.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/modules/animations-extended.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/modules/animations-extended.min.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/modules/animations-extended.min.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/css/style.css` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/css/style.css`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.eot` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.eot`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.ttf` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff2` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.eot` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.eot`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.ttf` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff2` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Light.woff2`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.eot` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.eot`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.ttf` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff2` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Medium.woff2`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.eot` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.eot`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.ttf` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff2` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.eot` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.eot`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.ttf` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff2` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/font/roboto/Roboto-Thin.woff2`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/default-skin.png` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/default-skin.png`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/default-skin.svg` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/default-skin.svg`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/lightbox/preloader.gif` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/lightbox/preloader.gif`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/img/sample.jpg` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/img/sample.jpg`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables-select.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables-select.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables-select.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables-select.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/datatables.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/datatables.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/addons/rating.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/addons/rating.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/bootstrap.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/bootstrap.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/jquery-3.3.1.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/mdb.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/mdb.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/mdb.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/mdb.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/chart.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/chart.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/default-file-input.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/default-file-input.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/enhanced-modals.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/enhanced-modals.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/forms-free.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/forms-free.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/jquery.easing.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/jquery.easing.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/velocity.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/velocity.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/velocity.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/velocity.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/waves.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/waves.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/modules/wow.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/modules/wow.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/js/popper.min.js` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/_custom-skin.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/_custom-skin.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/_datatables-select.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/_datatables-select.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/_datatables.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/_datatables.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/addons/_directives.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/addons/_directives.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_colors.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_colors.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_global.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_global.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_helpers.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_helpers.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_masks.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_masks.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_mixins.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_mixins.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_typography.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_typography.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_variables.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_variables.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/_waves.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/_waves.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/_functions.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/_rfs.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/_rfs.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/core/bootstrap/_variables.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/core/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_animations-basic.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_animations-basic.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_buttons.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_buttons.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_cards.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_cards.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_carousels.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_carousels.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_forms.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_forms.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_input-group.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_input-group.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_list-group.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_list-group.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_modals.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_modals.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_msc.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_msc.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_navbars.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_navbars.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_pagination.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_pagination.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_steppers.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_steppers.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_switch.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_switch.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/_tables.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/_tables.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/_module.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/free/modules/animations-extended/_module.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/mdb.lite.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/mdb.lite.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/mdb.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/mdb.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/static/amatak_shop/scss/style.scss` & `amatak-shop-1.1.0/amatak_shop/static/amatak_shop/scss/style.scss`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/account_update.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/account_update.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/base.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/base.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/email_confirmation_message.txt` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email/password_reset_key_message.txt` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/email_confirm.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/login.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/login.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/logout.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/logout.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_reset.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/password_reset_from_key.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/profile/view.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/profile/view.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/signup.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/signup.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/account/verified_email_required.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/customer_create.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/customer_create.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/customer_list.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/customer_list.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/customer_update.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/customer_update.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/customer/tags/customer_table.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/customer/tags/customer_table.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/legal/policy.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/legal/policy.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/legal/terms.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/legal/terms.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/connections.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/signup.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/socialaccount/snippets/provider_list.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/tags/brand.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/tags/brand.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/static/tags/scripts.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/static/tags/scripts.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/base.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/base.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/checkout.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/checkout.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/footer.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/footer.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/home.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/home.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/navbar.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/navbar.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/order_snippet.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/order_snippet.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/order_summary.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/order_summary.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/payment.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/payment.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/product.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/product.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/store/scripts.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/store/scripts.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/vendor_create.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/vendor_create.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/vendor_list.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/vendor_list.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templates/amatak_shop/vendor/vendor_update.html` & `amatak-shop-1.1.0/amatak_shop/templates/amatak_shop/vendor/vendor_update.html`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/templatetags/amatak_shop.py` & `amatak-shop-1.1.0/amatak_shop/templatetags/amatak_shop.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/tests/__init__.py` & `amatak-shop-1.1.0/amatak_shop/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/urls/__init__.py` & `amatak-shop-1.1.0/amatak_shop/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/urls/home.py` & `amatak-shop-1.1.0/amatak_shop/urls/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/__init__.py` & `amatak-shop-1.1.0/amatak_shop/views/__init__.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/add_coupon.py` & `amatak-shop-1.1.0/amatak_shop/views/add_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/add_to_cart.py` & `amatak-shop-1.1.0/amatak_shop/views/add_to_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/checkout.py` & `amatak-shop-1.1.0/amatak_shop/views/checkout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/get_coupon.py` & `amatak-shop-1.1.0/amatak_shop/views/get_coupon.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/home.py` & `amatak-shop-1.1.0/amatak_shop/views/home.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/is_valid_form.py` & `amatak-shop-1.1.0/amatak_shop/views/is_valid_form.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/login.py` & `amatak-shop-1.1.0/amatak_shop/views/login.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/logout.py` & `amatak-shop-1.1.0/amatak_shop/views/logout.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/order_summary.py` & `amatak-shop-1.1.0/amatak_shop/views/order_summary.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/payment.py` & `amatak-shop-1.1.0/amatak_shop/views/payment.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/policy.py` & `amatak-shop-1.1.0/amatak_shop/views/policy.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/products.py` & `amatak-shop-1.1.0/amatak_shop/views/products.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/remove_from_cart.py` & `amatak-shop-1.1.0/amatak_shop/views/remove_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/remove_single_item_from_cart.py` & `amatak-shop-1.1.0/amatak_shop/views/remove_single_item_from_cart.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/request_refund.py` & `amatak-shop-1.1.0/amatak_shop/views/request_refund.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/sign_up.py` & `amatak-shop-1.1.0/amatak_shop/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop/views/terms.py` & `amatak-shop-1.1.0/amatak_shop/views/terms.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/amatak_shop.egg-info/PKG-INFO` & `amatak-shop-1.1.0/amatak_shop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amatak-shop
-Version: 1.0.9
+Version: 1.1.0
 Summary: Amatak OpenSource Online Shop 
 Author-email: Rony MAN <amatak.io@outlook.com>
 Project-URL: Homepage, https://github.com/amatak-org/AmatakOnlineShop
 Project-URL: Bug Tracker, https://github.com/amatak-org/AmatakOnlineShop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `amatak-shop-1.0.9/amatak_shop.egg-info/SOURCES.txt` & `amatak-shop-1.1.0/amatak_shop.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+amatak_shop/__init__.py
+amatak_shop/admin.py
+amatak_shop/apps.py
 amatak_shop.egg-info/PKG-INFO
 amatak_shop.egg-info/SOURCES.txt
 amatak_shop.egg-info/dependency_links.txt
 amatak_shop.egg-info/top_level.txt
 amatak_shop/forms/__init__.py
 amatak_shop/forms/checkout.py
 amatak_shop/forms/coupon.py
```

### Comparing `amatak-shop-1.0.9/eCommerce/settings/AmatakShopDev.py` & `amatak-shop-1.1.0/eCommerce/settings/AmatakShopDev.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/eCommerce/settings/base.py` & `amatak-shop-1.1.0/eCommerce/settings/base.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/eCommerce/settings/production.py` & `amatak-shop-1.1.0/eCommerce/settings/production.py`

 * *Files identical despite different names*

### Comparing `amatak-shop-1.0.9/pyproject.toml` & `amatak-shop-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amatak-shop"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Rony MAN", email="amatak.io@outlook.com" },
 ]
 description = "Amatak OpenSource Online Shop "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

