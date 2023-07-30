# Comparing `tmp/bodhi_server-7.2.0.tar.gz` & `tmp/bodhi_server-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_server-7.2.0.tar", max compression
+gzip compressed data, was "bodhi_server-7.2.1.tar", max compression
```

## Comparing `bodhi_server-7.2.0.tar` & `bodhi_server-7.2.1.tar`

### file list

```diff
@@ -1,340 +1,341 @@
--rw-r--r--   0        0        0    18018 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/COPYING
--rw-r--r--   0        0        0     1655 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/README.rst
--rw-r--r--   0        0        0     1258 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/alembic.ini
--rw-r--r--   0        0        0      580 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/apache/bodhi.conf
--rw-r--r--   0        0        0      260 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/apache/bodhi.wsgi
--rw-r--r--   0        0        0    13319 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/__init__.py
--rw-r--r--   0        0        0      220 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/constants.py
--rw-r--r--   0        0        0     5960 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/fedora.py
--rw-r--r--   0        0        0     2604 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/oauth.py
--rw-r--r--   0        0        0     2794 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/oauth_015.py
--rw-r--r--   0        0        0     3597 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/oauth_1.py
--rw-r--r--   0        0        0     5965 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/utils.py
--rw-r--r--   0        0        0     3960 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/views.py
--rw-r--r--   0        0        0    12401 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/bugs.py
--rw-r--r--   0        0        0    30159 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/buildsys.py
--rw-r--r--   0        0        0    25877 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/config.py
--rw-r--r--   0        0        0     3616 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/consumers/__init__.py
--rw-r--r--   0        0        0     8807 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/consumers/automatic_updates.py
--rw-r--r--   0        0        0     4009 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/consumers/ci.py
--rw-r--r--   0        0        0     2863 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/consumers/resultsdb.py
--rw-r--r--   0        0        0     5651 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/consumers/signed.py
--rw-r--r--   0        0        0     2728 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/consumers/util.py
--rw-r--r--   0        0        0     2569 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/consumers/waiverdb.py
--rw-r--r--   0        0        0     1040 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_errata_template.tpl
--rw-r--r--   0        0        0     1070 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl
--rw-r--r--   0        0        0     1051 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_errata_template.tpl
--rw-r--r--   0        0        0     1059 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_modular_errata_template.tpl
--rw-r--r--   0        0        0      261 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/maillist_template.tpl
--rw-r--r--   0        0        0     1249 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/exceptions.py
--rw-r--r--   0        0        0     7154 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/ffmarkdown.py
--rw-r--r--   0        0        0        0 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/locale/.placeholder
--rw-r--r--   0        0        0     3641 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/logging.py
--rw-r--r--   0        0        0    14666 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/mail.py
--rw-r--r--   0        0        0    12964 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/metadata.py
--rw-r--r--   0        0        0      706 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/README.rst
--rw-r--r--   0        0        0      845 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/__init__.py
--rw-r--r--   0        0        0     3808 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/env.py
--rw-r--r--   0        0        0     1181 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/script.py.mako
--rw-r--r--   0        0        0     2918 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py
--rw-r--r--   0        0        0     1333 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py
--rw-r--r--   0        0        0     1380 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py
--rw-r--r--   0        0        0     1443 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py
--rw-r--r--   0        0        0     3846 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py
--rw-r--r--   0        0        0     2732 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py
--rw-r--r--   0        0        0     3041 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py
--rw-r--r--   0        0        0     1822 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py
--rw-r--r--   0        0        0     2279 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py
--rw-r--r--   0        0        0     2187 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py
--rw-r--r--   0        0        0     2586 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py
--rw-r--r--   0        0        0     2708 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py
--rw-r--r--   0        0        0     1741 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py
--rw-r--r--   0        0        0     2812 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py
--rw-r--r--   0        0        0     1503 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py
--rw-r--r--   0        0        0     1368 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py
--rw-r--r--   0        0        0     1501 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py
--rw-r--r--   0        0        0      843 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/__init__.py
--rw-r--r--   0        0        0     1321 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py
--rw-r--r--   0        0        0     2991 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py
--rw-r--r--   0        0        0     1346 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py
--rw-r--r--   0        0        0     1808 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py
--rw-r--r--   0        0        0     2341 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py
--rw-r--r--   0        0        0     2593 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py
--rw-r--r--   0        0        0     2316 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py
--rw-r--r--   0        0        0     1296 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py
--rw-r--r--   0        0        0     1329 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py
--rw-r--r--   0        0        0     1403 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py
--rw-r--r--   0        0        0     1670 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py
--rw-r--r--   0        0        0     1421 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py
--rw-r--r--   0        0        0     1403 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py
--rw-r--r--   0        0        0     1312 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py
--rw-r--r--   0        0        0     1345 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py
--rw-r--r--   0        0        0     1469 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py
--rw-r--r--   0        0        0     1353 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py
--rw-r--r--   0        0        0     1347 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py
--rw-r--r--   0        0        0   198699 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/models.py
--rw-r--r--   0        0        0     3016 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/notifications.py
--rw-r--r--   0        0        0    11988 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/push.py
--rw-r--r--   0        0        0     7143 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/renderers.py
--rw-r--r--   0        0        0    22381 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/schemas.py
--rw-r--r--   0        0        0      849 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/bshell.py
--rw-r--r--   0        0        0     3871 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/compat.py
--rw-r--r--   0        0        0     1847 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/initializedb.py
--rw-r--r--   0        0        0     4238 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/sar.py
--rw-r--r--   0        0        0    29485 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/skopeo_lite.py
--rw-r--r--   0        0        0     3839 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/untag_branched.py
--rw-r--r--   0        0        0     6158 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/security.py
--rw-r--r--   0        0        0      815 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/__init__.py
--rw-r--r--   0        0        0     5182 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/builds.py
--rw-r--r--   0        0        0     8633 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/comments.py
--rw-r--r--   0        0        0     3936 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/composes.py
--rw-r--r--   0        0        0     2058 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/csrf.py
--rw-r--r--   0        0        0     3793 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/errors.py
--rw-r--r--   0        0        0     1969 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/markdown.py
--rw-r--r--   0        0        0     1916 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/metrics_tween.py
--rw-r--r--   0        0        0    12983 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/overrides.py
--rw-r--r--   0        0        0     3724 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/packages.py
--rw-r--r--   0        0        0    16707 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/services/releases.py
--rw-r--r--   0        0        0     3481 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/schemas.py
--rw-r--r--   0        0        0    28875 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/updates.py
--rw-r--r--   0        0        0     6612 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/user.py
--rw-r--r--   0        0        0      832 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/__init__.py
--rw-r--r--   0        0        0    10425 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/bodhi-logo.svg
--rw-r--r--   0        0        0     6423 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/css/site.css
--rw-r--r--   0        0        0   124988 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/FontAwesome.otf
--rw-r--r--   0        0        0    76518 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot
--rw-r--r--   0        0        0   391622 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg
--rw-r--r--   0        0        0   152796 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    90412 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff
--rw-r--r--   0        0        0    71896 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    35152 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome.css
--rwxr-xr-x   0        0        0   139140 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot
--rwxr-xr-x   0        0        0   146800 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot
--rwxr-xr-x   0        0        0   143488 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot
--rwxr-xr-x   0        0        0   137266 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot
--rwxr-xr-x   0        0        0    28782 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot
--rwxr-xr-x   0        0        0    31454 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot
--rwxr-xr-x   0        0        0    30512 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot
--rwxr-xr-x   0        0        0    28527 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot
--rwxr-xr-x   0        0        0   389828 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf
--rwxr-xr-x   0        0        0   398888 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf
--rwxr-xr-x   0        0        0   393880 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf
--rwxr-xr-x   0        0        0   387660 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf
--rwxr-xr-x   0        0        0    73056 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf
--rwxr-xr-x   0        0        0    77808 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf
--rwxr-xr-x   0        0        0    76444 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf
--rwxr-xr-x   0        0        0    73256 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf
--rwxr-xr-x   0        0        0   171820 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff
--rwxr-xr-x   0        0        0   180204 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff
--rwxr-xr-x   0        0        0   176864 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff
--rwxr-xr-x   0        0        0   168376 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff
--rwxr-xr-x   0        0        0    31964 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff
--rwxr-xr-x   0        0        0    34720 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff
--rwxr-xr-x   0        0        0    33556 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff
--rwxr-xr-x   0        0        0    31584 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff
--rwxr-xr-x   0        0        0   124552 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2
--rwxr-xr-x   0        0        0   131588 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2
--rwxr-xr-x   0        0        0   128624 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2
--rwxr-xr-x   0        0        0   122888 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2
--rwxr-xr-x   0        0        0    25884 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2
--rwxr-xr-x   0        0        0    28232 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2
--rwxr-xr-x   0        0        0    27576 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2
--rwxr-xr-x   0        0        0    25696 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2
--rw-r--r--   0        0        0     1947 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack.css
--rw-r--r--   0        0        0    31896 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot
--rw-r--r--   0        0        0   254253 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg
--rw-r--r--   0        0        0    68444 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf
--rw-r--r--   0        0        0    33704 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff
--rw-r--r--   0        0        0    23816 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2
--rw-r--r--   0        0        0    30763 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot
--rw-r--r--   0        0        0   258568 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg
--rw-r--r--   0        0        0    64668 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf
--rw-r--r--   0        0        0    32300 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff
--rw-r--r--   0        0        0    22220 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2
--rw-r--r--   0        0        0    32088 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot
--rw-r--r--   0        0        0   254724 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg
--rw-r--r--   0        0        0    68776 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf
--rw-r--r--   0        0        0    33876 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff
--rw-r--r--   0        0        0    23652 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2
--rw-r--r--   0        0        0    30546 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot
--rw-r--r--   0        0        0   257617 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg
--rw-r--r--   0        0        0    65236 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf
--rw-r--r--   0        0        0    32180 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff
--rw-r--r--   0        0        0    22176 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2
--rw-r--r--   0        0        0    30880 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot
--rw-r--r--   0        0        0   258434 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg
--rw-r--r--   0        0        0    65072 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf
--rw-r--r--   0        0        0    32212 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff
--rw-r--r--   0        0        0    22196 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2
--rw-r--r--   0        0        0    31491 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot
--rw-r--r--   0        0        0   255338 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg
--rw-r--r--   0        0        0    66740 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf
--rw-r--r--   0        0        0    33060 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff
--rw-r--r--   0        0        0    23048 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2
--rw-r--r--   0        0        0     4956 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans.css
--rw-r--r--   0        0        0     4255 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/ico/favicon.ico
--rw-r--r--   0        0        0    13117 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.png
--rw-r--r--   0        0        0    17444 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.svg
--rw-r--r--   0        0        0    30769 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/logo-large.png
--rw-r--r--   0        0        0     4388 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/logo.png
--rw-r--r--   0        0        0     1775 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/comment_form.js
--rw-r--r--   0        0        0     4723 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/js/forms.js
--rw-r--r--   0        0        0     3238 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/override_form.js
--rw-r--r--   0        0        0     3485 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/search.js
--rw-r--r--   0        0        0     1475 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/site.js
--rw-r--r--   0        0        0    14397 2023-04-29 08:26:58.000000 bodhi_server-7.2.0/bodhi/server/static/js/update_form.js
--rw-r--r--   0        0        0   197005 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/chartjs/chart.min.js
--rw-r--r--   0        0        0   199088 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css
--rw-r--r--   0        0        0    75244 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map
--rw-r--r--   0        0        0    79790 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js
--rw-r--r--   0        0        0   330849 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map
--rw-r--r--   0        0        0    89501 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js
--rw-r--r--   0        0        0   137972 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map
--rw-r--r--   0        0        0    12438 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css
--rw-r--r--   0        0        0    48148 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js
--rw-r--r--   0        0        0     5855 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-spinner.css
--rw-r--r--   0        0        0    12969 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css
--rw-r--r--   0        0        0     3908 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css
--rw-r--r--   0        0        0    13273 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css
--rw-r--r--   0        0        0    16828 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css
--rw-r--r--   0        0        0     4399 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css
--rw-r--r--   0        0        0     3086 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger.css
--rw-r--r--   0        0        0     1281 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js
--rw-r--r--   0        0        0     1301 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js
--rw-r--r--   0        0        0    40813 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.js
--rw-r--r--   0        0        0    19068 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.min.js
--rw-r--r--   0        0        0    32364 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/moment/moment.min.js
--rw-r--r--   0        0        0    66344 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js
--rw-r--r--   0        0        0   335718 2022-11-14 19:44:00.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.0.min.js
--rw-r--r--   0        0        0   126299 2022-11-17 17:24:15.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.1.js
--rw-r--r--   0        0        0   336699 2022-11-17 17:24:15.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.1.min.js
--rw-r--r--   0        0        0   126299 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.js
--rw-r--r--   0        0        0    55382 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js
--rw-r--r--   0        0        0     9368 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css
--rw-r--r--   0        0        0    36947 2022-11-14 19:44:00.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.0.css
--rw-r--r--   0        0        0    37022 2022-11-17 17:24:15.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.1.css
--rw-r--r--   0        0        0    14594 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css
--rw-r--r--   0        0        0   104302 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/typeahead/typeahead.bundle.js
--rw-r--r--   0        0        0     6095 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/__init__.py
--rw-r--r--   0        0        0     7848 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/approve_testing.py
--rw-r--r--   0        0        0     2158 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/check_policies.py
--rw-r--r--   0        0        0     4591 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/check_signed_builds.py
--rw-r--r--   0        0        0     2397 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/clean_old_composes.py
--rw-r--r--   0        0        0    62185 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/tasks/composer.py
--rw-r--r--   0        0        0     2035 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/expire_overrides.py
--rw-r--r--   0        0        0     1785 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/fetch_test_cases.py
--rw-r--r--   0        0        0     2833 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/handle_side_and_related_tags.py
--rw-r--r--   0        0        0     1469 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/tag_update_builds.py
--rw-r--r--   0        0        0     3706 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/work_on_bugs.py
--rw-r--r--   0        0        0      105 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/comment.html
--rw-r--r--   0        0        0     1331 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/comments.html
--rw-r--r--   0        0        0     3575 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/compose.html
--rw-r--r--   0        0        0     1270 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/composes.html
--rw-r--r--   0        0        0      352 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/errors.html
--rw-r--r--   0        0        0    15764 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/templates/fragments.html
--rw-r--r--   0        0        0     5525 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/home.html
--rw-r--r--   0        0        0    10635 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/master.html
--rw-r--r--   0        0        0    20775 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/templates/new_update.html
--rw-r--r--   0        0        0     9352 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/override.html
--rw-r--r--   0        0        0     9731 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/templates/overrides.html
--rw-r--r--   0        0        0      882 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/pager.html
--rw-r--r--   0        0        0    12532 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/release.html
--rw-r--r--   0        0        0     2938 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/templates/releases.html
--rw-r--r--   0        0        0    55990 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/templates/update.html
--rw-r--r--   0        0        0    15964 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/templates/updates.html
--rw-r--r--   0        0        0     4796 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/user.html
--rw-r--r--   0        0        0    50365 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/util.py
--rw-r--r--   0        0        0    51587 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/validators.py
--rw-r--r--   0        0        0      812 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/views/__init__.py
--rw-r--r--   0        0        0    22706 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/views/generic.py
--rw-r--r--   0        0        0     3545 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/webapp.py
--rw-r--r--   0        0        0     1592 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/celeryconfig.py
--rw-r--r--   0        0        0      776 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/Makefile
--rw-r--r--   0        0        0     1757 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/conf.py
--rw-r--r--   0        0        0        0 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/index.rst
--rw-r--r--   0        0        0     1244 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-push.rst
--rw-r--r--   0        0        0      797 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-sar.rst
--rw-r--r--   0        0        0      523 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-shell.rst
--rw-r--r--   0        0        0     1866 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-skopeo-lite.rst
--rw-r--r--   0        0        0      718 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-untag-branched.rst
--rw-r--r--   0        0        0      623 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/initialize_bodhi_db.rst
--rw-r--r--   0        0        0    24410 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/production.ini
--rw-r--r--   0        0        0     4911 2023-04-30 06:59:12.000000 bodhi_server-7.2.0/pyproject.toml
--rw-r--r--   0        0        0      418 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/setup.cfg
--rw-r--r--   0        0        0      816 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/__init__.py
--rw-r--r--   0        0        0       39 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/__init__.py
--rw-r--r--   0        0        0     4790 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/test_fedora.py
--rw-r--r--   0        0        0    16947 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/test_oauth.py
--rw-r--r--   0        0        0     5487 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/test_utils.py
--rw-r--r--   0        0        0     5442 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/auth/test_views.py
--rw-r--r--   0        0        0     2293 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/auth/utils.py
--rw-r--r--   0        0        0    19037 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/base.py
--rw-r--r--   0        0        0     2214 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/conftest.py
--rw-r--r--   0        0        0      821 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/__init__.py
--rwxr-xr-x   0        0        0      335 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/fake-pungi.sh
--rw-r--r--   0        0        0       76 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/pungi.module.conf
--rw-r--r--   0        0        0       76 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/pungi.rpm.conf
--rw-r--r--   0        0        0      210 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/variants.module.xml.j2
--rw-r--r--   0        0        0       76 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/variants.rpm.xml.j2
--rw-r--r--   0        0        0    20022 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/consumers/test_automatic_updates.py
--rw-r--r--   0        0        0    11457 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/test_ci.py
--rw-r--r--   0        0        0     4779 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/test_consumers.py
--rw-r--r--   0        0        0    14326 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/consumers/test_resultsdb.py
--rw-r--r--   0        0        0    13241 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/consumers/test_signed.py
--rw-r--r--   0        0        0    10129 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/consumers/test_waiverdb.py
--rw-r--r--   0        0        0      913 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/functional/__init__.py
--rw-r--r--   0        0        0     2571 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/functional/test_packages.py
--rw-r--r--   0        0        0     8272 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/functional/test_users.py
--rw-r--r--   0        0        0      819 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_bshell.py
--rw-r--r--   0        0        0     5128 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_compat.py
--rw-r--r--   0        0        0     3597 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_initializedb.py
--rw-r--r--   0        0        0     5341 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_sar.py
--rw-r--r--   0        0        0    26242 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_skopeo_lite.py
--rw-r--r--   0        0        0    15411 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_untag_branched.py
--rw-r--r--   0        0        0      820 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/__init__.py
--rw-r--r--   0        0        0     4067 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_builds.py
--rw-r--r--   0        0        0    27002 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_comments.py
--rw-r--r--   0        0        0     6469 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_composes.py
--rw-r--r--   0        0        0     1512 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_csrf.py
--rw-r--r--   0        0        0     1827 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_errors.py
--rw-r--r--   0        0        0    31133 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_overrides.py
--rw-r--r--   0        0        0    30447 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/services/test_releases.py
--rw-r--r--   0        0        0     3801 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_schemas.py
--rw-r--r--   0        0        0   299158 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/tests/services/test_updates.py
--rw-r--r--   0        0        0      817 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1531 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/base.py
--rw-r--r--   0        0        0    42724 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/tasks/test_approve_testing.py
--rw-r--r--   0        0        0    29342 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/tasks/test_check_policies.py
--rw-r--r--   0        0        0     8649 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/tasks/test_check_signed_builds.py
--rw-r--r--   0        0        0     5949 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_clean_old_composes.py
--rw-r--r--   0        0        0   175797 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/tasks/test_composer.py
--rw-r--r--   0        0        0     3792 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_expire_overrides.py
--rw-r--r--   0        0        0     3677 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/tasks/test_fetch_test_cases.py
--rw-r--r--   0        0        0     2799 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_handle_side_and_related_tags.py
--rw-r--r--   0        0        0     2321 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_tag_update_builds.py
--rw-r--r--   0        0        0     5085 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_work_on_bugs.py
--rw-r--r--   0        0        0    11553 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/test___init__.py
--rw-r--r--   0        0        0     2185 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_alembic.py
--rw-r--r--   0        0        0    28061 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_bugs.py
--rw-r--r--   0        0        0    17610 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_buildsys.py
--rw-r--r--   0        0        0    16269 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_config.py
--rw-r--r--   0        0        0     4319 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_logging.py
--rw-r--r--   0        0        0    15586 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_mail.py
--rw-r--r--   0        0        0    25674 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_metadata.py
--rw-r--r--   0        0        0   216666 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/test_models.py
--rw-r--r--   0        0        0     3897 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_notifications.py
--rw-r--r--   0        0        0    72085 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/test_push.py
--rw-r--r--   0        0        0     2238 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_renderers.py
--rw-r--r--   0        0        0     1642 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_schemas.py
--rw-r--r--   0        0        0     7195 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_security.py
--rw-r--r--   0        0        0    69803 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/test_util.py
--rw-r--r--   0        0        0    44272 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/test_validators.py
--rw-r--r--   0        0        0     2614 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_webapp.py
--rw-r--r--   0        0        0     4217 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/testing.ini
--rw-r--r--   0        0        0      992 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/utils.py
--rw-r--r--   0        0        0      817 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/views/__init__.py
--rw-r--r--   0        0        0    23763 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/views/test_generic.py
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 bodhi_server-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0    18018 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/COPYING
+-rw-r--r--   0        0        0     1655 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/README.rst
+-rw-r--r--   0        0        0     1258 2023-07-30 09:10:09.000000 bodhi_server-7.2.1/alembic.ini
+-rw-r--r--   0        0        0      580 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/apache/bodhi.conf
+-rw-r--r--   0        0        0      260 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/apache/bodhi.wsgi
+-rw-r--r--   0        0        0    13319 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/constants.py
+-rw-r--r--   0        0        0     5960 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/fedora.py
+-rw-r--r--   0        0        0     2604 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/oauth.py
+-rw-r--r--   0        0        0     2794 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/oauth_015.py
+-rw-r--r--   0        0        0     3597 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/oauth_1.py
+-rw-r--r--   0        0        0     5965 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/utils.py
+-rw-r--r--   0        0        0     3960 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/auth/views.py
+-rw-r--r--   0        0        0    12401 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/bugs.py
+-rw-r--r--   0        0        0    30159 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/buildsys.py
+-rw-r--r--   0        0        0    25877 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/config.py
+-rw-r--r--   0        0        0     3616 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/consumers/__init__.py
+-rw-r--r--   0        0        0     8807 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/consumers/automatic_updates.py
+-rw-r--r--   0        0        0     4009 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/consumers/ci.py
+-rw-r--r--   0        0        0     2863 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/consumers/resultsdb.py
+-rw-r--r--   0        0        0     5651 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/consumers/signed.py
+-rw-r--r--   0        0        0     2728 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/consumers/util.py
+-rw-r--r--   0        0        0     2569 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/consumers/waiverdb.py
+-rw-r--r--   0        0        0     1040 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/email/templates/fedora_epel_errata_template.tpl
+-rw-r--r--   0        0        0     1070 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl
+-rw-r--r--   0        0        0     1051 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/email/templates/fedora_errata_template.tpl
+-rw-r--r--   0        0        0     1059 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/email/templates/fedora_modular_errata_template.tpl
+-rw-r--r--   0        0        0      261 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/email/templates/maillist_template.tpl
+-rw-r--r--   0        0        0     1249 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/exceptions.py
+-rw-r--r--   0        0        0     7154 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/ffmarkdown.py
+-rw-r--r--   0        0        0        0 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/locale/.placeholder
+-rw-r--r--   0        0        0     3641 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/logging.py
+-rw-r--r--   0        0        0    14666 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/mail.py
+-rw-r--r--   0        0        0    12964 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/metadata.py
+-rw-r--r--   0        0        0      706 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/README.rst
+-rw-r--r--   0        0        0      845 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/__init__.py
+-rw-r--r--   0        0        0     3808 2023-07-30 09:39:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/env.py
+-rw-r--r--   0        0        0     1181 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/script.py.mako
+-rw-r--r--   0        0        0     2918 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py
+-rw-r--r--   0        0        0     1333 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py
+-rw-r--r--   0        0        0     1380 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py
+-rw-r--r--   0        0        0     1443 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py
+-rw-r--r--   0        0        0     3846 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py
+-rw-r--r--   0        0        0     2732 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py
+-rw-r--r--   0        0        0     3041 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py
+-rw-r--r--   0        0        0     1822 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py
+-rw-r--r--   0        0        0     2279 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py
+-rw-r--r--   0        0        0     2187 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py
+-rw-r--r--   0        0        0     2586 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py
+-rw-r--r--   0        0        0     2708 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py
+-rw-r--r--   0        0        0     1741 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py
+-rw-r--r--   0        0        0     2812 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py
+-rw-r--r--   0        0        0     1503 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py
+-rw-r--r--   0        0        0     1368 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py
+-rw-r--r--   0        0        0     1501 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py
+-rw-r--r--   0        0        0      843 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     1321 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py
+-rw-r--r--   0        0        0     2991 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py
+-rw-r--r--   0        0        0     1346 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py
+-rw-r--r--   0        0        0     1808 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py
+-rw-r--r--   0        0        0     2341 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py
+-rw-r--r--   0        0        0     2593 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py
+-rw-r--r--   0        0        0     2316 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py
+-rw-r--r--   0        0        0     1296 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py
+-rw-r--r--   0        0        0     1329 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py
+-rw-r--r--   0        0        0     1403 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py
+-rw-r--r--   0        0        0     1670 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py
+-rw-r--r--   0        0        0     1421 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py
+-rw-r--r--   0        0        0     1403 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py
+-rw-r--r--   0        0        0     1312 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py
+-rw-r--r--   0        0        0     1345 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py
+-rw-r--r--   0        0        0     1469 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py
+-rw-r--r--   0        0        0     1353 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py
+-rw-r--r--   0        0        0     1347 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py
+-rw-r--r--   0        0        0   198785 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/bodhi/server/models.py
+-rw-r--r--   0        0        0     3016 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/notifications.py
+-rw-r--r--   0        0        0    11988 2023-05-31 08:23:37.000000 bodhi_server-7.2.1/bodhi/server/push.py
+-rw-r--r--   0        0        0     7143 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/renderers.py
+-rw-r--r--   0        0        0    22381 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/schemas.py
+-rw-r--r--   0        0        0      849 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/scripts/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/scripts/bshell.py
+-rw-r--r--   0        0        0     3871 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/scripts/compat.py
+-rw-r--r--   0        0        0     1847 2023-05-21 12:57:14.000000 bodhi_server-7.2.1/bodhi/server/scripts/initializedb.py
+-rw-r--r--   0        0        0     4238 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/scripts/sar.py
+-rw-r--r--   0        0        0    29485 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/scripts/skopeo_lite.py
+-rw-r--r--   0        0        0     3839 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/scripts/untag_branched.py
+-rw-r--r--   0        0        0     6158 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/security.py
+-rw-r--r--   0        0        0      815 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/__init__.py
+-rw-r--r--   0        0        0     5182 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/builds.py
+-rw-r--r--   0        0        0     8633 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/comments.py
+-rw-r--r--   0        0        0     3936 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/composes.py
+-rw-r--r--   0        0        0     2058 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/csrf.py
+-rw-r--r--   0        0        0     3793 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/errors.py
+-rw-r--r--   0        0        0     1969 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/markdown.py
+-rw-r--r--   0        0        0     1916 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/metrics_tween.py
+-rw-r--r--   0        0        0    12983 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/overrides.py
+-rw-r--r--   0        0        0     3724 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/packages.py
+-rw-r--r--   0        0        0    16707 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/releases.py
+-rw-r--r--   0        0        0     3481 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/services/schemas.py
+-rw-r--r--   0        0        0    28875 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/updates.py
+-rw-r--r--   0        0        0     6612 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/services/user.py
+-rw-r--r--   0        0        0      832 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/__init__.py
+-rw-r--r--   0        0        0    10425 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/bodhi-logo.svg
+-rw-r--r--   0        0        0     6423 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/css/site.css
+-rw-r--r--   0        0        0   124988 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/FontAwesome.otf
+-rw-r--r--   0        0        0    76518 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   391622 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   152796 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    90412 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    71896 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    35152 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome.css
+-rwxr-xr-x   0        0        0   139140 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot
+-rwxr-xr-x   0        0        0   146800 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot
+-rwxr-xr-x   0        0        0   143488 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot
+-rwxr-xr-x   0        0        0   137266 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot
+-rwxr-xr-x   0        0        0    28782 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot
+-rwxr-xr-x   0        0        0    31454 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot
+-rwxr-xr-x   0        0        0    30512 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot
+-rwxr-xr-x   0        0        0    28527 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot
+-rwxr-xr-x   0        0        0   389828 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf
+-rwxr-xr-x   0        0        0   398888 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf
+-rwxr-xr-x   0        0        0   393880 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf
+-rwxr-xr-x   0        0        0   387660 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf
+-rwxr-xr-x   0        0        0    73056 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    77808 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    76444 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    73256 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf
+-rwxr-xr-x   0        0        0   171820 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff
+-rwxr-xr-x   0        0        0   180204 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff
+-rwxr-xr-x   0        0        0   176864 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff
+-rwxr-xr-x   0        0        0   168376 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff
+-rwxr-xr-x   0        0        0    31964 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff
+-rwxr-xr-x   0        0        0    34720 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff
+-rwxr-xr-x   0        0        0    33556 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff
+-rwxr-xr-x   0        0        0    31584 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff
+-rwxr-xr-x   0        0        0   124552 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2
+-rwxr-xr-x   0        0        0   131588 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2
+-rwxr-xr-x   0        0        0   128624 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2
+-rwxr-xr-x   0        0        0   122888 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2
+-rwxr-xr-x   0        0        0    25884 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    28232 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    27576 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    25696 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2
+-rw-r--r--   0        0        0     1947 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/hack.css
+-rw-r--r--   0        0        0    31896 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot
+-rw-r--r--   0        0        0   254253 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg
+-rw-r--r--   0        0        0    68444 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf
+-rw-r--r--   0        0        0    33704 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff
+-rw-r--r--   0        0        0    23816 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2
+-rw-r--r--   0        0        0    30763 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot
+-rw-r--r--   0        0        0   258568 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg
+-rw-r--r--   0        0        0    64668 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf
+-rw-r--r--   0        0        0    32300 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff
+-rw-r--r--   0        0        0    22220 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2
+-rw-r--r--   0        0        0    32088 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot
+-rw-r--r--   0        0        0   254724 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg
+-rw-r--r--   0        0        0    68776 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf
+-rw-r--r--   0        0        0    33876 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff
+-rw-r--r--   0        0        0    23652 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2
+-rw-r--r--   0        0        0    30546 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot
+-rw-r--r--   0        0        0   257617 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg
+-rw-r--r--   0        0        0    65236 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf
+-rw-r--r--   0        0        0    32180 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff
+-rw-r--r--   0        0        0    22176 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2
+-rw-r--r--   0        0        0    30880 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot
+-rw-r--r--   0        0        0   258434 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg
+-rw-r--r--   0        0        0    65072 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf
+-rw-r--r--   0        0        0    32212 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff
+-rw-r--r--   0        0        0    22196 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2
+-rw-r--r--   0        0        0    31491 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot
+-rw-r--r--   0        0        0   255338 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg
+-rw-r--r--   0        0        0    66740 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf
+-rw-r--r--   0        0        0    33060 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff
+-rw-r--r--   0        0        0    23048 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2
+-rw-r--r--   0        0        0     4956 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans.css
+-rw-r--r--   0        0        0     4255 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/ico/favicon.ico
+-rw-r--r--   0        0        0    13117 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/img/bodhi-logo.png
+-rw-r--r--   0        0        0    17444 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/img/bodhi-logo.svg
+-rw-r--r--   0        0        0    30769 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/img/logo-large.png
+-rw-r--r--   0        0        0     4388 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/img/logo.png
+-rw-r--r--   0        0        0     1775 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/js/comment_form.js
+-rw-r--r--   0        0        0     4723 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/js/forms.js
+-rw-r--r--   0        0        0     3238 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/js/override_form.js
+-rw-r--r--   0        0        0     3485 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/js/search.js
+-rw-r--r--   0        0        0     1475 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/js/site.js
+-rw-r--r--   0        0        0    14397 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/js/update_form.js
+-rw-r--r--   0        0        0   197005 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/chartjs/chart.min.js
+-rw-r--r--   0        0        0   199088 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css
+-rw-r--r--   0        0        0    75244 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map
+-rw-r--r--   0        0        0    79790 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js
+-rw-r--r--   0        0        0   330849 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map
+-rw-r--r--   0        0        0    89501 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0   137972 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map
+-rw-r--r--   0        0        0    12438 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css
+-rw-r--r--   0        0        0    48148 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js
+-rw-r--r--   0        0        0     5855 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-spinner.css
+-rw-r--r--   0        0        0    12969 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css
+-rw-r--r--   0        0        0     3908 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css
+-rw-r--r--   0        0        0    13273 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css
+-rw-r--r--   0        0        0    16828 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css
+-rw-r--r--   0        0        0     4399 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css
+-rw-r--r--   0        0        0     3086 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger.css
+-rw-r--r--   0        0        0     1281 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js
+-rw-r--r--   0        0        0     1301 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js
+-rw-r--r--   0        0        0    40813 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger.js
+-rw-r--r--   0        0        0    19068 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger.min.js
+-rw-r--r--   0        0        0    32364 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0    66344 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js
+-rw-r--r--   0        0        0   335718 2022-11-14 19:44:00.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.0.min.js
+-rw-r--r--   0        0        0   126299 2022-11-17 17:24:15.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.1.js
+-rw-r--r--   0        0        0   336699 2022-11-17 17:24:15.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.1.min.js
+-rw-r--r--   0        0        0   126299 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.js
+-rw-r--r--   0        0        0    55382 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js
+-rw-r--r--   0        0        0     9368 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css
+-rw-r--r--   0        0        0    36947 2022-11-14 19:44:00.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.0.css
+-rw-r--r--   0        0        0    37022 2022-11-17 17:24:15.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.1.css
+-rw-r--r--   0        0        0    14594 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css
+-rw-r--r--   0        0        0   104302 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/static/vendor/typeahead/typeahead.bundle.js
+-rw-r--r--   0        0        0     6095 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/__init__.py
+-rw-r--r--   0        0        0     7848 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/approve_testing.py
+-rw-r--r--   0        0        0     2158 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/check_policies.py
+-rw-r--r--   0        0        0     4591 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/check_signed_builds.py
+-rw-r--r--   0        0        0     2397 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/clean_old_composes.py
+-rw-r--r--   0        0        0    62185 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/tasks/composer.py
+-rw-r--r--   0        0        0     2035 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/expire_overrides.py
+-rw-r--r--   0        0        0     1785 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/fetch_test_cases.py
+-rw-r--r--   0        0        0     2833 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/handle_side_and_related_tags.py
+-rw-r--r--   0        0        0     1469 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/tag_update_builds.py
+-rw-r--r--   0        0        0     3706 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/tasks/work_on_bugs.py
+-rw-r--r--   0        0        0      105 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/comment.html
+-rw-r--r--   0        0        0     1331 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/comments.html
+-rw-r--r--   0        0        0     3575 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/compose.html
+-rw-r--r--   0        0        0     1270 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/composes.html
+-rw-r--r--   0        0        0      352 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/errors.html
+-rw-r--r--   0        0        0    15764 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/templates/fragments.html
+-rw-r--r--   0        0        0     5525 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/templates/home.html
+-rw-r--r--   0        0        0    10635 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/templates/master.html
+-rw-r--r--   0        0        0    20775 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/templates/new_update.html
+-rw-r--r--   0        0        0     9352 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/templates/override.html
+-rw-r--r--   0        0        0     9731 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/templates/overrides.html
+-rw-r--r--   0        0        0      882 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/pager.html
+-rw-r--r--   0        0        0    12532 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/templates/release.html
+-rw-r--r--   0        0        0     2938 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/bodhi/server/templates/releases.html
+-rw-r--r--   0        0        0    58854 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/bodhi/server/templates/update.html
+-rw-r--r--   0        0        0    15964 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/templates/updates.html
+-rw-r--r--   0        0        0     4796 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/templates/user.html
+-rw-r--r--   0        0        0    50367 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/bodhi/server/util.py
+-rw-r--r--   0        0        0    51587 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/bodhi/server/validators.py
+-rw-r--r--   0        0        0      812 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/views/__init__.py
+-rw-r--r--   0        0        0    22706 2023-07-30 14:36:52.000000 bodhi_server-7.2.1/bodhi/server/views/generic.py
+-rw-r--r--   0        0        0     3545 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/bodhi/server/webapp.py
+-rw-r--r--   0        0        0     1592 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/celeryconfig.py
+-rw-r--r--   0        0        0      776 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1757 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/conf.py
+-rw-r--r--   0        0        0        0 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/index.rst
+-rw-r--r--   0        0        0     1244 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/man_pages/bodhi-push.rst
+-rw-r--r--   0        0        0      797 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/man_pages/bodhi-sar.rst
+-rw-r--r--   0        0        0      523 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/man_pages/bodhi-shell.rst
+-rw-r--r--   0        0        0     1866 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/man_pages/bodhi-skopeo-lite.rst
+-rw-r--r--   0        0        0      718 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/man_pages/bodhi-untag-branched.rst
+-rw-r--r--   0        0        0      623 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/docs/man_pages/initialize_bodhi_db.rst
+-rw-r--r--   0        0        0    24410 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/production.ini
+-rw-r--r--   0        0        0     4959 2023-07-30 14:40:41.000000 bodhi_server-7.2.1/pyproject.toml
+-rw-r--r--   0        0        0      418 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/setup.cfg
+-rw-r--r--   0        0        0      816 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/auth/__init__.py
+-rw-r--r--   0        0        0     4790 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/auth/test_fedora.py
+-rw-r--r--   0        0        0    16947 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/auth/test_oauth.py
+-rw-r--r--   0        0        0     5487 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/auth/test_utils.py
+-rw-r--r--   0        0        0     5442 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/auth/test_views.py
+-rw-r--r--   0        0        0     2293 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/auth/utils.py
+-rw-r--r--   0        0        0    19141 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/base.py
+-rw-r--r--   0        0        0     2214 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      821 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/__init__.py
+-rwxr-xr-x   0        0        0      335 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/pungi.basepath/fake-pungi.sh
+-rw-r--r--   0        0        0       76 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/pungi.basepath/pungi.module.conf
+-rw-r--r--   0        0        0       76 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/pungi.basepath/pungi.rpm.conf
+-rw-r--r--   0        0        0      210 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/pungi.basepath/variants.module.xml.j2
+-rw-r--r--   0        0        0       76 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/pungi.basepath/variants.rpm.xml.j2
+-rw-r--r--   0        0        0    20022 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/test_automatic_updates.py
+-rw-r--r--   0        0        0    11457 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/test_ci.py
+-rw-r--r--   0        0        0     4779 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/consumers/test_consumers.py
+-rw-r--r--   0        0        0    14326 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/tests/consumers/test_resultsdb.py
+-rw-r--r--   0        0        0    13241 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/consumers/test_signed.py
+-rw-r--r--   0        0        0    10129 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/tests/consumers/test_waiverdb.py
+-rw-r--r--   0        0        0      913 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/functional/__init__.py
+-rw-r--r--   0        0        0     2571 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/functional/test_packages.py
+-rw-r--r--   0        0        0     8272 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/functional/test_users.py
+-rw-r--r--   0        0        0      819 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     2072 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/test_bshell.py
+-rw-r--r--   0        0        0     5128 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/test_compat.py
+-rw-r--r--   0        0        0     3597 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/test_initializedb.py
+-rw-r--r--   0        0        0     5341 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/test_sar.py
+-rw-r--r--   0        0        0    26242 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/test_skopeo_lite.py
+-rw-r--r--   0        0        0    15411 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/scripts/test_untag_branched.py
+-rw-r--r--   0        0        0      820 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/__init__.py
+-rw-r--r--   0        0        0     4067 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_builds.py
+-rw-r--r--   0        0        0    27002 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_comments.py
+-rw-r--r--   0        0        0     6469 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_composes.py
+-rw-r--r--   0        0        0     1512 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_csrf.py
+-rw-r--r--   0        0        0     1827 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_errors.py
+-rw-r--r--   0        0        0    31133 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_overrides.py
+-rw-r--r--   0        0        0    30447 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/tests/services/test_releases.py
+-rw-r--r--   0        0        0     3801 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/services/test_schemas.py
+-rw-r--r--   0        0        0   298709 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/services/test_updates.py
+-rw-r--r--   0        0        0      817 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1531 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/base.py
+-rw-r--r--   0        0        0    42724 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/tasks/test_approve_testing.py
+-rw-r--r--   0        0        0    29342 2023-05-14 16:00:16.000000 bodhi_server-7.2.1/tests/tasks/test_check_policies.py
+-rw-r--r--   0        0        0     8649 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_check_signed_builds.py
+-rw-r--r--   0        0        0     5949 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_clean_old_composes.py
+-rw-r--r--   0        0        0   175797 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/tasks/test_composer.py
+-rw-r--r--   0        0        0     3792 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_expire_overrides.py
+-rw-r--r--   0        0        0     3677 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_fetch_test_cases.py
+-rw-r--r--   0        0        0     2799 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_handle_side_and_related_tags.py
+-rw-r--r--   0        0        0     2321 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_tag_update_builds.py
+-rw-r--r--   0        0        0     5085 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/tasks/test_work_on_bugs.py
+-rw-r--r--   0        0        0    11553 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/tests/test___init__.py
+-rw-r--r--   0        0        0     2185 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_alembic.py
+-rw-r--r--   0        0        0    28061 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_bugs.py
+-rw-r--r--   0        0        0    17610 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_buildsys.py
+-rw-r--r--   0        0        0    16269 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_config.py
+-rw-r--r--   0        0        0     4319 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_logging.py
+-rw-r--r--   0        0        0    15586 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_mail.py
+-rw-r--r--   0        0        0    25674 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_metadata.py
+-rw-r--r--   0        0        0   218469 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/test_models.py
+-rw-r--r--   0        0        0     3897 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_notifications.py
+-rw-r--r--   0        0        0    72085 2023-05-20 13:22:54.000000 bodhi_server-7.2.1/tests/test_push.py
+-rw-r--r--   0        0        0     2238 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_renderers.py
+-rw-r--r--   0        0        0     1642 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_schemas.py
+-rw-r--r--   0        0        0     7195 2023-07-02 08:57:04.000000 bodhi_server-7.2.1/tests/test_security.py
+-rw-r--r--   0        0        0    69803 2023-07-26 16:45:28.000000 bodhi_server-7.2.1/tests/test_util.py
+-rw-r--r--   0        0        0    44301 2023-07-30 14:37:08.000000 bodhi_server-7.2.1/tests/test_validators.py
+-rw-r--r--   0        0        0     2614 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/test_webapp.py
+-rw-r--r--   0        0        0     4217 2023-05-20 16:26:19.000000 bodhi_server-7.2.1/tests/testing.ini
+-rw-r--r--   0        0        0      992 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/utils.py
+-rw-r--r--   0        0        0      817 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/views/__init__.py
+-rw-r--r--   0        0        0    23763 2023-05-13 08:55:56.000000 bodhi_server-7.2.1/tests/views/test_generic.py
+-rw-r--r--   0        0        0     5806 1970-01-01 00:00:00.000000 bodhi_server-7.2.1/setup.py
+-rw-r--r--   0        0        0     4036 1970-01-01 00:00:00.000000 bodhi_server-7.2.1/PKG-INFO
```

### Comparing `bodhi_server-7.2.0/COPYING` & `bodhi_server-7.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/README.rst` & `bodhi_server-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/alembic.ini` & `bodhi_server-7.2.1/alembic.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/apache/bodhi.conf` & `bodhi_server-7.2.1/apache/bodhi.conf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/__init__.py` & `bodhi_server-7.2.1/bodhi/server/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/__init__.py` & `bodhi_server-7.2.1/bodhi/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/fedora.py` & `bodhi_server-7.2.1/bodhi/server/auth/fedora.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/oauth.py` & `bodhi_server-7.2.1/bodhi/server/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/oauth_015.py` & `bodhi_server-7.2.1/bodhi/server/auth/oauth_015.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/oauth_1.py` & `bodhi_server-7.2.1/bodhi/server/auth/oauth_1.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/utils.py` & `bodhi_server-7.2.1/bodhi/server/auth/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/auth/views.py` & `bodhi_server-7.2.1/bodhi/server/auth/views.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/bugs.py` & `bodhi_server-7.2.1/bodhi/server/bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/buildsys.py` & `bodhi_server-7.2.1/bodhi/server/buildsys.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/config.py` & `bodhi_server-7.2.1/bodhi/server/config.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/__init__.py` & `bodhi_server-7.2.1/bodhi/server/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/automatic_updates.py` & `bodhi_server-7.2.1/bodhi/server/consumers/automatic_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/ci.py` & `bodhi_server-7.2.1/bodhi/server/consumers/ci.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/resultsdb.py` & `bodhi_server-7.2.1/bodhi/server/consumers/resultsdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/signed.py` & `bodhi_server-7.2.1/bodhi/server/consumers/signed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/util.py` & `bodhi_server-7.2.1/bodhi/server/consumers/util.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/consumers/waiverdb.py` & `bodhi_server-7.2.1/bodhi/server/consumers/waiverdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_errata_template.tpl` & `bodhi_server-7.2.1/bodhi/server/email/templates/fedora_epel_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl` & `bodhi_server-7.2.1/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_errata_template.tpl` & `bodhi_server-7.2.1/bodhi/server/email/templates/fedora_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_modular_errata_template.tpl` & `bodhi_server-7.2.1/bodhi/server/email/templates/fedora_modular_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/exceptions.py` & `bodhi_server-7.2.1/bodhi/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/ffmarkdown.py` & `bodhi_server-7.2.1/bodhi/server/ffmarkdown.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/logging.py` & `bodhi_server-7.2.1/bodhi/server/logging.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/mail.py` & `bodhi_server-7.2.1/bodhi/server/mail.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/metadata.py` & `bodhi_server-7.2.1/bodhi/server/metadata.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/README.rst` & `bodhi_server-7.2.1/bodhi/server/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/__init__.py` & `bodhi_server-7.2.1/bodhi/server/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/env.py` & `bodhi_server-7.2.1/bodhi/server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/script.py.mako` & `bodhi_server-7.2.1/bodhi/server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/__init__.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py` & `bodhi_server-7.2.1/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/models.py` & `bodhi_server-7.2.1/bodhi/server/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3160,25 +3160,25 @@
                             action = UpdateRequest.testing
 
         # Add the appropriate 'pending' koji tag to this update, so tools like
         # AutoQA can compose repositories of them for testing.
         # If it's a new side-tag update, koji tags are managed by the celery task
         if action is UpdateRequest.testing and not self.from_tag:
             self.add_tag(self.release.pending_signing_tag)
+            if self.release.candidate_tag not in self.get_tags():
+                self.add_tag(self.release.candidate_tag)
         elif action is UpdateRequest.stable:
             self.add_tag(self.release.pending_stable_tag)
             if self.request == UpdateRequest.testing:
                 self.remove_tag(self.release.pending_testing_tag)
 
         # If an obsolete/unpushed build is being re-submitted, return
         # it to the pending state, and make sure it's tagged as a candidate
         if self.status in (UpdateStatus.obsolete, UpdateStatus.unpushed):
             self.status = UpdateStatus.pending
-            if self.release.candidate_tag not in self.get_tags():
-                self.add_tag(self.release.candidate_tag)
 
         self.request = action
 
         notes = notes and '. '.join(notes) + '.' or ''
         flash_notes = flash_notes and '. %s' % flash_notes
         log.debug(
             "%s has been submitted for %s. %s%s" % (
@@ -3247,15 +3247,16 @@
 
         for requirement in self._unsatisfied_requirements:
 
             if tests and requirement['testcase'] not in tests:
                 continue
 
             data = {
-                'subject': requirement['item'],
+                'subject_type': requirement['subject_type'],
+                'subject_identifier': requirement['subject_identifier'],
                 'testcase': requirement['testcase'],
                 'scenario': requirement.get('scenario', None),
                 'product_version': self.product_version,
                 'waived': True,
                 'username': username,
                 'comment': comment
             }
```

### Comparing `bodhi_server-7.2.0/bodhi/server/notifications.py` & `bodhi_server-7.2.1/bodhi/server/notifications.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/push.py` & `bodhi_server-7.2.1/bodhi/server/push.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/renderers.py` & `bodhi_server-7.2.1/bodhi/server/renderers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/schemas.py` & `bodhi_server-7.2.1/bodhi/server/schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/__init__.py` & `bodhi_server-7.2.1/bodhi/server/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/bshell.py` & `bodhi_server-7.2.1/bodhi/server/scripts/bshell.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/compat.py` & `bodhi_server-7.2.1/bodhi/server/scripts/compat.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/initializedb.py` & `bodhi_server-7.2.1/bodhi/server/scripts/initializedb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/sar.py` & `bodhi_server-7.2.1/bodhi/server/scripts/sar.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/skopeo_lite.py` & `bodhi_server-7.2.1/bodhi/server/scripts/skopeo_lite.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/scripts/untag_branched.py` & `bodhi_server-7.2.1/bodhi/server/scripts/untag_branched.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/security.py` & `bodhi_server-7.2.1/bodhi/server/security.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/__init__.py` & `bodhi_server-7.2.1/bodhi/server/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/builds.py` & `bodhi_server-7.2.1/bodhi/server/services/builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/comments.py` & `bodhi_server-7.2.1/bodhi/server/services/comments.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/composes.py` & `bodhi_server-7.2.1/bodhi/server/services/composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/csrf.py` & `bodhi_server-7.2.1/bodhi/server/services/csrf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/errors.py` & `bodhi_server-7.2.1/bodhi/server/services/errors.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/markdown.py` & `bodhi_server-7.2.1/bodhi/server/services/markdown.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/metrics_tween.py` & `bodhi_server-7.2.1/bodhi/server/services/metrics_tween.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/overrides.py` & `bodhi_server-7.2.1/bodhi/server/services/overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/packages.py` & `bodhi_server-7.2.1/bodhi/server/services/packages.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/releases.py` & `bodhi_server-7.2.1/bodhi/server/services/releases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/schemas.py` & `bodhi_server-7.2.1/bodhi/server/services/schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/updates.py` & `bodhi_server-7.2.1/bodhi/server/services/updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/services/user.py` & `bodhi_server-7.2.1/bodhi/server/services/user.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/__init__.py` & `bodhi_server-7.2.1/bodhi/server/static/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/bodhi-logo.svg` & `bodhi_server-7.2.1/bodhi/server/static/bodhi-logo.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/css/site.css` & `bodhi_server-7.2.1/bodhi/server/static/css/site.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/FontAwesome.otf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome.css` & `bodhi_server-7.2.1/bodhi/server/static/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/hack.css` & `bodhi_server-7.2.1/bodhi/server/static/fonts/hack.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans.css` & `bodhi_server-7.2.1/bodhi/server/static/fonts/open-sans.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/ico/favicon.ico` & `bodhi_server-7.2.1/bodhi/server/static/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.png` & `bodhi_server-7.2.1/bodhi/server/static/img/bodhi-logo.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.svg` & `bodhi_server-7.2.1/bodhi/server/static/img/bodhi-logo.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/img/logo-large.png` & `bodhi_server-7.2.1/bodhi/server/static/img/logo-large.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/img/logo.png` & `bodhi_server-7.2.1/bodhi/server/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/js/comment_form.js` & `bodhi_server-7.2.1/bodhi/server/static/js/comment_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/js/forms.js` & `bodhi_server-7.2.1/bodhi/server/static/js/forms.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/js/override_form.js` & `bodhi_server-7.2.1/bodhi/server/static/js/override_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/js/search.js` & `bodhi_server-7.2.1/bodhi/server/static/js/search.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/js/site.js` & `bodhi_server-7.2.1/bodhi/server/static/js/site.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/js/update_form.js` & `bodhi_server-7.2.1/bodhi/server/static/js/update_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/chartjs/chart.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/chartjs/chart.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map` & `bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map` & `bodhi_server-7.2.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map` & `bodhi_server-7.2.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-spinner.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-spinner.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/css/messenger.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/messenger/js/messenger.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/moment/moment.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.0.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.0.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.1.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.1.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.1.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.1.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.0.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.0.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.1.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.1.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css` & `bodhi_server-7.2.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/static/vendor/typeahead/typeahead.bundle.js` & `bodhi_server-7.2.1/bodhi/server/static/vendor/typeahead/typeahead.bundle.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/__init__.py` & `bodhi_server-7.2.1/bodhi/server/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/approve_testing.py` & `bodhi_server-7.2.1/bodhi/server/tasks/approve_testing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/check_policies.py` & `bodhi_server-7.2.1/bodhi/server/tasks/check_policies.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/check_signed_builds.py` & `bodhi_server-7.2.1/bodhi/server/tasks/check_signed_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/clean_old_composes.py` & `bodhi_server-7.2.1/bodhi/server/tasks/clean_old_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/composer.py` & `bodhi_server-7.2.1/bodhi/server/tasks/composer.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/expire_overrides.py` & `bodhi_server-7.2.1/bodhi/server/tasks/expire_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/fetch_test_cases.py` & `bodhi_server-7.2.1/bodhi/server/tasks/fetch_test_cases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/handle_side_and_related_tags.py` & `bodhi_server-7.2.1/bodhi/server/tasks/handle_side_and_related_tags.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/tag_update_builds.py` & `bodhi_server-7.2.1/bodhi/server/tasks/tag_update_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/tasks/work_on_bugs.py` & `bodhi_server-7.2.1/bodhi/server/tasks/work_on_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/comments.html` & `bodhi_server-7.2.1/bodhi/server/templates/comments.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/compose.html` & `bodhi_server-7.2.1/bodhi/server/templates/compose.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/composes.html` & `bodhi_server-7.2.1/bodhi/server/templates/composes.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/fragments.html` & `bodhi_server-7.2.1/bodhi/server/templates/fragments.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/home.html` & `bodhi_server-7.2.1/bodhi/server/templates/home.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/master.html` & `bodhi_server-7.2.1/bodhi/server/templates/master.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/new_update.html` & `bodhi_server-7.2.1/bodhi/server/templates/new_update.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/override.html` & `bodhi_server-7.2.1/bodhi/server/templates/override.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/overrides.html` & `bodhi_server-7.2.1/bodhi/server/templates/overrides.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/pager.html` & `bodhi_server-7.2.1/bodhi/server/templates/pager.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/release.html` & `bodhi_server-7.2.1/bodhi/server/templates/release.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/releases.html` & `bodhi_server-7.2.1/bodhi/server/templates/releases.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/update.html` & `bodhi_server-7.2.1/bodhi/server/templates/update.html`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
             % endif
           </p>
           % endif
 
           % if install_command:
           <div class="pt-2">
           <h4>How to install</h4>
+            <p class="mb-1">Updates may require up to 24 hours to propagate to mirrors. If the following command doesn't work, please retry later:</p>
             <pre style="position: relative;"><span class="badge text-bg-secondary" id="copybutton" style="position: absolute; top: 0px; right: 0px; cursor: pointer;" title="Copy to clipboard"><i class="fa fa-copy"></i></span><code id="commandtext">${install_command}</code></pre>
           </div>
           % endif
 
           <div class="pt-2 mt-4 border-top">
             <!--<h4>Comments <span class="badge text-bg-secondary">${len(update.comments)}</span>
               <small><a href="${request.route_url('comments_rss')}?updates=${update.alias}">
@@ -631,14 +632,20 @@
         % endfor
       </div>
     </div>
 
     <div class="tab-pane" id="automatedtests-tab-pane" role="tabpanel" aria-labelledby="automatedtests-tab" tabindex="0">
       <div id="resultsdb">
         <h3>Automated Test Results</h3>
+        % if update.test_gating_status == models.TestGatingStatus.failed:
+        <div class="alert alert-danger" role="alert">
+          For help debugging failed Fedora CI tests (fedora-ci.*), contact <a href="https://web.libera.chat/?channels=#fedora-ci" target="_blank">#fedora-ci on Libera.chat</a><br/>
+          For help debugging failed openQA tests (update.*), contact <a href="https://matrix.to/#/#quality:fedoraproject.org" target="_blank">the Fedora Quality team</a>, who will usually investigate and diagnose all failures within 24 hours
+        </div>
+        % endif
         <div id="gating-summary-tab">
           <a class="gating-summary notblue">${update.test_gating_status}</a>
           <i class="fa spinner fa-spinner fa-spin fa-fw"></i>
         </div>
       </div>
     </div>
 
@@ -776,16 +783,20 @@
     // These are the required taskotron tests
     var requirements = ${update.requirements_json | h};
     // These are the known waivers of failed testcases.
     var waivers = {};
     // show the Greenwave decision
     var greenwave_api_url = '${request.registry.settings["greenwave_api_url"]}';
     var missing_tests = {};
-    var reqs_counter = 0;
+    var invalid_gating_repos = [];
+    var missing_gating_repos = [];
+    var failed_fetch_gating_repos = [];
+    var test_reqs_counter = 0;
     var unsatisfied_reqs_counter = 0;
+    var remoteerror_reqs_counter = 0;
     var missing_reqs_counter = 0;
     var running_reqs_counter = 0;
     var greenwave_errors = 0;
 
     // handle Greenwave decision
     var handle_unsatisfied_requirements = function(data){
         $.each(data['unsatisfied_requirements'], function(i, requirement) {
@@ -797,14 +808,25 @@
                 else {
                     missing_reqs_counter++;
                     if (missing_tests[requirement.subject_identifier] === undefined)
                         missing_tests[requirement.subject_identifier] = [];
                     missing_tests[requirement.subject_identifier].push(requirement);
                 }
             }
+            if (requirement.type.match('gating-yaml')) {
+                remoteerror_reqs_counter++;
+                // these aren't 'test results' exactly
+                test_reqs_counter--;
+                if (requirement.type == 'invalid-gating-yaml')
+                    invalid_gating_repos.push(requirement.subject_identifier);
+                if (requirement.type == 'missing-gating-yaml')
+                    missing_gating_repos.push(requirement.subject_identifier);
+                if (requirement.type == 'failed-fetch-gating-yaml')
+                    failed_fetch_gating_repos.push(requirement.subject_identifier);
+            }
             // the user may have already specified this in the required taskotron tests
             if ($.inArray(requirement.testcase, requirements) == -1) {
                 requirements.push(requirement.testcase);
             }
             $('#failed_requirements').append('<li class="list-group-item">' + requirement.testcase + '</li>');
 
             // there is at least one unsatisfied requirement, so show the button to be able to waive.
@@ -823,26 +845,29 @@
           label_class = classes['FAILED'];
           icon_class = icons['FAILED'];
         } else {
           label_class = classes['PASSED'];
           icon_class = icons['PASSED'];
         }
         var summary = [];
-        failed_reqs_counter = unsatisfied_reqs_counter - missing_reqs_counter - running_reqs_counter;
-        if (reqs_counter == 0) {
+        failed_reqs_counter = unsatisfied_reqs_counter - missing_reqs_counter - running_reqs_counter - remoteerror_reqs_counter;
+        if (test_reqs_counter == 0) {
             summary = ['no tests are required'];
         } else {
             if (failed_reqs_counter > 0) {
-                summary.push(failed_reqs_counter + ' of ' + reqs_counter + ' required tests failed');
+                summary.push(failed_reqs_counter + ' of ' + test_reqs_counter + ' required tests failed');
             }
             if (running_reqs_counter > 0) {
-                summary.push(running_reqs_counter + ' of ' + reqs_counter + ' required tests running');
+                summary.push(running_reqs_counter + ' of ' + test_reqs_counter + ' required tests running');
             }
             if (missing_reqs_counter > 0) {
-                summary.push(missing_reqs_counter + ' of ' + reqs_counter + ' required test results missing');
+                summary.push(missing_reqs_counter + ' of ' + test_reqs_counter + ' required test results missing');
+            }
+            if (remoteerror_reqs_counter > 0) {
+                summary.push(remoteerror_reqs_counter + ' errors handling remote rules');
             }
             if (summary.length == 0) {
                 summary = ['All required tests passed'];
             }
         }
         summary = summary.join(', ')
 
@@ -890,16 +915,22 @@
             data: JSON.stringify(request),
             success: function(data) {
                 $.each(data.waivers, function(i, waiver) {
                   if (!(waiver.testcase in waivers)) { waivers[waiver.testcase] = []; }
                   waivers[waiver.testcase].push(waiver);
                 });
                 handle_unsatisfied_requirements(data);
-                reqs_counter += data['unsatisfied_requirements'].length;
-                reqs_counter += data['satisfied_requirements'].length;
+                $.each(data['satisfied_requirements'], function(i, requirement) {
+                    // the user may have already specified this in the required taskotron tests
+                    if ($.inArray(requirement.testcase, requirements) == -1) {
+                        requirements.push(requirement.testcase);
+                    }
+                });
+                test_reqs_counter += data['unsatisfied_requirements'].length;
+                test_reqs_counter += data['satisfied_requirements'].length;
                 handle_results(data.results, request.subject);
                 after_success();
             },
             error: function (jqxhr, status, error) {
                greenwave_errors = 1;
                finish();
             },
@@ -1009,26 +1040,53 @@
         if (!(buildname in missing_tests) && results.length === 0) {
           $("#resultsdb").append("<p>No results reported for this build.</p>");
           return;
         }
 
         var table = $("<table class='table table-hover'><tbody></tbody></table>").appendTo("#resultsdb");
 
-        // show missing tests first
+        // show missing tests and remote rule yaml problems first
         if (buildname in missing_tests) {
           $.each(missing_tests[buildname], function(i, result) {
             table.append(make_row(
               'ABSENT',
               result.testcase,
               '',
               '',
               ''
             ));
           });
         }
+        $.each(invalid_gating_repos, function (i, repo) {
+          table.append(make_row(
+            'FAILED',
+            repo,
+            'remote policy gating.yaml parsing failed',
+            '',
+            ''
+          ));
+        });
+        $.each(missing_gating_repos, function (i, repo) {
+          table.append(make_row(
+            'FAILED',
+            repo,
+            'remote policy gating.yaml missing',
+            '',
+            ''
+          ));
+        });
+        $.each(failed_fetch_gating_repos, function (i, repo) {
+          table.append(make_row(
+            'FAILED',
+            repo,
+            'remote policy gating.yaml retrieval failed',
+            '',
+            ''
+          ));
+        });
 
         $.each(results, function(i, result) {
           var scenario = 'no_scenario';
           if (result.data.scenario) {
               scenario = result.data.scenario[0];
           }
```

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/updates.html` & `bodhi_server-7.2.1/bodhi/server/templates/updates.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/templates/user.html` & `bodhi_server-7.2.1/bodhi/server/templates/user.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/util.py` & `bodhi_server-7.2.1/bodhi/server/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         # Now call out to DNF to check if the repo is usable
         # "tests" is a list of tuples with (dnf args, expected output) to run.
         # For every test, DNF is run with the arguments, and if the expected output is not found,
         #  an error is raised.
         tests = []
 
         if repo_type in ('yum', 'source'):
-            tests.append((['list', 'available'], 'testrepo'))
+            tests.append((['list', '--available'], 'testrepo'))
         else:  # repo_type == 'module', verified above
             tests.append((['module', 'list'], '.*'))
 
         for test in tests:
             dnfargs, expout = test
 
             # Make sure every DNF test runs in a new temp dir
```

### Comparing `bodhi_server-7.2.0/bodhi/server/validators.py` & `bodhi_server-7.2.1/bodhi/server/validators.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/views/__init__.py` & `bodhi_server-7.2.1/bodhi/server/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/views/generic.py` & `bodhi_server-7.2.1/bodhi/server/views/generic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/bodhi/server/webapp.py` & `bodhi_server-7.2.1/bodhi/server/webapp.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/celeryconfig.py` & `bodhi_server-7.2.1/celeryconfig.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/Makefile` & `bodhi_server-7.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/conf.py` & `bodhi_server-7.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/man_pages/bodhi-push.rst` & `bodhi_server-7.2.1/docs/man_pages/bodhi-push.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/man_pages/bodhi-sar.rst` & `bodhi_server-7.2.1/docs/man_pages/bodhi-sar.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/man_pages/bodhi-shell.rst` & `bodhi_server-7.2.1/docs/man_pages/bodhi-shell.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/man_pages/bodhi-skopeo-lite.rst` & `bodhi_server-7.2.1/docs/man_pages/bodhi-skopeo-lite.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/man_pages/bodhi-untag-branched.rst` & `bodhi_server-7.2.1/docs/man_pages/bodhi-untag-branched.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/docs/man_pages/initialize_bodhi_db.rst` & `bodhi_server-7.2.1/docs/man_pages/initialize_bodhi_db.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/production.ini` & `bodhi_server-7.2.1/production.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/pyproject.toml` & `bodhi_server-7.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-server"
-version = "7.2.0"
+version = "7.2.1"
 description = "Bodhi server"
 readme = "README.rst"
 authors = ["Fedora Infrastructure Team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 repository = "https://github.com/fedora-infra/bodhi"
 homepage = "https://bodhi.fedoraproject.rog"
 keywords = ["web", "fedora", "pyramid"]
@@ -62,14 +62,17 @@
     { path = "docs", format = "sdist" },
         ]
 exclude = [
     { path = "development.ini", format = "sdist" },
     { path = "docs/_build", format = "sdist" }
         ]
 
+[tool.poetry.build]
+generate-setup-file = true
+
 [tool.poetry.dev-dependencies]
 bodhi-messages = {path = "../bodhi-messages"}
 pytest = ">=6.2.2"
 pytest-cov = ">=2.11.1"
 pytest-mock = ">=3.5.1"
 diff-cover = ">=4.2.1"
 responses = ">=0.10.15"
```

### Comparing `bodhi_server-7.2.0/tests/__init__.py` & `bodhi_server-7.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/auth/test_fedora.py` & `bodhi_server-7.2.1/tests/auth/test_fedora.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/auth/test_oauth.py` & `bodhi_server-7.2.1/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/auth/test_utils.py` & `bodhi_server-7.2.1/tests/auth/test_utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/auth/test_views.py` & `bodhi_server-7.2.1/tests/auth/test_views.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/auth/utils.py` & `bodhi_server-7.2.1/tests/auth/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/base.py` & `bodhi_server-7.2.1/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,15 +503,23 @@
     <_name>Testable</_name>
     <_description>comps group for testing</_description>
     <packagelist>
       <packagereq>testpkg</packagereq>
     </packagelist>
   </group>
 </comps>'''
-    updateinfofile = 'something<id>someID</id>something'
+
+    updateinfofile = '''<?xml version="1.0" encoding="UTF-8"?>
+<updates>
+  <update>
+    <id>someID</id>
+    <title>something</title>
+  </update>
+</updates>'''
+
     if not os.path.isdir(path):
         os.makedirs(path)
     if not comps and not source:
         comps = os.path.join(path, 'comps.xml')
         with open(comps, 'w') as f:
             f.write(compsfile)
     if updateinfo is None:
```

### Comparing `bodhi_server-7.2.0/tests/conftest.py` & `bodhi_server-7.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/consumers/__init__.py` & `bodhi_server-7.2.1/tests/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/consumers/test_automatic_updates.py` & `bodhi_server-7.2.1/tests/consumers/test_automatic_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/consumers/test_ci.py` & `bodhi_server-7.2.1/tests/consumers/test_ci.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/consumers/test_consumers.py` & `bodhi_server-7.2.1/tests/consumers/test_consumers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/consumers/test_resultsdb.py` & `bodhi_server-7.2.1/tests/consumers/test_resultsdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/consumers/test_signed.py` & `bodhi_server-7.2.1/tests/consumers/test_signed.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,8 +321,8 @@
                 self.handler(self.sample_side_tag_message_2)
 
         assert update.builds[0].signed is True
         assert update.builds[0].update.request == UpdateRequest.testing
         assert update.status == UpdateStatus.pending
         assert update.pushed is False
         assert update.test_gating_status == TestGatingStatus.passed
-        assert add_tag.not_called()
+        add_tag.assert_not_called()
```

### Comparing `bodhi_server-7.2.0/tests/consumers/test_waiverdb.py` & `bodhi_server-7.2.1/tests/consumers/test_waiverdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/functional/__init__.py` & `bodhi_server-7.2.1/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/functional/test_packages.py` & `bodhi_server-7.2.1/tests/functional/test_packages.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/functional/test_users.py` & `bodhi_server-7.2.1/tests/functional/test_users.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/__init__.py` & `bodhi_server-7.2.1/tests/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/test_bshell.py` & `bodhi_server-7.2.1/tests/scripts/test_bshell.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/test_compat.py` & `bodhi_server-7.2.1/tests/scripts/test_compat.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/test_initializedb.py` & `bodhi_server-7.2.1/tests/scripts/test_initializedb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/test_sar.py` & `bodhi_server-7.2.1/tests/scripts/test_sar.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/test_skopeo_lite.py` & `bodhi_server-7.2.1/tests/scripts/test_skopeo_lite.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/scripts/test_untag_branched.py` & `bodhi_server-7.2.1/tests/scripts/test_untag_branched.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/__init__.py` & `bodhi_server-7.2.1/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_builds.py` & `bodhi_server-7.2.1/tests/services/test_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_comments.py` & `bodhi_server-7.2.1/tests/services/test_comments.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_composes.py` & `bodhi_server-7.2.1/tests/services/test_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_csrf.py` & `bodhi_server-7.2.1/tests/services/test_csrf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_errors.py` & `bodhi_server-7.2.1/tests/services/test_errors.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_overrides.py` & `bodhi_server-7.2.1/tests/services/test_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_releases.py` & `bodhi_server-7.2.1/tests/services/test_releases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_schemas.py` & `bodhi_server-7.2.1/tests/services/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/services/test_updates.py` & `bodhi_server-7.2.1/tests/services/test_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -6222,18 +6222,16 @@
             self, greenwave_api_post, waiverdb_api_post, *args):
         """Ensure that waiverdb and greenwaved are properly called when greenwave returns only one
         unsatisfied requirements."""
         nvr = 'bodhi-2.0-1.fc17'
         greenwave_api_post.return_value = {
             'unsatisfied_requirements': [
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'dist.rpmdeplint',
                     'type': 'test-result-failed'
                 }
             ],
         }
 
@@ -6262,17 +6260,16 @@
             {
                 'username': 'guest',
                 'comment': 'This is expected',
                 'waived': True,
                 'product_version': 'fedora-17',
                 'testcase': 'dist.rpmdeplint',
                 'scenario': None,
-                'subject': {
-                    'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                }
+                'subject_identifier': 'bodhi-2.0-1.fc17',
+                'subject_type': 'koji_build'
             }
         )
 
         assert list(res.json_body.keys()) == ['update']
         assert res.json_body['update'] == up.__json__()
         assert res.json_body['update']['test_gating_status'] == 'waiting'
         up = self.db.query(Build).filter_by(nvr=nvr).one().update
@@ -6292,27 +6289,23 @@
             self, greenwave_api_post, waiverdb_api_post, *args):
         """Ensure that waiverdb and greenwaved are properly called when greenwave returns two
         unsatisfied requirements."""
         nvr = 'bodhi-2.0-1.fc17'
         greenwave_api_post.return_value = {
             'unsatisfied_requirements': [
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'dist.rpmdeplint',
                     'type': 'test-result-failed'
                 },
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'atomic_ci_pipeline_results',
                     'type': 'test-result-failed'
                 }
             ],
         }
 
@@ -6342,31 +6335,29 @@
                 {
                     'username': 'guest',
                     'comment': None,
                     'waived': True,
                     'product_version': 'fedora-17',
                     'testcase': 'dist.rpmdeplint',
                     'scenario': None,
-                    'subject': {
-                        'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                    }
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build'
                 }
             ),
             mock.call(
                 'https://waiverdb-web-waiverdb.app.os.fedoraproject.org/api/v1.0/waivers/',
                 {
                     'username': 'guest',
                     'comment': None,
                     'waived': True,
                     'product_version': 'fedora-17',
                     'testcase': 'atomic_ci_pipeline_results',
                     'scenario': None,
-                    'subject': {
-                        'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                    }
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build'
                 }
             )
         ]
         assert waiverdb_api_post.mock_calls == calls
 
         assert list(res.json_body.keys()) == ['update']
         assert res.json_body['update'] == up.__json__()
@@ -6388,27 +6379,23 @@
             self, greenwave_api_post, waiverdb_api_post, *args):
         """Ensure that waiverdb and greenwaved are properly called when greenwave returns only two
         unsatisfied requirements but only one of them is waived."""
         nvr = 'bodhi-2.0-1.fc17'
         greenwave_api_post.return_value = {
             'unsatisfied_requirements': [
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'dist.rpmdeplint',
                     'type': 'test-result-failed'
                 },
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'atomic_ci_pipeline_results',
                     'type': 'test-result-failed'
                 }
             ],
         }
 
@@ -6441,17 +6428,16 @@
             {
                 'username': 'guest',
                 'comment': None,
                 'waived': True,
                 'product_version': 'fedora-17',
                 'testcase': 'atomic_ci_pipeline_results',
                 'scenario': None,
-                'subject': {
-                    'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                }
+                'subject_identifier': 'bodhi-2.0-1.fc17',
+                'subject_type': 'koji_build'
             }
         )
 
         assert list(res.json_body.keys()) == ['update']
         assert res.json_body['update'] == up.__json__()
         assert res.json_body['update']['test_gating_status'] == 'waiting'
         up = self.db.query(Build).filter_by(nvr=nvr).one().update
@@ -6471,27 +6457,23 @@
             self, greenwave_api_post, waiverdb_api_post, *args):
         """Ensure that waiverdb and greenwaved are properly called when greenwave returns only two
         unsatisfied requirements and both of them are waived."""
         nvr = 'bodhi-2.0-1.fc17'
         greenwave_api_post.return_value = {
             'unsatisfied_requirements': [
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'dist.rpmdeplint',
                     'type': 'test-result-failed'
                 },
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'atomic_ci_pipeline_results',
                     'type': 'test-result-failed'
                 }
             ],
         }
 
@@ -6525,31 +6507,29 @@
                 {
                     'username': 'guest',
                     'comment': None,
                     'waived': True,
                     'product_version': 'fedora-17',
                     'testcase': 'dist.rpmdeplint',
                     'scenario': None,
-                    'subject': {
-                        'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                    }
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build'
                 }
             ),
             mock.call(
                 'https://waiverdb-web-waiverdb.app.os.fedoraproject.org/api/v1.0/waivers/',
                 {
                     'username': 'guest',
                     'comment': None,
                     'waived': True,
                     'product_version': 'fedora-17',
                     'testcase': 'atomic_ci_pipeline_results',
                     'scenario': None,
-                    'subject': {
-                        'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                    }
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build'
                 }
             )
         ]
         assert waiverdb_api_post.mock_calls == calls
 
         assert list(res.json_body.keys()) == ['update']
         assert res.json_body['update'] == up.__json__()
@@ -6571,27 +6551,23 @@
             self, greenwave_api_post, waiverdb_api_post, *args):
         """Ensure that waiverdb and greenwaved are properly called when greenwave returns only two
         unsatisfied requirements and one of the two asked to be waived isn't a requirement."""
         nvr = 'bodhi-2.0-1.fc17'
         greenwave_api_post.return_value = {
             'unsatisfied_requirements': [
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'dist.rpmdeplint',
                     'type': 'test-result-failed'
                 },
                 {
-                    'item': {
-                        'item': 'bodhi-2.0-1.fc17',
-                        'type': 'koji_build'
-                    },
+                    'subject_identifier': 'bodhi-2.0-1.fc17',
+                    'subject_type': 'koji_build',
                     'scenario': None,
                     'testcase': 'atomic_ci_pipeline_results',
                     'type': 'test-result-failed'
                 }
             ],
         }
 
@@ -6624,17 +6600,16 @@
             {
                 'username': 'guest',
                 'comment': None,
                 'waived': True,
                 'product_version': 'fedora-17',
                 'testcase': 'dist.rpmdeplint',
                 'scenario': None,
-                'subject': {
-                    'item': 'bodhi-2.0-1.fc17', 'type': 'koji_build'
-                }
+                'subject_identifier': 'bodhi-2.0-1.fc17',
+                'subject_type': 'koji_build'
             }
         )
 
         assert list(res.json_body.keys()) == ['update']
         assert res.json_body['update'] == up.__json__()
         assert res.json_body['update']['test_gating_status'] == 'waiting'
         up = self.db.query(Build).filter_by(nvr=nvr).one().update
```

### Comparing `bodhi_server-7.2.0/tests/tasks/__init__.py` & `bodhi_server-7.2.1/tests/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/base.py` & `bodhi_server-7.2.1/tests/tasks/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_approve_testing.py` & `bodhi_server-7.2.1/tests/tasks/test_approve_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,15 +697,15 @@
             assert remove_tag.call_args_list == \
                 [call('f17-updates-testing-pending'), call('f17-updates-pending'),
                  call('f17-updates-signing-pending'), call('f17-updates-testing'),
                  call('f17-updates-candidate')]
 
             assert add_tag.call_args_list == \
                 [call('f17-updates')]
-            assert delete_tag.not_called()
+            delete_tag.assert_not_called()
         else:
             assert remove_tag.call_args_list == \
                 [call(f'{from_side_tag}-signing-pending'),
                  call(f'{from_side_tag}-testing-pending'),
                  call(from_side_tag)]
 
             assert add_tag.call_args_list == \
```

### Comparing `bodhi_server-7.2.0/tests/tasks/test_check_policies.py` & `bodhi_server-7.2.1/tests/tasks/test_check_policies.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_check_signed_builds.py` & `bodhi_server-7.2.1/tests/tasks/test_check_signed_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_clean_old_composes.py` & `bodhi_server-7.2.1/tests/tasks/test_clean_old_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_composer.py` & `bodhi_server-7.2.1/tests/tasks/test_composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3376,17 +3376,17 @@
         assert update.request == UpdateRequest.stable
         now = datetime.datetime.utcnow()
         assert (now - update.date_stable) < datetime.timedelta(seconds=5)
         assert update.date_testing is None
         assert (now - update.date_pushed) < datetime.timedelta(seconds=5)
         assert update.pushed
         if from_side_tag:
-            assert delete_tag.called_with('f34-build-side-0000')
+            delete_tag.assert_called_with('f34-build-side-0000')
         else:
-            assert delete_tag.not_called()
+            delete_tag.assert_not_called()
 
     def test_testing_update(self):
         """Assert that a testing update gets the right status."""
         update = Update.query.one()
         update.status = UpdateStatus.pending
         update.request = UpdateRequest.testing
         t = ComposerThread(self.semmock, self._make_task()['composes'][0],
```

### Comparing `bodhi_server-7.2.0/tests/tasks/test_expire_overrides.py` & `bodhi_server-7.2.1/tests/tasks/test_expire_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_fetch_test_cases.py` & `bodhi_server-7.2.1/tests/tasks/test_fetch_test_cases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_handle_side_and_related_tags.py` & `bodhi_server-7.2.1/tests/tasks/test_handle_side_and_related_tags.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_tag_update_builds.py` & `bodhi_server-7.2.1/tests/tasks/test_tag_update_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/tasks/test_work_on_bugs.py` & `bodhi_server-7.2.1/tests/tasks/test_work_on_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test___init__.py` & `bodhi_server-7.2.1/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_alembic.py` & `bodhi_server-7.2.1/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_bugs.py` & `bodhi_server-7.2.1/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_buildsys.py` & `bodhi_server-7.2.1/tests/test_buildsys.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_config.py` & `bodhi_server-7.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_logging.py` & `bodhi_server-7.2.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_mail.py` & `bodhi_server-7.2.1/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_metadata.py` & `bodhi_server-7.2.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_models.py` & `bodhi_server-7.2.1/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4002,14 +4002,43 @@
         assert self.obj.status == UpdateStatus.pending
 
         self.obj = mock.Mock()
         self.obj.remove_tag(self.obj.release.pending_testing_tag)
         self.obj.remove_tag.assert_called_once_with(self.obj.release.pending_testing_tag)
 
     @mock.patch('bodhi.server.models.buildsys.get_session')
+    def test_set_request_testing_ejected(self, get_session):
+        """
+        Ensure that set_request() adds the candidate tag back to an update which was
+        previously ejected from push.
+        """
+        req = DummyRequest(user=DummyUser())
+        req.errors = cornice.Errors()
+        req.koji = get_session.return_value
+        self.obj.status = UpdateStatus.pending
+        self.obj.request = None
+        expected_message = update_schemas.UpdateRequestTestingV1.from_dict(
+            {'update': self.obj, 'agent': req.user.name})
+
+        with mock_sends(expected_message):
+            self.obj.set_request(self.db, 'testing', req.user.name)
+            # set_request alters the update a bit, so we need to adjust the expected message to
+            # reflect those changes so the mock_sends() check will pass.
+            expected_message.body['update']['status'] = 'pending'
+            expected_message.body['update']['request'] = 'testing'
+            expected_message.body['update']['comments'] = self.obj.__json__()['comments']
+            self.db.commit()
+
+        assert self.obj.status == UpdateStatus.pending
+        assert self.obj.request == UpdateRequest.testing
+        assert get_session.return_value.tagBuild.mock_calls == (
+            [mock.call(self.obj.release.pending_signing_tag, self.obj.builds[0].nvr, force=True),
+             mock.call(self.obj.release.candidate_tag, self.obj.builds[0].nvr, force=True)])
+
+    @mock.patch('bodhi.server.models.buildsys.get_session')
     def test_set_request_resubmit_candidate_tag_missing(self, get_session):
         """Ensure that set_request() adds the candidate tag back to a resubmitted build."""
         req = DummyRequest(user=DummyUser())
         req.errors = cornice.Errors()
         req.koji = get_session.return_value
         self.obj.status = UpdateStatus.unpushed
         self.obj.request = None
@@ -4782,20 +4811,34 @@
         self.obj.status = UpdateStatus.testing
         self.obj.test_gating_status = TestGatingStatus.failed
         greenwave_api_post.return_value = {
             "policies_satisfied": False,
             "summary": "3 of 15 required tests failed",
             "applicable_policies": ["1"],
             "unsatisfied_requirements": [
-                {'item': {"item": "bodhi-3.6.0-1.fc28", "type": "koji_build"}, 'result_id': "123",
-                 'testcase': 'dist.depcheck', 'type': 'test-result-failed'},
-                {'item': {"item": "bodhi-3.6.0-1.fc28", "type": "koji_build"}, 'result_id': "124",
-                 'testcase': 'dist.rpmdeplint', 'type': 'test-result-failed'},
-                {'item': {"item": "bodhi-3.6.0-1.fc28", "type": "koji_build"}, 'result_id': "125",
-                 'testcase': 'dist.someothertest', 'type': 'test-result-failed'}]}
+                {
+                    'subject_identifier': "bodhi-3.6.0-1.fc28",
+                    'subject_type': "koji_build",
+                    'testcase': 'dist.depcheck',
+                    'type': 'test-result-failed'
+                },
+                {
+                    'subject_identifier': "bodhi-3.6.0-1.fc28",
+                    'subject_type': "koji_build",
+                    'testcase': 'dist.rpmdeplint',
+                    'type': 'test-result-failed'
+                },
+                {
+                    'subject_identifier': "bodhi-3.6.0-1.fc28",
+                    'subject_type': "koji_build",
+                    'testcase': 'dist.someothertest',
+                    'type': 'test-result-failed'
+                }
+            ]
+        }
         post.return_value.status_code = 200
 
         config.update({
             'test_gating.required': True,
             'waiverdb.access_token': 'abc',
         })
         self.obj.waive_test_results('foo', 'this is not true!')
@@ -4807,15 +4850,17 @@
         expected_calls = []
         for test in ('dist.depcheck', 'dist.rpmdeplint', 'dist.someothertest'):
             data = {
                 "username": "foo", "comment": "this is not true!", "waived": True,
                 "product_version": "{}".format(self.obj.product_version),
                 "testcase": "{}".format(test),
                 "scenario": None,
-                "subject": {"item": "bodhi-3.6.0-1.fc28", "type": "koji_build"}}
+                "subject_identifier": "bodhi-3.6.0-1.fc28",
+                "subject_type": "koji_build"
+            }
             expected_calls.append(mock.call(
                 '{}/waivers/'.format(config.get('waiverdb_api_url')),
                 data=json.dumps(data),
                 headers={'Content-Type': 'application/json', 'Authorization': 'Bearer abc'},
                 timeout=60))
             expected_calls.append(mock.call().json())
         for i, v in enumerate(expected_calls):
@@ -4842,30 +4887,31 @@
         update.test_gating_status = TestGatingStatus.failed
         decision = {
             "policies_satisfied": False,
             "summary": "1 of 15 required tests failed",
             "applicable_policies": ["1"],
             "unsatisfied_requirements": [
                 {
-                    'item': {"item": "%s" % update.builds[0].nvr, "type": "koji_build"},
-                    'result_id': "123",
+                    'subject_identifier': "%s" % update.builds[0].nvr,
+                    'subject_type': "koji_build",
                     'testcase': 'dist.depcheck',
                     'scenario': 'kde',
                     'type': 'test-result-failed'
                 }
             ]
         }
         mock_greenwave.return_value = decision
         config.update({
             'test_gating.required': True,
             'waiverdb.access_token': 'abc',
         })
         update.waive_test_results('foo', 'this is not true!')
         wdata = {
-            'subject': {"item": "%s" % update.builds[0].nvr, "type": "koji_build"},
+            'subject_identifier': "%s" % update.builds[0].nvr,
+            'subject_type': "koji_build",
             'testcase': 'dist.depcheck',
             'scenario': 'kde',
             'product_version': update.product_version,
             'waived': True,
             'username': 'foo',
             'comment': 'this is not true!'
         }
```

### Comparing `bodhi_server-7.2.0/tests/test_notifications.py` & `bodhi_server-7.2.1/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_push.py` & `bodhi_server-7.2.1/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_renderers.py` & `bodhi_server-7.2.1/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_schemas.py` & `bodhi_server-7.2.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_security.py` & `bodhi_server-7.2.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_util.py` & `bodhi_server-7.2.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/test_validators.py` & `bodhi_server-7.2.1/tests/test_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,17 @@
         """ Test validate_acls when an Exception is raised on getting package committers."""
         mock_request = self.get_mock_request()
         mock_gpcfp.side_effect = ValueError('some error')
         validators.validate_acls(mock_request)
         assert len(mock_request.errors) == 0
         mock_access.assert_called_once()
         mock_gpcfp.assert_called_once()
-        warning.called_once_with('Unable to retrieve committers list from Pagure for bodhi.')
+        warning.assert_called_once_with(
+            'Unable to retrieve committers list from Pagure for bodhi.'
+        )
 
     @mock.patch.dict('bodhi.server.validators.config', {'acl_system': 'dummy'})
     def test_validate_acls_dummy(self):
         """ Test validate_acls when the acl system is dummy.
         """
         mock_request = self.get_mock_request()
         validators.validate_acls(mock_request)
```

### Comparing `bodhi_server-7.2.0/tests/test_webapp.py` & `bodhi_server-7.2.1/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/testing.ini` & `bodhi_server-7.2.1/tests/testing.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/utils.py` & `bodhi_server-7.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/views/__init__.py` & `bodhi_server-7.2.1/tests/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/tests/views/test_generic.py` & `bodhi_server-7.2.1/tests/views/test_generic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.2.0/PKG-INFO` & `bodhi_server-7.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-server
-Version: 7.2.0
+Version: 7.2.1
 Summary: Bodhi server
 Home-page: https://bodhi.fedoraproject.rog
 License: GPL-2.0-or-later
 Keywords: web,fedora,pyramid
 Author: Fedora Infrastructure Team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
@@ -17,18 +17,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: System :: Software Distribution
 Requires-Dist: Jinja2 (>=2.11.3)
 Requires-Dist: Markdown (>=3.3.6)
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: SQLAlchemy (>=1.3.24,<2.0.0)
```

