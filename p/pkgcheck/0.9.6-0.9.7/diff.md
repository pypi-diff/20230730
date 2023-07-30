# Comparing `tmp/pkgcheck-0.9.6.tar.gz` & `tmp/pkgcheck-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgcheck-0.9.6.tar", last modified: Fri Mar 26 22:46:45 2021, max compression
+gzip compressed data, was "pkgcheck-0.9.7.tar", last modified: Sat Mar 27 17:23:49 2021, max compression
```

## Comparing `pkgcheck-0.9.6.tar` & `pkgcheck-0.9.7.tar`

### file list

```diff
@@ -1,1551 +1,1551 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      371 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    45547 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3866 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/bin/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/bin/pkgcheck -> ../src/pkgcheck/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/completion/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (121)     8098 2021-03-26 22:43:43.090679 pkgcheck-0.9.6/completion/zsh/_pkgcheck
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/data/
--rwxr-xr-x   0 runner    (1001) docker     (121)      414 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/data/ci.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/data/perl-version.pl
--rw-r--r--   0 runner    (1001) docker     (121)      717 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/data/pkgcheck.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11029 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/doc/generate/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/doc/generate/pkgcheck/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2286 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/generate/pkgcheck/checks.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2115 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/generate/pkgcheck/keywords.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1166 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/generate/pkgcheck/reporters.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/doc/man/
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/man/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/man/pkgcheck.rst
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/doc/news.rst -> ../NEWS.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.880338 pkgcheck-0.9.6/man/
--rw-r--r--   0 runner    (1001) docker     (121)    94303 2021-03-26 22:46:44.884338 pkgcheck-0.9.6/man/pkgcheck.1
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-03-26 22:46:45.084340 pkgcheck-0.9.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.936339 pkgcheck-0.9.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/dist.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/requirements/tox.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     7175 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.084340 pkgcheck-0.9.6/src/pkgcheck/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-26 22:46:45.084340 pkgcheck-0.9.6/src/pkgcheck/_verinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/src/pkgcheck/addons/
--rw-r--r--   0 runner    (1001) docker     (121)    12253 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4834 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/addons/caches.py
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/addons/eclass.py
--rw-r--r--   0 runner    (1001) docker     (121)    21039 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/addons/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/addons/net.py
--rw-r--r--   0 runner    (1001) docker     (121)    19003 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/addons/profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6804 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/src/pkgcheck/bash/
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/bash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/src/pkgcheck/checks/
--rw-r--r--   0 runner    (1001) docker     (121)     6941 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/acct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)    32059 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/codingstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/dropped_keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)    11140 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/eclass.py
--rw-r--r--   0 runner    (1001) docker     (121)    23974 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/glsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/header.py
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/imlate.py
--rw-r--r--   0 runner    (1001) docker     (121)    52229 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    17790 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/metadata_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)    11003 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/network.py
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/overlays.py
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/perl.py
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/pkgdir.py
--rw-r--r--   0 runner    (1001) docker     (121)    14780 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    13182 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)    25198 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/repo_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/stablereq.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/unstable_only.py
--rw-r--r--   0 runner    (1001) docker     (121)    14103 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/visibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/checks/whitespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-03-26 22:43:43.094679 pkgcheck-0.9.6/src/pkgcheck/feeds.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     6305 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)    10281 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     9853 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/reporters.py
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/results.py
--rw-r--r--   0 runner    (1001) docker     (121)     3786 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/src/pkgcheck/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1496 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14357 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/argparse_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/argparsers.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_replay.py
--rw-r--r--   0 runner    (1001) docker     (121)    18372 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     6289 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_show.py
--rw-r--r--   0 runner    (1001) docker     (121)    13180 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/src/pkgcheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/eclass/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/eclass/EapiCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/testdata/data/repos/eclass/EapiCheck/UnsupportedEclassEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EapiCheck/UnsupportedEclassEapi/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EapiCheck/UnsupportedEclassEapi/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassBashSyntaxError/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassBashSyntaxError/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassBashSyntaxError/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.940338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocError/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocError/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocError/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingFunc/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingFunc/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingFunc/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      609 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/InternalEclassUsage/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/InternalEclassUsage/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/InternalEclassUsage/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/MissingInherits/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/MissingInherits/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/MissingInherits/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/UnusedInherits/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/UnusedInherits/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/eclass/InheritsCheck/UnusedInherits/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/gentoo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/CatMissingMetadataXml/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/CatMissingMetadataXml/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/CatMissingMetadataXml/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      609 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidCopyright/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidCopyright/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      963 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassNonGentooAuthorsCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassNonGentooAuthorsCopyright/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      458 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassNonGentooAuthorsCopyright/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassOldGentooCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassOldGentooCopyright/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      462 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassOldGentooCopyright/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.888338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.944338 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      635 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-03-26 22:43:43.098679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/gentoo/PkgDirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       60 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/fix.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoDirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       12 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/fix.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       35 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/trigger.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/LaggingProfileEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/LaggingProfileEapi/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/LaggingProfileEapi/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/NonexistentCategories/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/NonexistentCategories/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/NonexistentCategories/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/ProfileWarning/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/ProfileWarning/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/ProfileWarning/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/UnknownCategoryDirs/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/UnknownCategoryDirs/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/RepoProfilesCheck/UnknownCategoryDirs/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/gentoo/UnstableOnlyCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/gentoo/UnstableOnlyCheck/UnstableOnly/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/UnstableOnlyCheck/UnstableOnly/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/gentoo/UnstableOnlyCheck/UnstableOnly/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/network/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/DeadUrl/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/RedirectedUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/RedirectedUrl/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/SSLCertificateError/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/FetchablesUrlCheck/SSLCertificateError/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/DeadUrl/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/DeadUrl-connection-error/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/DeadUrl-connection-error/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/HttpsUrlAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/HttpsUrlAvailable/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/RedirectedUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/RedirectedUrl/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/SSLCertificateError/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/HomepageUrlCheck/SSLCertificateError/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/DeadUrl/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.948339 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/HttpsUrlAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/HttpsUrlAvailable/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/RedirectedUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/RedirectedUrl/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/SSLCertificateError/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/network/MetadataUrlCheck/SSLCertificateError/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/overlay/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/profiledir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      934 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/
--rw-r--r--   0 runner    (1001) docker     (121)      513 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageUse/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/ArchesWithoutProfiles/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/ArchesWithoutProfiles/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       57 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/ArchesWithoutProfiles/fix.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/NonexistentProfilePath/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/NonexistentProfilePath/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/NonexistentProfilePath/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/ProfileError/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/ProfileError/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/ProfileError/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/UnusedProfileDirs/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/UnusedProfileDirs/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/profiledir/RepoProfilesCheck/UnusedProfileDirs/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/python/PythonCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/python/PythonCheck/PythonMissingDeps/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/python/PythonCheck/PythonMissingDeps/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/python/PythonCheck/PythonMissingDeps/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.892338 pkgcheck-0.9.6/testdata/data/repos/python/PythonCompatCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/BannedEapiCommand/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/BannedEapiCommand/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/BannedEapiCommand/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      502 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      527 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlEmptyElement/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlEmptyElement/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      484 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlEmptyElement/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      566 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.952339 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      582 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/BadDependency/
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/BadDependency/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/BadDependency/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidBdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidBdepend/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-26 22:43:43.102679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidBdepend/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidDepend/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidDepend/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      463 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidDepend/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidPdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidPdepend/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidPdepend/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidRdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidRdepend/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/InvalidRdepend/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      463 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/DescriptionCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DescriptionCheck/BadDescription/
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DescriptionCheck/BadDescription/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DescriptionCheck/BadDescription/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/DroppedKeywordsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/BannedEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/BannedEapi/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/BannedEapi/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/DeprecatedEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/DeprecatedEapi/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EapiCheck/DeprecatedEapi/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/EclassUsageCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/EqualVersionsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUse/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       52 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUse/fix.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUseExpand/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUseExpand/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUseExpand/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/HomepageCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/HomepageCheck/BadHomepage/
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/HomepageCheck/BadHomepage/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/HomepageCheck/BadHomepage/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/InsintoCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.956339 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/BadKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/BadKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/BadKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/DuplicateKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/DuplicateKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/DuplicateKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/OverlappingKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/OverlappingKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/OverlappingKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnknownKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnknownKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnknownKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.896338 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/
--rw-r--r--   0 runner    (1001) docker     (121)      577 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicense/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicense/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicense/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseFile/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseFile/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseFile/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnnecessaryLicense/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnnecessaryLicense/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnnecessaryLicense/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseGroupsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseGroupsCheck/UnknownLicenses/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseGroupsCheck/UnknownLicenses/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseGroupsCheck/UnknownLicenses/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MatchingGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MatchingGlobalUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MatchingGlobalUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-03-26 22:43:43.106679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableGlobalUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableGlobalUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      856 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnusedLocalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnusedLocalUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnusedLocalUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingChksum/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingChksum/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      797 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingChksum/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingManifest/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingManifest/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      917 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      943 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.960339 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingSlotDepCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingUnpackerDepCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/DuplicateFiles/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/DuplicateFiles/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/DuplicateFiles/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/EmptyFile/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/EmptyFile/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       49 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/EmptyFile/fix.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/ExecutableFile/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/ExecutableFile/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       65 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/ExecutableFile/fix.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/ProjectMetadataCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.964339 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/InvalidProperties/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/InvalidProperties/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/InvalidProperties/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnknownProperties/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnknownProperties/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnknownProperties/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      467 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/ReadonlyVariableCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      545 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/RedundantDodirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.900338 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/InvalidRestrict/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/InvalidRestrict/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/InvalidRestrict/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnknownRestrict/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-26 22:43:43.110679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnknownRestrict/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      469 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnknownRestrict/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictTestCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictTestCheck/MissingTestRestrict/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictTestCheck/MissingTestRestrict/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/RestrictTestCheck/MissingTestRestrict/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/SourcingError/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/SourcingError/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/SourcingError/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadFilename/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadFilename/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadFilename/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      632 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/MissingUri/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/MissingUri/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/MissingUri/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.968339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedEclassesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedEclassesCheck/UnusedEclasses/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedEclassesCheck/UnusedEclasses/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedEclassesCheck/UnusedEclasses/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedLicensesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedLicensesCheck/UnusedLicenses/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedLicensesCheck/UnusedLicenses/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedLicensesCheck/UnusedLicenses/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedMirrorsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedMirrorsCheck/UnusedMirrors/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedMirrorsCheck/UnusedMirrors/expected.json
--rwxr-xr-x   0 runner    (1001) docker     (121)       59 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/UnusedMirrorsCheck/UnusedMirrors/fix.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/VariableScopeCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      536 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/
--rw-r--r--   0 runner    (1001) docker     (121)      517 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      887 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/
--rw-r--r--   0 runner    (1001) docker     (121)      722 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/DoubleEmptyLine/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/DoubleEmptyLine/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/DoubleEmptyLine/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/NoFinalNewline/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/NoFinalNewline/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/NoFinalNewline/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/TrailingEmptyLine/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/TrailingEmptyLine/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/TrailingEmptyLine/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/visibility/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/visibility/DependencyCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected-verbose.json
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/fix.patch
--rwxr-xr-x   0 runner    (1001) docker     (121)     1509 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/pkgcheck
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.908338 pkgcheck-0.9.6/testdata/repos/eclass/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/repos/eclass/EapiCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/repos/eclass/EapiCheck/UnsupportedEclassEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/EapiCheck/UnsupportedEclassEapi/UnsupportedEclassEapi-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/repos/eclass/EclassUsageCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/repos/eclass/EclassUsageCheck/DeprecatedEclass/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/EclassUsageCheck/DeprecatedEclass/DeprecatedEclass-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/EclassUsageCheck/DeprecatedEclass/DeprecatedEclass-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/repos/eclass/EclassUsageCheck/MisplacedEclassVar/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/EclassUsageCheck/MisplacedEclassVar/MisplacedEclassVar-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.904338 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/InternalEclassUsage/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/InternalEclassUsage/InternalEclassUsage-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/MissingInherits/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/MissingInherits/MissingInherits-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/MissingInherits/MissingInherits-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.972339 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/UnusedInherits/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/InheritsCheck/UnusedInherits/UnusedInherits-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/eclass/eclass/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/bad.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/deprecated.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/deprecated2.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      414 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/inherit.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/missing-docs.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/no-maintainer.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/pre-inherit.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/replacement.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/stub.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/unused.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/eclass/vcs.eclass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/eclass/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/licenses/BSD -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/eclass/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.114679 pkgcheck-0.9.6/testdata/repos/eclass/metadata/layout.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/eclass/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/eclass/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.908338 pkgcheck-0.9.6/testdata/repos/eclass/stub/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/eclass/stub/stub1/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/eclass/stub/stub1/stub1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.908338 pkgcheck-0.9.6/testdata/repos/gentoo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.908338 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/stub1/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/stub1/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/stub1/stub1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/stub2/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/stub2/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/CatMissingMetadataXml/stub2/stub2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/EbuildInvalidCopyright-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/EbuildInvalidLicenseHeader-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/EbuildInvalidLicenseHeader-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/EbuildNonGentooAuthorsCopyright-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/EbuildOldGentooCopyright-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EbuildHeaderCheck/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EmptyCategoryDir/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EmptyCategoryDir/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EmptyDirsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/EmptyDirsCheck/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/MaintainerNeeded-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded2/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded2/MaintainerNeeded2-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded2/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/MaintainerWithoutProxy-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.976339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy2/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy2/MaintainerWithoutProxy2-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy2/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/NonexistentProjectMaintainer-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/PkgMissingMetadataXml-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/ProxyWithoutProxied-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied2/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied2/ProxyWithoutProxied2-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied2/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied3/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied3/ProxyWithoutProxied3-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied3/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/RedundantLongDescription-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.980339 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/WrongMaintainerType-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PackageMetadataXmlCheck/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/UnknownPkgDirEntry-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/bar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/bar/.stub
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/foo
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/PkgDirCheck/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/UnstableOnlyCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/UnstableOnlyCheck/UnstableOnly/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/UnstableOnlyCheck/UnstableOnly/UnstableOnly-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/UnstableOnlyCheck/UnstableOnly/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/UnstableOnlyCheck/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/eclass/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/eclass/invalid-copyright.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/eclass/invalid-license-header.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/eclass/missing-license-header.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/eclass/non-gentoo-copyright.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/eclass/old-gentoo-copyright.eclass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/licenses/BSD -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.984339 pkgcheck-0.9.6/testdata/repos/gentoo/metadata/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/gentoo/metadata/glsa/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/metadata/glsa/glsa-000000-00.xml
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/metadata/layout.conf
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/metadata/projects.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/arch.list
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/arches.desc
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/categories
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/eapi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/linux/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/linux/eapi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/linux/lagging/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/linux/lagging/parent
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/linux/make.defaults
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/linux/parent
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/default/make.defaults
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/eapi
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/profiles.desc
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/gentoo/unknown/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/gentoo/unknown/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/network/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.908338 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.988339 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/DeadUrl/DeadUrl-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/DeadUrl/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/DeadUrl/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.992339 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/HttpsUrlAvailable-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      418 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.992339 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/RedirectedUrl-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.992339 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/SSLCertificateError-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.992339 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/ftp-DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/ftp-DeadUrl/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/FetchablesUrlCheck/ftp-DeadUrl/ftp-DeadUrl-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.992339 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/DeadUrl/DeadUrl-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/DeadUrl/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.992339 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/DeadUrl-connection-error/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/DeadUrl-connection-error/DeadUrl-connection-error-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/DeadUrl-connection-error/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.996339 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/HttpsUrlAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/HttpsUrlAvailable/HttpsUrlAvailable-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      396 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/HttpsUrlAvailable/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.996339 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/RedirectedUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/RedirectedUrl/RedirectedUrl-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-03-26 22:43:43.118679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/RedirectedUrl/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.996339 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/SSLCertificateError/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/SSLCertificateError/SSLCertificateError-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/SSLCertificateError/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.996339 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/ftp-DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/HomepageUrlCheck/ftp-DeadUrl/ftp-DeadUrl-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.996339 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl/DeadUrl-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.996339 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl-missingfile/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl-missingfile/DeadUrl-missingfile-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/DeadUrl-missingfile/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/HttpsUrlAvailable-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/RedirectedUrl-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/SSLCertificateError-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/network/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/licenses/BSD -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/network/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/metadata/layout.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/network/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/network/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/overlay/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/UnusedInMastersEclasses-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/UnusedInMastersGlobalUse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.000339 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/UnusedInMastersLicenses-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/UnusedInMastersMirrors-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlay/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/metadata/layout.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlay/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlay/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/overlayed/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlayed/eclass/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/eclass/unused.eclass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlayed/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/licenses/BSD -> ../../../../LICENSE
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/licenses/unused -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlayed/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/metadata/layout.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/arch.list
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/default/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/default/make.defaults
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/profiles.desc
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/repo_name
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/thirdpartymirrors
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/profiles/use.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/overlayed/stub/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/overlayed/stub/stub1/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/overlayed/stub/stub1/stub1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/profiledir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/profiledir/cat/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg1/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg1/pkg1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg2/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg2/pkg2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.004339 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg3/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg3/pkg3-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg4/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/cat/pkg4/pkg4-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/licenses/BSD -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/metadata/layout.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/arch.list
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/bad_parent/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/bad_parent/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/forgotten/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/forgotten/eapi
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/make.defaults
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/default/package.use
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/deprecated/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/deprecated/empty/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/deprecated/empty/deprecated
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/deprecated/nonexistent/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/deprecated/nonexistent/deprecated
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/profiles.desc
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.008339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_kwds/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_kwds/package.accept_keywords
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_kwds/package.keywords
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.012339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_pkgs/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_pkgs/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_pkgs/package.unmask
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_pkgs/package.use
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_pkgs/packages
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.012339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.012339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/eapi
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/use.force
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/use.stable.force
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.012339 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/eapi
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/use.mask
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/use.stable.mask
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/use.force
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/use.mask
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/use.stable.force
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/unknown_use/use.stable.mask
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/profiledir/profiles/use.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/python/PythonCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.012339 pkgcheck-0.9.6/testdata/repos/python/PythonCheck/PythonMissingDeps/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-03-26 22:43:43.122679 pkgcheck-0.9.6/testdata/repos/python/PythonCheck/PythonMissingDeps/PythonMissingDeps-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/python/PythonCompatCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.012339 pkgcheck-0.9.6/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/PythonCompatUpdate-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/PythonCompatUpdate-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/PythonCompatUpdate-2.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.912338 pkgcheck-0.9.6/testdata/repos/python/dev-lang/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/dev-lang/python/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/dev-lang/python/python-2.7.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/dev-lang/python/python-3.7.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/dev-lang/python/python-3.8.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/dev-lang/python/python-3.9.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/eclass/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/eclass/python-any-r1.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/eclass/python-r1.eclass
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/eclass/python-single-r1.eclass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/licenses/BSD -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/metadata/layout.conf
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/metadata/stubs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/profiles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/profiles/desc/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/profiles/desc/python_single_target.desc
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/profiles/desc/python_targets.desc
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/python/stub/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep-old1/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep-old1/python-dep-old1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep-old2/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep-old2/python-dep-old2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.016339 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep1/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep1/python-dep1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep2/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python-dep2/python-dep2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/python/stub/python2-locked/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python2-locked/python2-locked-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python2-locked/python2-locked-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/python2-locked/python2-locked-2.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/python/stub/stub1/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/stub1/stub1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/python/stub/stub2/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/stub2/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/python/stub/stub2/stub2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/BadCommandsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/BadCommandsCheck/BannedEapiCommand/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/BadCommandsCheck/BannedEapiCommand/BannedEapiCommand-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/DeprecatedEapiCommand-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/CatBadlyFormedXml/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatBadlyFormedXml/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/CatBadlyFormedXml/stub/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatBadlyFormedXml/stub/stub-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/CatInvalidXml/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatInvalidXml/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/CatInvalidXml/stub/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatInvalidXml/stub/stub-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlEmptyElement/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlEmptyElement/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.020339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlEmptyElement/stub/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlEmptyElement/stub/stub-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlIndentation/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlIndentation/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlIndentation/stub/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlIndentation/stub/stub-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/stub/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/stub/stub-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/stub/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/stub/stub-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/BadDependency/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/BadDependency/BadDependency-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidBdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidBdepend/InvalidBdepend-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidDepend/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidDepend/InvalidDepend-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidPdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidPdepend/InvalidPdepend-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidRdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/InvalidRdepend/InvalidRdepend-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/MissingPackageRevision/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/MissingPackageRevision/MissingPackageRevision-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/MissingUseDepDefault/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/MissingUseDepDefault/MissingUseDepDefault-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.024339 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DependencyCheck/UnstatedIuse/UnstatedIuse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.028339 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/BadDescription/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-2.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-3.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-4.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/DroppedKeywordsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.028339 pkgcheck-0.9.6/testdata/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/DroppedKeywords-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/DroppedKeywords-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/EapiCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.028339 pkgcheck-0.9.6/testdata/repos/standalone/EapiCheck/BannedEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EapiCheck/BannedEapi/BannedEapi-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.028339 pkgcheck-0.9.6/testdata/repos/standalone/EapiCheck/DeprecatedEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EapiCheck/DeprecatedEapi/DeprecatedEapi-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/EclassUsageCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.028339 pkgcheck-0.9.6/testdata/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/DuplicateEclassInherit-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/DuplicateEclassInherit-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/EqualVersionsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.028339 pkgcheck-0.9.6/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0-r0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0-r01.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0-r1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/GlobalUseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.032339 pkgcheck-0.9.6/testdata/repos/standalone/GlobalUseCheck/PotentialGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/GlobalUseCheck/PotentialGlobalUse/PotentialGlobalUse-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/GlobalUseCheck/PotentialGlobalUse/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.032339 pkgcheck-0.9.6/testdata/repos/standalone/GlobalUseCheck/PotentialLocalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/GlobalUseCheck/PotentialLocalUse/PotentialLocalUse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.916338 pkgcheck-0.9.6/testdata/repos/standalone/HomepageCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.032339 pkgcheck-0.9.6/testdata/repos/standalone/HomepageCheck/BadHomepage/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-2.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-3.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/InsintoCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.032339 pkgcheck-0.9.6/testdata/repos/standalone/InsintoCheck/DeprecatedInsinto/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/InsintoCheck/DeprecatedInsinto/DeprecatedInsinto-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      396 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/InsintoCheck/DeprecatedInsinto/DeprecatedInsinto-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/InvalidUseFlags/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/InvalidUseFlags/InvalidUseFlags-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/InvalidUseFlags/InvalidUseFlags-4.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/InvalidUseFlags/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/UnknownUseFlags/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/UnknownUseFlags/UnknownUseFlags-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/IuseCheck/UnknownUseFlags/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/BadKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/BadKeywords/BadKeywords-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/DuplicateKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/DuplicateKeywords/DuplicateKeywords-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/OverlappingKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/OverlappingKeywords/OverlappingKeywords-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/UnknownKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/UnknownKeywords/UnknownKeywords-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/UnsortedKeywords/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-26 22:43:43.126679 pkgcheck-0.9.6/testdata/repos/standalone/KeywordsCheck/UnsortedKeywords/UnsortedKeywords-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/InvalidLicense/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/InvalidLicense/InvalidLicense-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/InvalidLicense/InvalidLicense-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/InvalidLicense/InvalidLicense-2.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicense/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicense/MissingLicense-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.036339 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicenseFile/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicenseFile/MissingLicenseFile-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/MissingLicenseRestricts-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/MissingLicenseRestricts-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LicenseCheck/UnstatedIuse/UnstatedIuse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/MatchingGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/MatchingGlobalUse/MatchingGlobalUse-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/MatchingGlobalUse/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/MissingLocalUseDesc/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/MissingLocalUseDesc/MissingLocalUseDesc-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/MissingLocalUseDesc/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/ProbableGlobalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/ProbableGlobalUse/ProbableGlobalUse-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/ProbableGlobalUse/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/ProbableUseExpand/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/ProbableUseExpand/ProbableUseExpand-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      269 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/ProbableUseExpand/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/UnderscoreInUseFlag-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.040339 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/UnusedLocalUse/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/UnusedLocalUse/UnusedLocalUse-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/LocalUseCheck/UnusedLocalUse/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/DeprecatedChksum/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/DeprecatedChksum/DeprecatedChksum-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/DeprecatedChksum/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/InvalidManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/InvalidManifest/InvalidManifest-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/InvalidManifest/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/MissingChksum/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/MissingChksum/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/MissingChksum/MissingChksum-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/MissingManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/MissingManifest/MissingManifest-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnknownManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnknownManifest/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnknownManifest/UnknownManifest-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/UnnecessaryManifest-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/ConflictingChksums/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/ConflictingChksums/ConflictingChksums-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/ConflictingChksums/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.044339 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/MatchingChksums/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/MatchingChksums/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ManifestCollisionCheck/MatchingChksums/MatchingChksums-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/HomepageInSrcUri/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/HomepageInSrcUri/HomepageInSrcUri-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/HomepageInSrcUri/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/MultipleKeywordsLines-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/MultipleKeywordsLines-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/ReferenceInMetadataVar-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/ReferenceInMetadataVar-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/StaticSrcUri/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/StaticSrcUri/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MetadataVarCheck/StaticSrcUri/StaticSrcUri-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/MissingSlotDepCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/MissingSlotDepCheck/MissingSlotDep/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MissingSlotDepCheck/MissingSlotDep/MissingSlotDep-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.920338 pkgcheck-0.9.6/testdata/repos/standalone/MissingUnpackerDepCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/MissingUnpackerDep-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/PkgBadlyFormedXml-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/PkgInvalidXml-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.052339 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/PkgMetadataXmlEmptyElement-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/PkgMetadataXmlIndentation-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/PkgMetadataXmlInvalidCatRef-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/PkgMetadataXmlInvalidPkgRef-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/RedundantLongDescription-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/DuplicateFiles-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/files/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/files/1
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/files/2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/EmptyFile/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/EmptyFile/EmptyFile-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/EmptyFile/files/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/EmptyFile/files/empty
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/ExecutableFile/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/ExecutableFile/ExecutableFile-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.056340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/ExecutableFile/files/
--rwxr-xr-x   0 runner    (1001) docker     (121)        2 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/ExecutableFile/files/executable
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/InvalidPN/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/InvalidPN/InvalidPN.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/MismatchedPN/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/MismatchedPN/Mismatched-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/UnknownPkgDirEntry/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/UnknownPkgDirEntry/UnknownPkgDirEntry-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PkgDirCheck/UnknownPkgDirEntry/foo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/InvalidProperties/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/InvalidProperties/InvalidProperties-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/UnknownProperties/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/UnknownProperties/UnknownProperties-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/PropertiesCheck/UnstatedIuse/UnstatedIuse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/ReadonlyVariableCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/ReadonlyVariable-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/RedundantDodirCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/RedundantDodirCheck/RedundantDodir/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RedundantDodirCheck/RedundantDodir/RedundantDodir-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/InvalidRequiredUse-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/InvalidRequiredUse-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/InvalidRequiredUse-2.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/RequiredUseDefaults/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/RequiredUseDefaults/RequiredUseDefaults-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/RequiredUseDefaults/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.060340 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/UnstatedIuse/UnstatedIuse-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RequiredUseCheck/UnstatedIuse/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/InvalidRestrict/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-26 22:43:43.130679 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/InvalidRestrict/InvalidRestrict-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/UnknownRestrict/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/UnknownRestrict/UnknownRestrict-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/RestrictCheck/UnstatedIuse/UnstatedIuse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/RestrictTestCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/RestrictTestCheck/MissingTestRestrict/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/RestrictTestCheck/MissingTestRestrict/MissingTestRestrict-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.924338 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidEapi/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidEapi/InvalidEapi-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidEapi/InvalidEapi-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-2.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-3.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-4.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-5.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/SourcingError/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SourcingCheck/SourcingError/SourcingError-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadFilename/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadFilename/BadFilename-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      893 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadFilename/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadProtocol/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadProtocol/BadProtocol-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadProtocol/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/InvalidSrcUri-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/InvalidSrcUri-1.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/InvalidSrcUri-2.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/MissingUri/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/MissingUri/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/MissingUri/MissingUri-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/
--rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/RedundantUriRename-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/RedundantUriRename-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/TarballAvailable/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/TarballAvailable/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/TarballAvailable/TarballAvailable-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/UnknownMirror/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/UnknownMirror/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/UnknownMirror/UnknownMirror-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/UnstatedIuse/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/UnstatedIuse/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/UnstatedIuse/UnstatedIuse-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/VariableScopeCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/VariableScopeCheck/EbuildVariableScope/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/VariableScopeCheck/EbuildVariableScope/EbuildVariableScope-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/VisibilityCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/VisibilityCheck/NonexistentDeps/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/VisibilityCheck/NonexistentDeps/NonexistentDeps-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/VisibilityCheck/VisibleVcsPkg/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/VisibilityCheck/VisibleVcsPkg/VisibleVcsPkg-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/VisibilityCheck/VisibleVcsPkg/VisibleVcsPkg-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.064339 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/BadWhitespaceCharacter-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/DoubleEmptyLine/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/DoubleEmptyLine/DoubleEmptyLine-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/NoFinalNewline/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/NoFinalNewline/NoFinalNewline-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/TrailingEmptyLine/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/WhitespaceCheck/TrailingEmptyLine/TrailingEmptyLine-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/app-arch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/app-arch/unzip/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/app-arch/unzip/unzip-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/eclass/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/eclass/stub.eclass
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/eclass/unused.eclass
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/eclass/vcs.eclass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/licenses/BSD -> ../../../../LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/licenses/eula
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/licenses/unused
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/metadata/layout.conf
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/metadata/projects.xml
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/metadata/stubs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/arch.list
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/profiles/default/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/profiles/default/amd64/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/default/amd64/make.defaults
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/profiles/default/x86/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/default/x86/make.defaults
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/profiles/desc/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/desc/use_expand.desc
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/license_groups
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/profiles.desc
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/repo_name
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/thirdpartymirrors
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/use.desc
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/profiles/use.local.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/stub/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global1/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global1/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global1/potential-global1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global2/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global2/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global2/potential-global2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global3/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global3/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global3/potential-global3-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global4/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global4/metadata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/potential-global4/potential-global4-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/slotted/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/slotted/slotted-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/slotted/slotted-1.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub1/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub1/stub1-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub2/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub2/stub2-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub3/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub3/stub3-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub4/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/stub/stub4/stub4-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/test/ConflictingChksums/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/test/ConflictingChksums/ConflictingChksums-0.ebuild
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/test/ConflictingChksums/Manifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/test/MatchingChksums/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/test/MatchingChksums/Manifest
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/test/MatchingChksums/MatchingChksums-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/standalone/virtual/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/standalone/virtual/UnnecessaryLicense/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/standalone/virtual/UnnecessaryLicense/UnnecessaryLicense-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.928338 pkgcheck-0.9.6/testdata/repos/visibility/DeprecatedDep/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/visibility/DeprecatedDep/nonoptional/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/DeprecatedDep/nonoptional/nonoptional-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/visibility/DeprecatedDep/optional/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/DeprecatedDep/optional/optional-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInDev/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInDev/masked/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInDev/masked/masked-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInExp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInExp/masked/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInExp/masked/masked-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInStable/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.068340 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInStable/masked/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInStable/masked/masked-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInStable/unstable/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/NonsolvableDepsInStable/unstable/unstable-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/licenses/
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.134679 pkgcheck-0.9.6/testdata/repos/visibility/licenses/BSD -> ../../../../LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/metadata/layout.conf
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/metadata/pkgcheck-args
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/profiles/arch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/arch/amd64/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/arch/amd64/make.defaults
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/arch/x86/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/arch/x86/make.defaults
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/arch.list
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/package.deprecated
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/profiles.desc
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/repo_name
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/dev/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/dev/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/dev/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/exp/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/exp/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/exp/parent
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/stable/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/stable/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/amd64/stable/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/dev/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/dev/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/dev/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/exp/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/exp/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/exp/parent
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/stable/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/stable/package.mask
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/profiles/visibility/x86/stable/parent
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:44.932338 pkgcheck-0.9.6/testdata/repos/visibility/stub/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/stub/deprecated/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/stub/deprecated/deprecated-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/stub/masked/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/stub/masked/masked-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/stub/stable/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/stub/stable/stable-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/testdata/repos/visibility/stub/unstable/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/testdata/repos/visibility/stub/unstable/unstable-0.ebuild
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.072340 pkgcheck-0.9.6/tests/addons/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16621 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/addons/test_addons.py
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/addons/test_eclass.py
--rw-r--r--   0 runner    (1001) docker     (121)    29875 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/addons/test_git.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/tests/checks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3857 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_acct.py
--rw-r--r--   0 runner    (1001) docker     (121)     4750 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_all.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)    11889 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_codingstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2930 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_dropped_keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)    25906 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_git.py
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_glsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     4313 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     5615 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_imlate.py
--rw-r--r--   0 runner    (1001) docker     (121)    56056 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_perl.py
--rw-r--r--   0 runner    (1001) docker     (121)    19451 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_pkgdir.py
--rw-r--r--   0 runner    (1001) docker     (121)    22321 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_repo_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     7290 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_stablereq.py
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/checks/test_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7870 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16152 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_argparse_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_pkgcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_pkgcheck_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_pkgcheck_ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_pkgcheck_replay.py
--rw-r--r--   0 runner    (1001) docker     (121)    27976 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_pkgcheck_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/scripts/test_pkgcheck_show.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5612 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     6684 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tests/test_reporters.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/tree-sitter-bash/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-03-26 22:43:43.138679 pkgcheck-0.9.6/tree-sitter-bash/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/tree-sitter-bash/src/
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-03-26 22:43:43.142679 pkgcheck-0.9.6/tree-sitter-bash/src/binding.cc
--rw-r--r--   0 runner    (1001) docker     (121)    58690 2021-03-26 22:43:43.142679 pkgcheck-0.9.6/tree-sitter-bash/src/grammar.json
--rw-r--r--   0 runner    (1001) docker     (121)    28024 2021-03-26 22:43:43.142679 pkgcheck-0.9.6/tree-sitter-bash/src/node-types.json
--rw-r--r--   0 runner    (1001) docker     (121)  3523435 2021-03-26 22:43:43.150679 pkgcheck-0.9.6/tree-sitter-bash/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (121)    10414 2021-03-26 22:43:43.150679 pkgcheck-0.9.6/tree-sitter-bash/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 22:46:45.076340 pkgcheck-0.9.6/tree-sitter-bash/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (121)     5326 2021-03-26 22:43:43.150679 pkgcheck-0.9.6/tree-sitter-bash/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    45686 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3866 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/bin/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/bin/pkgcheck -> ../src/pkgcheck/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/completion/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (121)     8098 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/completion/zsh/_pkgcheck
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/data/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      414 2021-03-27 17:20:47.480464 pkgcheck-0.9.7/data/ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/data/perl-version.pl
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/data/pkgcheck.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11029 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/doc/generate/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/doc/generate/pkgcheck/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2286 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/generate/pkgcheck/checks.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2115 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/generate/pkgcheck/keywords.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1166 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/generate/pkgcheck/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/doc/man/
+-rw-r--r--   0 runner    (1001) docker     (121)     2420 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/man/config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/man/pkgcheck.rst
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/doc/news.rst -> ../NEWS.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.042366 pkgcheck-0.9.7/man/
+-rw-r--r--   0 runner    (1001) docker     (121)    94303 2021-03-27 17:23:49.042366 pkgcheck-0.9.7/man/pkgcheck.1
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-03-27 17:23:49.194364 pkgcheck-0.9.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/dist.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/requirements/tox.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7175 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.194364 pkgcheck-0.9.7/src/pkgcheck/
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-27 17:23:49.194364 pkgcheck-0.9.7/src/pkgcheck/_verinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/src/pkgcheck/addons/
+-rw-r--r--   0 runner    (1001) docker     (121)    12253 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4834 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/addons/caches.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/addons/eclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21039 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/addons/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/addons/net.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19003 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/addons/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6804 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.102365 pkgcheck-0.9.7/src/pkgcheck/bash/
+-rw-r--r--   0 runner    (1001) docker     (121)     4611 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/bash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/src/pkgcheck/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)     6941 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3835 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/acct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2512 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32059 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/codingstyle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/dropped_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11140 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/eclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23974 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2816 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/glsa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4706 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/imlate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52229 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17790 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/metadata_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11003 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/overlays.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3499 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/perl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11728 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/pkgdir.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14780 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13182 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25198 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/repo_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/stablereq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/unstable_only.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14103 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/checks/whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3015 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1357 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6305 2021-03-27 17:20:47.484464 pkgcheck-0.9.7/src/pkgcheck/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10281 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9853 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/results.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3786 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/src/pkgcheck/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1496 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14357 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/argparse_actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2795 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/argparsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3259 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_replay.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18372 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6289 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_show.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13153 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/src/pkgcheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/repos/eclass/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/repos/eclass/EapiCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EapiCheck/UnsupportedEclassEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EapiCheck/UnsupportedEclassEapi/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EapiCheck/UnsupportedEclassEapi/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassBashSyntaxError/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassBashSyntaxError/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassBashSyntaxError/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocError/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocError/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocError/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingFunc/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingFunc/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingFunc/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/InternalEclassUsage/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/InternalEclassUsage/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/InternalEclassUsage/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/MissingInherits/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/MissingInherits/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/MissingInherits/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/UnusedInherits/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/UnusedInherits/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/eclass/InheritsCheck/UnusedInherits/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.046366 pkgcheck-0.9.7/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/CatMissingMetadataXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/CatMissingMetadataXml/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/CategoryMetadataXmlCheck/CatMissingMetadataXml/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidCopyright/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidCopyright/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.106365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassNonGentooAuthorsCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassNonGentooAuthorsCopyright/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassNonGentooAuthorsCopyright/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassOldGentooCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassOldGentooCopyright/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassOldGentooCopyright/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/PkgDirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       60 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/fix.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoDirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       12 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/fix.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)       35 2021-03-27 17:20:47.488464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoDirCheck/BinaryFile/trigger.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/LaggingProfileEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/LaggingProfileEapi/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/LaggingProfileEapi/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/NonexistentCategories/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/NonexistentCategories/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/NonexistentCategories/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/ProfileWarning/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/ProfileWarning/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/ProfileWarning/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/UnknownCategoryDirs/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/UnknownCategoryDirs/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/RepoProfilesCheck/UnknownCategoryDirs/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/gentoo/UnstableOnlyCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/gentoo/UnstableOnlyCheck/UnstableOnly/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/UnstableOnlyCheck/UnstableOnly/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/gentoo/UnstableOnlyCheck/UnstableOnly/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/network/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/DeadUrl/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/RedirectedUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/RedirectedUrl/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/SSLCertificateError/
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/FetchablesUrlCheck/SSLCertificateError/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/DeadUrl/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/DeadUrl-connection-error/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/DeadUrl-connection-error/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/HttpsUrlAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/HttpsUrlAvailable/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/RedirectedUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/RedirectedUrl/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/SSLCertificateError/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/HomepageUrlCheck/SSLCertificateError/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/DeadUrl/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/HttpsUrlAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/HttpsUrlAvailable/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/RedirectedUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/RedirectedUrl/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/SSLCertificateError/
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/network/MetadataUrlCheck/SSLCertificateError/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/overlay/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.110365 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/profiledir/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.050366 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.054366 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/ArchesWithoutProfiles/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/ArchesWithoutProfiles/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       57 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/ArchesWithoutProfiles/fix.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/NonexistentProfilePath/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/NonexistentProfilePath/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/NonexistentProfilePath/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/ProfileError/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/ProfileError/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/ProfileError/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/UnusedProfileDirs/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/UnusedProfileDirs/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/profiledir/RepoProfilesCheck/UnusedProfileDirs/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.054366 pkgcheck-0.9.7/testdata/data/repos/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.054366 pkgcheck-0.9.7/testdata/data/repos/python/PythonCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/python/PythonCheck/PythonMissingDeps/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/python/PythonCheck/PythonMissingDeps/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/python/PythonCheck/PythonMissingDeps/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.054366 pkgcheck-0.9.7/testdata/data/repos/python/PythonCompatCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/standalone/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.054366 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/BannedEapiCommand/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/BannedEapiCommand/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/BannedEapiCommand/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.054366 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlEmptyElement/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlEmptyElement/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlEmptyElement/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.114365 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/BadDependency/
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/BadDependency/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/BadDependency/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidBdepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidBdepend/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidBdepend/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidDepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidDepend/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidDepend/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidPdepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidPdepend/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidPdepend/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidRdepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidRdepend/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/InvalidRdepend/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-27 17:20:47.492464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/UnstatedIuse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/DescriptionCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DescriptionCheck/BadDescription/
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DescriptionCheck/BadDescription/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2661 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DescriptionCheck/BadDescription/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/DroppedKeywordsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.118365 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/BannedEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/BannedEapi/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/BannedEapi/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/DeprecatedEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/DeprecatedEapi/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EapiCheck/DeprecatedEapi/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/EclassUsageCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/EqualVersionsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUse/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       52 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUse/fix.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUseExpand/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUseExpand/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/UnusedGlobalUseExpand/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/HomepageCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/HomepageCheck/BadHomepage/
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/HomepageCheck/BadHomepage/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/HomepageCheck/BadHomepage/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/InsintoCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.062366 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/BadKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/BadKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/BadKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/DuplicateKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/DuplicateKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/DuplicateKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/OverlappingKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/OverlappingKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/OverlappingKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnknownKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnknownKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnknownKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/KeywordsCheck/UnsortedKeywords/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.122365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicense/
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicense/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicense/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseFile/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseFile/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseFile/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnnecessaryLicense/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnnecessaryLicense/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-03-27 17:20:47.496464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnnecessaryLicense/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/UnstatedIuse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseGroupsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseGroupsCheck/UnknownLicenses/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseGroupsCheck/UnknownLicenses/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseGroupsCheck/UnknownLicenses/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MatchingGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MatchingGlobalUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MatchingGlobalUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableGlobalUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableGlobalUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnusedLocalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnusedLocalUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnusedLocalUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingChksum/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingChksum/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingChksum/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingManifest/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingManifest/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1442 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.126365 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingSlotDepCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.066366 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingUnpackerDepCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.130365 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/DuplicateFiles/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/DuplicateFiles/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/DuplicateFiles/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/EmptyFile/
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/EmptyFile/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       49 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/EmptyFile/fix.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/ExecutableFile/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/ExecutableFile/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       65 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/ExecutableFile/fix.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/ProjectMetadataCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/InvalidProperties/
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/InvalidProperties/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/InvalidProperties/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnknownProperties/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnknownProperties/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnknownProperties/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/PropertiesCheck/UnstatedIuse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/ReadonlyVariableCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/RedundantDodirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.134365 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1667 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2021-03-27 17:20:47.500464 pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/UnstatedIuse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/InvalidRestrict/
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/InvalidRestrict/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/InvalidRestrict/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnknownRestrict/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnknownRestrict/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnknownRestrict/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictCheck/UnstatedIuse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictTestCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictTestCheck/MissingTestRestrict/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictTestCheck/MissingTestRestrict/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/RestrictTestCheck/MissingTestRestrict/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2730 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/SourcingError/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/SourcingError/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/SourcingError/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadFilename/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadFilename/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadFilename/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/MissingUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/MissingUri/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/MissingUri/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnstatedIuse/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedEclassesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedEclassesCheck/UnusedEclasses/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedEclassesCheck/UnusedEclasses/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedEclassesCheck/UnusedEclasses/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedLicensesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.138365 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedLicensesCheck/UnusedLicenses/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedLicensesCheck/UnusedLicenses/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedLicensesCheck/UnusedLicenses/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedMirrorsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedMirrorsCheck/UnusedMirrors/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedMirrorsCheck/UnusedMirrors/expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)       59 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/UnusedMirrorsCheck/UnusedMirrors/fix.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.070366 pkgcheck-0.9.7/testdata/data/repos/standalone/VariableScopeCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/DoubleEmptyLine/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/DoubleEmptyLine/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/DoubleEmptyLine/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/NoFinalNewline/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/NoFinalNewline/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/NoFinalNewline/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/TrailingEmptyLine/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/TrailingEmptyLine/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/TrailingEmptyLine/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/visibility/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/visibility/DependencyCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInDev/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInExp/fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected-verbose.json
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/fix.patch
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1509 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/pkgcheck
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/repos/eclass/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/repos/eclass/EapiCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/EapiCheck/UnsupportedEclassEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/EapiCheck/UnsupportedEclassEapi/UnsupportedEclassEapi-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/repos/eclass/EclassUsageCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/EclassUsageCheck/DeprecatedEclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/EclassUsageCheck/DeprecatedEclass/DeprecatedEclass-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/EclassUsageCheck/DeprecatedEclass/DeprecatedEclass-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/EclassUsageCheck/MisplacedEclassVar/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/EclassUsageCheck/MisplacedEclassVar/MisplacedEclassVar-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/InternalEclassUsage/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/InternalEclassUsage/InternalEclassUsage-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/MissingInherits/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/MissingInherits/MissingInherits-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/MissingInherits/MissingInherits-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/UnusedInherits/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/InheritsCheck/UnusedInherits/UnusedInherits-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/eclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/bad.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/deprecated.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/deprecated2.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/inherit.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/missing-docs.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/no-maintainer.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/pre-inherit.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/replacement.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/stub.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/unused.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/eclass/vcs.eclass
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/licenses/BSD -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/metadata/layout.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/repos/eclass/stub/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.142365 pkgcheck-0.9.7/testdata/repos/eclass/stub/stub1/
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/eclass/stub/stub1/stub1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/gentoo/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.074365 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/stub1/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/stub1/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/stub1/stub1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/stub2/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/stub2/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/gentoo/CatMissingMetadataXml/stub2/stub2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-27 17:20:47.504464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/EbuildInvalidCopyright-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/EbuildInvalidLicenseHeader-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/EbuildInvalidLicenseHeader-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/EbuildNonGentooAuthorsCopyright-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/EbuildOldGentooCopyright-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EbuildHeaderCheck/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EmptyCategoryDir/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EmptyCategoryDir/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EmptyDirsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/EmptyDirsCheck/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/MaintainerNeeded-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded2/
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded2/MaintainerNeeded2-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded2/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/MaintainerWithoutProxy-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy2/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy2/MaintainerWithoutProxy2-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy2/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/NonexistentProjectMaintainer-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/PkgMissingMetadataXml-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/ProxyWithoutProxied-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied2/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied2/ProxyWithoutProxied2-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied2/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied3/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied3/ProxyWithoutProxied3-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied3/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/RedundantLongDescription-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/WrongMaintainerType-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PackageMetadataXmlCheck/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/UnknownPkgDirEntry-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/bar/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/bar/.stub
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/foo
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/UnknownPkgDirEntry/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/PkgDirCheck/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/UnstableOnlyCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/UnstableOnlyCheck/UnstableOnly/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/UnstableOnlyCheck/UnstableOnly/UnstableOnly-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/UnstableOnlyCheck/UnstableOnly/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/UnstableOnlyCheck/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.146365 pkgcheck-0.9.7/testdata/repos/gentoo/eclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/eclass/invalid-copyright.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/eclass/invalid-license-header.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/eclass/missing-license-header.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/eclass/non-gentoo-copyright.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/eclass/old-gentoo-copyright.eclass
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/licenses/BSD -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/metadata/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/metadata/glsa/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/metadata/glsa/glsa-000000-00.xml
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/metadata/layout.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/metadata/projects.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/arch.list
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/arches.desc
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/categories
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/eapi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/linux/eapi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/linux/lagging/
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/linux/lagging/parent
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/linux/make.defaults
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/linux/parent
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/default/make.defaults
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/eapi
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/profiles.desc
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/gentoo/unknown/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/gentoo/unknown/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/network/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/DeadUrl/DeadUrl-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/DeadUrl/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/DeadUrl/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/HttpsUrlAvailable-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/HttpsUrlAvailable/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/RedirectedUrl-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/RedirectedUrl/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/SSLCertificateError-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/SSLCertificateError/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/ftp-DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/ftp-DeadUrl/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/FetchablesUrlCheck/ftp-DeadUrl/ftp-DeadUrl-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/DeadUrl/DeadUrl-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/DeadUrl/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/DeadUrl-connection-error/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/DeadUrl-connection-error/DeadUrl-connection-error-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/DeadUrl-connection-error/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/HttpsUrlAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/HttpsUrlAvailable/HttpsUrlAvailable-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/HttpsUrlAvailable/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/RedirectedUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/RedirectedUrl/RedirectedUrl-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/RedirectedUrl/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/SSLCertificateError/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/SSLCertificateError/SSLCertificateError-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/SSLCertificateError/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/ftp-DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/HomepageUrlCheck/ftp-DeadUrl/ftp-DeadUrl-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl/DeadUrl-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl-missingfile/
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl-missingfile/DeadUrl-missingfile-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/DeadUrl-missingfile/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/HttpsUrlAvailable-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/HttpsUrlAvailable/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.150364 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/RedirectedUrl-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-03-27 17:20:47.508464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/RedirectedUrl/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/SSLCertificateError-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/network/MetadataUrlCheck/SSLCertificateError/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/network/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/network/licenses/BSD -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/network/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/network/metadata/layout.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/network/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/network/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/overlay/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.078365 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersEclasses/UnusedInMastersEclasses-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersGlobalUse/UnusedInMastersGlobalUse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersLicenses/UnusedInMastersLicenses-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/UnusedInMastersCheck/UnusedInMastersMirrors/UnusedInMastersMirrors-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlay/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/metadata/layout.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlay/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlay/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/overlayed/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlayed/eclass/
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/eclass/unused.eclass
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlayed/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/licenses/BSD -> ../../../../LICENSE
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/licenses/unused -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlayed/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/metadata/layout.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/arch.list
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/default/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/default/make.defaults
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/profiles.desc
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/repo_name
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/thirdpartymirrors
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/profiles/use.desc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/overlayed/stub/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/overlayed/stub/stub1/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/overlayed/stub/stub1/stub1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/profiledir/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/profiledir/cat/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg1/pkg1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg2/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg2/pkg2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg3/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg3/pkg3-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg4/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/cat/pkg4/pkg4-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/licenses/BSD -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/metadata/layout.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/arch.list
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/bad_parent/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/bad_parent/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/forgotten/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/forgotten/eapi
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/make.defaults
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/default/package.use
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/deprecated/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/deprecated/empty/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/deprecated/empty/deprecated
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/deprecated/nonexistent/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/deprecated/nonexistent/deprecated
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/profiles.desc
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_kwds/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_kwds/package.accept_keywords
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_kwds/package.keywords
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_pkgs/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_pkgs/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_pkgs/package.unmask
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_pkgs/package.use
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_pkgs/packages
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.154364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/eapi
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/use.force
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use/use.stable.force
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/eapi
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/use.mask
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/unknown_stable_use_mask/use.stable.mask
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/use.force
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/use.mask
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/use.stable.force
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/unknown_use/use.stable.mask
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/profiledir/profiles/use.desc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/python/PythonCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/PythonCheck/PythonMissingDeps/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/PythonCheck/PythonMissingDeps/PythonMissingDeps-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/python/PythonCompatCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/PythonCompatUpdate-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/PythonCompatUpdate-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/PythonCompatUpdate-2.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/PythonCompatCheck/PythonCompatUpdate/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/python/dev-lang/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/dev-lang/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/dev-lang/python/python-2.7.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/dev-lang/python/python-3.7.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/dev-lang/python/python-3.8.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/dev-lang/python/python-3.9.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/eclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/eclass/python-any-r1.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/eclass/python-r1.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/eclass/python-single-r1.eclass
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/licenses/BSD -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/metadata/layout.conf
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/metadata/stubs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/profiles/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/profiles/desc/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/profiles/desc/python_single_target.desc
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/profiles/desc/python_targets.desc
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/python/stub/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep-old1/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep-old1/python-dep-old1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep-old2/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep-old2/python-dep-old2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep1/
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep1/python-dep1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep2/
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python-dep2/python-dep2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/python2-locked/
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python2-locked/python2-locked-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python2-locked/python2-locked-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/python2-locked/python2-locked-2.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/stub1/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/stub1/stub1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/python/stub/stub2/
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/stub2/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/python/stub/stub2/stub2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/standalone/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.082365 pkgcheck-0.9.7/testdata/repos/standalone/BadCommandsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/BadCommandsCheck/BannedEapiCommand/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/BadCommandsCheck/BannedEapiCommand/BannedEapiCommand-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/BadCommandsCheck/DeprecatedEapiCommand/DeprecatedEapiCommand-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatBadlyFormedXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatBadlyFormedXml/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatBadlyFormedXml/stub/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatBadlyFormedXml/stub/stub-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatInvalidXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatInvalidXml/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatInvalidXml/stub/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatInvalidXml/stub/stub-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlEmptyElement/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlEmptyElement/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlEmptyElement/stub/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlEmptyElement/stub/stub-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlIndentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlIndentation/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlIndentation/stub/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlIndentation/stub/stub-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/stub/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidCatRef/stub/stub-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/stub/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/CatMetadataXmlInvalidPkgRef/stub/stub-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/BadDependency/
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/BadDependency/BadDependency-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidBdepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidBdepend/InvalidBdepend-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.158364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidDepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.512464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidDepend/InvalidDepend-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidPdepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidPdepend/InvalidPdepend-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidRdepend/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/InvalidRdepend/InvalidRdepend-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/MissingPackageRevision/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/MissingPackageRevision/MissingPackageRevision-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/MissingUseDepDefault/
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/MissingUseDepDefault/MissingUseDepDefault-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DependencyCheck/UnstatedIuse/UnstatedIuse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/BadDescription/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-2.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-3.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DescriptionCheck/BadDescription/BadDescription-4.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/DroppedKeywordsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/DroppedKeywords-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/DroppedKeywords-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/EapiCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/EapiCheck/BannedEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EapiCheck/BannedEapi/BannedEapi-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/EapiCheck/DeprecatedEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EapiCheck/DeprecatedEapi/DeprecatedEapi-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/EclassUsageCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/DuplicateEclassInherit-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/DuplicateEclassInherit-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/EqualVersionsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0-r0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0-r01.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0-r1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/EqualVersionsCheck/EqualVersions/EqualVersions-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/GlobalUseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/GlobalUseCheck/PotentialGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/GlobalUseCheck/PotentialGlobalUse/PotentialGlobalUse-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/GlobalUseCheck/PotentialGlobalUse/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/GlobalUseCheck/PotentialLocalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/GlobalUseCheck/PotentialLocalUse/PotentialLocalUse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/HomepageCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/HomepageCheck/BadHomepage/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-2.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/HomepageCheck/BadHomepage/BadHomepage-3.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/InsintoCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/InsintoCheck/DeprecatedInsinto/
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/InsintoCheck/DeprecatedInsinto/DeprecatedInsinto-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/InsintoCheck/DeprecatedInsinto/DeprecatedInsinto-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/InvalidUseFlags/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/InvalidUseFlags/InvalidUseFlags-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/InvalidUseFlags/InvalidUseFlags-4.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/InvalidUseFlags/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/UnknownUseFlags/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/UnknownUseFlags/UnknownUseFlags-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/IuseCheck/UnknownUseFlags/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/BadKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/BadKeywords/BadKeywords-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/DuplicateKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/DuplicateKeywords/DuplicateKeywords-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/OverlappingKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/OverlappingKeywords/OverlappingKeywords-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/UnknownKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/UnknownKeywords/UnknownKeywords-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/UnsortedKeywords/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/KeywordsCheck/UnsortedKeywords/UnsortedKeywords-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.086365 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/InvalidLicense/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/InvalidLicense/InvalidLicense-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/InvalidLicense/InvalidLicense-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/InvalidLicense/InvalidLicense-2.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicense/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicense/MissingLicense-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicenseFile/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicenseFile/MissingLicenseFile-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/MissingLicenseRestricts-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/MissingLicenseRestricts/MissingLicenseRestricts-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LicenseCheck/UnstatedIuse/UnstatedIuse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.162364 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/MatchingGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/MatchingGlobalUse/MatchingGlobalUse-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/MatchingGlobalUse/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/MissingLocalUseDesc/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/MissingLocalUseDesc/MissingLocalUseDesc-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/MissingLocalUseDesc/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/ProbableGlobalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/ProbableGlobalUse/ProbableGlobalUse-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/ProbableGlobalUse/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/ProbableUseExpand/
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/ProbableUseExpand/ProbableUseExpand-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/ProbableUseExpand/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/UnderscoreInUseFlag-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/UnusedLocalUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/UnusedLocalUse/UnusedLocalUse-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/LocalUseCheck/UnusedLocalUse/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/DeprecatedChksum/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/DeprecatedChksum/DeprecatedChksum-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/DeprecatedChksum/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/InvalidManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/InvalidManifest/InvalidManifest-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/InvalidManifest/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/MissingChksum/
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/MissingChksum/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/MissingChksum/MissingChksum-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/MissingManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/MissingManifest/MissingManifest-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnknownManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnknownManifest/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnknownManifest/UnknownManifest-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/UnnecessaryManifest-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/ConflictingChksums/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/ConflictingChksums/ConflictingChksums-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/ConflictingChksums/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/MatchingChksums/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/MatchingChksums/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/ManifestCollisionCheck/MatchingChksums/MatchingChksums-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/HomepageInSrcUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/HomepageInSrcUri/HomepageInSrcUri-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/HomepageInSrcUri/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/MultipleKeywordsLines-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/MultipleKeywordsLines-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/ReferenceInMetadataVar-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/ReferenceInMetadataVar-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/StaticSrcUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/StaticSrcUri/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MetadataVarCheck/StaticSrcUri/StaticSrcUri-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/MissingSlotDepCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/MissingSlotDepCheck/MissingSlotDep/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MissingSlotDepCheck/MissingSlotDep/MissingSlotDep-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/MissingUnpackerDepCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/MissingUnpackerDep-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/PkgBadlyFormedXml-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/PkgInvalidXml-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/PkgMetadataXmlEmptyElement-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/PkgMetadataXmlIndentation-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/PkgMetadataXmlInvalidCatRef-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2021-03-27 17:20:47.516464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/PkgMetadataXmlInvalidPkgRef-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/RedundantLongDescription-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.166364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/DuplicateFiles-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/files/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/files/1
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/DuplicateFiles/files/2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/EmptyFile/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/EmptyFile/EmptyFile-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/EmptyFile/files/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/EmptyFile/files/empty
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/ExecutableFile/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/ExecutableFile/ExecutableFile-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/ExecutableFile/files/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        2 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/ExecutableFile/files/executable
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/InvalidPN/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/InvalidPN/InvalidPN.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/MismatchedPN/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/MismatchedPN/Mismatched-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/UnknownPkgDirEntry/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/UnknownPkgDirEntry/UnknownPkgDirEntry-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PkgDirCheck/UnknownPkgDirEntry/foo
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/InvalidProperties/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/InvalidProperties/InvalidProperties-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/UnknownProperties/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/UnknownProperties/UnknownProperties-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/PropertiesCheck/UnstatedIuse/UnstatedIuse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.090365 pkgcheck-0.9.7/testdata/repos/standalone/ReadonlyVariableCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/ReadonlyVariable-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/RedundantDodirCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RedundantDodirCheck/RedundantDodir/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RedundantDodirCheck/RedundantDodir/RedundantDodir-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/InvalidRequiredUse-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/InvalidRequiredUse-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/InvalidRequiredUse-2.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/InvalidRequiredUse/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/RequiredUseDefaults/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/RequiredUseDefaults/RequiredUseDefaults-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/RequiredUseDefaults/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/UnstatedIuse/UnstatedIuse-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RequiredUseCheck/UnstatedIuse/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/InvalidRestrict/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/InvalidRestrict/InvalidRestrict-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/UnknownRestrict/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/UnknownRestrict/UnknownRestrict-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RestrictCheck/UnstatedIuse/UnstatedIuse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/RestrictTestCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/RestrictTestCheck/MissingTestRestrict/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/RestrictTestCheck/MissingTestRestrict/MissingTestRestrict-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidEapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidEapi/InvalidEapi-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidEapi/InvalidEapi-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-2.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-3.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-4.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/InvalidSlot/InvalidSlot-5.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/SourcingError/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SourcingCheck/SourcingError/SourcingError-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadFilename/
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadFilename/BadFilename-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadFilename/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadProtocol/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadProtocol/BadProtocol-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadProtocol/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/InvalidSrcUri-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/InvalidSrcUri-1.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/InvalidSrcUri/InvalidSrcUri-2.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.170364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/MissingUri/
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/MissingUri/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/MissingUri/MissingUri-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/RedundantUriRename-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/RedundantUriRename-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/TarballAvailable/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/TarballAvailable/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/TarballAvailable/TarballAvailable-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/UnknownMirror/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/UnknownMirror/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/UnknownMirror/UnknownMirror-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/UnstatedIuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/UnstatedIuse/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/UnstatedIuse/UnstatedIuse-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/VariableScopeCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/VariableScopeCheck/EbuildVariableScope/
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/VariableScopeCheck/EbuildVariableScope/EbuildVariableScope-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/VisibilityCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/VisibilityCheck/NonexistentDeps/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/VisibilityCheck/NonexistentDeps/NonexistentDeps-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/VisibilityCheck/VisibleVcsPkg/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/VisibilityCheck/VisibleVcsPkg/VisibleVcsPkg-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/VisibilityCheck/VisibleVcsPkg/VisibleVcsPkg-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/BadWhitespaceCharacter-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/DoubleEmptyLine/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/DoubleEmptyLine/DoubleEmptyLine-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/NoFinalNewline/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/NoFinalNewline/NoFinalNewline-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/TrailingEmptyLine/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/WhitespaceCheck/TrailingEmptyLine/TrailingEmptyLine-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/app-arch/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/app-arch/unzip/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/app-arch/unzip/unzip-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/eclass/
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/eclass/stub.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/eclass/unused.eclass
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/eclass/vcs.eclass
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/licenses/BSD -> ../../../../LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/licenses/eula
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/licenses/unused
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/metadata/layout.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/metadata/projects.xml
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/metadata/stubs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/arch.list
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.094365 pkgcheck-0.9.7/testdata/repos/standalone/profiles/default/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/profiles/default/amd64/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/default/amd64/make.defaults
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/profiles/default/x86/
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/default/x86/make.defaults
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/profiles/desc/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/desc/use_expand.desc
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/license_groups
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/profiles.desc
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/repo_name
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/thirdpartymirrors
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/use.desc
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/profiles/use.local.desc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/standalone/stub/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global1/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global1/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global1/potential-global1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global2/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global2/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global2/potential-global2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global3/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global3/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global3/potential-global3-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global4/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global4/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-27 17:20:47.520464 pkgcheck-0.9.7/testdata/repos/standalone/stub/potential-global4/potential-global4-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/slotted/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/stub/slotted/slotted-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/stub/slotted/slotted-1.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub1/
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub1/stub1-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub2/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub2/stub2-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub3/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub3/stub3-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub4/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/stub/stub4/stub4-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/standalone/test/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/test/ConflictingChksums/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/test/ConflictingChksums/ConflictingChksums-0.ebuild
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/test/ConflictingChksums/Manifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/test/MatchingChksums/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/test/MatchingChksums/Manifest
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/test/MatchingChksums/MatchingChksums-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/standalone/virtual/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.174364 pkgcheck-0.9.7/testdata/repos/standalone/virtual/UnnecessaryLicense/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/standalone/virtual/UnnecessaryLicense/UnnecessaryLicense-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/DeprecatedDep/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/DeprecatedDep/nonoptional/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/DeprecatedDep/nonoptional/nonoptional-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/DeprecatedDep/optional/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/DeprecatedDep/optional/optional-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInDev/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInDev/masked/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInDev/masked/masked-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInExp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInExp/masked/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInExp/masked/masked-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInStable/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInStable/masked/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInStable/masked/masked-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInStable/unstable/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/NonsolvableDepsInStable/unstable/unstable-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/licenses/
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/licenses/BSD -> ../../../../LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/metadata/layout.conf
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/metadata/pkgcheck-args
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/profiles/arch/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/arch/amd64/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/arch/amd64/make.defaults
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/arch/x86/
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/arch/x86/make.defaults
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/arch.list
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/package.deprecated
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/profiles.desc
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/repo_name
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/dev/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/dev/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/exp/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/exp/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/exp/parent
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/stable/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/stable/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/amd64/stable/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/dev/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/dev/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/exp/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/exp/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/exp/parent
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/stable/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/stable/package.mask
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/profiles/visibility/x86/stable/parent
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.098365 pkgcheck-0.9.7/testdata/repos/visibility/stub/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/stub/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/stub/deprecated/deprecated-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/stub/masked/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/stub/masked/masked-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/stub/stable/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/stub/stable/stable-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.178364 pkgcheck-0.9.7/testdata/repos/visibility/stub/unstable/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/testdata/repos/visibility/stub/unstable/unstable-0.ebuild
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tests/addons/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16621 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/addons/test_addons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6453 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/addons/test_eclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29875 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/addons/test_git.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tests/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3857 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_acct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4750 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11889 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_codingstyle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2930 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_dropped_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25906 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3136 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_glsa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4313 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5615 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_imlate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56056 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5217 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2972 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_perl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19451 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_pkgdir.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22321 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5501 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_repo_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7290 2021-03-27 17:20:47.524464 pkgcheck-0.9.7/tests/checks/test_stablereq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5300 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/checks/test_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7870 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16152 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_argparse_actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_pkgcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4147 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_pkgcheck_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_pkgcheck_ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3417 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_pkgcheck_replay.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27976 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_pkgcheck_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/scripts/test_pkgcheck_show.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3283 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5612 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6684 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tests/test_reporters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tree-sitter-bash/
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tree-sitter-bash/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tree-sitter-bash/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tree-sitter-bash/src/binding.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    58690 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tree-sitter-bash/src/grammar.json
+-rw-r--r--   0 runner    (1001) docker     (121)    28024 2021-03-27 17:20:47.528463 pkgcheck-0.9.7/tree-sitter-bash/src/node-types.json
+-rw-r--r--   0 runner    (1001) docker     (121)  3523435 2021-03-27 17:20:47.540463 pkgcheck-0.9.7/tree-sitter-bash/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (121)    10414 2021-03-27 17:20:47.540463 pkgcheck-0.9.7/tree-sitter-bash/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 17:23:49.182364 pkgcheck-0.9.7/tree-sitter-bash/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (121)     5326 2021-03-27 17:20:47.540463 pkgcheck-0.9.7/tree-sitter-bash/src/tree_sitter/parser.h
```

### Comparing `pkgcheck-0.9.6/LICENSE` & `pkgcheck-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/NEWS.rst` & `pkgcheck-0.9.7/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 =============
 Release Notes
 =============
 
 ---------------------------
+pkgcheck 0.9.7 (2021-03-27)
+---------------------------
+
+- pkgcheck scan: Fix raw repo creation for overlays.
+
+---------------------------
 pkgcheck 0.9.6 (2021-03-26)
 ---------------------------
 
 - Add support for identifying misplaced eclass spec variables (#309).
 
 ---------------------------
 pkgcheck 0.9.5 (2021-03-20)
```

### Comparing `pkgcheck-0.9.6/PKG-INFO` & `pkgcheck-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgcheck
-Version: 0.9.6
+Version: 0.9.7
 Summary: pkgcore-based QA utility for ebuild repos
 Home-page: https://github.com/pkgcore/pkgcheck
 Author: Tim Harder
 Author-email: radhermit@gmail.com
 License: BSD
 Description: |pypi| |test| |coverage|
```

### Comparing `pkgcheck-0.9.6/README.rst` & `pkgcheck-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/completion/zsh/_pkgcheck` & `pkgcheck-0.9.7/completion/zsh/_pkgcheck`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/data/pkgcheck.conf` & `pkgcheck-0.9.7/data/pkgcheck.conf`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/doc/conf.py` & `pkgcheck-0.9.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/doc/generate/pkgcheck/checks.py` & `pkgcheck-0.9.7/doc/generate/pkgcheck/checks.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/doc/generate/pkgcheck/keywords.py` & `pkgcheck-0.9.7/doc/generate/pkgcheck/keywords.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/doc/generate/pkgcheck/reporters.py` & `pkgcheck-0.9.7/doc/generate/pkgcheck/reporters.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/doc/man/config.rst` & `pkgcheck-0.9.7/doc/man/config.rst`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/man/pkgcheck.1` & `pkgcheck-0.9.7/man/pkgcheck.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PKGCHECK" "1" "Mar 26, 2021" "0.9.6" "pkgcheck"
+.TH "PKGCHECK" "1" "Mar 27, 2021" "0.9.7" "pkgcheck"
 .SH NAME
 pkgcheck \- pkgcore-based QA utility for ebuild repos
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcheck-0.9.6/setup.py` & `pkgcheck-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/__init__.py` & `pkgcheck-0.9.7/src/pkgcheck/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .api import keywords, scan
 from .base import PkgcheckException
 from .results import Result
 
 __all__ = ('keywords', 'scan', 'PkgcheckException', 'Result')
 __title__ = 'pkgcheck'
-__version__ = '0.9.6'
+__version__ = '0.9.7'
 
 
 def __getattr__(name):
     """Provide import access to keyword classes."""
     if name in keywords:
         return keywords[name]
```

### Comparing `pkgcheck-0.9.6/src/pkgcheck/addons/__init__.py` & `pkgcheck-0.9.7/src/pkgcheck/addons/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/addons/caches.py` & `pkgcheck-0.9.7/src/pkgcheck/addons/caches.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/addons/eclass.py` & `pkgcheck-0.9.7/src/pkgcheck/addons/eclass.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/addons/git.py` & `pkgcheck-0.9.7/src/pkgcheck/addons/git.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/addons/net.py` & `pkgcheck-0.9.7/src/pkgcheck/addons/net.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/addons/profiles.py` & `pkgcheck-0.9.7/src/pkgcheck/addons/profiles.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/api.py` & `pkgcheck-0.9.7/src/pkgcheck/api.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/base.py` & `pkgcheck-0.9.7/src/pkgcheck/base.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/bash/__init__.py` & `pkgcheck-0.9.7/src/pkgcheck/bash/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/__init__.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/acct.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/acct.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/cleanup.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/cleanup.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/codingstyle.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/codingstyle.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/dropped_keywords.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/dropped_keywords.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/eclass.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/eclass.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/git.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/git.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/glsa.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/glsa.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/header.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/header.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/imlate.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/imlate.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/metadata.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/metadata_xml.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/metadata_xml.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/network.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/network.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/overlays.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/overlays.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/perl.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/perl.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/pkgdir.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/pkgdir.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/profiles.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/profiles.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/python.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/python.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/repo.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/repo.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/repo_metadata.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/repo_metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/stablereq.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/stablereq.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/unstable_only.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/unstable_only.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/visibility.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/visibility.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/checks/whitespace.py` & `pkgcheck-0.9.7/src/pkgcheck/checks/whitespace.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/cli.py` & `pkgcheck-0.9.7/src/pkgcheck/cli.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/const.py` & `pkgcheck-0.9.7/src/pkgcheck/const.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/feeds.py` & `pkgcheck-0.9.7/src/pkgcheck/feeds.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/objects.py` & `pkgcheck-0.9.7/src/pkgcheck/objects.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/packages.py` & `pkgcheck-0.9.7/src/pkgcheck/packages.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/pipeline.py` & `pkgcheck-0.9.7/src/pkgcheck/pipeline.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/reporters.py` & `pkgcheck-0.9.7/src/pkgcheck/reporters.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/results.py` & `pkgcheck-0.9.7/src/pkgcheck/results.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/runners.py` & `pkgcheck-0.9.7/src/pkgcheck/runners.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/__init__.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/argparse_actions.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/argparse_actions.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/argparsers.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/argparsers.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_cache.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_cache.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_ci.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_ci.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_replay.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_replay.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_scan.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_scan.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/scripts/pkgcheck_show.py` & `pkgcheck-0.9.7/src/pkgcheck/scripts/pkgcheck_show.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/src/pkgcheck/sources.py` & `pkgcheck-0.9.7/src/pkgcheck/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from collections import defaultdict, deque
 from collections.abc import Set
 from dataclasses import dataclass
 from operator import attrgetter
 
 from pkgcore.ebuild.profiles import ProfileError
-from pkgcore.ebuild.repository import UnconfiguredTree
+from pkgcore.ebuild.repository import UnconfiguredTree, tree
 from pkgcore.restrictions import packages
 from snakeoil import klass
 from snakeoil.osutils import listdir_files, pjoin
 
 from . import addons, base
 from .bash import ParseTree
 from .addons.eclass import Eclass, EclassAddon
@@ -213,17 +213,14 @@
                 if root[self._prefix_len:] not in self.non_profile_dirs:
                     yield Profile(ProfileNode(root), set(files))
 
 
 class _RawRepo(UnconfiguredTree):
     """Repository that allows matching against mismatched/invalid package names."""
 
-    def __init__(self, repo):
-        super().__init__(repo.location)
-
     def _get_versions(self, catpkg):
         """Pass through all packages that end with ".ebuild" extension.
 
         Deviates from parent in that no package name check is done.
         """
         cppath = pjoin(self.base, catpkg[0], catpkg[1])
         pkg = f'{catpkg[-1]}-'
@@ -239,15 +236,15 @@
             raise KeyError(f'failed fetching versions for package {path}: {e}') from e
 
 
 class RawRepoSource(RepoSource):
     """Ebuild repository source returning raw CPV objects."""
 
     def __init__(self, options):
-        source = _RawRepo(options.target_repo)
+        source = tree(options.config, options.target_repo.config, tree_cls=_RawRepo)
         super().__init__(options, source)
 
     def itermatch(self, restrict, **kwargs):
         yield from super().itermatch(restrict, raw_pkg_cls=RawCPV, **kwargs)
 
 
 class RestrictionRepoSource(RepoSource):
```

### Comparing `pkgcheck-0.9.6/src/pkgcheck/utils.py` & `pkgcheck-0.9.7/src/pkgcheck/utils.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/eclass/EclassCheck/EclassDocMissingVar/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/DeprecatedEclass/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/eclass/EclassUsageCheck/MisplacedEclassVar/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidCopyright/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildInvalidLicenseHeader/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildNonGentooAuthorsCopyright/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EbuildHeaderCheck/EbuildOldGentooCopyright/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EclassHeaderCheck/EclassInvalidLicenseHeader/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyCategoryDir/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/EmptyDirsCheck/EmptyPackageDir/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerNeeded/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/MaintainerWithoutProxy/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/NonexistentProjectMaintainer/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/PkgMissingMetadataXml/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/ProxyWithoutProxied/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/gentoo/PackageMetadataXmlCheck/WrongMaintainerType/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/ProfileError/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackage/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfilePackageKeywords/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/profiledir/ProfilesCheck/UnknownProfileUse/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/python/PythonCompatCheck/PythonCompatUpdate/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatBadlyFormedXml/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatInvalidXml/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlIndentation/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidCatRef/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/CategoryMetadataXmlCheck/CatMetadataXmlInvalidPkgRef/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/BadDependency/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/BadDependency/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/BadDependency/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/BadDependency/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingPackageRevision/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DependencyCheck/MissingUseDepDefault/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DescriptionCheck/BadDescription/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DescriptionCheck/BadDescription/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DescriptionCheck/BadDescription/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DescriptionCheck/BadDescription/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/DroppedKeywordsCheck/DroppedKeywords/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/EclassUsageCheck/DuplicateEclassInherit/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/EqualVersionsCheck/EqualVersions/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialGlobalUse/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/GlobalUseCheck/PotentialLocalUse/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/HomepageCheck/BadHomepage/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/HomepageCheck/BadHomepage/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/HomepageCheck/BadHomepage/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/HomepageCheck/BadHomepage/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/InsintoCheck/DeprecatedInsinto/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/InvalidUseFlags/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/IuseCheck/UnknownUseFlags/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/InvalidLicense/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/LicenseCheck/MissingLicenseRestricts/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/MissingLocalUseDesc/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/ProbableUseExpand/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/LocalUseCheck/UnderscoreInUseFlag/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/DeprecatedChksum/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/InvalidManifest/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingChksum/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingChksum/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/MissingManifest/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/MissingManifest/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnknownManifest/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCheck/UnnecessaryManifest/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/ConflictingChksums/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ManifestCollisionCheck/MatchingChksums/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/HomepageInSrcUri/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/MultipleKeywordsLines/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/ReferenceInMetadataVar/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/MetadataVarCheck/StaticSrcUri/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/MissingSlotDepCheck/MissingSlotDep/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/MissingUnpackerDepCheck/MissingUnpackerDep/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgBadlyFormedXml/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgInvalidXml/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlEmptyElement/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlIndentation/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidCatRef/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/PkgMetadataXmlInvalidPkgRef/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PackageMetadataXmlCheck/RedundantLongDescription/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/InvalidPN/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/PkgDirCheck/MismatchedPN/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ProjectMetadataCheck/EmptyProject/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/ReadonlyVariableCheck/ReadonlyVariable/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/RedundantDodirCheck/RedundantDodir/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/InvalidRequiredUse/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/RequiredUseCheck/RequiredUseDefaults/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidEapi/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SourcingCheck/InvalidSlot/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadFilename/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadFilename/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/BadProtocol/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/InvalidSrcUri/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/RedundantUriRename/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/TarballAvailable/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/SrcUriCheck/UnknownMirror/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/VariableScopeCheck/EbuildVariableScope/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/NonexistentDeps/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/expected-verbose.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/expected-verbose.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/VisibilityCheck/VisibleVcsPkg/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/standalone/WhitespaceCheck/BadWhitespaceCharacter/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/visibility/DependencyCheck/DeprecatedDep/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected-verbose.json` & `pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected-verbose.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected.json` & `pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/expected.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/fix.patch` & `pkgcheck-0.9.7/testdata/data/repos/visibility/VisibilityCheck/NonsolvableDepsInStable/fix.patch`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/pkgcheck` & `pkgcheck-0.9.7/testdata/pkgcheck`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/python/eclass/python-any-r1.eclass` & `pkgcheck-0.9.7/testdata/repos/python/eclass/python-any-r1.eclass`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/python/eclass/python-r1.eclass` & `pkgcheck-0.9.7/testdata/repos/python/eclass/python-r1.eclass`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/python/eclass/python-single-r1.eclass` & `pkgcheck-0.9.7/testdata/repos/python/eclass/python-single-r1.eclass`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnknownManifest/Manifest` & `pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnknownManifest/Manifest`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/Manifest` & `pkgcheck-0.9.7/testdata/repos/standalone/ManifestCheck/UnnecessaryManifest/Manifest`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/BadFilename/Manifest` & `pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/BadFilename/Manifest`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/Manifest` & `pkgcheck-0.9.7/testdata/repos/standalone/SrcUriCheck/RedundantUriRename/Manifest`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/addons/test_addons.py` & `pkgcheck-0.9.7/tests/addons/test_addons.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/addons/test_eclass.py` & `pkgcheck-0.9.7/tests/addons/test_eclass.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/addons/test_git.py` & `pkgcheck-0.9.7/tests/addons/test_git.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_acct.py` & `pkgcheck-0.9.7/tests/checks/test_acct.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_all.py` & `pkgcheck-0.9.7/tests/checks/test_all.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_cleanup.py` & `pkgcheck-0.9.7/tests/checks/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_codingstyle.py` & `pkgcheck-0.9.7/tests/checks/test_codingstyle.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_dropped_keywords.py` & `pkgcheck-0.9.7/tests/checks/test_dropped_keywords.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_git.py` & `pkgcheck-0.9.7/tests/checks/test_git.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_glsa.py` & `pkgcheck-0.9.7/tests/checks/test_glsa.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_header.py` & `pkgcheck-0.9.7/tests/checks/test_header.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_imlate.py` & `pkgcheck-0.9.7/tests/checks/test_imlate.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_metadata.py` & `pkgcheck-0.9.7/tests/checks/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_network.py` & `pkgcheck-0.9.7/tests/checks/test_network.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_perl.py` & `pkgcheck-0.9.7/tests/checks/test_perl.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_pkgdir.py` & `pkgcheck-0.9.7/tests/checks/test_pkgdir.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_python.py` & `pkgcheck-0.9.7/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_repo.py` & `pkgcheck-0.9.7/tests/checks/test_repo.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_repo_metadata.py` & `pkgcheck-0.9.7/tests/checks/test_repo_metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_stablereq.py` & `pkgcheck-0.9.7/tests/checks/test_stablereq.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/checks/test_whitespace.py` & `pkgcheck-0.9.7/tests/checks/test_whitespace.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/conftest.py` & `pkgcheck-0.9.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/misc.py` & `pkgcheck-0.9.7/tests/misc.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_argparse_actions.py` & `pkgcheck-0.9.7/tests/scripts/test_argparse_actions.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_pkgcheck.py` & `pkgcheck-0.9.7/tests/scripts/test_pkgcheck.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_pkgcheck_cache.py` & `pkgcheck-0.9.7/tests/scripts/test_pkgcheck_cache.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_pkgcheck_ci.py` & `pkgcheck-0.9.7/tests/scripts/test_pkgcheck_ci.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_pkgcheck_replay.py` & `pkgcheck-0.9.7/tests/scripts/test_pkgcheck_replay.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_pkgcheck_scan.py` & `pkgcheck-0.9.7/tests/scripts/test_pkgcheck_scan.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/scripts/test_pkgcheck_show.py` & `pkgcheck-0.9.7/tests/scripts/test_pkgcheck_show.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/test_api.py` & `pkgcheck-0.9.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/test_base.py` & `pkgcheck-0.9.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/test_cli.py` & `pkgcheck-0.9.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/test_feeds.py` & `pkgcheck-0.9.7/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tests/test_reporters.py` & `pkgcheck-0.9.7/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/LICENSE` & `pkgcheck-0.9.7/tree-sitter-bash/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/src/binding.cc` & `pkgcheck-0.9.7/tree-sitter-bash/src/binding.cc`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/src/grammar.json` & `pkgcheck-0.9.7/tree-sitter-bash/src/grammar.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/src/node-types.json` & `pkgcheck-0.9.7/tree-sitter-bash/src/node-types.json`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/src/parser.c` & `pkgcheck-0.9.7/tree-sitter-bash/src/parser.c`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/src/scanner.cc` & `pkgcheck-0.9.7/tree-sitter-bash/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `pkgcheck-0.9.6/tree-sitter-bash/src/tree_sitter/parser.h` & `pkgcheck-0.9.7/tree-sitter-bash/src/tree_sitter/parser.h`

 * *Files identical despite different names*

