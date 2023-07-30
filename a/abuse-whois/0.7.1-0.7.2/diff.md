# Comparing `tmp/abuse_whois-0.7.1.tar.gz` & `tmp/abuse_whois-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuse_whois-0.7.1.tar", max compression
+gzip compressed data, was "abuse_whois-0.7.2.tar", max compression
```

## Comparing `abuse_whois-0.7.1.tar` & `abuse_whois-0.7.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1070 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/LICENSE
--rw-r--r--   0        0        0     3827 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/README.md
--rw-r--r--   0        0        0      130 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/api/endpoints/__init__.py
--rw-r--r--   0        0        0      194 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/api/endpoints/index.py
--rw-r--r--   0        0        0      609 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/api/endpoints/whois.py
--rw-r--r--   0        0        0      490 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/api/main.py
--rw-r--r--   0        0        0       98 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/errors.py
--rw-r--r--   0        0        0     2105 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/main.py
--rw-r--r--   0        0        0        0 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/__init__.py
--rw-r--r--   0        0        0      269 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/__init__.py
--rw-r--r--   0        0        0      193 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rule.py
--rw-r--r--   0        0        0      303 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/000webhost.yaml
--rw-r--r--   0        0        0      252 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/adobe.yaml
--rw-r--r--   0        0        0      263 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/backblaze.yaml
--rw-r--r--   0        0        0      298 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/bitly.yaml
--rw-r--r--   0        0        0      294 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/blogger.yaml
--rw-r--r--   0        0        0     3466 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/changeip.yaml
--rw-r--r--   0        0        0      271 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/cloudflare.yaml
--rw-r--r--   0        0        0      365 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/firebase.yaml
--rw-r--r--   0        0        0      258 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/glitch.yaml
--rw-r--r--   0        0        0      275 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/godaddy.yaml
--rw-r--r--   0        0        0      324 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/google_cloud.yaml
--rw-r--r--   0        0        0      347 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/google_site.yaml
--rw-r--r--   0        0        0      296 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/jimdo.yaml
--rw-r--r--   0        0        0      280 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/micorosoft.yaml
--rw-r--r--   0        0        0      242 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/netlify.yaml
--rw-r--r--   0        0        0      360 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/notion.yaml
--rw-r--r--   0        0        0      233 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/replit.yaml
--rw-r--r--   0        0        0      254 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/softlayer.yaml
--rw-r--r--   0        0        0      240 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/square.yaml
--rw-r--r--   0        0        0      266 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/telegram.yaml
--rw-r--r--   0        0        0      251 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/weebly.yaml
--rw-r--r--   0        0        0      262 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/wordpress.yaml
--rw-r--r--   0        0        0      399 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/yola.yaml
--rw-r--r--   0        0        0      548 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules.py
--rw-r--r--   0        0        0     1938 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/__init__.py
--rw-r--r--   0        0        0      294 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rule.py
--rw-r--r--   0        0        0      424 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/alibaba_cloud.yaml
--rw-r--r--   0        0        0      272 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/cloudflare.yaml
--rw-r--r--   0        0        0      340 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/digitalocean.yaml
--rw-r--r--   0        0        0      264 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/dynadot.yaml
--rw-r--r--   0        0        0      286 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/fran_tech.yaml
--rw-r--r--   0        0        0      268 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/godaddy.yaml
--rw-r--r--   0        0        0      303 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/hostinger.yaml
--rw-r--r--   0        0        0      249 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/name.yaml
--rw-r--r--   0        0        0      286 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/namecheap.yaml
--rw-r--r--   0        0        0      316 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/namesilo.yaml
--rw-r--r--   0        0        0     2451 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/noip.yaml
--rw-r--r--   0        0        0      254 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/orange.yaml
--rw-r--r--   0        0        0      343 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/publicdomainregistry.yaml
--rw-r--r--   0        0        0      265 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/registrareu.yaml
--rw-r--r--   0        0        0      289 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/tucows.yaml
--rw-r--r--   0        0        0      497 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/matchers/whois/rules.py
--rw-r--r--   0        0        0      193 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/schemas/__init__.py
--rw-r--r--   0        0        0      214 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/schemas/api_model.py
--rw-r--r--   0        0        0     1308 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/schemas/contact.py
--rw-r--r--   0        0        0      166 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/schemas/query.py
--rw-r--r--   0        0        0      136 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/schemas/rule.py
--rw-r--r--   0        0        0      775 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/schemas/whois.py
--rw-r--r--   0        0        0     1649 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/settings.py
--rw-r--r--   0        0        0     3260 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/utils.py
--rw-r--r--   0        0        0     1398 2023-07-22 00:30:59.657924 abuse_whois-0.7.1/abuse_whois/whois.py
--rw-r--r--   0        0        0     1415 2023-07-22 00:31:21.830916 abuse_whois-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 abuse_whois-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3827 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/README.md
+-rw-r--r--   0        0        0      130 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/api/endpoints/__init__.py
+-rw-r--r--   0        0        0      194 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/api/endpoints/index.py
+-rw-r--r--   0        0        0      609 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/api/endpoints/whois.py
+-rw-r--r--   0        0        0      490 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/api/main.py
+-rw-r--r--   0        0        0      148 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/errors.py
+-rw-r--r--   0        0        0     2105 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/main.py
+-rw-r--r--   0        0        0        0 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rule.py
+-rw-r--r--   0        0        0      303 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/000webhost.yaml
+-rw-r--r--   0        0        0      252 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/adobe.yaml
+-rw-r--r--   0        0        0      263 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/backblaze.yaml
+-rw-r--r--   0        0        0      298 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/bitly.yaml
+-rw-r--r--   0        0        0      294 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/blogger.yaml
+-rw-r--r--   0        0        0     3466 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/changeip.yaml
+-rw-r--r--   0        0        0      271 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/cloudflare.yaml
+-rw-r--r--   0        0        0      365 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/firebase.yaml
+-rw-r--r--   0        0        0      258 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/glitch.yaml
+-rw-r--r--   0        0        0      275 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/godaddy.yaml
+-rw-r--r--   0        0        0      324 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/google_cloud.yaml
+-rw-r--r--   0        0        0      347 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/google_site.yaml
+-rw-r--r--   0        0        0      296 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/jimdo.yaml
+-rw-r--r--   0        0        0      280 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/micorosoft.yaml
+-rw-r--r--   0        0        0      242 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/netlify.yaml
+-rw-r--r--   0        0        0      360 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/notion.yaml
+-rw-r--r--   0        0        0      233 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/replit.yaml
+-rw-r--r--   0        0        0      254 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/softlayer.yaml
+-rw-r--r--   0        0        0      240 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/square.yaml
+-rw-r--r--   0        0        0      266 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/telegram.yaml
+-rw-r--r--   0        0        0      251 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/weebly.yaml
+-rw-r--r--   0        0        0      262 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/wordpress.yaml
+-rw-r--r--   0        0        0      399 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/yola.yaml
+-rw-r--r--   0        0        0      548 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules.py
+-rw-r--r--   0        0        0     1938 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rule.py
+-rw-r--r--   0        0        0      424 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/alibaba_cloud.yaml
+-rw-r--r--   0        0        0      272 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/cloudflare.yaml
+-rw-r--r--   0        0        0      340 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/digitalocean.yaml
+-rw-r--r--   0        0        0      264 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/dynadot.yaml
+-rw-r--r--   0        0        0      286 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/fran_tech.yaml
+-rw-r--r--   0        0        0      268 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/godaddy.yaml
+-rw-r--r--   0        0        0      303 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/hostinger.yaml
+-rw-r--r--   0        0        0      249 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/name.yaml
+-rw-r--r--   0        0        0      286 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/namecheap.yaml
+-rw-r--r--   0        0        0      316 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/namesilo.yaml
+-rw-r--r--   0        0        0     2451 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/noip.yaml
+-rw-r--r--   0        0        0      254 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/orange.yaml
+-rw-r--r--   0        0        0      343 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/publicdomainregistry.yaml
+-rw-r--r--   0        0        0      265 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/registrareu.yaml
+-rw-r--r--   0        0        0      289 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/tucows.yaml
+-rw-r--r--   0        0        0      497 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/matchers/whois/rules.py
+-rw-r--r--   0        0        0      193 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/schemas/__init__.py
+-rw-r--r--   0        0        0      214 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/schemas/api_model.py
+-rw-r--r--   0        0        0     1308 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/schemas/contact.py
+-rw-r--r--   0        0        0      166 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/schemas/query.py
+-rw-r--r--   0        0        0      136 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/schemas/rule.py
+-rw-r--r--   0        0        0      775 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/schemas/whois.py
+-rw-r--r--   0        0        0     1648 2023-07-30 09:55:52.292340 abuse_whois-0.7.2/abuse_whois/settings.py
+-rw-r--r--   0        0        0     3260 2023-07-30 09:55:52.296340 abuse_whois-0.7.2/abuse_whois/utils.py
+-rw-r--r--   0        0        0     1611 2023-07-30 09:55:52.296340 abuse_whois-0.7.2/abuse_whois/whois.py
+-rw-r--r--   0        0        0     1425 2023-07-30 09:56:09.012686 abuse_whois-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5098 1970-01-01 00:00:00.000000 abuse_whois-0.7.2/PKG-INFO
```

### Comparing `abuse_whois-0.7.1/LICENSE` & `abuse_whois-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/README.md` & `abuse_whois-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/api/endpoints/whois.py` & `abuse_whois-0.7.2/abuse_whois/api/endpoints/whois.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/main.py` & `abuse_whois-0.7.2/abuse_whois/main.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules/changeip.yaml` & `abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules/changeip.yaml`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/matchers/shared_hosting/rules.py` & `abuse_whois-0.7.2/abuse_whois/matchers/shared_hosting/rules.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/matchers/whois/__init__.py` & `abuse_whois-0.7.2/abuse_whois/matchers/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/matchers/whois/rules/noip.yaml` & `abuse_whois-0.7.2/abuse_whois/matchers/whois/rules/noip.yaml`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/schemas/contact.py` & `abuse_whois-0.7.2/abuse_whois/schemas/contact.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/schemas/whois.py` & `abuse_whois-0.7.2/abuse_whois/schemas/whois.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/settings.py` & `abuse_whois-0.7.2/abuse_whois/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 WHOIS_LOOKUP_MAX_RETRIES: int = config("WHOIS_LOOKUP_MAX_RETRIES", cast=int, default=3)
 WHOIS_LOOKUP_TIMEOUT: int = config("WHOIS_LOOKUP_TIMEOUT", cast=int, default=10)
 WHOIS_LOOKUP_CACHE_SIZE: int = config("WHOIS_LOOKUP_CACHE_SIZE", cast=int, default=1024)
 WHOIS_LOOKUP_CACHE_TTL: int = config(
     "WHOIS_LOOKUP_CACHE_TTL", cast=int, default=60 * 60
 )
 
-
 IP_ADDRESS_LOOKUP_TIMEOUT: int = config(
     "IP_ADDRESS_LOOKUP_TIMEOUT", cast=int, default=10
 )
 IP_ADDRESS_LOOKUP_CACHE_SIZE: int = config(
     "IP_ADDRESS_LOOKUP_CACHE_SIZE", cast=int, default=1024
 )
 IP_ADDRESS_LOOKUP_CACHE_TTL: int = config(
```

### Comparing `abuse_whois-0.7.1/abuse_whois/utils.py` & `abuse_whois-0.7.2/abuse_whois/utils.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.7.1/abuse_whois/whois.py` & `abuse_whois-0.7.2/abuse_whois/whois.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 import asyncio
 from dataclasses import asdict
 
 import stamina
 from asyncache import cached
 from asyncwhois.query import DomainQuery, NumberQuery
 from cachetools import TTLCache
-from whois_parser import WhoisParser
+from whois_parser import WhoisParser, WhoisRecord
 
 from . import schemas, settings
+from .errors import RateLimitError
 from .utils import get_registered_domain, is_domain, is_ip_address
 
 whois_parser = WhoisParser()
 
 
 def parse(
     raw_text: str, hostname: str, *, parser: WhoisParser = whois_parser
-) -> schemas.WhoisRecord:
-    record = parser.parse(raw_text, hostname=hostname)
-    return schemas.WhoisRecord.model_validate(asdict(record))
+) -> WhoisRecord:
+    return parser.parse(raw_text, hostname=hostname)
 
 
 async def query(address: str, *, timeout: int = settings.WHOIS_LOOKUP_TIMEOUT) -> str:
     klass = DomainQuery if is_domain(address) else NumberQuery
     query = await klass.new_aio(address, timeout=timeout)
     return query.query_output
 
 
-@stamina.retry(on=asyncio.TimeoutError, attempts=settings.WHOIS_LOOKUP_MAX_RETRIES)
+@stamina.retry(
+    on=(asyncio.TimeoutError, RateLimitError),
+    attempts=settings.WHOIS_LOOKUP_MAX_RETRIES,
+    timeout=None,
+)
 @cached(
     cache=TTLCache(
         maxsize=settings.WHOIS_LOOKUP_CACHE_SIZE, ttl=settings.WHOIS_LOOKUP_CACHE_TTL
     )
 )
 async def get_whois_record(
-    hostname: str, *, timeout: int = settings.WHOIS_LOOKUP_TIMEOUT
+    hostname: str,
+    *,
+    timeout: int = settings.WHOIS_LOOKUP_TIMEOUT,
+    parser: WhoisParser = whois_parser
 ) -> schemas.WhoisRecord:
     if not is_ip_address(hostname):
         hostname = get_registered_domain(hostname) or hostname
 
     query_result = await query(hostname, timeout=timeout)
     query_result = "\n".join(query_result.splitlines())
 
-    return parse(query_result, hostname)
+    parsed = parse(query_result, hostname, parser=parser)
+    if parsed.is_rate_limited:
+        raise RateLimitError()
+
+    return schemas.WhoisRecord.model_validate(asdict(parsed))
```

### Comparing `abuse_whois-0.7.1/pyproject.toml` & `abuse_whois-0.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "abuse_whois"
-version = "0.7.1"
+version = "0.7.2"
 description = "Find where to report a domain for abuse"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/ninoseki/abuse_whois"
 repository = "https://github.com/ninoseki/abuse_whois"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 asyncache = "^0.3"
 asyncer = "^0.0"
 asyncwhois = "^1.0"
 azuma = "^0.3"
 cachetools = "^5.3"
-fastapi = "^0.100.0"
+fastapi = "^0.100"
 gunicorn = { version = "^21.2", optional = true }
 loguru = "^0.7"
 pydantic = "^2.0"
 pyhumps = "^3.8"
 PyYAML = "^6.0"
 stamina = "^23.1"
 tldextract = "^3.4"
 typer = "^0.9"
 uvicorn = { extras = ["standard"], version = "^0.23", optional = true }
 validators = "^0.20"
-whois-parser = "^0.2"
+whois-parser = ">=0.3.1,<1.0"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.2"
 autopep8 = "^2.0"
 black = "^23.7"
 coveralls = "^3.3"
 isort = "^5.12"
@@ -39,15 +39,15 @@
 pytest = "^7.4"
 pytest-asyncio = "^0.21"
 pytest-cov = "^4.1"
 pytest-mock = "^3.11"
 pytest-pretty = "^1.2"
 pytest-randomly = "^3.13"
 pyupgrade = "^3.9"
-urllib3 = "1.26.16"
+urllib3 = ">=1.26,<2.0"
 
 [tool.poetry.extras]
 api = ["uvicorn", "gunicorn"]
 
 [tool.poetry.scripts]
 abuse_whois = "abuse_whois.main:app"
```

### Comparing `abuse_whois-0.7.1/PKG-INFO` & `abuse_whois-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abuse-whois
-Version: 0.7.1
+Version: 0.7.2
 Summary: Find where to report a domain for abuse
 Home-page: https://github.com/ninoseki/abuse_whois
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,25 +14,25 @@
 Provides-Extra: api
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: asyncache (>=0.3,<0.4)
 Requires-Dist: asyncer (>=0.0,<0.1)
 Requires-Dist: asyncwhois (>=1.0,<2.0)
 Requires-Dist: azuma (>=0.3,<0.4)
 Requires-Dist: cachetools (>=5.3,<6.0)
-Requires-Dist: fastapi (>=0.100.0,<0.101.0)
+Requires-Dist: fastapi (>=0.100,<0.101)
 Requires-Dist: gunicorn (>=21.2,<22.0) ; extra == "api"
 Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyhumps (>=3.8,<4.0)
 Requires-Dist: stamina (>=23.1,<24.0)
 Requires-Dist: tldextract (>=3.4,<4.0)
 Requires-Dist: typer (>=0.9,<0.10)
 Requires-Dist: uvicorn[standard] (>=0.23,<0.24) ; extra == "api"
 Requires-Dist: validators (>=0.20,<0.21)
-Requires-Dist: whois-parser (>=0.2,<0.3)
+Requires-Dist: whois-parser (>=0.3.1,<1.0)
 Project-URL: Repository, https://github.com/ninoseki/abuse_whois
 Description-Content-Type: text/markdown
 
 # abuse_whois
 
 [![PyPI version](https://badge.fury.io/py/abuse-whois.svg)](https://badge.fury.io/py/abuse-whois)
 [![Python CI](https://github.com/ninoseki/abuse_whois/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/abuse_whois/actions/workflows/test.yml)
```

