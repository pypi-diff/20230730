# Comparing `tmp/reflex-0.2.3a7.tar.gz` & `tmp/reflex-0.2.3a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.3a7.tar", max compression
+gzip compressed data, was "reflex-0.2.3a8.tar", max compression
```

## Comparing `reflex-0.2.3a7.tar` & `reflex-0.2.3a8.tar`

### file list

```diff
@@ -1,178 +1,179 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a7/LICENSE
--rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a7/README.md
--rw-r--r--   0        0        0     2002 2023-07-27 02:12:09.661733 reflex-0.2.3a7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a7/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-26 04:50:13.391602 reflex-0.2.3a7/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a7/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.3a7/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a7/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a7/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a7/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a7/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a7/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a7/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a7/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a7/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a7/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a7/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a7/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a7/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a7/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a7/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10127 2023-07-27 02:10:59.437571 reflex-0.2.3a7/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.3a7/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a7/reflex/admin.py
--rw-r--r--   0        0        0    24459 2023-07-26 22:57:11.741737 reflex-0.2.3a7/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a7/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a7/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a7/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a7/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a7/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a7/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a7/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a7/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a7/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a7/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a7/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a7/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a7/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a7/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a7/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a7/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a7/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a7/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a7/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a7/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a7/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a7/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a7/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a7/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a7/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a7/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a7/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a7/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a7/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a7/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a7/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a7/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a7/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a7/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a7/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a7/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a7/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a7/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a7/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a7/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a7/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a7/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a7/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a7/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a7/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a7/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a7/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a7/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-21 23:52:40.428089 reflex-0.2.3a7/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a7/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a7/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a7/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a7/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a7/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a7/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a7/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a7/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a7/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a7/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a7/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a7/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a7/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a7/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a7/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a7/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a7/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a7/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a7/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a7/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a7/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a7/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a7/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a7/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a7/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a7/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a7/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a7/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a7/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a7/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a7/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a7/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a7/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a7/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a7/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a7/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a7/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a7/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a7/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a7/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.3a7/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a7/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a7/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a7/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a7/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a7/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a7/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a7/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a7/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a7/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a7/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a7/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a7/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a7/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a7/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a7/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-07-27 02:10:59.437877 reflex-0.2.3a7/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a7/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a7/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-07-27 02:10:59.438075 reflex-0.2.3a7/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a7/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3593 2023-07-27 02:10:59.438276 reflex-0.2.3a7/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a7/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a7/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7692 2023-07-27 01:47:00.564666 reflex-0.2.3a7/reflex/config.py
--rw-r--r--   0        0        0    11209 2023-07-27 02:11:07.178831 reflex-0.2.3a7/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a7/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a7/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a7/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a7/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a7/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a7/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a7/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a7/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a7/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a7/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a7/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a7/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.3a7/reflex/model.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a7/reflex/py.typed
--rw-r--r--   0        0        0    11041 2023-07-27 02:11:07.179265 reflex-0.2.3a7/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.3a7/reflex/route.py
--rw-r--r--   0        0        0    32314 2023-07-27 02:11:44.068790 reflex-0.2.3a7/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a7/reflex/style.py
--rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.3a7/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a7/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7971 2023-07-27 01:47:00.567138 reflex-0.2.3a7/reflex/utils/build.py
--rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.3a7/reflex/utils/console.py
--rw-r--r--   0        0        0     4225 2023-07-27 01:47:00.567438 reflex-0.2.3a7/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-07-21 23:46:28.128377 reflex-0.2.3a7/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-07-26 22:57:11.745697 reflex-0.2.3a7/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a7/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    14208 2023-07-27 02:11:07.179634 reflex-0.2.3a7/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     4105 2023-07-27 01:47:00.568031 reflex-0.2.3a7/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a7/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a7/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a7/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a7/reflex/vars.py
--rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a7/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a8/LICENSE
+-rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a8/README.md
+-rw-r--r--   0        0        0     2001 2023-07-30 04:08:40.489186 reflex-0.2.3a8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a8/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-27 23:45:03.452394 reflex-0.2.3a8/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a8/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-27 23:45:03.453010 reflex-0.2.3a8/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a8/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a8/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a8/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a8/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a8/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a8/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a8/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a8/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a8/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a8/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a8/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a8/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a8/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a8/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10172 2023-07-27 23:45:03.453483 reflex-0.2.3a8/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1996 2023-07-27 23:45:03.454124 reflex-0.2.3a8/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a8/reflex/admin.py
+-rw-r--r--   0        0        0    24864 2023-07-28 19:12:55.971292 reflex-0.2.3a8/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a8/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a8/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a8/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a8/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a8/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a8/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a8/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a8/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a8/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a8/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a8/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a8/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a8/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a8/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a8/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a8/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a8/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a8/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a8/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a8/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a8/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a8/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a8/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a8/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a8/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a8/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a8/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a8/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a8/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a8/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a8/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a8/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a8/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a8/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a8/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a8/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a8/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a8/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a8/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a8/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a8/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a8/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a8/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a8/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a8/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a8/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a8/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a8/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-29 23:01:33.748219 reflex-0.2.3a8/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a8/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a8/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a8/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a8/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a8/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a8/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a8/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a8/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a8/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a8/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a8/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a8/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a8/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a8/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a8/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a8/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a8/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a8/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a8/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a8/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a8/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a8/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a8/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a8/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a8/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a8/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a8/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a8/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a8/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a8/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a8/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a8/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a8/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a8/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a8/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a8/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a8/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a8/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a8/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a8/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2919 2023-07-29 01:05:18.595845 reflex-0.2.3a8/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a8/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a8/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a8/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a8/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a8/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a8/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a8/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a8/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a8/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a8/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a8/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a8/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a8/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a8/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a8/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5150 2023-07-27 23:45:03.454877 reflex-0.2.3a8/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a8/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a8/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-27 23:45:03.455160 reflex-0.2.3a8/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a8/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     4679 2023-07-27 23:45:03.455385 reflex-0.2.3a8/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a8/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a8/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7564 2023-07-27 23:45:03.455544 reflex-0.2.3a8/reflex/config.py
+-rw-r--r--   0        0        0    12451 2023-07-29 23:18:00.803629 reflex-0.2.3a8/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a8/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a8/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a8/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a8/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a8/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a8/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a8/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a8/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a8/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a8/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a8/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a8/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9598 2023-07-29 02:57:05.377850 reflex-0.2.3a8/reflex/model.py
+-rw-r--r--   0        0        0     1832 2023-07-27 23:45:03.455818 reflex-0.2.3a8/reflex/page.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a8/reflex/py.typed
+-rw-r--r--   0        0        0    10573 2023-07-30 02:48:40.517517 reflex-0.2.3a8/reflex/reflex.py
+-rw-r--r--   0        0        0     3934 2023-07-27 23:45:03.456240 reflex-0.2.3a8/reflex/route.py
+-rw-r--r--   0        0        0    32524 2023-07-29 03:11:02.108051 reflex-0.2.3a8/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a8/reflex/style.py
+-rw-r--r--   0        0        0    15133 2023-07-30 02:59:25.316492 reflex-0.2.3a8/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a8/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     6212 2023-07-29 04:28:04.850394 reflex-0.2.3a8/reflex/utils/build.py
+-rw-r--r--   0        0        0     3743 2023-07-30 03:08:01.692245 reflex-0.2.3a8/reflex/utils/console.py
+-rw-r--r--   0        0        0     3795 2023-07-29 22:49:09.601795 reflex-0.2.3a8/reflex/utils/exec.py
+-rw-r--r--   0        0        0    12342 2023-07-29 01:05:18.597732 reflex-0.2.3a8/reflex/utils/format.py
+-rw-r--r--   0        0        0      590 2023-07-27 23:45:03.457502 reflex-0.2.3a8/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a8/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    16639 2023-07-30 02:54:45.030336 reflex-0.2.3a8/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     6387 2023-07-29 23:11:18.706469 reflex-0.2.3a8/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a8/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a8/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a8/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a8/reflex/vars.py
+-rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a8/PKG-INFO
```

### Comparing `reflex-0.2.3a7/LICENSE` & `reflex-0.2.3a8/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/README.md` & `reflex-0.2.3a8/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/pyproject.toml` & `reflex-0.2.3a8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.3a7"
+version = "0.2.3a8"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
@@ -62,15 +62,15 @@
     {version = "^1.1", python = ">=3.7, <3.8"}
 ]
 asynctest = "^0.13.0"
 pre-commit = {version = "^3.2.1", python = ">=3.8,<4.0"}
 selenium = "^4.10.0"
 
 [tool.poetry.scripts]
-reflex = "reflex.reflex:main"
+reflex = "reflex.reflex:cli"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
```

### Comparing `reflex-0.2.3a7/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.3a8/reflex/.templates/apps/counter/counter.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,10 +44,10 @@
         padding_y="5em",
         font_size="2em",
         text_align="center",
     )
 
 
 # Add state and page to the app.
-app = rx.App(state=State)
+app = rx.App()
 app.add_page(index, title="Counter")
 app.compile()
```

### Comparing `reflex-0.2.3a7/reflex/.templates/apps/default/default.py` & `reflex-0.2.3a8/reflex/.templates/apps/default/default.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,10 +36,10 @@
             font_size="2em",
             padding_top="10%",
         ),
     )
 
 
 # Add state and page to the app.
-app = rx.App(state=State)
+app = rx.App()
 app.add_page(index)
 app.compile()
```

### Comparing `reflex-0.2.3a7/reflex/.templates/assets/favicon.ico` & `reflex-0.2.3a8/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.3a8/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.3a8/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/web/bun.lockb` & `reflex-0.2.3a8/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/web/package.json` & `reflex-0.2.3a8/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/web/pages/_app.js` & `reflex-0.2.3a8/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.3a8/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/.templates/web/utils/state.js` & `reflex-0.2.3a8/reflex/.templates/web/utils/state.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -403,13 +403,16 @@
 
 /**
  * Get the value from a ref.
  * @param ref The ref to get the value from.
  * @returns The value.
  */
 export const getRefValue = (ref) => {
+    if (!ref || !ref.current) {
+        return;
+    }
     if (ref.current.type == "checkbox") {
         return ref.current.checked;
     } else {
         return ref.current.value;
     }
 }
```

### Comparing `reflex-0.2.3a7/reflex/__init__.py` & `reflex-0.2.3a8/reflex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .event import set_focus as set_focus
 from .event import set_local_storage as set_local_storage
 from .event import set_value as set_value
 from .event import window_alert as window_alert
 from .middleware import Middleware as Middleware
 from .model import Model as Model
 from .model import session as session
+from .page import page as page
 from .route import route as route
 from .state import ComputedVar as var
 from .state import State as State
 from .style import color_mode as color_mode
 from .style import toggle_color_mode as toggle_color_mode
 from .vars import Var as Var
 from .vars import cached_var as cached_var
```

### Comparing `reflex-0.2.3a7/reflex/app.py` & `reflex-0.2.3a8/reflex/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 from reflex.compiler import utils as compiler_utils
 from reflex.components.component import Component, ComponentStyle
 from reflex.components.layout.fragment import Fragment
 from reflex.config import get_config
 from reflex.event import Event, EventHandler, EventSpec
 from reflex.middleware import HydrateMiddleware, Middleware
 from reflex.model import Model
+from reflex.page import (
+    DECORATED_PAGES,
+)
 from reflex.route import (
-    DECORATED_ROUTES,
     catchall_in_route,
     catchall_prefix,
     get_route_args,
     verify_route_validity,
 )
 from reflex.state import DefaultState, State, StateManager, StateUpdate
 from reflex.utils import console, format, types
@@ -102,30 +104,32 @@
         Raises:
             ValueError: If the event namespace is not provided in the config.
                         Also, if there are multiple client subclasses of rx.State(Subclasses of rx.State should consist
                         of the DefaultState and the client app state).
         """
         super().__init__(*args, **kwargs)
         state_subclasses = State.__subclasses__()
+        inferred_state = state_subclasses[-1]
         is_testing_env = constants.PYTEST_CURRENT_TEST in os.environ
 
         # Special case to allow test cases have multiple subclasses of rx.State.
         if not is_testing_env:
             # Only the default state and the client state should be allowed as subclasses.
             if len(state_subclasses) > 2:
                 raise ValueError(
                     "rx.State has been subclassed multiple times. Only one subclass is allowed"
                 )
-            if self.state != DefaultState:
-                console.deprecate(
-                    "Passing the state as keyword argument to `rx.App` is deprecated. "
-                    "The base state will automatically be inferred as the subclass of `rx.State`."
-                )
-            self.state = state_subclasses[-1]
 
+            # verify that provided state is valid
+            if self.state not in [DefaultState, inferred_state]:
+                console.warn(
+                    f"Using substate ({self.state.__name__}) as root state in `rx.App` is currently not supported."
+                    f" Defaulting to root state: ({inferred_state.__name__})"
+                )
+            self.state = inferred_state
         # Get the config
         config = get_config()
 
         # Add middleware.
         self.middleware.append(HydrateMiddleware())
 
         # Set up the state manager.
@@ -463,31 +467,31 @@
         progress = Progress(
             *Progress.get_default_columns()[:-1],
             MofNCompleteColumn(),
             TimeElapsedColumn(),
         )
         task = progress.add_task("Compiling: ", total=len(self.pages))
 
-        for render, kwargs in DECORATED_ROUTES:
+        # TODO: include all work done in progress indicator, not just self.pages
+        for render, kwargs in DECORATED_PAGES:
             self.add_page(render, **kwargs)
 
         # Get the env mode.
         config = get_config()
 
-        # Empty the .web pages directory
-        compiler.purge_web_pages_dir()
-
         # Store the compile results.
         compile_results = []
 
         # Compile the pages in parallel.
         custom_components = set()
+        # TODO Anecdotally, processes=2 works 10% faster (cpu_count=12)
         thread_pool = ThreadPool()
         with progress:
             for route, component in self.pages.items():
+                # TODO: this progress does not reflect actual threaded task completion
                 progress.advance(task)
                 component.add_style(self.style)
                 compile_results.append(
                     thread_pool.apply_async(
                         compiler.compile_page,
                         args=(
                             route,
@@ -501,14 +505,16 @@
                 custom_components |= component.get_custom_components()
         thread_pool.close()
         thread_pool.join()
 
         # Get the results.
         compile_results = [result.get() for result in compile_results]
 
+        # TODO the compile tasks below may also benefit from parallelization too
+
         # Compile the custom components.
         compile_results.append(compiler.compile_components(custom_components))
 
         # Compile the root document with base styles and fonts.
         compile_results.append(compiler.compile_document_root(self.stylesheets))
 
         # Compile the theme.
@@ -517,18 +523,20 @@
         # Compile the Tailwind config.
         if config.tailwind is not None:
             config.tailwind["content"] = config.tailwind.get(
                 "content", constants.TAILWIND_CONTENT
             )
             compile_results.append(compiler.compile_tailwind(config.tailwind))
 
+        # Empty the .web pages directory
+        compiler.purge_web_pages_dir()
+
         # Write the pages at the end to trigger the NextJS hot reload only once.
         thread_pool = ThreadPool()
         for output_path, code in compile_results:
-            compiler_utils.write_page(output_path, code)
             thread_pool.apply_async(compiler_utils.write_page, args=(output_path, code))
         thread_pool.close()
         thread_pool.join()
 
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
```

### Comparing `reflex-0.2.3a7/reflex/base.py` & `reflex-0.2.3a8/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/compiler/compiler.py` & `reflex-0.2.3a8/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/compiler/templates.py` & `reflex-0.2.3a8/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/compiler/utils.py` & `reflex-0.2.3a8/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/__init__.py` & `reflex-0.2.3a8/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/base/bare.py` & `reflex-0.2.3a8/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/base/document.py` & `reflex-0.2.3a8/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/base/link.py` & `reflex-0.2.3a8/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/base/meta.py` & `reflex-0.2.3a8/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/base/script.py` & `reflex-0.2.3a8/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/component.py` & `reflex-0.2.3a8/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/code.py` & `reflex-0.2.3a8/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/datatable.py` & `reflex-0.2.3a8/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/divider.py` & `reflex-0.2.3a8/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/list.py` & `reflex-0.2.3a8/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/stat.py` & `reflex-0.2.3a8/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/table.py` & `reflex-0.2.3a8/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/datadisplay/tag.py` & `reflex-0.2.3a8/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/disclosure/accordion.py` & `reflex-0.2.3a8/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/disclosure/tabs.py` & `reflex-0.2.3a8/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/disclosure/transition.py` & `reflex-0.2.3a8/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/feedback/alert.py` & `reflex-0.2.3a8/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/feedback/circularprogress.py` & `reflex-0.2.3a8/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/feedback/progress.py` & `reflex-0.2.3a8/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/feedback/skeleton.py` & `reflex-0.2.3a8/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/feedback/spinner.py` & `reflex-0.2.3a8/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/__init__.py` & `reflex-0.2.3a8/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/button.py` & `reflex-0.2.3a8/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/checkbox.py` & `reflex-0.2.3a8/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.3a8/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.3a8/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/debounce.py` & `reflex-0.2.3a8/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/editable.py` & `reflex-0.2.3a8/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/form.py` & `reflex-0.2.3a8/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/iconbutton.py` & `reflex-0.2.3a8/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/input.py` & `reflex-0.2.3a8/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/multiselect.py` & `reflex-0.2.3a8/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/numberinput.py` & `reflex-0.2.3a8/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/pininput.py` & `reflex-0.2.3a8/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/radio.py` & `reflex-0.2.3a8/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/rangeslider.py` & `reflex-0.2.3a8/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/select.py` & `reflex-0.2.3a8/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/slider.py` & `reflex-0.2.3a8/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/switch.py` & `reflex-0.2.3a8/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/textarea.py` & `reflex-0.2.3a8/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/forms/upload.py` & `reflex-0.2.3a8/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/graphing/plotly.py` & `reflex-0.2.3a8/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/graphing/victory.py` & `reflex-0.2.3a8/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/__init__.py` & `reflex-0.2.3a8/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/box.py` & `reflex-0.2.3a8/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/card.py` & `reflex-0.2.3a8/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/cond.py` & `reflex-0.2.3a8/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/flex.py` & `reflex-0.2.3a8/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/foreach.py` & `reflex-0.2.3a8/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/grid.py` & `reflex-0.2.3a8/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/html.py` & `reflex-0.2.3a8/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/responsive.py` & `reflex-0.2.3a8/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/stack.py` & `reflex-0.2.3a8/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/layout/wrap.py` & `reflex-0.2.3a8/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/libs/react_player.py` & `reflex-0.2.3a8/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/media/avatar.py` & `reflex-0.2.3a8/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/media/icon.py` & `reflex-0.2.3a8/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/media/image.py` & `reflex-0.2.3a8/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.3a8/reflex/components/navigation/breadcrumb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Breadcrumb components."""
 
 from reflex.components.component import Component
+from reflex.components.layout.foreach import Foreach
 from reflex.components.libs.chakra import ChakraComponent
+from reflex.components.navigation.link import Link
 from reflex.vars import Var
 
 
 class Breadcrumb(ChakraComponent):
     """The parent container for breadcrumbs."""
 
     tag = "Breadcrumb"
@@ -27,19 +29,26 @@
             items (list): The items of the breadcrumb: (label, link)
             props: The properties of the component.
 
         Returns:
             The breadcrumb component.
         """
         if len(children) == 0:
-            children = []
-            for label, link in items or []:
-                children.append(
-                    BreadcrumbItem.create(BreadcrumbLink.create(label, href=link))
-                )
+            if isinstance(items, Var):
+                children = [
+                    Foreach.create(
+                        items,
+                        lambda item: BreadcrumbItem.create(label=item[0], href=item[1]),
+                    ),
+                ]
+
+            else:
+                children = []
+                for label, link in items or []:
+                    children.append(BreadcrumbItem.create(label=label, href=link))
         return super().create(*children, **props)
 
 
 class BreadcrumbItem(ChakraComponent):
     """Individual breadcrumb element containing a link and a divider."""
 
     tag = "BreadcrumbItem"
@@ -52,24 +61,38 @@
 
     # The visual separator between each breadcrumb item
     separator: Var[str]
 
     # The left and right margin applied to the separator
     spacing: Var[str]
 
-    # The href of the item.
-    href: Var[str]
+    @classmethod
+    def create(cls, *children, label=None, href=None, **props):
+        """Create a Breadcrumb Item component.
+
+        Args:
+            children: The children of the component.
+            label: The label used in the link. Defaults to None.
+            href: The URL of the link. Defaults to None.
+            props: The properties of the component.
+
+        Returns:
+            The BreadcrumbItem component
+        """
+        if len(children) == 0:
+            children = [BreadcrumbLink.create(label or "", href=href or "")]  # type: ignore
+        return super().create(*children, **props)
 
 
 class BreadcrumbSeparator(ChakraComponent):
     """The visual separator between each breadcrumb."""
 
     tag = "BreadcrumbSeparator"
 
 
-class BreadcrumbLink(ChakraComponent):
+class BreadcrumbLink(Link):
     """The breadcrumb link."""
 
     tag = "BreadcrumbLink"
 
     # Is the current page of the breadcrumb.
     is_current_page: Var[bool]
```

### Comparing `reflex-0.2.3a7/reflex/components/navigation/link.py` & `reflex-0.2.3a8/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.3a8/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/navigation/stepper.py` & `reflex-0.2.3a8/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/__init__.py` & `reflex-0.2.3a8/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/alertdialog.py` & `reflex-0.2.3a8/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/banner.py` & `reflex-0.2.3a8/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/drawer.py` & `reflex-0.2.3a8/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/menu.py` & `reflex-0.2.3a8/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/modal.py` & `reflex-0.2.3a8/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/popover.py` & `reflex-0.2.3a8/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/overlay/tooltip.py` & `reflex-0.2.3a8/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/tags/iter_tag.py` & `reflex-0.2.3a8/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/tags/tag.py` & `reflex-0.2.3a8/reflex/components/tags/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,54 +63,56 @@
 
         Returns:
             The formatted prop to display within a tag.
 
         Raises:
             TypeError: If the prop is not a valid type.
         """
-        # Handle var props.
-        if isinstance(prop, Var):
-            if not prop.is_local or prop.is_string:
-                return str(prop)
-            if types._issubclass(prop.type_, str):
-                return format.json_dumps(prop.full_name)
-            prop = prop.full_name
-
-        # Handle event props.
-        elif isinstance(prop, EventChain):
-            if prop.full_control:
-                # Full control component events.
-                event = format.format_full_control_event(prop)
+        try:
+            # Handle var props.
+            if isinstance(prop, Var):
+                if not prop.is_local or prop.is_string:
+                    return str(prop)
+                if types._issubclass(prop.type_, str):
+                    return format.json_dumps(prop.full_name)
+                prop = prop.full_name
+
+            # Handle event props.
+            elif isinstance(prop, EventChain):
+                if prop.full_control:
+                    # Full control component events.
+                    event = format.format_full_control_event(prop)
+                else:
+                    # All other events.
+                    chain = ",".join(
+                        [format.format_event(event) for event in prop.events]
+                    )
+                    event = f"Event([{chain}], {EVENT_ARG})"
+                prop = f"{EVENT_ARG} => {event}"
+
+            # Handle other types.
+            elif isinstance(prop, str):
+                if format.is_wrapped(prop, "{"):
+                    return prop
+                return format.json_dumps(prop)
+
+            elif isinstance(prop, Figure):
+                prop = json.loads(to_json(prop))["data"]  # type: ignore
+
+            # For dictionaries, convert any properties to strings.
+            elif isinstance(prop, dict):
+                prop = format.format_dict(prop)
+
             else:
-                # All other events.
-                chain = ",".join([format.format_event(event) for event in prop.events])
-                event = f"Event([{chain}], {EVENT_ARG})"
-            prop = f"{EVENT_ARG} => {event}"
-
-        # Handle other types.
-        elif isinstance(prop, str):
-            if format.is_wrapped(prop, "{"):
-                return prop
-            return format.json_dumps(prop)
-
-        elif isinstance(prop, Figure):
-            prop = json.loads(to_json(prop))["data"]  # type: ignore
-
-        # For dictionaries, convert any properties to strings.
-        elif isinstance(prop, dict):
-            prop = format.format_dict(prop)
-
-        else:
-            # Dump the prop as JSON.
-            try:
+                # Dump the prop as JSON.
                 prop = format.json_dumps(prop)
-            except TypeError as e:
-                raise TypeError(
-                    f"Could not format prop: {prop} of type {type(prop)}"
-                ) from e
+        except TypeError as e:
+            raise TypeError(
+                f"Could not format prop: {prop} of type {type(prop)}"
+            ) from e
 
         # Wrap the variable in braces.
         assert isinstance(prop, str), "The prop must be a string."
         return format.wrap(prop, "{", check_first=False)
 
     def format_props(self) -> List:
         """Format the tag's props.
```

### Comparing `reflex-0.2.3a7/reflex/components/tags/tagless.py` & `reflex-0.2.3a8/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/components/typography/highlight.py` & `reflex-0.2.3a8/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/config.py` & `reflex-0.2.3a8/reflex/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,20 +161,14 @@
 
     # The rxdeploy url.
     rxdeploy_url: Optional[str] = None
 
     # The environment mode.
     env: constants.Env = constants.Env.DEV
 
-    # The path to the bun executable.
-    bun_path: str = constants.BUN_PATH
-
-    # Disable bun.
-    disable_bun: bool = False
-
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
     # The Admin Dash.
     admin_dash: Optional[AdminDash] = None
 
     # Backend transport methods.
```

### Comparing `reflex-0.2.3a7/reflex/constants.py` & `reflex-0.2.3a8/reflex/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Constants used throughout the package."""
+from __future__ import annotations
 
 import os
+import platform
 import re
 from enum import Enum
 from types import SimpleNamespace
 from typing import Any, Type
 
 # importlib is only available for Python 3.8+ so we need the backport for Python 3.7
 try:
@@ -39,35 +41,67 @@
 
 
 # App names and versions.
 # The name of the Reflex package.
 MODULE_NAME = "reflex"
 # The current version of Reflex.
 VERSION = metadata.version(MODULE_NAME)
-# Minimum version of Node.js required to run Reflex.
-MIN_NODE_VERSION = "16.8.0"
-
-# Valid bun versions.
-MIN_BUN_VERSION = "0.5.9"
-MAX_BUN_VERSION = "0.6.9"
 
 # Files and directories used to init a new project.
+# The directory to store reflex dependencies.
+REFLEX_DIR = os.path.expandvars(os.path.join("$HOME", f".{MODULE_NAME}"))
 # The root directory of the reflex library.
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # The name of the assets directory.
 APP_ASSETS_DIR = "assets"
 # The template directory used during reflex init.
 TEMPLATE_DIR = os.path.join(ROOT_DIR, MODULE_NAME, ".templates")
 # The web subdirectory of the template directory.
 WEB_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "web")
 # The assets subdirectory of the template directory.
 ASSETS_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, APP_ASSETS_DIR)
 # The jinja template directory.
 JINJA_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "jinja")
 
+# Bun config.
+# The Bun version.
+BUN_VERSION = "0.7.0"
+# The directory to store the bun.
+BUN_ROOT_PATH = os.path.join(REFLEX_DIR, ".bun")
+# The bun path.
+BUN_PATH = os.path.join(BUN_ROOT_PATH, "bin", "bun")
+# URL to bun install script.
+BUN_INSTALL_URL = "https://bun.sh/install"
+
+# NVM / Node config.
+# The NVM version.
+NVM_VERSION = "0.39.1"
+# The Node version.
+NODE_VERSION = "18.17.0"
+# The minimum required node version.
+NODE_VERSION_MIN = "16.8.0"
+# The directory to store nvm.
+NVM_DIR = os.path.join(REFLEX_DIR, ".nvm")
+# The nvm path.
+NVM_PATH = os.path.join(NVM_DIR, "nvm.sh")
+# The node bin path.
+NODE_BIN_PATH = os.path.join(NVM_DIR, "versions", "node", f"v{NODE_VERSION}", "bin")
+# The default path where node is installed.
+NODE_PATH = (
+    "node" if platform.system() == "Windows" else os.path.join(NODE_BIN_PATH, "node")
+)
+# The default path where npm is installed.
+NPM_PATH = (
+    "npm" if platform.system() == "Windows" else os.path.join(NODE_BIN_PATH, "npm")
+)
+# The URL to the nvm install script.
+NVM_INSTALL_URL = (
+    f"https://raw.githubusercontent.com/nvm-sh/nvm/v{NVM_VERSION}/install.sh"
+)
+
 # The frontend directories in a project.
 # The web folder where the NextJS app is compiled to.
 WEB_DIR = ".web"
 # The name of the utils file.
 UTILS_DIR = "utils"
 # The name of the output static directory.
 STATIC_DIR = "_static"
@@ -106,20 +140,14 @@
 FRONTEND_PORT = get_value("FRONTEND_PORT", "3000")
 # The backend default port.
 BACKEND_PORT = get_value("BACKEND_PORT", "8000")
 # The backend api url.
 API_URL = get_value("API_URL", "http://localhost:8000")
 # The deploy url
 DEPLOY_URL = get_value("DEPLOY_URL")
-# bun root location
-BUN_ROOT_PATH = "$HOME/.bun"
-# The default path where bun is installed.
-BUN_PATH = get_value("BUN_PATH", f"{BUN_ROOT_PATH}/bin/bun")
-# Command to install bun.
-INSTALL_BUN = f"curl -fsSL https://bun.sh/install | bash -s -- bun-v{MAX_BUN_VERSION}"
 # Default host in dev mode.
 BACKEND_HOST = get_value("BACKEND_HOST", "0.0.0.0")
 # The default timeout when launching the gunicorn server.
 TIMEOUT = get_value("TIMEOUT", 120, type_=int)
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
@@ -200,14 +228,15 @@
 # The event namespace for websocket
 EVENT_NAMESPACE = get_value("EVENT_NAMESPACE")
 
 # Testing variables.
 # Testing os env set by pytest when running a test case.
 PYTEST_CURRENT_TEST = "PYTEST_CURRENT_TEST"
 
+
 # Env modes
 class Env(str, Enum):
     """The environment modes."""
 
     DEV = "dev"
     PROD = "prod"
 
@@ -217,14 +246,27 @@
     """The log levels."""
 
     DEBUG = "debug"
     INFO = "info"
     WARNING = "warning"
     ERROR = "error"
     CRITICAL = "critical"
+    QUIET = "quiet"
+
+    def __le__(self, other: LogLevel) -> bool:
+        """Compare log levels.
+
+        Args:
+            other: The other log level.
+
+        Returns:
+            True if the log level is less than or equal to the other log level.
+        """
+        levels = list(LogLevel)
+        return levels.index(self) <= levels.index(other)
 
 
 # Templates
 class Template(str, Enum):
     """The templates to use for the app."""
 
     DEFAULT = "default"
@@ -328,14 +370,15 @@
 class RouteVar(SimpleNamespace):
     """Names of variables used in the router_data dict stored in State."""
 
     CLIENT_IP = "ip"
     CLIENT_TOKEN = "token"
     HEADERS = "headers"
     PATH = "pathname"
+    ORIGIN = "asPath"
     SESSION_ID = "sid"
     QUERY = "query"
     COOKIE = "cookie"
 
 
 class RouteRegex(SimpleNamespace):
     """Regex used for extracting route args in route."""
```

### Comparing `reflex-0.2.3a7/reflex/el/constants/html.py` & `reflex-0.2.3a8/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/el/constants/react.py` & `reflex-0.2.3a8/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/el/constants/reflex.py` & `reflex-0.2.3a8/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/el/element.py` & `reflex-0.2.3a8/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/el/elements/__init__.py` & `reflex-0.2.3a8/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/el/precompile.py` & `reflex-0.2.3a8/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/event.py` & `reflex-0.2.3a8/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.3a8/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/middleware/middleware.py` & `reflex-0.2.3a8/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/model.py` & `reflex-0.2.3a8/reflex/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         ValueError: If the database url is None.
     """
     conf = get_config()
     url = url or conf.db_url
     if url is None:
         raise ValueError("No database url configured")
     if not Path(constants.ALEMBIC_CONFIG).exists():
-        console.print(
-            "[red]Database is not initialized, run [bold]reflex db init[/bold] first."
+        console.warn(
+            "Database is not initialized, run [bold]reflex db init[/bold] first."
         )
     echo_db_query = False
     if conf.env == constants.Env.DEV and constants.SQLALCHEMY_ECHO:
         echo_db_query = True
     return sqlmodel.create_engine(
         url,
         echo=echo_db_query,
```

### Comparing `reflex-0.2.3a7/reflex/reflex.py` & `reflex-0.2.3a8/reflex/reflex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,145 @@
 """Reflex CLI to create, run, and deploy apps."""
 
 import os
-import platform
 import signal
 import threading
 from pathlib import Path
 
 import httpx
 import typer
 from alembic.util.exc import CommandError
 
 from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import build, console, exec, prerequisites, processes, telemetry
 
 # Create the app.
-cli = typer.Typer()
+cli = typer.Typer(add_completion=False)
 
 
-@cli.command()
-def version():
-    """Get the Reflex version."""
-    console.print(constants.VERSION)
+def version(value: bool):
+    """Get the Reflex version.
+
+    Args:
+        value: Whether the version flag was passed.
+
+    Raises:
+        typer.Exit: If the version flag was passed.
+    """
+    if value:
+        console.print(constants.VERSION)
+        raise typer.Exit()
+
+
+@cli.callback()
+def main(
+    version: bool = typer.Option(
+        None,
+        "-v",
+        "--version",
+        callback=version,
+        help="Get the Reflex version.",
+        is_eager=True,
+    ),
+):
+    """Reflex CLI to create, run, and deploy apps."""
+    pass
 
 
 @cli.command()
 def init(
     name: str = typer.Option(None, help="Name of the app to be initialized."),
     template: constants.Template = typer.Option(
         constants.Template.DEFAULT, help="Template to use for the app."
     ),
+    loglevel: constants.LogLevel = typer.Option(
+        constants.LogLevel.INFO, help="The log level to use."
+    ),
 ):
     """Initialize a new Reflex app in the current directory."""
-    app_name = prerequisites.get_default_app_name() if name is None else name
-
-    # Make sure they don't name the app "reflex".
-    if app_name == constants.MODULE_NAME:
-        console.print(
-            f"[red]The app directory cannot be named [bold]{constants.MODULE_NAME}."
-        )
-        raise typer.Exit()
+    # Set the log level.
+    console.set_log_level(loglevel)
 
+    # Get the app name.
+    app_name = prerequisites.get_default_app_name() if name is None else name
     console.rule(f"[bold]Initializing {app_name}")
-    # Set up the web directory.
-    prerequisites.validate_and_install_bun()
-    prerequisites.initialize_web_directory()
+
+    # Set up the web project.
+    prerequisites.initialize_frontend_dependencies()
 
     # Migrate Pynecone projects to Reflex.
     prerequisites.migrate_to_reflex()
 
     # Set up the app directory, only if the config doesn't exist.
+    config = get_config()
     if not os.path.exists(constants.CONFIG_FILE):
         prerequisites.create_config(app_name)
         prerequisites.initialize_app_directory(app_name, template)
         build.set_reflex_project_hash()
-        telemetry.send("init", get_config().telemetry_enabled)
+        telemetry.send("init", config.telemetry_enabled)
     else:
-        build.set_reflex_project_hash()
-        telemetry.send("reinit", get_config().telemetry_enabled)
+        telemetry.send("reinit", config.telemetry_enabled)
 
     # Initialize the .gitignore.
     prerequisites.initialize_gitignore()
+
     # Finish initializing the app.
-    console.log(f"[bold green]Finished Initializing: {app_name}")
+    console.success(f"Finished Initializing: {app_name}")
 
 
 @cli.command()
 def run(
     env: constants.Env = typer.Option(
         get_config().env, help="The environment to run the app in."
     ),
     frontend: bool = typer.Option(
         False, "--frontend-only", help="Execute only frontend."
     ),
     backend: bool = typer.Option(False, "--backend-only", help="Execute only backend."),
-    loglevel: constants.LogLevel = typer.Option(
-        constants.LogLevel.ERROR, help="The log level to use."
-    ),
     frontend_port: str = typer.Option(None, help="Specify a different frontend port."),
     backend_port: str = typer.Option(None, help="Specify a different backend port."),
     backend_host: str = typer.Option(None, help="Specify the backend host."),
+    loglevel: constants.LogLevel = typer.Option(
+        constants.LogLevel.INFO, help="The log level to use."
+    ),
 ):
     """Run the app in the current directory."""
-    if platform.system() == "Windows":
-        console.print(
-            "[yellow][WARNING] We strongly advise you to use Windows Subsystem for Linux (WSL) for optimal performance when using Reflex. Due to compatibility issues with one of our dependencies, Bun, you may experience slower performance on Windows. By using WSL, you can expect to see a significant speed increase."
-        )
+    # Set the log level.
+    console.set_log_level(loglevel)
+
+    # Check that the app is initialized.
+    prerequisites.check_initialized(frontend=frontend)
+
     # Set ports as os env variables to take precedence over config and
     # .env variables(if override_os_envs flag in config is set to False).
     build.set_os_env(
         frontend_port=frontend_port,
         backend_port=backend_port,
         backend_host=backend_host,
     )
 
-    frontend_port = (
-        get_config().frontend_port if frontend_port is None else frontend_port
-    )
-    backend_port = get_config().backend_port if backend_port is None else backend_port
-    backend_host = get_config().backend_host if backend_host is None else backend_host
+    # Get the ports from the config.
+    config = get_config()
+    frontend_port = config.frontend_port if frontend_port is None else frontend_port
+    backend_port = config.backend_port if backend_port is None else backend_port
+    backend_host = config.backend_host if backend_host is None else backend_host
 
     # If no --frontend-only and no --backend-only, then turn on frontend and backend both
     if not frontend and not backend:
         frontend = True
         backend = True
 
     # If something is running on the ports, ask the user if they want to kill or change it.
     if frontend and processes.is_process_on_port(frontend_port):
         frontend_port = processes.change_or_terminate_port(frontend_port, "frontend")
 
     if backend and processes.is_process_on_port(backend_port):
         backend_port = processes.change_or_terminate_port(backend_port, "backend")
 
-    # Check that the app is initialized.
-    if frontend and not prerequisites.is_initialized():
-        console.print(
-            "[red]The app is not initialized. Run [bold]reflex init[/bold] first."
-        )
-        raise typer.Exit()
-
-    # Check that the template is up to date.
-    if frontend and not prerequisites.is_latest_template():
-        console.print(
-            "[red]The base app template has updated. Run [bold]reflex init[/bold] again."
-        )
-        raise typer.Exit()
-
     # Get the app module.
     console.rule("[bold]Starting Reflex App")
     app = prerequisites.get_app()
 
     # Check the admin dashboard settings.
     prerequisites.check_admin_settings()
 
@@ -149,47 +159,44 @@
             build.setup_frontend_prod,
             exec.run_frontend_prod,
             exec.run_backend_prod,
         )
     assert setup_frontend and frontend_cmd and backend_cmd, "Invalid env"
 
     # Post a telemetry event.
-    telemetry.send(f"run-{env.value}", get_config().telemetry_enabled)
+    telemetry.send(f"run-{env.value}", config.telemetry_enabled)
 
     # Run the frontend and backend.
     if frontend:
-        setup_frontend(Path.cwd(), loglevel)
-        threading.Thread(
-            target=frontend_cmd, args=(Path.cwd(), frontend_port, loglevel)
-        ).start()
+        setup_frontend(Path.cwd())
+        threading.Thread(target=frontend_cmd, args=(Path.cwd(), frontend_port)).start()
     if backend:
         threading.Thread(
             target=backend_cmd,
-            args=(app.__name__, backend_host, backend_port, loglevel),
+            args=(app.__name__, backend_host, backend_port),
         ).start()
 
     # Display custom message when there is a keyboard interrupt.
     signal.signal(signal.SIGINT, processes.catch_keyboard_interrupt)
 
 
 @cli.command()
 def deploy(dry_run: bool = typer.Option(False, help="Whether to run a dry run.")):
     """Deploy the app to the Reflex hosting service."""
     # Get the app config.
     config = get_config()
-    config.api_url = prerequisites.get_production_backend_url()
 
     # Check if the deploy url is set.
     if config.rxdeploy_url is None:
         typer.echo("This feature is coming soon!")
         return
 
     # Compile the app in production mode.
     typer.echo("Compiling production app")
-    export(for_reflex_deploy=True)
+    export()
 
     # Exit early if this is a dry run.
     if dry_run:
         return
 
     # Deploy the app.
     data = {"userId": config.username, "projectId": config.app_name}
@@ -213,74 +220,80 @@
     ),
     frontend: bool = typer.Option(
         True, "--backend-only", help="Export only backend.", show_default=False
     ),
     backend: bool = typer.Option(
         True, "--frontend-only", help="Export only frontend.", show_default=False
     ),
-    for_reflex_deploy: bool = typer.Option(
-        False,
-        "--for-reflex-deploy",
-        help="Whether export the app for Reflex Deploy Service.",
+    loglevel: constants.LogLevel = typer.Option(
+        constants.LogLevel.INFO, help="The log level to use."
     ),
 ):
     """Export the app to a zip file."""
-    config = get_config()
+    # Set the log level.
+    console.set_log_level(loglevel)
 
-    if for_reflex_deploy:
-        # Get the app config and modify the api_url base on username and app_name.
-        config.api_url = prerequisites.get_production_backend_url()
+    # Check that the app is initialized.
+    prerequisites.check_initialized(frontend=frontend)
 
     # Compile the app in production mode and export it.
     console.rule("[bold]Compiling production app and preparing for export.")
 
     if frontend:
-        # ensure module can be imported and app.compile() is called
+        # Ensure module can be imported and app.compile() is called.
         prerequisites.get_app()
-        # set up .web directory and install frontend dependencies
+        # Set up .web directory and install frontend dependencies.
         build.setup_frontend(Path.cwd())
 
-    build.export_app(
+    # Export the app.
+    config = get_config()
+    build.export(
         backend=backend,
         frontend=frontend,
         zip=zipping,
         deploy_url=config.deploy_url,
     )
 
     # Post a telemetry event.
-    telemetry.send("export", get_config().telemetry_enabled)
+    telemetry.send("export", config.telemetry_enabled)
 
     if zipping:
-        console.rule(
+        console.log(
             """Backend & Frontend compiled. See [green bold]backend.zip[/green bold]
             and [green bold]frontend.zip[/green bold]."""
         )
     else:
-        console.rule(
+        console.log(
             """Backend & Frontend compiled. See [green bold]app[/green bold]
             and [green bold].web/_static[/green bold] directories."""
         )
 
 
 db_cli = typer.Typer()
 
 
 @db_cli.command(name="init")
 def db_init():
     """Create database schema and migration configuration."""
+    # Check the database url.
     if get_config().db_url is None:
-        console.print("[red]db_url is not configured, cannot initialize.")
+        console.error("db_url is not configured, cannot initialize.")
+        return
+
+    # Check the alembic config.
     if Path(constants.ALEMBIC_CONFIG).exists():
-        console.print(
-            "[red]Database is already initialized. Use "
+        console.error(
+            "Database is already initialized. Use "
             "[bold]reflex db makemigrations[/bold] to create schema change "
             "scripts and [bold]reflex db migrate[/bold] to apply migrations "
             "to a new or existing database.",
         )
         return
+
+    # Initialize the database.
     prerequisites.get_app()
     model.Model.alembic_init()
     model.Model.migrate(autogenerate=True)
 
 
 @db_cli.command()
 def migrate():
@@ -304,17 +317,16 @@
         return
     with model.Model.get_db_engine().connect() as connection:
         try:
             model.Model.alembic_autogenerate(connection=connection, message=message)
         except CommandError as command_error:
             if "Target database is not up to date." not in str(command_error):
                 raise
-            console.print(
-                f"[red]{command_error} Run [bold]reflex db migrate[/bold] to update database."
+            console.error(
+                f"{command_error} Run [bold]reflex db migrate[/bold] to update database."
             )
 
 
-cli.add_typer(db_cli, name="db", help="Subcommands for managing the database schema")
-main = cli
+cli.add_typer(db_cli, name="db", help="Subcommands for managing the database schema.")
 
 if __name__ == "__main__":
-    main()
+    cli()
```

### Comparing `reflex-0.2.3a7/reflex/route.py` & `reflex-0.2.3a8/reflex/route.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 
 import re
 from typing import Dict, List, Optional, Union
 
 from reflex import constants
 from reflex.event import EventHandler
-
-DECORATED_ROUTES = []
+from reflex.page import page
+from reflex.utils.console import deprecate
 
 
 def route(
     route: Optional[str] = None,
     title: Optional[str] = None,
     image: Optional[str] = None,
     description: Optional[str] = None,
@@ -33,33 +33,23 @@
         image: The favicon of the page.
         description: The description of the page
         on_load: The event handler(s) called when the page load.
 
     Returns:
         The decorated function.
     """
+    deprecate("@rx.route is deprecated and is being replaced by @rx.page instead")
 
-    def decorator(render_fn):
-        kwargs = {}
-        if route:
-            kwargs["route"] = route
-        if title:
-            kwargs["title"] = title
-        if image:
-            kwargs["image"] = image
-        if description:
-            kwargs["description"] = description
-        if on_load:
-            kwargs["on_load"] = on_load
-
-        DECORATED_ROUTES.append((render_fn, kwargs))
-
-        return render_fn
-
-    return decorator
+    return page(
+        route=route,
+        title=title,
+        image=image,
+        description=description,
+        on_load=on_load,
+    )
 
 
 def verify_route_validity(route: str) -> None:
     """Verify if the route is valid, and throw an error if not.
 
     Args:
         route: The route that need to be checked
```

### Comparing `reflex-0.2.3a7/reflex/state.py` & `reflex-0.2.3a8/reflex/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,21 +472,27 @@
         """Return the IP of the client associated with this state.
 
         Returns:
             The IP of the client.
         """
         return self.router_data.get(constants.RouteVar.CLIENT_IP, "")
 
-    def get_current_page(self) -> str:
+    def get_current_page(self, origin=False) -> str:
         """Obtain the path of current page from the router data.
 
+        Args:
+            origin: whether to return the base route as shown in browser
+
         Returns:
             The current page.
         """
-        return self.router_data.get(constants.RouteVar.PATH, "")
+        if origin:
+            return self.router_data.get(constants.RouteVar.ORIGIN, "")
+        else:
+            return self.router_data.get(constants.RouteVar.PATH, "")
 
     def get_query_params(self) -> Dict[str, str]:
         """Obtain the query parameters for the queried page.
 
         The query object contains both the URI parameters and the GET parameters.
 
         Returns:
```

### Comparing `reflex-0.2.3a7/reflex/style.py` & `reflex-0.2.3a8/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/testing.py` & `reflex-0.2.3a8/reflex/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 TimeoutType = Optional[Union[int, float]]
 
 if platform.system == "Windows":
     FRONTEND_POPEN_ARGS["creationflags"] = subprocess.CREATE_NEW_PROCESS_GROUP  # type: ignore
 else:
     FRONTEND_POPEN_ARGS["start_new_session"] = True
 
+
 # borrowed from py3.11
 class chdir(contextlib.AbstractContextManager):
     """Non thread-safe context manager to change the current working directory."""
 
     def __init__(self, path):
         """Prepare contextmanager.
 
@@ -146,14 +147,15 @@
             source_code = textwrap.dedent(
                 "".join(inspect.getsource(self.app_source).splitlines(True)[1:]),
             )
             with chdir(self.app_path):
                 reflex.reflex.init(
                     name=self.app_name,
                     template=reflex.constants.Template.DEFAULT,
+                    loglevel=reflex.constants.LogLevel.INFO,
                 )
                 self.app_module_path.write_text(source_code)
         with chdir(self.app_path):
             self.app_module = reflex.utils.prerequisites.get_app()
         self.app_instance = self.app_module.app
 
     def _start_backend(self):
@@ -175,15 +177,15 @@
             config.api_url = "http://{0}:{1}".format(
                 *self._poll_for_servers().getsockname(),
             )
             reflex.utils.build.setup_frontend(self.app_path)
         frontend_env = os.environ.copy()
         frontend_env["PORT"] = "0"
         self.frontend_process = subprocess.Popen(
-            [reflex.utils.prerequisites.get_package_manager(), "run", "dev"],
+            [reflex.utils.prerequisites.get_install_package_manager(), "run", "dev"],
             stdout=subprocess.PIPE,
             encoding="utf-8",
             cwd=self.app_path / reflex.constants.WEB_DIR,
             env=frontend_env,
             **FRONTEND_POPEN_ARGS,
         )
```

### Comparing `reflex-0.2.3a7/reflex/utils/build.py` & `reflex-0.2.3a8/reflex/utils/build.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 import json
 import os
 import random
 import subprocess
 from pathlib import Path
 from typing import Optional, Union
 
-from rich.progress import MofNCompleteColumn, Progress, TimeElapsedColumn
-
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, path_ops, prerequisites
-from reflex.utils.processes import new_process
+from reflex.utils.processes import new_process, show_progress
 
 
 def update_json_file(file_path: str, update_dict: dict[str, Union[int, str]]):
     """Update the contents of a json file.
 
     Args:
         file_path: the path to the JSON file.
@@ -35,15 +33,17 @@
         json_object.update(update_dict)
     with open(fp, "w") as f:
         json.dump(json_object, f, ensure_ascii=False)
 
 
 def set_reflex_project_hash():
     """Write the hash of the Reflex project to a REFLEX_JSON."""
-    update_json_file(constants.REFLEX_JSON, {"project_hash": random.getrandbits(128)})
+    project_hash = random.getrandbits(128)
+    console.debug(f"Setting project hash to {project_hash}.")
+    update_json_file(constants.REFLEX_JSON, {"project_hash": project_hash})
 
 
 def set_environment_variables():
     """Write the upload url to a REFLEX_JSON."""
     update_json_file(
         constants.ENV_JSON,
         {
@@ -82,88 +82,55 @@
         }
     )
 
     with open(constants.SITEMAP_CONFIG_FILE, "w") as f:
         f.write(templates.SITEMAP_CONFIG(config=config))
 
 
-def export_app(
+def export(
     backend: bool = True,
     frontend: bool = True,
     zip: bool = False,
     deploy_url: Optional[str] = None,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
-    """Zip up the app for deployment.
+    """Export the app for deployment.
 
     Args:
         backend: Whether to zip up the backend app.
         frontend: Whether to zip up the frontend app.
         zip: Whether to zip the app.
         deploy_url: The URL of the deployed app.
-        loglevel: The log level to use.
     """
     # Remove the static folder.
     path_ops.rm(constants.WEB_STATIC_DIR)
 
     # Generate the sitemap file.
     command = "export"
     if deploy_url is not None:
         generate_sitemap_config(deploy_url)
         command = "export-sitemap"
 
-    # Create a progress object
-    progress = Progress(
-        *Progress.get_default_columns()[:-1],
-        MofNCompleteColumn(),
-        TimeElapsedColumn(),
-    )
-
     checkpoints = [
         "Linting and checking ",
         "Compiled successfully",
         "Route (pages)",
         "Collecting page data",
         "automatically rendered as static HTML",
         'Copying "static build" directory',
         'Copying "public" directory',
         "Finalizing page optimization",
         "Export successful",
     ]
 
-    # Add a single task to the progress object
-    task = progress.add_task("Creating Production Build: ", total=len(checkpoints))
-
     # Start the subprocess with the progress bar.
-    try:
-        with progress, new_process(
-            [prerequisites.get_package_manager(), "run", command],
-            cwd=constants.WEB_DIR,
-        ) as export_process:
-            assert export_process.stdout is not None, "No stdout for export process."
-            for line in export_process.stdout:
-                if loglevel == constants.LogLevel.DEBUG:
-                    print(line, end="")
-
-                # Check for special strings and update the progress bar.
-                for special_string in checkpoints:
-                    if special_string in line:
-                        if special_string == "Export successful":
-                            progress.update(task, completed=len(checkpoints))
-                            break  # Exit the loop if the completion message is found
-                        else:
-                            progress.update(task, advance=1)
-                            break
-
-    except Exception as e:
-        console.print(f"[red]Export process errored: {e}")
-        console.print(
-            "[red]Run in with [bold]--loglevel debug[/bold] to see the full error."
-        )
-        os._exit(1)
+    process = new_process(
+        [prerequisites.get_package_manager(), "run", command],
+        cwd=constants.WEB_DIR,
+    )
+    show_progress(process, "Creating Production Build", checkpoints)
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
@@ -199,40 +166,32 @@
     if backend:
         cmd = r"zip -r backend.zip ./* -x .web/\* ./assets\* ./frontend.zip\* ./backend.zip\*"
         os.system(cmd)
 
 
 def setup_frontend(
     root: Path,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
     disable_telemetry: bool = True,
 ):
-    """Set up the frontend.
+    """Set up the frontend to run the app.
 
     Args:
         root: The root path of the project.
-        loglevel: The log level to use.
         disable_telemetry: Whether to disable the Next telemetry.
     """
-    # Validate bun version.
-    prerequisites.validate_and_install_bun(initialize=False)
-
-    # Initialize the web directory if it doesn't exist.
-    web_dir = prerequisites.create_web_directory(root)
-
     # Install frontend packages.
-    prerequisites.install_frontend_packages(web_dir)
+    prerequisites.install_frontend_packages()
 
     # Copy asset files to public folder.
     path_ops.cp(
         src=str(root / constants.APP_ASSETS_DIR),
         dest=str(root / constants.WEB_ASSETS_DIR),
     )
 
-    # set the environment variables in client(env.json)
+    # Set the environment variables in client (env.json).
     set_environment_variables()
 
     # Disable the Next telemetry.
     if disable_telemetry:
         new_process(
             [
                 prerequisites.get_package_manager(),
@@ -244,19 +203,17 @@
             cwd=constants.WEB_DIR,
             stdout=subprocess.DEVNULL,
         )
 
 
 def setup_frontend_prod(
     root: Path,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
     disable_telemetry: bool = True,
 ):
     """Set up the frontend for prod mode.
 
     Args:
         root: The root path of the project.
-        loglevel: The log level to use.
         disable_telemetry: Whether to disable the Next telemetry.
     """
-    setup_frontend(root, loglevel, disable_telemetry)
-    export_app(loglevel=loglevel, deploy_url=get_config().deploy_url)
+    setup_frontend(root, disable_telemetry)
+    export(deploy_url=get_config().deploy_url)
```

### Comparing `reflex-0.2.3a7/reflex/utils/exec.py` & `reflex-0.2.3a8/reflex/utils/exec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Everything regarding execution of the built app."""
 
 from __future__ import annotations
 
 import os
 import platform
-import subprocess
 from pathlib import Path
 
-from rich import print
-
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites, processes
 from reflex.utils.processes import new_process
 from reflex.utils.watch import AssetFolderWatch
 
 
@@ -24,79 +21,69 @@
     """
     asset_watch = AssetFolderWatch(root)
     asset_watch.start()
 
 
 def run_process_and_launch_url(
     run_command: list[str],
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the process and launch the URL.
 
     Args:
         run_command: The command to run.
-        loglevel: The log level to use.
     """
     process = new_process(
         run_command,
         cwd=constants.WEB_DIR,
     )
 
     if process.stdout:
         for line in process.stdout:
             if "ready started server on" in line:
                 url = line.split("url: ")[-1].strip()
-                print(f"App running at: [bold green]{url}")
-            if loglevel == constants.LogLevel.DEBUG:
-                print(line, end="")
+                console.info(f"App running at: [bold green]{url}")
+            else:
+                console.debug(line)
 
 
 def run_frontend(
     root: Path,
     port: str,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the frontend.
 
     Args:
         root: The root path of the project.
         port: The port to run the frontend on.
-        loglevel: The log level to use.
     """
     # Start watching asset folder.
     start_watching_assets_folder(root)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().frontend_port if port is None else port
-    run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "dev"], loglevel
-    )
+    run_process_and_launch_url([prerequisites.get_package_manager(), "run", "dev"])
 
 
 def run_frontend_prod(
     root: Path,
     port: str,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the frontend.
 
     Args:
         root: The root path of the project (to keep same API as run_frontend).
         port: The port to run the frontend on.
-        loglevel: The log level to use.
     """
     # Set the port.
     os.environ["PORT"] = get_config().frontend_port if port is None else port
 
     # Run the frontend in production mode.
     console.rule("[bold green]App Running")
-    run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "prod"], loglevel
-    )
+    run_process_and_launch_url([constants.NPM_PATH, "run", "prod"])
 
 
 def run_backend(
     app_name: str,
     host: str,
     port: int,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
@@ -105,33 +92,31 @@
 
     Args:
         host: The app host
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
-    cmd = [
-        "uvicorn",
-        f"{app_name}:{constants.APP_VAR}.{constants.API_VAR}",
-        "--host",
-        host,
-        "--port",
-        str(port),
-        "--log-level",
-        loglevel,
-        "--reload",
-        "--reload-dir",
-        app_name.split(".")[0],
-    ]
-    process = subprocess.Popen(cmd)
-
-    try:
-        process.wait()
-    except KeyboardInterrupt:
-        process.terminate()
+    new_process(
+        [
+            "uvicorn",
+            f"{app_name}:{constants.APP_VAR}.{constants.API_VAR}",
+            "--host",
+            host,
+            "--port",
+            str(port),
+            "--log-level",
+            loglevel,
+            "--reload",
+            "--reload-dir",
+            app_name.split(".")[0],
+        ],
+        run=True,
+        show_logs=True,
+    )
 
 
 def run_backend_prod(
     app_name: str,
     host: str,
     port: int,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
@@ -167,8 +152,8 @@
 
     command += [
         "--log-level",
         loglevel.value,
         "--workers",
         str(num_workers),
     ]
-    subprocess.run(command)
+    new_process(command, run=True, show_logs=True)
```

### Comparing `reflex-0.2.3a7/reflex/utils/format.py` & `reflex-0.2.3a8/reflex/utils/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import base64
 import io
 import json
 import os
+import os.path as op
 import re
 import sys
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type
 
 import plotly.graph_objects as go
 from plotly.io import to_json
 
@@ -456,14 +457,32 @@
     fprop = re.sub('}"', "", fprop)
     fprop = re.sub('\\\\"', '"', fprop)
 
     # Return the formatted dict.
     return fprop
 
 
+def format_breadcrumbs(route: str) -> list[tuple[str, str]]:
+    """Take a route and return a list of tuple for use in breadcrumb.
+
+    Args:
+        route: The route to transform.
+
+    Returns:
+        list[tuple[str, str]]: the list of tuples for the breadcrumb.
+    """
+    route_parts = route.lstrip("/").split("/")
+
+    # create and return breadcrumbs
+    return [
+        (part, op.join("/", *route_parts[: i + 1]))
+        for i, part in enumerate(route_parts)
+    ]
+
+
 def json_dumps(obj: Any) -> str:
     """Takes an object and returns a jsonified string.
 
     Args:
         obj: The object to be serialized.
 
     Returns:
```

### Comparing `reflex-0.2.3a7/reflex/utils/imports.py` & `reflex-0.2.3a8/reflex/utils/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from reflex.vars import ImportVar
 
 ImportDict = Dict[str, Set[ImportVar]]
 
 
 def merge_imports(*imports) -> ImportDict:
-    """Merge two import dicts together.
+    """Merge multiple import dicts together.
 
     Args:
         *imports: The list of import dicts to merge.
 
     Returns:
         The merged import dicts.
     """
```

### Comparing `reflex-0.2.3a7/reflex/utils/path_ops.py` & `reflex-0.2.3a8/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/utils/prerequisites.py` & `reflex-0.2.3a8/reflex/utils/prerequisites.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,101 +3,116 @@
 from __future__ import annotations
 
 import glob
 import json
 import os
 import platform
 import re
-import subprocess
 import sys
-from datetime import datetime
+import tempfile
+import threading
 from fileinput import FileInput
 from pathlib import Path
 from types import ModuleType
 from typing import Optional
 
+import httpx
 import typer
 from alembic.util.exc import CommandError
 from packaging import version
 from redis import Redis
 
 from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import console, path_ops
+from reflex.utils.processes import new_process, show_logs
 
+IS_WINDOWS = platform.system() == "Windows"
 
-def check_node_version(min_version=constants.MIN_NODE_VERSION):
-    """Check the version of Node.js.
 
-    Args:
-        min_version: The minimum version of Node.js required.
+def check_node_version() -> bool:
+    """Check the version of Node.js.
 
     Returns:
-        Whether the version of Node.js is high enough.
+        Whether the version of Node.js is valid.
     """
     try:
-        # Run the node -v command and capture the output
-        result = subprocess.run(
-            ["node", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
-        )
-        # The output will be in the form "vX.Y.Z", but version.parse() can handle it
-        current_version = version.parse(result.stdout.decode())
-        # Compare the version numbers
-        return current_version >= version.parse(min_version)
-    except Exception:
+        # Run the node -v command and capture the output.
+        result = new_process([constants.NODE_PATH, "-v"], run=True)
+    except FileNotFoundError:
         return False
 
+    # The output will be in the form "vX.Y.Z", but version.parse() can handle it
+    current_version = version.parse(result.stdout)  # type: ignore
+    # Compare the version numbers
+    return (
+        current_version >= version.parse(constants.NODE_VERSION_MIN)
+        if IS_WINDOWS
+        else current_version == version.parse(constants.NODE_VERSION)
+    )
+
 
 def get_bun_version() -> Optional[version.Version]:
     """Get the version of bun.
 
     Returns:
         The version of bun.
     """
     try:
         # Run the bun -v command and capture the output
-        result = subprocess.run(
-            [os.path.expandvars(get_config().bun_path), "-v"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        return version.parse(result.stdout.decode().strip())
-    except Exception:
+        result = new_process([constants.BUN_PATH, "-v"], run=True)
+        return version.parse(result.stdout)  # type: ignore
+    except FileNotFoundError:
         return None
 
 
-def get_package_manager() -> str:
-    """Get the package manager executable.
+def get_windows_package_manager() -> str:
+    """Get the package manager for windows.
 
     Returns:
-        The path to the package manager.
+        The path to the package manager for windows.
 
     Raises:
         FileNotFoundError: If bun or npm is not installed.
-        Exit: If the app directory is invalid.
-
     """
-    config = get_config()
+    npm_path = path_ops.which("npm")
+    if npm_path is None:
+        raise FileNotFoundError("Reflex requires npm to be installed on Windows.")
+    return npm_path
 
-    # Check that the node version is valid.
-    if not check_node_version():
-        console.print(
-            f"[red]Node.js version {constants.MIN_NODE_VERSION} or higher is required to run Reflex."
-        )
-        raise typer.Exit()
+
+def get_install_package_manager() -> str:
+    """Get the package manager executable for installation.
+      currently on unix systems, bun is used for installation only.
+
+    Returns:
+        The path to the package manager.
+    """
+    get_config()
 
     # On Windows, we use npm instead of bun.
-    if platform.system() == "Windows" or config.disable_bun:
-        npm_path = path_ops.which("npm")
-        if npm_path is None:
-            raise FileNotFoundError("Reflex requires npm to be installed on Windows.")
-        return npm_path
+    if platform.system() == "Windows":
+        return get_windows_package_manager()
 
     # On other platforms, we use bun.
-    return os.path.expandvars(get_config().bun_path)
+    return constants.BUN_PATH
+
+
+def get_package_manager() -> str:
+    """Get the package manager executable for running app.
+      currently on unix systems, npm is used for running the app only.
+
+    Returns:
+        The path to the package manager.
+    """
+    get_config()
+
+    if platform.system() == "Windows":
+        return get_windows_package_manager()
+    return constants.NPM_PATH
 
 
 def get_app() -> ModuleType:
     """Get the app module based on the default config.
 
     Returns:
         The app based on the default config.
@@ -114,15 +129,15 @@
     Returns:
         The redis client.
     """
     config = get_config()
     if config.redis_url is None:
         return None
     redis_url, redis_port = config.redis_url.split(":")
-    print("Using redis at", config.redis_url)
+    console.info(f"Using redis at {config.redis_url}")
     return Redis(host=redis_url, port=int(redis_port), db=0)
 
 
 def get_production_backend_url() -> str:
     """Get the production backend URL.
 
     Returns:
@@ -138,58 +153,58 @@
 def get_default_app_name() -> str:
     """Get the default app name.
 
     The default app name is the name of the current directory.
 
     Returns:
         The default app name.
+
+    Raises:
+        Exit: if the app directory name is reflex.
     """
-    return os.getcwd().split(os.path.sep)[-1].replace("-", "_")
+    app_name = os.getcwd().split(os.path.sep)[-1].replace("-", "_")
+
+    # Make sure the app is not named "reflex".
+    if app_name == constants.MODULE_NAME:
+        console.error(
+            f"The app directory cannot be named [bold]{constants.MODULE_NAME}[/bold]."
+        )
+        raise typer.Exit()
+
+    return app_name
 
 
 def create_config(app_name: str):
     """Create a new rxconfig file.
 
     Args:
         app_name: The name of the app.
     """
     # Import here to avoid circular imports.
     from reflex.compiler import templates
 
     config_name = f"{re.sub(r'[^a-zA-Z]', '', app_name).capitalize()}Config"
     with open(constants.CONFIG_FILE, "w") as f:
+        console.debug(f"Creating {constants.CONFIG_FILE}")
         f.write(templates.RXCONFIG.render(app_name=app_name, config_name=config_name))
 
 
-def create_web_directory(root: Path) -> str:
-    """Creates a web directory in the given root directory
-    and returns the path to the directory.
-
-    Args:
-        root (Path): The root directory of the project.
-
-    Returns:
-        The path to the web directory.
-    """
-    web_dir = str(root / constants.WEB_DIR)
-    path_ops.cp(constants.WEB_TEMPLATE_DIR, web_dir, overwrite=False)
-    return web_dir
-
-
 def initialize_gitignore():
     """Initialize the template .gitignore file."""
     # The files to add to the .gitignore file.
     files = constants.DEFAULT_GITIGNORE
 
     # Subtract current ignored files.
     if os.path.exists(constants.GITIGNORE_FILE):
         with open(constants.GITIGNORE_FILE, "r") as f:
             files |= set([line.strip() for line in f.readlines()])
+
     # Write files to the .gitignore file.
     with open(constants.GITIGNORE_FILE, "w") as f:
+        console.debug(f"Creating {constants.GITIGNORE_FILE}")
         f.write(f"{(path_ops.join(sorted(files))).lstrip()}")
 
 
 def initialize_app_directory(app_name: str, template: constants.Template):
     """Initialize the app directory on reflex init.
 
     Args:
@@ -228,124 +243,184 @@
 
     # Write the current version of distributed reflex package to a REFLEX_JSON."""
     with open(constants.REFLEX_JSON, "w") as f:
         reflex_json = {"version": constants.VERSION}
         json.dump(reflex_json, f, ensure_ascii=False)
 
 
-def validate_and_install_bun(initialize=True):
-    """Check that bun version requirements are met. If they are not,
-    ask user whether to install required version.
-
-    Args:
-        initialize: whether this function is called on `reflex init` or `reflex run`.
-
-    Raises:
-        Exit: If the bun version is not supported.
+def initialize_bun():
+    """Check that bun requirements are met, and install if not."""
+    if IS_WINDOWS:
+        # Bun is not supported on Windows.
+        console.debug("Skipping bun installation on Windows.")
+        return
 
-    """
+    # Check the bun version.
     bun_version = get_bun_version()
-    if bun_version is not None and (
-        bun_version < version.parse(constants.MIN_BUN_VERSION)
-        or bun_version > version.parse(constants.MAX_BUN_VERSION)
-    ):
-        console.print(
-            f"""[red]Bun version {bun_version} is not supported by Reflex. Please change your to bun version to be between {constants.MIN_BUN_VERSION} and {constants.MAX_BUN_VERSION}."""
-        )
-        action = console.ask(
-            "Enter 'yes' to install the latest supported bun version or 'no' to exit.",
-            choices=["yes", "no"],
-            default="no",
+    if bun_version != version.parse(constants.BUN_VERSION):
+        console.debug(
+            f"Current bun version ({bun_version}) does not match ({constants.BUN_VERSION})."
         )
-
-        if action == "yes":
-            remove_existing_bun_installation()
-            install_bun()
-            return
-        else:
-            raise typer.Exit()
-
-    if initialize:
+        remove_existing_bun_installation()
         install_bun()
 
 
 def remove_existing_bun_installation():
     """Remove existing bun installation."""
-    package_manager = get_package_manager()
-    if os.path.exists(package_manager):
-        console.log("Removing bun...")
-        path_ops.rm(os.path.expandvars(constants.BUN_ROOT_PATH))
+    console.debug("Removing existing bun installation.")
+    if os.path.exists(constants.BUN_PATH):
+        path_ops.rm(constants.BUN_ROOT_PATH)
 
 
-def install_bun():
-    """Install bun onto the user's system.
+def initialize_node():
+    """Validate nodejs have install or not."""
+    if not check_node_version():
+        install_node()
+
+
+def download_and_run(url: str, *args, **env):
+    """Download and run a script.
+
+    Args:
+        url: The url of the script.
+        args: The arguments to pass to the script.
+        env: The environment variables to use.
+    """
+    # Download the script
+    console.debug(f"Downloading {url}")
+    response = httpx.get(url)
+    if response.status_code != httpx.codes.OK:
+        response.raise_for_status()
+
+    # Save the script to a temporary file.
+    script = tempfile.NamedTemporaryFile()
+    with open(script.name, "w") as f:
+        f.write(response.text)
+
+    # Run the script.
+    env = {
+        **os.environ,
+        **env,
+    }
+    process = new_process(["bash", f.name, *args], env=env)
+    show_logs(f"Installing {url}", process)
+
+
+def install_node():
+    """Install nvm and nodejs for use by Reflex.
+       Independent of any existing system installations.
 
     Raises:
-        FileNotFoundError: if unzip or curl packages are not found.
         Exit: if installation failed
     """
-    # Bun is not supported on Windows.
-    if platform.system() == "Windows":
-        console.log("Skipping bun installation on Windows.")
-        return
-
-    # Only install if bun is not already installed.
-    if not os.path.exists(get_package_manager()):
-        console.log("Installing bun...")
+    # NVM is not supported on Windows.
+    if IS_WINDOWS:
+        console.error(
+            f"Node.js version {constants.NODE_VERSION} or higher is required to run Reflex."
+        )
+        raise typer.Exit()
 
-        # Check if curl is installed
-        curl_path = path_ops.which("curl")
-        if curl_path is None:
-            raise FileNotFoundError("Reflex requires curl to be installed.")
+    # Create the nvm directory and install.
+    path_ops.mkdir(constants.NVM_DIR)
+    env = {**os.environ, "NVM_DIR": constants.NVM_DIR}
+    download_and_run(constants.NVM_INSTALL_URL, **env)
+
+    # Install node.
+    # We use bash -c as we need to source nvm.sh to use nvm.
+    process = new_process(
+        [
+            "bash",
+            "-c",
+            f". {constants.NVM_DIR}/nvm.sh && nvm install {constants.NODE_VERSION}",
+        ],
+        env=env,
+    )
+    show_logs("Installing node", process)
 
-        # Check if unzip is installed
-        unzip_path = path_ops.which("unzip")
-        if unzip_path is None:
-            raise FileNotFoundError("Reflex requires unzip to be installed.")
 
-        result = subprocess.run(constants.INSTALL_BUN, shell=True)
+def install_bun():
+    """Install bun onto the user's system.
 
-        if result.returncode != 0:
-            raise typer.Exit(code=result.returncode)
+    Raises:
+        FileNotFoundError: If required packages are not found.
+    """
+    # Bun is not supported on Windows.
+    if IS_WINDOWS:
+        console.debug("Skipping bun installation on Windows.")
+        return
 
+    # Skip if bun is already installed.
+    if os.path.exists(constants.BUN_PATH):
+        console.debug("Skipping bun installation as it is already installed.")
+        return
 
-def install_frontend_packages(web_dir: str):
-    """Installs the base and custom frontend packages
-    into the given web directory.
+    #  if unzip is installed
+    unzip_path = path_ops.which("unzip")
+    if unzip_path is None:
+        raise FileNotFoundError("Reflex requires unzip to be installed.")
+
+    # Run the bun install script.
+    download_and_run(
+        constants.BUN_INSTALL_URL,
+        f"bun-v{constants.BUN_VERSION}",
+        BUN_INSTALL=constants.BUN_ROOT_PATH,
+    )
 
-    Args:
-        web_dir: The directory where the frontend code is located.
-    """
-    # Install the frontend packages.
-    console.rule("[bold]Installing frontend packages")
 
+def install_frontend_packages():
+    """Installs the base and custom frontend packages."""
     # Install the base packages.
-    subprocess.run(
-        [get_package_manager(), "install"],
-        cwd=web_dir,
-        stdout=subprocess.PIPE,
+    process = new_process(
+        [get_install_package_manager(), "install"],
+        cwd=constants.WEB_DIR,
     )
+    show_logs("Installing base frontend packages", process)
 
     # Install the app packages.
     packages = get_config().frontend_packages
     if len(packages) > 0:
-        subprocess.run(
-            [get_package_manager(), "add", *packages],
-            cwd=web_dir,
-            stdout=subprocess.PIPE,
+        process = new_process(
+            [get_install_package_manager(), "add", *packages],
+            cwd=constants.WEB_DIR,
         )
+        show_logs("Installing custom frontend packages", process)
 
 
-def is_initialized() -> bool:
-    """Check whether the app is initialized.
+def check_initialized(frontend: bool = True):
+    """Check that the app is initialized.
 
-    Returns:
-        Whether the app is initialized in the current directory.
+    Args:
+        frontend: Whether to check if the frontend is initialized.
+
+    Raises:
+        Exit: If the app is not initialized.
     """
-    return os.path.exists(constants.CONFIG_FILE) and os.path.exists(constants.WEB_DIR)
+    has_config = os.path.exists(constants.CONFIG_FILE)
+    has_reflex_dir = IS_WINDOWS or os.path.exists(constants.REFLEX_DIR)
+    has_web_dir = not frontend or os.path.exists(constants.WEB_DIR)
+
+    # Check if the app is initialized.
+    if not (has_config and has_reflex_dir and has_web_dir):
+        console.error(
+            f"The app is not initialized. Run [bold]{constants.MODULE_NAME} init[/bold] first."
+        )
+        raise typer.Exit()
+
+    # Check that the template is up to date.
+    if frontend and not is_latest_template():
+        console.error(
+            "The base app template has updated. Run [bold]reflex init[/bold] again."
+        )
+        raise typer.Exit()
+
+    # Print a warning for Windows users.
+    if IS_WINDOWS:
+        console.warn(
+            "We strongly advise using Windows Subsystem for Linux (WSL) for optimal performance with reflex."
+        )
 
 
 def is_latest_template() -> bool:
     """Whether the app is using the latest template.
 
     Returns:
         Whether the app is using the latest template.
@@ -353,41 +428,61 @@
     if not os.path.exists(constants.REFLEX_JSON):
         return False
     with open(constants.REFLEX_JSON) as f:  # type: ignore
         app_version = json.load(f)["version"]
     return app_version == constants.VERSION
 
 
+def initialize_frontend_dependencies():
+    """Initialize all the frontend dependencies."""
+    # Create the reflex directory.
+    path_ops.mkdir(constants.REFLEX_DIR)
+
+    # Install the frontend dependencies.
+    threads = [
+        threading.Thread(target=initialize_bun),
+        threading.Thread(target=initialize_node),
+    ]
+    for thread in threads:
+        thread.start()
+
+    # Set up the web directory.
+    initialize_web_directory()
+
+    # Wait for the threads to finish.
+    for thread in threads:
+        thread.join()
+
+
 def check_admin_settings():
     """Check if admin settings are set and valid for logging in cli app."""
     admin_dash = get_config().admin_dash
-    current_time = datetime.now()
     if admin_dash:
         if not admin_dash.models:
-            console.print(
-                f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin dashboard enabled, but no models defined in [bold magenta]rxconfig.py[/bold magenta]. Time: {current_time}"
+            console.log(
+                f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin dashboard enabled, but no models defined in [bold magenta]rxconfig.py[/bold magenta]."
             )
         else:
-            console.print(
-                f"[yellow][Admin Dashboard][/yellow] Admin enabled, building admin dashboard. Time: {current_time}"
+            console.log(
+                f"[yellow][Admin Dashboard][/yellow] Admin enabled, building admin dashboard."
             )
-            console.print(
+            console.log(
                 "Admin dashboard running at: [bold green]http://localhost:8000/admin[/bold green]"
             )
 
 
 def check_db_initialized() -> bool:
     """Check if the database migrations are initialized.
 
     Returns:
         True if alembic is initialized (or if database is not used).
     """
     if get_config().db_url is not None and not Path(constants.ALEMBIC_CONFIG).exists():
-        console.print(
-            "[red]Database is not initialized. Run [bold]reflex db init[/bold] first."
+        console.error(
+            "Database is not initialized. Run [bold]reflex db init[/bold] first."
         )
         return False
     return True
 
 
 def check_schema_up_to_date():
     """Check if the sqlmodel metadata matches the current database schema."""
@@ -395,22 +490,22 @@
         return
     with model.Model.get_db_engine().connect() as connection:
         try:
             if model.Model.alembic_autogenerate(
                 connection=connection,
                 write_migration_scripts=False,
             ):
-                console.print(
-                    "[red]Detected database schema changes. Run [bold]reflex db makemigrations[/bold] "
+                console.error(
+                    "Detected database schema changes. Run [bold]reflex db makemigrations[/bold] "
                     "to generate migration scripts.",
                 )
         except CommandError as command_error:
             if "Target database is not up to date." in str(command_error):
-                console.print(
-                    f"[red]{command_error} Run [bold]reflex db migrate[/bold] to update database."
+                console.error(
+                    f"{command_error} Run [bold]reflex db migrate[/bold] to update database."
                 )
 
 
 def migrate_to_reflex():
     """Migration from Pynecone to Reflex."""
     # Check if the old config file exists.
     if not os.path.exists(constants.OLD_CONFIG_FILE):
@@ -421,15 +516,15 @@
         "Pynecone project detected. Automatically upgrade to Reflex?",
         choices=["y", "n"],
     )
     if action == "n":
         return
 
     # Rename pcconfig to rxconfig.
-    console.print(
+    console.log(
         f"[bold]Renaming {constants.OLD_CONFIG_FILE} to {constants.CONFIG_FILE}"
     )
     os.rename(constants.OLD_CONFIG_FILE, constants.CONFIG_FILE)
 
     # Find all python files in the app directory.
     file_pattern = os.path.join(get_config().app_name, "**/*.py")
     file_list = glob.glob(file_pattern, recursive=True)
```

### Comparing `reflex-0.2.3a7/reflex/utils/telemetry.py` & `reflex-0.2.3a8/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/utils/types.py` & `reflex-0.2.3a8/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/utils/watch.py` & `reflex-0.2.3a8/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/reflex/vars.py` & `reflex-0.2.3a8/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a7/PKG-INFO` & `reflex-0.2.3a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.3a7
+Version: 0.2.3a8
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

