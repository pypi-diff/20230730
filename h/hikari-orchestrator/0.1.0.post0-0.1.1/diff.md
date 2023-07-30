# Comparing `tmp/hikari_orchestrator-0.1.0.post0.tar.gz` & `tmp/hikari_orchestrator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_orchestrator-0.1.0.post0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hikari_orchestrator-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hikari_orchestrator-0.1.0.post0.tar` & `hikari_orchestrator-0.1.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0       14 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.gitattributes
--rw-r--r--   0        0        0       26 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/FUNDING.yml
--rw-r--r--   0        0        0      459 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/dependabot.yml
--rw-r--r--   0        0        0     1146 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0     1036 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1518 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/pr-docs.yml
--rw-r--r--   0        0        0      874 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      982 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1265 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/release-docs.yml
--rw-r--r--   0        0        0     1027 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      838 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1188 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1223 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1062 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0      856 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/.github/workflows/verify-types.yml
--rw-r--r--   0        0        0     1748 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/.gitignore
--rw-r--r--   0        0        0       85 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/.gitmodules
--rw-r--r--   0        0        0      501 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/CHANGELOG.md
--rw-r--r--   0        0        0     1515 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/LICENSE
--rw-r--r--   0        0        0      147 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/README.md
--rw-r--r--   0        0        0      115 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/constraints.in
--rw-r--r--   0        0        0    51506 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/constraints.txt
--rw-r--r--   0        0        0      141 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    71040 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0       17 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs/changelog.md
--rw-r--r--   0        0        0     3004 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs/index.md
--rw-r--r--   0        0        0       64 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs/reference.md
--rw-r--r--   0        0        0     7048 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs_src/LICENSE
--rw-r--r--   0        0        0      996 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs_src/index.py
--rw-r--r--   0        0        0     1941 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__init__.py
--rw-r--r--   0        0        0     4017 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__main__.py
--rw-r--r--   0        0        0    12623 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_bot.py
--rw-r--r--   0        0        0    21207 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_client.py
--rw-r--r--   0        0        0     1684 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/__init__.py
--rw-r--r--   0        0        0     6393 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.py
--rw-r--r--   0        0        0     8359 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.pyi
--rw-r--r--   0        0        0    11416 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.py
--rw-r--r--   0        0        0     4808 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.pyi
--rw-r--r--   0        0        0    17603 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_service.py
--rw-r--r--   0        0        0     3155 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_ssl.py
--rw-r--r--   0        0        0        0 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/py.typed
--rw-r--r--   0        0        0     1698 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/mkdocs.yml
--rw-r--r--   0        0        0     1714 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/noxfile.py
--rw-r--r--   0        0        0       14 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.gitattributes
--rw-r--r--   0        0        0      458 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/dependabot.yml
--rw-r--r--   0        0        0     1240 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0      959 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/lint.yml
--rw-r--r--   0        0        0      976 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1032 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      832 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1182 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1217 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1114 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0     1751 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.gitignore
--rw-r--r--   0        0        0     1520 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/LICENSE
--rw-r--r--   0        0        0      138 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/README.md
--rw-r--r--   0        0        0       50 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/.env.example
--rw-r--r--   0        0        0      612 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/Dockerfile
--rw-r--r--   0        0        0    30763 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/main.py
--rw-r--r--   0        0        0       10 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/requirements-extra.txt
--rw-r--r--   0        0        0      194 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/requirements.in
--rw-r--r--   0        0        0    25212 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/requirements.txt
--rw-r--r--   0        0        0      933 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.in
--rw-r--r--   0        0        0    20370 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.txt
--rw-r--r--   0        0        0       10 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking-extra.txt
--rw-r--r--   0        0        0      112 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    34990 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0      250 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/docker-compose.yml
--rw-r--r--   0        0        0       26 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/FUNDING.yml
--rw-r--r--   0        0        0      764 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/clippy.yml
--rw-r--r--   0        0        0     1133 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/freeze-for-pr.yml
--rw-r--r--   0        0        0     1271 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/lint.yml
--rw-r--r--   0        0        0     1577 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/pr-docs.yml
--rw-r--r--   0        0        0      964 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/publish.yml
--rw-r--r--   0        0        0     2399 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/py-test.yml
--rw-r--r--   0        0        0     1013 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/reformat.yml
--rw-r--r--   0        0        0     1373 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/release-docs.yml
--rw-r--r--   0        0        0     1075 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/resync-piped.yml
--rw-r--r--   0        0        0     1223 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/rustfmt.yml
--rw-r--r--   0        0        0      869 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/type-check.yml
--rw-r--r--   0        0        0     1191 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/update-licence.yml
--rw-r--r--   0        0        0     1226 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/upgrade-locks.yml
--rw-r--r--   0        0        0     1130 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-locks.yml
--rw-r--r--   0        0        0      887 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-types.yml
--rw-r--r--   0        0        0      550 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/dependabot.yml
--rw-r--r--   0        0        0      524 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/pull_request_template.md
--rw-r--r--   0        0        0     1713 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/noxfile.py
--rw-r--r--   0        0        0     4853 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/pyproject.toml
--rw-r--r--   0        0        0      115 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/docs.in
--rw-r--r--   0        0        0    31882 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/docs.txt
--rw-r--r--   0        0        0       90 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/flake8.in
--rw-r--r--   0        0        0     1671 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/flake8.txt
--rw-r--r--   0        0        0       32 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/freeze-locks.in
--rw-r--r--   0        0        0    58539 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/freeze-locks.txt
--rw-r--r--   0        0        0     1070 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.in
--rw-r--r--   0        0        0    30104 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.txt
--rw-r--r--   0        0        0       58 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/lint.in
--rw-r--r--   0        0        0     5453 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/lint.txt
--rw-r--r--   0        0        0       60 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/nox.in
--rw-r--r--   0        0        0    16594 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/nox.txt
--rw-r--r--   0        0        0       12 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/publish.in
--rw-r--r--   0        0        0     8587 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/publish.txt
--rw-r--r--   0        0        0       78 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/reformat.in
--rw-r--r--   0        0        0    15634 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/reformat.txt
--rw-r--r--   0        0        0       64 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/tests.in
--rw-r--r--   0        0        0     8070 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/tests.txt
--rw-r--r--   0        0        0       29 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/type-checking.in
--rw-r--r--   0        0        0     3965 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/type-checking.txt
--rw-r--r--   0        0        0    24265 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/noxfile.py
--rw-r--r--   0        0        0     1714 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/noxfile.template.py
--rw-r--r--   0        0        0     4527 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/piped_shared/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/piped_shared/py.typed
--rw-r--r--   0        0        0      334 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/pyproject.toml
--rw-r--r--   0        0        0     6974 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/pyproject.toml
--rw-r--r--   0        0        0     2604 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/schema.proto
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 hikari_orchestrator-0.1.0.post0/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.gitattributes
+-rw-r--r--   0        0        0       26 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      459 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1146 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1036 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1518 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/pr-docs.yml
+-rw-r--r--   0        0        0      874 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      982 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1265 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1027 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      838 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1188 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1223 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1062 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0      856 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.github/workflows/verify-types.yml
+-rw-r--r--   0        0        0     1748 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.gitignore
+-rw-r--r--   0        0        0       85 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/.gitmodules
+-rw-r--r--   0        0        0      774 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1515 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/LICENSE
+-rw-r--r--   0        0        0      147 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/README.md
+-rw-r--r--   0        0        0      115 2023-07-30 14:33:36.212637 hikari_orchestrator-0.1.1/dev-requirements/constraints.in
+-rw-r--r--   0        0        0    51506 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/dev-requirements/constraints.txt
+-rw-r--r--   0        0        0      141 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    71041 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0       17 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/docs/changelog.md
+-rw-r--r--   0        0        0     3095 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/docs/index.md
+-rw-r--r--   0        0        0       64 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/docs/reference.md
+-rw-r--r--   0        0        0     7048 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/docs_src/LICENSE
+-rw-r--r--   0        0        0      996 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/docs_src/index.py
+-rw-r--r--   0        0        0     1941 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/__init__.py
+-rw-r--r--   0        0        0     4105 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/__main__.py
+-rw-r--r--   0        0        0    12623 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_bot.py
+-rw-r--r--   0        0        0    21207 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_client.py
+-rw-r--r--   0        0        0     1684 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/__init__.py
+-rw-r--r--   0        0        0     6393 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2.py
+-rw-r--r--   0        0        0     8359 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2.pyi
+-rw-r--r--   0        0        0    11416 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     4808 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2_grpc.pyi
+-rw-r--r--   0        0        0    17603 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_service.py
+-rw-r--r--   0        0        0     3155 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/_ssl.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/hikari_orchestrator/py.typed
+-rw-r--r--   0        0        0     1698 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     1714 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/noxfile.py
+-rw-r--r--   0        0        0       14 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.gitattributes
+-rw-r--r--   0        0        0      458 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/dependabot.yml
+-rw-r--r--   0        0        0     1240 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0      959 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      976 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1032 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      832 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1182 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1217 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1114 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0     1751 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/.gitignore
+-rw-r--r--   0        0        0     1520 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/LICENSE
+-rw-r--r--   0        0        0      138 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/README.md
+-rw-r--r--   0        0        0       50 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/bot/.env.example
+-rw-r--r--   0        0        0      612 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/bot/Dockerfile
+-rw-r--r--   0        0        0    30763 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/bot/main.py
+-rw-r--r--   0        0        0       10 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/bot/requirements-extra.txt
+-rw-r--r--   0        0        0      194 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/bot/requirements.in
+-rw-r--r--   0        0        0    25212 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/bot/requirements.txt
+-rw-r--r--   0        0        0      933 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/dev-requirements/flake8.in
+-rw-r--r--   0        0        0    20370 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0       10 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/dev-requirements/type-checking-extra.txt
+-rw-r--r--   0        0        0      112 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    34990 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0      250 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/docker-compose.yml
+-rw-r--r--   0        0        0       26 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2023-07-30 14:33:36.804711 hikari_orchestrator-0.1.1/piped/github/FUNDING.yml
+-rw-r--r--   0        0        0      764 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/clippy.yml
+-rw-r--r--   0        0        0     1133 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1271 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/lint.yml
+-rw-r--r--   0        0        0     1577 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/pr-docs.yml
+-rw-r--r--   0        0        0      964 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/publish.yml
+-rw-r--r--   0        0        0     2399 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/py-test.yml
+-rw-r--r--   0        0        0     1013 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/reformat.yml
+-rw-r--r--   0        0        0     1373 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/release-docs.yml
+-rw-r--r--   0        0        0     1075 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/resync-piped.yml
+-rw-r--r--   0        0        0     1223 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/rustfmt.yml
+-rw-r--r--   0        0        0      869 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/type-check.yml
+-rw-r--r--   0        0        0     1191 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/update-licence.yml
+-rw-r--r--   0        0        0     1226 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/upgrade-locks.yml
+-rw-r--r--   0        0        0     1130 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/verify-locks.yml
+-rw-r--r--   0        0        0      887 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/actions/verify-types.yml
+-rw-r--r--   0        0        0      550 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/dependabot.yml
+-rw-r--r--   0        0        0      524 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/github/pull_request_template.md
+-rw-r--r--   0        0        0     1713 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/noxfile.py
+-rw-r--r--   0        0        0     4853 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/docs.in
+-rw-r--r--   0        0        0    31882 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/docs.txt
+-rw-r--r--   0        0        0       90 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/flake8.in
+-rw-r--r--   0        0        0     1671 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/flake8.txt
+-rw-r--r--   0        0        0       32 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/freeze-locks.in
+-rw-r--r--   0        0        0    58539 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/freeze-locks.txt
+-rw-r--r--   0        0        0     1070 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/library-flake8.in
+-rw-r--r--   0        0        0    30104 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/library-flake8.txt
+-rw-r--r--   0        0        0       58 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/lint.in
+-rw-r--r--   0        0        0     5453 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/lint.txt
+-rw-r--r--   0        0        0       60 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/nox.in
+-rw-r--r--   0        0        0    16594 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/nox.txt
+-rw-r--r--   0        0        0       12 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/publish.in
+-rw-r--r--   0        0        0     8587 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/publish.txt
+-rw-r--r--   0        0        0       78 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/reformat.in
+-rw-r--r--   0        0        0    15634 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/reformat.txt
+-rw-r--r--   0        0        0       64 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/tests.in
+-rw-r--r--   0        0        0     8070 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/tests.txt
+-rw-r--r--   0        0        0       29 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/type-checking.in
+-rw-r--r--   0        0        0     3965 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/base-requirements/type-checking.txt
+-rw-r--r--   0        0        0    24265 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/noxfile.py
+-rw-r--r--   0        0        0     1714 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/noxfile.template.py
+-rw-r--r--   0        0        0     4527 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/piped_shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/piped_shared/py.typed
+-rw-r--r--   0        0        0      334 2023-07-30 14:33:36.808712 hikari_orchestrator-0.1.1/piped/python/pyproject.toml
+-rw-r--r--   0        0        0     6969 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2604 2023-07-30 14:33:36.216637 hikari_orchestrator-0.1.1/schema.proto
+-rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 hikari_orchestrator-0.1.1/PKG-INFO
```

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/freeze-for-pr.yml` & `hikari_orchestrator-0.1.1/.github/workflows/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/lint.yml` & `hikari_orchestrator-0.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/pr-docs.yml` & `hikari_orchestrator-0.1.1/.github/workflows/pr-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/publish.yml` & `hikari_orchestrator-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/reformat.yml` & `hikari_orchestrator-0.1.1/.github/workflows/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/release-docs.yml` & `hikari_orchestrator-0.1.1/.github/workflows/release-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/resync-piped.yml` & `hikari_orchestrator-0.1.1/.github/workflows/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/type-check.yml` & `hikari_orchestrator-0.1.1/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/update-licence.yml` & `hikari_orchestrator-0.1.1/.github/workflows/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/upgrade-locks.yml` & `hikari_orchestrator-0.1.1/.github/workflows/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/verify-locks.yml` & `hikari_orchestrator-0.1.1/.github/workflows/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.github/workflows/verify-types.yml` & `hikari_orchestrator-0.1.1/.github/workflows/verify-types.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/.gitignore` & `hikari_orchestrator-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/LICENSE` & `hikari_orchestrator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/dev-requirements/constraints.txt` & `hikari_orchestrator-0.1.1/dev-requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/dev-requirements/type-checking.txt` & `hikari_orchestrator-0.1.1/dev-requirements/type-checking.txt`

 * *Files 1% similar despite different names*

```diff
@@ -617,17 +617,17 @@
     --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
 nox==2023.4.22 ; python_full_version >= "3.10.0" and python_version < "3.12" \
     --hash=sha256:0b1adc619c58ab4fa57d6ab2e7823fe47a32e70202f287d78474adcc7bda1891 \
     --hash=sha256:46c0560b0dc609d7d967dc99e22cb463d3c4caf54a5fda735d6c11b5177e3a9f
 packaging==23.1 ; python_full_version >= "3.10.0" and python_version < "3.12" \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
-platformdirs==3.9.1 ; python_full_version >= "3.10.0" and python_version < "3.12" \
-    --hash=sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421 \
-    --hash=sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f
+platformdirs==3.10.0 ; python_full_version >= "3.10.0" and python_version < "3.12" \
+    --hash=sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d \
+    --hash=sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d
 protobuf==4.23.4 ; python_full_version >= "3.10.0" and python_version < "3.12" \
     --hash=sha256:0a5759f5696895de8cc913f084e27fd4125e8fb0914bb729a17816a33819f474 \
     --hash=sha256:351cc90f7d10839c480aeb9b870a211e322bf05f6ab3f55fcb2f51331f80a7d2 \
     --hash=sha256:5fea3c64d41ea5ecf5697b83e41d09b9589e6f20b677ab3c48e5f242d9b7897b \
     --hash=sha256:6dd9b9940e3f17077e820b75851126615ee38643c2c5332aa7a359988820c720 \
     --hash=sha256:7b19b6266d92ca6a2a87effa88ecc4af73ebc5cfde194dc737cf8ef23a9a3b12 \
     --hash=sha256:8547bf44fe8cec3c69e3042f5c4fb3e36eb2a7a013bb0a44c018fc1e427aafbd \
```

### Comparing `hikari_orchestrator-0.1.0.post0/docs/index.md` & `hikari_orchestrator-0.1.1/docs/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,36 +35,36 @@
 
 ```shell
 hikari_orchestrator tcp://localhost:6969 --token "Bot.Token"
 ```
 
 The CLI application has two required arguments:
 
-- The server's host address is the only positional argument. TCP will be used
-  if no scheme is included and more information on the supported schemes can be
-  found [here](https://github.com/grpc/grpc/blob/master/doc/naming.md).
-- `--token`: The Discord bot token for the bot being orchestrated.
-  It's recommended that you provide this via its env variable rather than as a
-  CLI argument .
+- (`ORCHESTRATOR_ADDRESS`): The server's host address is the only positional
+  argument. TCP will be used if no scheme is included and more information on
+  the supported schemes can be found
+  [here](https://github.com/grpc/grpc/blob/master/doc/naming.md).
+- `--token` (`DISCORD_TOKEN`): The Discord bot token for the bot being
+  orchestrated. It's recommended that you provide this via its env variable
+  rather than as a CLI argument .
 
 And several optional arguments:
 
-- `--intents`: The gateway intents the bot should declare. This defaults to
-  `ALL_UNPRIVILEGED` and supports passing either the raw integer flag or a
-  `|`-separated list of intent names as defined by [hikari.Intents][hikari.intents.Intents]
-  (e.g. `GUILD_MEMBERS|GUILD_MODERATION`).
-- `--log-level`: Name of the logging level the server should use.
+- `--intents` (`ORCHESTRATOR_INTENTS`): The gateway intents the bot should
+  declare. This defaults to `ALL_UNPRIVILEGED` and supports passing either the
+  raw integer flag or a `|`-separated list of intent names as defined by
+  [hikari.Intents][hikari.intents.Intents] (e.g. `"GUILD_MEMBERS|GUILD_MODERATION"`).
+- `--log-level` (`LOG_LEVEL`): Name of the logging level the server should use.
   Defaults to `"INFO"`.
-- `--ca-cert` & `--private-key`: Paths to the unencrypted PEM keys which act as
-  the certificate authority and private key for the server to use to SSL
-  encrypt TCP connections.
-
-These options and arguments can also be provided as environment variables
-(including as part of a `.env` file); to see the relevant env variable names
-use `hikari_orchestrator --help`.
+- `--ca-cert` & `--private-key` (`ORCHESTRATOR_CA_CERT` & `ORCHESTRATOR_PRIVATE_KEY`):
+  Paths to the unencrypted PEM keys which act as the certificate authority and
+  private key for the server to use to SSL encrypt TCP connections.
+
+These arguments can also be provided using the environment variables which are
+shown in brackets (including as part of a `.env` file).
 
 ```py
 --8<-- "./docs_src/index.py:27:31"
 ```
 
 Then you need to startup some child bot instances. For this you'll use
 Orchestrator's [Bot][hikari_orchestrator.Bot] implementation of
```

### Comparing `hikari_orchestrator-0.1.0.post0/docs_src/LICENSE` & `hikari_orchestrator-0.1.1/docs_src/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/docs_src/index.py` & `hikari_orchestrator-0.1.1/docs_src/index.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__init__.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__main__.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import click
 import dotenv
 import hikari
 
 from . import _service  # pyright: ignore[reportPrivateUsage]
 
 
-def _cast_token(value: str, /) -> hikari.Intents:
+def _cast_intents(value: str, /) -> hikari.Intents:
     try:
         int_value = int(value)
     except ValueError:
         pass
 
     else:
         return hikari.Intents(int_value)
@@ -72,31 +72,32 @@
 @click.argument("address", default="localhost:0", envvar="ORCHESTRATOR_ADDRESS")
 @click.option("--token", envvar="DISCORD_TOKEN", help="Discord token for the bot to orchestrate.", required=True)
 @click.option(
     "--intents",
     default=hikari.Intents.ALL_UNPRIVILEGED,
     envvar="ORCHESTRATOR_INTENTS",
     help="Gateway intents the bot should use. Defaults to ALL_UNPRIVILEGED",
-    type=_cast_token,
+    type=_cast_intents,
 )
 @click.option("--log-level", default="INFO", envvar="LOG_LEVEL", help="A Python logging level name. Defaults to INFO.")
 @click.option(
     "--ca-cert",
     default=None,
     envvar="ORCHESTRATOR_CA_CERT",
     help="Path to an unencrypted PEM certificate authority to use for encrypting TCP connections.",
     type=click.File("rb"),
 )
 @click.option(
     "--private-key",
     default=None,
+    envvar="ORCHESTRATOR_PRIVATE_KEY",
     help="Path to an unencrypted PEM private key to use for authenticating TCP connections.",
     type=click.File("rb"),
 )
-def main(
+def _cli_entry(
     address: str,
     token: str,
     ca_cert: io.BytesIO | None,
     intents: hikari.Intents,
     log_level: str,
     private_key: io.BytesIO | None,
 ) -> None:
@@ -114,10 +115,14 @@
 
     else:
         private_key_data = None
 
     _service.run_server(token, address, ca_cert=ca_cert_data, private_key=private_key_data, intents=intents)
 
 
-if __name__ == "__main__":
+def main() -> None:
     dotenv.load_dotenv()
+    _cli_entry()
+
+
+if __name__ == "__main__":
     main()
```

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_bot.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_bot.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_client.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_client.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/__init__.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.pyi` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.pyi` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_protos/schema_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_service.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_service.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_ssl.py` & `hikari_orchestrator-0.1.1/hikari_orchestrator/_ssl.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/mkdocs.yml` & `hikari_orchestrator-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/noxfile.py` & `hikari_orchestrator-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/freeze-for-pr.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/lint.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/reformat.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/resync-piped.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/type-check.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/update-licence.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/upgrade-locks.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/verify-locks.yml` & `hikari_orchestrator-0.1.1/piped/.github/workflows/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/.gitignore` & `hikari_orchestrator-0.1.1/piped/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/LICENSE` & `hikari_orchestrator-0.1.1/piped/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/bot/Dockerfile` & `hikari_orchestrator-0.1.1/piped/bot/Dockerfile`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/bot/main.py` & `hikari_orchestrator-0.1.1/piped/bot/main.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/bot/requirements.txt` & `hikari_orchestrator-0.1.1/piped/bot/requirements.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.in` & `hikari_orchestrator-0.1.1/piped/dev-requirements/flake8.in`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.txt` & `hikari_orchestrator-0.1.1/piped/dev-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking.txt` & `hikari_orchestrator-0.1.1/piped/dev-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/clippy.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/clippy.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/freeze-for-pr.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/lint.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/pr-docs.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/pr-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/publish.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/publish.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/py-test.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/py-test.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/reformat.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/release-docs.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/release-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/resync-piped.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/rustfmt.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/rustfmt.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/type-check.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/update-licence.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/upgrade-locks.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-locks.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-types.yml` & `hikari_orchestrator-0.1.1/piped/github/actions/verify-types.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/dependabot.yml` & `hikari_orchestrator-0.1.1/piped/github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/github/pull_request_template.md` & `hikari_orchestrator-0.1.1/piped/github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/noxfile.py` & `hikari_orchestrator-0.1.1/piped/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/pyproject.toml` & `hikari_orchestrator-0.1.1/piped/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/docs.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/flake8.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/freeze-locks.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/freeze-locks.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.in` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/library-flake8.in`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/library-flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/lint.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/nox.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/nox.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/publish.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/reformat.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/reformat.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/tests.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/type-checking.txt` & `hikari_orchestrator-0.1.1/piped/python/base-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/noxfile.py` & `hikari_orchestrator-0.1.1/piped/python/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/noxfile.template.py` & `hikari_orchestrator-0.1.1/piped/python/noxfile.template.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/piped/python/piped_shared/__init__.py` & `hikari_orchestrator-0.1.1/piped/python/piped_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/pyproject.toml` & `hikari_orchestrator-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.3,<4,!=3.7"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "hikari-orchestrator"
-version = "0.1.0.post"
+version = "0.1.1"
 readme = "README.md"
 requires-python = ">=3.10.0,<3.12"
 license = {file = "LICENSE"}
 authors = [ {name = "Faster Speeding", email="lucina@lmbyrne.dev"} ]
 keywords = ["hikari"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `hikari_orchestrator-0.1.0.post0/schema.proto` & `hikari_orchestrator-0.1.1/schema.proto`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0.post0/PKG-INFO` & `hikari_orchestrator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-orchestrator
-Version: 0.1.0.post0
+Version: 0.1.1
 Summary: System for managing hikari shards across processes/systems.
 Keywords: hikari
 Author-email: Faster Speeding <lucina@lmbyrne.dev>
 Requires-Python: >=3.10.0,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

