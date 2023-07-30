# Comparing `tmp/aa_discord_announcements-1.2.2.tar.gz` & `tmp/aa_discord_announcements-1.2.3.tar.gz`

## Comparing `aa_discord_announcements-1.2.2.tar` & `aa_discord_announcements-1.2.3.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/admin.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/app_settings.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/apps.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/constants.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/forms.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/models.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/urls.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/docs/screenshots/weblate/.gitkeep
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/helper/discord_webhook.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/django.pot
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0002_translation_updates.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/base.html
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/index.html
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/LICENSE
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/README.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/admin.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/app_settings.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/apps.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/constants.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/forms.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/models.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/urls.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/docs/screenshots/weblate/.gitkeep
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/helper/discord_webhook.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/django.pot
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/0002_translation_updates.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/css/aa-bootstrap-fix.css
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/base.html
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/index.html
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/LICENSE
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/README.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.3/PKG-INFO
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/admin.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/admin.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/apps.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/apps.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/forms.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/forms.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/models.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/urls.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/views.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/views.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/django.pot` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -162,46 +163,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,26 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
+
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Du möchtest helfen diese App in Deine Sprache zu übersetzen oder "
+"die bestehende Übersetzung verbessern? - %(weblate_link)s\n"
+"        "
 
 msgid "Additionally configured announcement targets"
 msgstr "Zusätzlich konfigurierte Ankündigungsziele"
 
 msgid "Announcement Channel"
 msgstr "Ankündigungskanal"
 
@@ -95,14 +106,17 @@
 "Ungültige Webhook-URL. Die eingegebene Webhook-URL stimmt mit keinem "
 "bekannten Format für einen Discord-Webhook überein. Bitte überprüfe die "
 "Webhook-URL."
 
 msgid "Is enabled"
 msgstr "Ist aktiviert"
 
+msgid "Join our team of translators!"
+msgstr "Tritt unserm Team von Übersetzern bei!"
+
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Pflichtangaben fehlen.<br>Um eine Ankündigung zu erstellen, müssen folgende "
 "Felder ausgefüllt sein:<br>» Ankündigungstext"
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/de/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
-"PO-Revision-Date: 2023-06-28 14:37+0000\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
+"PO-Revision-Date: 2023-07-28 22:39+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr "Discord-Ankündigungen"
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr "Gruppenname"
 
@@ -174,50 +174,67 @@
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Ungültige Webhook-URL. Die eingegebene Webhook-URL stimmt mit keinem "
 "bekannten Format für einen Discord-Webhook überein. Bitte überprüfe die "
 "Webhook-URL."
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr "Ankündigung Details"
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr "Formatierter Text der Ankündigung"
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Pflichtangaben fehlen.<br>Um eine Ankündigung zu erstellen, müssen folgende "
 "Felder ausgefüllt sein:<br>» Ankündigungstext"
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 "Fehler! Die Ankündigung wurde nicht in Ihre Zwischenablage kopiert. "
 "Möglicherweise unterstützt Dein Browser diese Funktion nicht."
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Erfolg! Der Ankündigungstext wurde in die Zwischenablage kopiert."
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr "Noch keine Ankündigung erstellt …"
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr "Kopiere Ankündigungstext"
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr "Tritt unserm Team von Übersetzern bei!"
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Du möchtest helfen diese App in Deine Sprache zu übersetzen oder "
+"die bestehende Übersetzung verbessern? - %(weblate_link)s\n"
+"        "
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr "Ankündigung erstellen"
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr "Keiner, einfach nur den Text formatieren"
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
-"PO-Revision-Date: 2023-04-18 23:17+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/es/>\n"
-"Language: es\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.4\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -43,15 +43,15 @@
 #: apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: forms.py:21
 msgid "This field is mandatory"
-msgstr "Este campo es obligatorio"
+msgstr ""
 
 #: forms.py:42
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:49
 #, python-brace-format
@@ -163,46 +163,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/fr/>\n"
-"Language: fr_FR\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -43,15 +43,15 @@
 #: apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: forms.py:21
 msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+msgstr "Questo campo è obbligatorio"
 
 #: forms.py:42
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:49
 #, python-brace-format
@@ -163,46 +163,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/it/>\n"
-"Language: it_IT\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/fr/>\n"
+"Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -43,15 +43,15 @@
 #: apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: forms.py:21
 msgid "This field is mandatory"
-msgstr "Questo campo è obbligatorio"
+msgstr "Ce champ est obligatoire"
 
 #: forms.py:42
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:49
 #, python-brace-format
@@ -163,46 +163,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/es/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
+"PO-Revision-Date: 2023-04-18 23:17+0000\n"
+"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -43,15 +43,15 @@
 #: apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: forms.py:21
 msgid "This field is mandatory"
-msgstr ""
+msgstr "Este campo es obligatorio"
 
 #: forms.py:42
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:49
 #, python-brace-format
@@ -163,46 +163,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/django.pot`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -162,46 +162,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,26 @@
 "apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
+
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Вы хотите помочь перевести это приложение на ваш язык или "
+"улучшить текущий перевод? - %(weblate_link)s\n"
+"        "
 
 msgid "Additionally configured announcement targets"
 msgstr "Дополнительно сконфигурированные цели объявлений"
 
 msgid "Announcement Channel"
 msgstr "Канал объявления"
 
@@ -95,14 +106,17 @@
 msgstr ""
 "Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
 "вебхуков Discord. Пожалуйста, проверьте URL."
 
 msgid "Is enabled"
 msgstr "Разрешен"
 
+msgid "Join our team of translators!"
+msgstr "Присоединяйтесь к нашей команде переводчиков!"
+
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Отсутствует необходимая информация. <br>Для создания объявления необходимо "
 "заполнить следующие поля:<br>» Текст объявления"
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
-"PO-Revision-Date: 2023-06-24 13:57+0000\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
+"PO-Revision-Date: 2023-07-29 23:45+0000\n"
 "Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr "Объявления Discord"
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr "Название группы"
 
@@ -172,50 +172,67 @@
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
 "вебхуков Discord. Пожалуйста, проверьте URL."
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr "Детали объявления"
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr "Отформатированный текст объявления"
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Отсутствует необходимая информация. <br>Для создания объявления необходимо "
 "заполнить следующие поля:<br>» Текст объявления"
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 "Ошибка! Объявление не было скопировано в буфер обмена. Вероятно Ваш браузер "
 "не предоставляет такую функциональность."
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Успех! Объявление скопировано в буфер обмена."
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr "Объявлений нет …"
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr "Скопировать текст объявления"
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr "Присоединяйтесь к нашей команде переводчиков!"
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Вы хотите помочь перевести это приложение на ваш язык или "
+"улучшить текущий перевод? - %(weblate_link)s\n"
+"        "
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr "Создать объявление"
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr "Нет, только отформатируй"
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,53 +8,57 @@
 "apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.17\n"
+"X-Generator: Weblate 4.18.2\n"
 
 msgid "Announcement Text"
 msgstr "Текст оголошення"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
 
-msgid "Discord Markdown"
-msgstr "Discord markdown"
-
 msgid "Discord Ping Target"
 msgstr "Ціль для пінгу в Discord"
 
 msgid "Discord Ping Targets"
 msgstr "Цілі для пінгу в Discord"
 
+msgid "Discord channel"
+msgstr "Канал діскорду"
+
 msgid "Don't Ping"
 msgstr "Не пінгувати"
 
 msgid "Form invalid. Please check your input."
 msgstr "Форма невірна. Будь ласка, перевірте свої дані."
 
-msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"Підказка: Ви можете використовувати {discord_markdown_link} для форматування "
-"тексту."
+msgid "Group name"
+msgstr "Назва групи"
+
+msgid "Group restrictions"
+msgstr "Групові обмеження"
 
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Неправильна URL-адреса веб-хука. Введена вами URL-адреса веб-хука не "
 "відповідає жодному з відомих форматів веб-хуків Discord. Будь ласка, "
 "перевірте URL-адресу веб-хука."
 
+msgid "Is enabled"
+msgstr "Дозволено"
+
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Ім'я ролі Discord, яку потрібно пінгувати. (Примітка: це має бути група "
 "Auth, яка синхронізована з Discord.)"
 
@@ -63,32 +67,35 @@
 
 msgid "No form data submitted."
 msgstr "Не подано жодних даних."
 
 msgid "None, just format it for me"
 msgstr "Ні, просто відформатуйте для мене"
 
-msgid "Restrict ping rights to the following group(s) …"
-msgstr "Обмежити права на пінг для наступних груп …"
-
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Виберіть канал для автоматичного відправлення оголошення."
 
+msgid "This field is mandatory"
+msgstr "Це поле обовʼязкове"
+
 msgid "This group has not been synced to Discord yet."
 msgstr "Цю групу ще не синхронізовано з Discord."
 
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL-адреса цього веб-хука, наприклад, https://discord.com/api/"
 "webhooks/123456/abcdef"
 
 msgid "Webhook"
 msgstr "Веб-хук"
 
+msgid "Webhook URL"
+msgstr "Веб-хук URL"
+
 msgid "Webhooks"
 msgstr "Веб-хуки"
 
 msgid "Whether this webhook is active or not"
 msgstr "Активний цей вебхук чи ні"
 
 msgid "Who do you want to ping?"
@@ -98,10 +105,7 @@
 msgstr "Ви можете додати примітки про цю конфігурацію тут, якщо хочете"
 
 msgid "You can add notes about this webhook here if you want"
 msgstr "Ви можете додати примітки про цей вебхук тут, якщо хочете"
 
 msgid "You might want to install the Discord service first …"
 msgstr "Можливо, ви захочете спочатку встановити службу Discord …"
-
-msgid "Your announcement…"
-msgstr "Ваше оголошення…"
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,59 +4,57 @@
 # Kristof <kristof@teh.ninja>, 2023.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
-"PO-Revision-Date: 2023-06-14 17:18+0000\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
+"PO-Revision-Date: 2023-07-27 15:39+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.17\n"
+"X-Generator: Weblate 4.18.2\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
-msgstr ""
+msgstr "Назва групи"
 
 #: admin.py:38 admin.py:72 models.py:102 models.py:190
 msgid "Group restrictions"
-msgstr ""
+msgstr "Групові обмеження"
 
 #: admin.py:61 models.py:168
 msgid "Discord channel"
-msgstr ""
+msgstr "Канал діскорду"
 
 #: admin.py:66 models.py:176
-#, fuzzy
-#| msgid "Webhook"
 msgid "Webhook URL"
-msgstr "Веб-хук"
+msgstr "Веб-хук URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: forms.py:21
 msgid "This field is mandatory"
-msgstr ""
+msgstr "Це поле обовʼязкове"
 
 #: forms.py:42
 #, fuzzy
 #| msgid "Discord Markdown"
 msgid "Discord Markdown"
 msgstr "Discord markdown"
 
@@ -133,15 +131,15 @@
 
 #: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr "Ви можете додати примітки про цю конфігурацію тут, якщо хочете"
 
 #: models.py:118 models.py:206
 msgid "Is enabled"
-msgstr ""
+msgstr "Дозволено"
 
 #: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
 #: models.py:127
 msgid "Discord Ping Target"
@@ -183,46 +181,59 @@
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Неправильна URL-адреса веб-хука. Введена вами URL-адреса веб-хука не "
 "відповідає жодному з відомих форматів веб-хуків Discord. Будь ласка, "
 "перевірте URL-адресу веб-хука."
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr "Ні, просто відформатуйте для мене"
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.3/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"POT-Creation-Date: 2023-07-27 22:33+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
+#: templates/aa_discord_announcements/index.html:6
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
 msgid "Group name"
 msgstr ""
 
@@ -163,46 +162,59 @@
 
 #: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:10
+#: templates/aa_discord_announcements/index.html:15
 msgid "Announcement Details"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:21
+#: templates/aa_discord_announcements/index.html:26
 msgid "Formatted Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:41
+#: templates/aa_discord_announcements/index.html:46
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:44
+#: templates/aa_discord_announcements/index.html:49
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: templates/aa_discord_announcements/index.html:45
+#: templates/aa_discord_announcements/index.html:50
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
 msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/aa_discord_announcements/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0002_translation_updates.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/0002_translation_updates.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-1.2.3/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 {% extends "aa_discord_announcements/base.html" %}
 
 {% load i18n %}
 
-{% block details %}
-    <div class="aa-discord-announcements row">
+{% block aa_discord_announcements_header %}
+    {% translate "Discord Announcements" as translated_header %}
+    {% include "aa_discord_announcements/partials/header/page-header.html" with header_text=translated_header %}
+{% endblock %}
+
+{% block aa_discord_announcements_body %}
+    <div class="row">
         <div class="col-md-6">
             <div class="panel panel-default">
                 <div class="panel-heading">
                     <span class="panel-title">{% translate "Announcement Details" %}</span>
                 </div>
                 <div class="panel-body">
                     {% include "aa_discord_announcements/partials/form/form.html" %}
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 {% extends "aa_discord_announcements/base.html" %} {% load i18n %} {% block
-details %}
+aa_discord_announcements_header %} {% translate "Discord Announcements" as
+translated_header %} {% include "aa_discord_announcements/partials/header/page-
+header.html" with header_text=translated_header %} {% endblock %} {% block
+aa_discord_announcements_body %}
 {% translate "Announcement Details" %}
 {% include "aa_discord_announcements/partials/form/form.html" %}
 {% translate "Formatted Announcement Text" %}
 {% include "aa_discord_announcements/partials/announcement/announcement.html"
 %}
  {% endblock %} {% block extra_javascript %} {% include "bundles/clipboard-
 js.html" %} {% include "aa_discord_announcements/bundles/discord-announcements-
```

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-1.2.3/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-1.2.3/aa_discord_announcements/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/LICENSE` & `aa_discord_announcements-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/README.md` & `aa_discord_announcements-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.2/pyproject.toml` & `aa_discord_announcements-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aa-discord-announcements"
-version = "1.2.2"
+version = "1.2.3"
 description = "Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth."
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = "~=3.8"
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
```

### Comparing `aa_discord_announcements-1.2.2/PKG-INFO` & `aa_discord_announcements-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-discord-announcements
-Version: 1.2.2
+Version: 1.2.3
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Project-URL: Homepage, https://github.com/ppfeufer/aa-discord-announcements
 Project-URL: Documentation, https://github.com/ppfeufer/aa-discord-announcements/blob/master/README.md
 Project-URL: Source, https://github.com/ppfeufer/aa-discord-announcements.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/ppfeufer/aa-discord-announcements/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>
```

