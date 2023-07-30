# Comparing `tmp/bdbag-1.6.4.tar.gz` & `tmp/bdbag-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdbag-1.6.4.tar", last modified: Fri Feb  3 00:23:05 2023, max compression
+gzip compressed data, was "bdbag-1.7.0.tar", last modified: Sun Jul 30 00:27:25 2023, max compression
```

## Comparing `bdbag-1.6.4.tar` & `bdbag-1.7.0.tar`

### file list

```diff
@@ -1,465 +1,467 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/
--rw-rw-rw-   0        0        0       18 2022-01-11 18:46:35.000000 bdbag-1.6.4/.gitattributes
--rw-rw-rw-   0        0        0      750 2022-05-27 21:57:05.000000 bdbag-1.6.4/.travis.yml
--rw-rw-rw-   0        0        0    18642 2023-02-02 23:43:21.000000 bdbag-1.6.4/CHANGELOG.md
--rw-rw-rw-   0        0        0    11357 2022-01-11 18:46:35.000000 bdbag-1.6.4/LICENSE
--rw-rw-rw-   0        0        0     8004 2023-02-03 00:23:05.411498 bdbag-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      197 2022-05-27 21:56:55.000000 bdbag-1.6.4/Pipfile
--rw-rw-rw-   0        0        0    35937 2023-02-02 23:55:50.000000 bdbag-1.6.4/Pipfile.lock
--rw-rw-rw-   0        0        0     5625 2022-02-11 20:26:50.000000 bdbag-1.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.771063 bdbag-1.6.4/bdbag/
--rw-rw-rw-   0        0        0    10050 2023-02-02 23:43:21.000000 bdbag-1.6.4/bdbag/__init__.py
--rw-rw-rw-   0        0        0    26315 2022-05-27 21:57:05.000000 bdbag-1.6.4/bdbag/bdbag_api.py
--rw-rw-rw-   0        0        0    19476 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/bdbag_cli.py
--rw-rw-rw-   0        0        0     9540 2022-12-01 20:46:50.000000 bdbag-1.6.4/bdbag/bdbag_config.py
--rw-rw-rw-   0        0        0    13883 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/bdbag_ro.py
--rw-rw-rw-   0        0        0    27410 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/bdbag_utils.py
--rw-rw-rw-   0        0        0    24599 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/bdbagit.py
--rw-rw-rw-   0        0        0     2357 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/bdbagit_profile.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.786715 bdbag-1.6.4/bdbag/fetch/
--rw-rw-rw-   0        0        0     2233 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/fetch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.802370 bdbag-1.6.4/bdbag/fetch/auth/
--rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/auth/__init__.py
--rw-rw-rw-   0        0        0     3282 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/fetch/auth/cookies.py
--rw-rw-rw-   0        0        0     6159 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/fetch/auth/keychain.py
--rw-rw-rw-   0        0        0     4980 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/fetcher.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.802370 bdbag-1.6.4/bdbag/fetch/resolvers/
--rw-rw-rw-   0        0        0     2486 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/resolvers/__init__.py
--rw-rw-rw-   0        0        0     2802 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/resolvers/ark_resolver.py
--rw-rw-rw-   0        0        0     3142 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/resolvers/base_resolver.py
--rw-rw-rw-   0        0        0     2271 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/resolvers/dataguid_resolver.py
--rw-rw-rw-   0        0        0     2600 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/resolvers/doi_resolver.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.818015 bdbag-1.6.4/bdbag/fetch/transports/
--rw-rw-rw-   0        0        0     2701 2022-12-01 20:46:50.000000 bdbag-1.6.4/bdbag/fetch/transports/__init__.py
--rw-rw-rw-   0        0        0     1057 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/transports/base_transport.py
--rw-rw-rw-   0        0        0     7061 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/fetch/transports/fetch_boto3.py
--rw-rw-rw-   0        0        0     3348 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/transports/fetch_ftp.py
--rw-rw-rw-   0        0        0     5071 2023-02-02 23:43:21.000000 bdbag-1.6.4/bdbag/fetch/transports/fetch_gcs.py
--rw-rw-rw-   0        0        0     5133 2022-02-11 20:26:50.000000 bdbag-1.6.4/bdbag/fetch/transports/fetch_globus.py
--rw-rw-rw-   0        0        0    12347 2022-05-27 21:57:06.000000 bdbag-1.6.4/bdbag/fetch/transports/fetch_http.py
--rw-rw-rw-   0        0        0     1389 2022-01-11 18:46:35.000000 bdbag-1.6.4/bdbag/fetch/transports/fetch_tag.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.786715 bdbag-1.6.4/bdbag.egg-info/
--rw-rw-rw-   0        0        0     8004 2023-02-03 00:23:03.000000 bdbag-1.6.4/bdbag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19220 2023-02-03 00:23:04.000000 bdbag-1.6.4/bdbag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 00:23:03.000000 bdbag-1.6.4/bdbag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-02-03 00:23:03.000000 bdbag-1.6.4/bdbag.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      241 2023-02-03 00:23:03.000000 bdbag-1.6.4/bdbag.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-03 00:23:03.000000 bdbag-1.6.4/bdbag.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.849283 bdbag-1.6.4/doc/
--rw-rw-rw-   0        0        0    38271 2023-02-02 23:43:21.000000 bdbag-1.6.4/doc/api.md
--rw-rw-rw-   0        0        0    38875 2023-02-02 23:43:21.000000 bdbag-1.6.4/doc/cli.md
--rw-rw-rw-   0        0        0    30574 2023-02-02 23:43:21.000000 bdbag-1.6.4/doc/config.md
--rw-rw-rw-   0        0        0    10987 2022-01-11 18:46:35.000000 bdbag-1.6.4/doc/utils.md
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.395954 bdbag-1.6.4/examples/
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.849283 bdbag-1.6.4/examples/bagofbags/
--rw-rw-rw-   0        0        0     1519 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/bagofbags/README.md
--rw-rw-rw-   0        0        0     7342 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/bagofbags/bagofbags.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.849283 bdbag-1.6.4/examples/bagofbags/images/
--rw-rw-rw-   0        0        0   127142 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/bagofbags/images/MetaBags.png
--rw-rw-rw-   0        0        0    48632 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/bagofbags/images/MetaBags.pptx
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.849283 bdbag-1.6.4/examples/metamanifests/
--rw-rw-rw-   0        0        0      840 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/metamanifests/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.395954 bdbag-1.6.4/examples/metamanifests/samples/
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.864714 bdbag-1.6.4/examples/metamanifests/samples/sample1/
--rw-rw-rw-   0        0        0      236 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/metamanifests/samples/sample1/metadata.json
--rw-rw-rw-   0        0        0      741 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/metamanifests/samples/sample1/remote-files.json
--rw-rw-rw-   0        0        0     4729 2022-01-11 18:46:35.000000 bdbag-1.6.4/examples/metamanifests/samples/sample1/ro_metadata.json
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.864714 bdbag-1.6.4/profiles/
--rw-rw-rw-   0        0        0      940 2022-01-11 18:46:35.000000 bdbag-1.6.4/profiles/bdbag-profile.json
--rw-rw-rw-   0        0        0     1091 2022-01-11 18:46:35.000000 bdbag-1.6.4/profiles/bdbag-ro-profile.json
--rw-rw-rw-   0        0        0      102 2021-01-28 23:53:34.000000 bdbag-1.6.4/pyproject.toml
--rw-rw-rw-   0        0        0      226 2023-02-03 00:23:05.411498 bdbag-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0     3137 2022-12-01 20:46:50.000000 bdbag-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.864714 bdbag-1.6.4/test/
--rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.708447 bdbag-1.6.4/test/test-data/
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.895608 bdbag-1.6.4/test/test-data/test-archives/
--rw-rw-rw-   0        0        0     2355 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag-fetch-http.zip
--rw-rw-rw-   0        0        0     2460 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag-multi-parent.tgz
--rw-rw-rw-   0        0        0     5253 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag-multi-parent.zip
--rw-rw-rw-   0        0        0     2369 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag-no-parent.tgz
--rw-rw-rw-   0        0        0     4596 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag-no-parent.zip
--rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag.7z
--rw-rw-rw-   0        0        0     2319 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag.bz2
--rw-rw-rw-   0        0        0    20480 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag.tar
--rw-rw-rw-   0        0        0     2370 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag.tgz
--rw-rw-rw-   0        0        0     5257 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-archives/test-bag.zip
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.911253 bdbag-1.6.4/test/test-data/test-bag/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.333143 bdbag-1.6.4/test/test-data/test-bag/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.348783 bdbag-1.6.4/test/test-data/test-bag/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.348783 bdbag-1.6.4/test/test-data/test-bag/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/data/test2/test2.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.927100 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/
--rw-rw-rw-   0        0        0      351 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/bagit.txt
--rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/fetch.txt
--rw-rw-rw-   0        0        0      124 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/manifest-md5.txt
--rw-rw-rw-   0        0        0      140 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/manifest-sha1.txt
--rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/manifest-sha256.txt
--rw-rw-rw-   0        0        0      316 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/manifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.927100 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/metadata/
--rw-rw-rw-   0        0        0     1207 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/metadata/manifest.json
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      459 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      651 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1163 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.942728 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.974012 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/data/README.txt
--rw-rw-rw-   0        0        0       53 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.942728 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.942728 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/data/README.txt
--rw-rw-rw-   0        0        0       44 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark-bad/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.942728 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.974012 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/data/README.txt
--rw-rw-rw-   0        0        0       62 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ark2/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.989400 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:04.989400 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/data/README.txt
--rw-rw-rw-   0        0        0       90 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-dataguid/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.005042 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.005042 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/data/README.txt
--rw-rw-rw-   0        0        0       59 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-doi/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.021015 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/
--rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.036664 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/data/
--rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/data/1KB.zip
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/data/README.txt
--rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/fetch.txt
--rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/manifest-md5.txt
--rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.036664 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/
--rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.036664 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/data/
--rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/data/1KB.zip
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/data/README.txt
--rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/fetch.txt
--rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/manifest-md5.txt
--rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.052128 bdbag-1.6.4/test/test-data/test-bag-fetch-http/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.130479 bdbag-1.6.4/test/test-data/test-bag-fetch-http/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/data/README.txt
--rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.067780 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.067780 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/data/README.txt
--rw-rw-rw-   0        0        0      409 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/fetch.txt
--rw-rw-rw-   0        0        0      232 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/manifest-md5.txt
--rw-rw-rw-   0        0        0      360 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-bad/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.099177 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.099177 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/data/README.txt
--rw-rw-rw-   0        0        0      153 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/fetch.txt
--rw-rw-rw-   0        0        0      111 2022-01-11 18:46:35.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/manifest-md5.txt
--rw-rw-rw-   0        0        0      175 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.114799 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.114799 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/data/README.txt
--rw-rw-rw-   0        0        0      269 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.130479 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.130479 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/data/README.txt
--rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.145807 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.145807 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/data/README.txt
--rw-rw-rw-   0        0        0       48 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/fetch.txt
--rw-rw-rw-   0        0        0      115 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-minid/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.161448 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.161448 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/data/README.txt
--rw-rw-rw-   0        0        0      113 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/fetch.txt
--rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/manifest-md5.txt
--rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-fetch-tag/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.176939 bdbag-1.6.4/test/test-data/test-bag-incomplete/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.192608 bdbag-1.6.4/test/test-data/test-bag-incomplete/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.192608 bdbag-1.6.4/test/test-data/test-bag-incomplete/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.192608 bdbag-1.6.4/test/test-data/test-bag-incomplete/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/data/test2/test2.txt
--rw-rw-rw-   0        0        0      188 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/fetch.txt
--rw-rw-rw-   0        0        0      219 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/manifest-sha1.txt
--rw-rw-rw-   0        0        0      444 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/manifest-sha512.txt
--rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.192608 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.192608 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/data/README.txt
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      282 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/fetch.txt
--rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-incomplete-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.208183 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.208183 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/README.txt
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      284 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.223808 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.223808 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/data/README.txt
--rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-identifier.txt
--rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.223808 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/
--rw-rw-rw-   0        0        0      320 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.223808 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/data/README.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      192 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-state-manifest-fetch/tagmanifest-md5.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.255462 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.255462 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.265091 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.265091 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/data/test2/test2.txt
--rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/fetch.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/manifest-sha512.txt
--rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.270956 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.286597 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.286597 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.286597 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/data/test2/test2.txt
--rw-rw-rw-   0        0        0      105 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/manifest-md5.txt
--rw-rw-rw-   0        0        0      121 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha1.txt
--rw-rw-rw-   0        0        0      169 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha256.txt
--rw-rw-rw-   0        0        0      297 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.302223 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.302223 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.302223 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/data/test1/test1.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.320622 bdbag-1.6.4/test/test-data/test-bag-no-data/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/bagit.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-no-data/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.320622 bdbag-1.6.4/test/test-data/test-bag-profile/
--rw-rw-rw-   0        0        0      294 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.333143 bdbag-1.6.4/test/test-data/test-bag-profile/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.333143 bdbag-1.6.4/test/test-data/test-bag-profile/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.333143 bdbag-1.6.4/test/test-data/test-bag-profile/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/data/test2/test2.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-profile/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.333143 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.333143 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/data/README.txt
--rw-rw-rw-   0        0        0      135 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/fetch.txt
--rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bag-update-invalid-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.348783 bdbag-1.6.4/test/test-data/test-bdbagit/
--rw-rw-rw-   0        0        0      221 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bdbagit/README
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.348783 bdbag-1.6.4/test/test-data/test-bdbagit/loc/
--rw-rw-rw-   0        0        0   139367 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg
--rw-rw-rw-   0        0        0   143435 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.364362 bdbag-1.6.4/test/test-data/test-bdbagit/si/
--rw-rw-rw-   0        0        0   381813 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg
--rw-rw-rw-   0        0        0   326929 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/test/test-data/test-config/
--rw-rw-rw-   0        0        0      415 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/base-config.json
--rw-rw-rw-   0        0        0      806 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-10.json
--rw-rw-rw-   0        0        0      513 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-11.json
--rw-rw-rw-   0        0        0      576 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-12.json
--rw-rw-rw-   0        0        0      401 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-2.json
--rw-rw-rw-   0        0        0     2773 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-3.json
--rw-rw-rw-   0        0        0     1243 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-4.json
--rw-rw-rw-   0        0        0     1199 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-5.json
--rw-rw-rw-   0        0        0     1052 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-6.json
--rw-rw-rw-   0        0        0      825 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-7.json
--rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-8.json
--rw-rw-rw-   0        0        0      828 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config-9.json
--rw-rw-rw-   0        0        0      354 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-config.json
--rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-cookies-1.txt
--rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-cookies-2.txt
--rw-rw-rw-   0        0        0       83 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-cookies-bad.txt
--rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest-2.json
--rw-rw-rw-   0        0        0     1574 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest-encoding.json
--rw-rw-rw-   0        0        0      616 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json
--rw-rw-rw-   0        0        0      944 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest.json
--rw-rw-rw-   0        0        0      312 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-invalid-fetch-manifest-1.json
--rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-invalid-fetch-manifest-2.json
--rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-1.json
--rw-rw-rw-   0        0        0      233 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-2.json
--rw-rw-rw-   0        0        0      288 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-3.json
--rw-rw-rw-   0        0        0      212 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-4.json
--rw-rw-rw-   0        0        0      191 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-5.json
--rw-rw-rw-   0        0        0      278 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-6.json
--rw-rw-rw-   0        0        0      279 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-7.json
--rw-rw-rw-   0        0        0      704 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-8.json
--rw-rw-rw-   0        0        0      672 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-9.json
--rw-rw-rw-   0        0        0      146 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-keychain-bad-1.json
--rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-metadata.json
--rw-rw-rw-   0        0        0     1259 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-config/test-ro-metadata.json
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/test/test-data/test-dir/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-dir/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/test/test-data/test-dir/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-dir/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/test/test-data/test-dir/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-dir/test2/test2.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/test/test-data/test-http/
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-http/test-fetch-http.txt
--rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-http/test-fetch-identifier.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 00:23:05.411498 bdbag-1.6.4/test/test-data/test-http-encoded/
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test-data/test-http-encoded/test fetch%http®.txt
--rw-rw-rw-   0        0        0    50654 2022-05-27 22:10:39.000000 bdbag-1.6.4/test/test_api.py
--rw-rw-rw-   0        0        0    49471 2022-05-26 22:19:59.000000 bdbag-1.6.4/test/test_bdbagit.py
--rw-rw-rw-   0        0        0    12743 2022-01-11 18:46:36.000000 bdbag-1.6.4/test/test_cli.py
--rw-rw-rw-   0        0        0     8155 2022-05-27 21:57:06.000000 bdbag-1.6.4/test/test_common.py
--rw-rw-rw-   0        0        0    57427 2022-05-27 22:10:39.000000 bdbag-1.6.4/test/test_remote.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/
+-rw-rw-rw-   0        0        0       18 2022-01-11 18:46:35.000000 bdbag-1.7.0/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.138764 bdbag-1.7.0/.github/
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.223412 bdbag-1.7.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1599 2023-07-21 21:19:21.000000 bdbag-1.7.0/.github/workflows/bdbag.yml
+-rw-rw-rw-   0        0        0      750 2022-05-27 21:39:45.000000 bdbag-1.7.0/.travis.yml
+-rw-rw-rw-   0        0        0    19388 2023-07-24 19:38:50.000000 bdbag-1.7.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11357 2022-01-11 18:46:35.000000 bdbag-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     7193 2023-07-30 00:27:25.909708 bdbag-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2022-05-26 23:02:23.000000 bdbag-1.7.0/Pipfile
+-rw-rw-rw-   0        0        0    36425 2023-07-21 21:50:32.000000 bdbag-1.7.0/Pipfile.lock
+-rw-rw-rw-   0        0        0     5771 2023-07-24 19:32:43.000000 bdbag-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.285920 bdbag-1.7.0/bdbag/
+-rw-rw-rw-   0        0        0     9985 2023-07-25 18:36:01.000000 bdbag-1.7.0/bdbag/__init__.py
+-rw-rw-rw-   0        0        0    26658 2023-07-24 18:23:35.000000 bdbag-1.7.0/bdbag/bdbag_api.py
+-rw-rw-rw-   0        0        0    20001 2023-07-25 16:48:58.000000 bdbag-1.7.0/bdbag/bdbag_cli.py
+-rw-rw-rw-   0        0        0     9578 2023-07-20 18:46:39.000000 bdbag-1.7.0/bdbag/bdbag_config.py
+-rw-rw-rw-   0        0        0    13883 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/bdbag_ro.py
+-rw-rw-rw-   0        0        0    27410 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/bdbag_utils.py
+-rw-rw-rw-   0        0        0    24599 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/bdbagit.py
+-rw-rw-rw-   0        0        0     2357 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/bdbagit_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.323696 bdbag-1.7.0/bdbag/fetch/
+-rw-rw-rw-   0        0        0     2233 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.339326 bdbag-1.7.0/bdbag/fetch/auth/
+-rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/auth/__init__.py
+-rw-rw-rw-   0        0        0     3282 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/auth/cookies.py
+-rw-rw-rw-   0        0        0     6159 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/auth/keychain.py
+-rw-rw-rw-   0        0        0     4980 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.354944 bdbag-1.7.0/bdbag/fetch/resolvers/
+-rw-rw-rw-   0        0        0     2486 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/__init__.py
+-rw-rw-rw-   0        0        0     2802 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/ark_resolver.py
+-rw-rw-rw-   0        0        0     3142 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/base_resolver.py
+-rw-rw-rw-   0        0        0     2271 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/dataguid_resolver.py
+-rw-rw-rw-   0        0        0     2600 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/doi_resolver.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.423979 bdbag-1.7.0/bdbag/fetch/transports/
+-rw-rw-rw-   0        0        0     2701 2022-11-15 21:11:09.000000 bdbag-1.7.0/bdbag/fetch/transports/__init__.py
+-rw-rw-rw-   0        0        0     1057 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/transports/base_transport.py
+-rw-rw-rw-   0        0        0     7061 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_boto3.py
+-rw-rw-rw-   0        0        0     3348 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_ftp.py
+-rw-rw-rw-   0        0        0     5193 2023-02-02 22:20:48.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_gcs.py
+-rw-rw-rw-   0        0        0     5133 2022-02-11 20:26:50.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_globus.py
+-rw-rw-rw-   0        0        0    12755 2023-07-19 21:57:14.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_http.py
+-rw-rw-rw-   0        0        0     1389 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_tag.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.308055 bdbag-1.7.0/bdbag.egg-info/
+-rw-rw-rw-   0        0        0     7193 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19233 2023-07-30 00:27:25.000000 bdbag-1.7.0/bdbag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      247 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.470859 bdbag-1.7.0/doc/
+-rw-rw-rw-   0        0        0    38271 2023-02-02 23:26:13.000000 bdbag-1.7.0/doc/api.md
+-rw-rw-rw-   0        0        0    39553 2023-07-25 19:26:55.000000 bdbag-1.7.0/doc/cli.md
+-rw-rw-rw-   0        0        0    30574 2023-02-02 23:26:13.000000 bdbag-1.7.0/doc/config.md
+-rw-rw-rw-   0        0        0    10987 2022-01-11 18:46:35.000000 bdbag-1.7.0/doc/utils.md
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.138764 bdbag-1.7.0/examples/
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.486484 bdbag-1.7.0/examples/bagofbags/
+-rw-rw-rw-   0        0        0     1519 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/README.md
+-rw-rw-rw-   0        0        0     7342 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/bagofbags.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.502105 bdbag-1.7.0/examples/bagofbags/images/
+-rw-rw-rw-   0        0        0   127142 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/images/MetaBags.png
+-rw-rw-rw-   0        0        0    48632 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/images/MetaBags.pptx
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.508616 bdbag-1.7.0/examples/metamanifests/
+-rw-rw-rw-   0        0        0      840 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.138764 bdbag-1.7.0/examples/metamanifests/samples/
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.524260 bdbag-1.7.0/examples/metamanifests/samples/sample1/
+-rw-rw-rw-   0        0        0      236 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/samples/sample1/metadata.json
+-rw-rw-rw-   0        0        0      741 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/samples/sample1/remote-files.json
+-rw-rw-rw-   0        0        0     4729 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/samples/sample1/ro_metadata.json
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.539884 bdbag-1.7.0/profiles/
+-rw-rw-rw-   0        0        0      940 2022-01-11 18:46:35.000000 bdbag-1.7.0/profiles/bdbag-profile.json
+-rw-rw-rw-   0        0        0     1091 2022-01-11 18:46:35.000000 bdbag-1.7.0/profiles/bdbag-ro-profile.json
+-rw-rw-rw-   0        0        0      539 2023-07-30 00:27:25.909708 bdbag-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3216 2023-07-24 19:44:55.000000 bdbag-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.555509 bdbag-1.7.0/test/
+-rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.170015 bdbag-1.7.0/test/test-data/
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.555509 bdbag-1.7.0/test/test-data/test-archives/
+-rw-rw-rw-   0        0        0     2355 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-fetch-http.zip
+-rw-rw-rw-   0        0        0     2460 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.tgz
+-rw-rw-rw-   0        0        0     5253 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.zip
+-rw-rw-rw-   0        0        0     2369 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.tgz
+-rw-rw-rw-   0        0        0     4596 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.zip
+-rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.7z
+-rw-rw-rw-   0        0        0     2319 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.bz2
+-rw-rw-rw-   0        0        0    20480 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.tar
+-rw-rw-rw-   0        0        0     2370 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.tgz
+-rw-rw-rw-   0        0        0     5257 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.zip
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.571127 bdbag-1.7.0/test/test-data/test-bag/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.586753 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/
+-rw-rw-rw-   0        0        0      351 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/bagit.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/fetch.txt
+-rw-rw-rw-   0        0        0      124 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-md5.txt
+-rw-rw-rw-   0        0        0      140 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      316 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.586753 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/metadata/
+-rw-rw-rw-   0        0        0     1207 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/metadata/manifest.json
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      459 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      651 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1163 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.586753 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/data/README.txt
+-rw-rw-rw-   0        0        0       53 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/data/README.txt
+-rw-rw-rw-   0        0        0       44 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/data/README.txt
+-rw-rw-rw-   0        0        0       62 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/data/README.txt
+-rw-rw-rw-   0        0        0       90 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/data/README.txt
+-rw-rw-rw-   0        0        0       59 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.640148 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/
+-rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/data/
+-rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/data/1KB.zip
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/data/README.txt
+-rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/fetch.txt
+-rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/manifest-md5.txt
+-rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/
+-rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/data/
+-rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/data/1KB.zip
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/data/README.txt
+-rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/fetch.txt
+-rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/manifest-md5.txt
+-rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-http/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.702648 bdbag-1.7.0/test/test-data/test-bag-fetch-http/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/data/README.txt
+-rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.671413 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.671413 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/data/README.txt
+-rw-rw-rw-   0        0        0      409 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/fetch.txt
+-rw-rw-rw-   0        0        0      232 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/manifest-md5.txt
+-rw-rw-rw-   0        0        0      360 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.671413 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.687024 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/data/README.txt
+-rw-rw-rw-   0        0        0      153 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/fetch.txt
+-rw-rw-rw-   0        0        0      111 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/manifest-md5.txt
+-rw-rw-rw-   0        0        0      175 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.687024 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.687024 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/data/README.txt
+-rw-rw-rw-   0        0        0      269 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.702648 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.702648 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/data/README.txt
+-rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.709161 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.709161 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/data/README.txt
+-rw-rw-rw-   0        0        0       48 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/fetch.txt
+-rw-rw-rw-   0        0        0      115 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.709161 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.724798 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/data/README.txt
+-rw-rw-rw-   0        0        0      113 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/fetch.txt
+-rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/manifest-md5.txt
+-rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.724798 bdbag-1.7.0/test/test-data/test-bag-incomplete/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/fetch.txt
+-rw-rw-rw-   0        0        0      219 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      444 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      282 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.756049 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.756049 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      284 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.756049 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.771674 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/README.txt
+-rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-identifier.txt
+-rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.771674 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/
+-rw-rw-rw-   0        0        0      320 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.771674 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/data/README.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      192 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/tagmanifest-md5.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      105 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-md5.txt
+-rw-rw-rw-   0        0        0      121 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      169 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      297 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.825072 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/test1/test1.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.825072 bdbag-1.7.0/test/test-data/test-bag-no-data/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/bagit.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/
+-rw-rw-rw-   0        0        0      294 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      135 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bdbagit/
+-rw-rw-rw-   0        0        0      221 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/README
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bdbagit/loc/
+-rw-rw-rw-   0        0        0   139367 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg
+-rw-rw-rw-   0        0        0   143435 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.871947 bdbag-1.7.0/test/test-data/test-bdbagit/si/
+-rw-rw-rw-   0        0        0   381813 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg
+-rw-rw-rw-   0        0        0   326929 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-config/
+-rw-rw-rw-   0        0        0      415 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/base-config.json
+-rw-rw-rw-   0        0        0      806 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-10.json
+-rw-rw-rw-   0        0        0      513 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-11.json
+-rw-rw-rw-   0        0        0      576 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-12.json
+-rw-rw-rw-   0        0        0      401 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-2.json
+-rw-rw-rw-   0        0        0     2773 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-3.json
+-rw-rw-rw-   0        0        0     1243 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-4.json
+-rw-rw-rw-   0        0        0     1199 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-5.json
+-rw-rw-rw-   0        0        0     1052 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-6.json
+-rw-rw-rw-   0        0        0      825 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-7.json
+-rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-8.json
+-rw-rw-rw-   0        0        0      828 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-9.json
+-rw-rw-rw-   0        0        0      354 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config.json
+-rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-cookies-1.txt
+-rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-cookies-2.txt
+-rw-rw-rw-   0        0        0       83 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-cookies-bad.txt
+-rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-2.json
+-rw-rw-rw-   0        0        0     1574 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-encoding.json
+-rw-rw-rw-   0        0        0      616 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json
+-rw-rw-rw-   0        0        0      944 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest.json
+-rw-rw-rw-   0        0        0      312 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-invalid-fetch-manifest-1.json
+-rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-invalid-fetch-manifest-2.json
+-rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-1.json
+-rw-rw-rw-   0        0        0      233 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-2.json
+-rw-rw-rw-   0        0        0      288 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-3.json
+-rw-rw-rw-   0        0        0      212 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-4.json
+-rw-rw-rw-   0        0        0      191 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-5.json
+-rw-rw-rw-   0        0        0      278 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-6.json
+-rw-rw-rw-   0        0        0      279 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-7.json
+-rw-rw-rw-   0        0        0      704 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-8.json
+-rw-rw-rw-   0        0        0      672 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-9.json
+-rw-rw-rw-   0        0        0      146 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-bad-1.json
+-rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-metadata.json
+-rw-rw-rw-   0        0        0     1259 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-ro-metadata.json
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-dir/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-dir/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-dir/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-dir/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-dir/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-dir/test2/test2.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-http/
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-http/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-http/test-fetch-identifier.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-http-encoded/
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-http-encoded/test fetch%http®.txt
+-rw-rw-rw-   0        0        0    51544 2023-07-21 22:52:04.000000 bdbag-1.7.0/test/test_api.py
+-rw-rw-rw-   0        0        0    49471 2022-05-26 22:19:59.000000 bdbag-1.7.0/test/test_bdbagit.py
+-rw-rw-rw-   0        0        0    13183 2023-07-24 18:49:12.000000 bdbag-1.7.0/test/test_cli.py
+-rw-rw-rw-   0        0        0     8155 2022-05-27 21:25:14.000000 bdbag-1.7.0/test/test_common.py
+-rw-rw-rw-   0        0        0    57435 2023-03-29 18:38:57.000000 bdbag-1.7.0/test/test_remote.py
```

### Comparing `bdbag-1.6.4/.travis.yml` & `bdbag-1.7.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/CHANGELOG.md` & `bdbag-1.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGE LOG
 
+## 1.7.0
+* PR: [#54](https://github.com/fair-research/bdbag/pull/54): Add support for passing a local profile path for profile validation. Thanks to [Bernhard Hampel-Waffenthal](https://github.com/prettybits) for the contribution.
+* [#40](https://github.com/fair-research/bdbag/issues/40): Replace deprecated use of `pkg_resources` with `importlib-metadata` and `packaging`.
+* Fix issue with HTTP fetch transport where bearer-token auth gets stripped from the session on a legitimate redirect but not restored for any potential new request on that same URL-bound session.
+* Unpin `tzlocal` unless Python<3.
+* Support for Python 3.5 and 3.6 has been dropped. Python 3.7 compatibility is deprecated but still officially supported in this release.
+
 ## 1.6.4
 
 ### Added Google Cloud Storage fetch handler for handling `gs://` URLs in _fetch.txt_. 
 Note that this is a soft dependency and you must install the [gcloud CLI](https://cloud.google.com/sdk/docs/install) on the system where you will be running 
 `bdbag` in order for this handler to function.
 
 ### Enabling "requester pays":
```

### Comparing `bdbag-1.6.4/LICENSE` & `bdbag-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/Pipfile.lock` & `bdbag-1.7.0/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9442340067340066%*

 * *Differences: {"'default'": "{'awscli': {'hashes': "*

 * *              "['sha256:f1298ebbbf4564448bd47775e7075dd66d547b0b30a9aba6db2f0b399025f4ff', "*

 * *              "'sha256:f77e55b3b2930f76c9e72c3c02ab061fda2091883e5ce066993fbdeedf9a360e'], "*

 * *              "'version': '==1.29.9'}, 'bdbag': {'version': '==1.7.0'}, 'boto3': {'hashes': "*

 * *              "['sha256:01f078047eb4d238c6b9c6cc623f2af33b4ae67980c5326691e35cb5493ff6c7', "*

 * *              "'sha256:4cc0c6005be910e52077227e670930ab55a41ba86cdb6d1c052571d08cd4d32c'], "*

 * *        […]*

```diff
@@ -12,19 +12,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "awscli": {
             "hashes": [
-                "sha256:4f07ca6ab0056d8aa538b1fce3c69e63fe1b2deabce14a4806446fe1e2b66dce",
-                "sha256:e833dbff001dd9761c29121aeeff168b10f43c5ced9bb518e99c7e2e88c4df40"
+                "sha256:f1298ebbbf4564448bd47775e7075dd66d547b0b30a9aba6db2f0b399025f4ff",
+                "sha256:f77e55b3b2930f76c9e72c3c02ab061fda2091883e5ce066993fbdeedf9a360e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.27.63"
+            "version": "==1.29.9"
         },
         "bagit": {
             "hashes": [
                 "sha256:37df1330d2e8640c8dee8ab6d0073ac701f0614d25f5252f9e05263409cee60c",
                 "sha256:d14dd7e373dd24d41f6748c42f123f7db77098dfa4a0125dbacb4c8bdf767c09"
             ],
             "version": "==1.8.1"
@@ -39,39 +39,39 @@
         },
         "bdbag": {
             "extras": [
                 "boto",
                 "globus"
             ],
             "path": ".",
-            "version": "==1.6.4"
+            "version": "==1.7.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:c84857aceccc422d9fb96c26bbc4ec2808b93b39a2886907efef811e6f0b5ea7",
-                "sha256:f688555dd427271e0493e6d166126ce76e1744dd89d626575ba7c2e62ba86e14"
+                "sha256:01f078047eb4d238c6b9c6cc623f2af33b4ae67980c5326691e35cb5493ff6c7",
+                "sha256:4cc0c6005be910e52077227e670930ab55a41ba86cdb6d1c052571d08cd4d32c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.63"
+            "version": "==1.28.9"
         },
         "botocore": {
             "hashes": [
-                "sha256:710864600818b80c865334e12af729923e2886cc760685c614c0eae9cbbfdd4d",
-                "sha256:9e14f8dba1252a03d0a7db7240dc48fa4a3ac470434a044b23c0001f648d6d4f"
+                "sha256:bd849d3ac95f1781385ed831d753a04a3ec870a59d6598175aaedd71dc2baf5f",
+                "sha256:e56ccd3536a90094ea5b176b5dd33bfe4f049efdf71af468ea1661bd424c787d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.63"
+            "version": "==1.31.9"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -136,282 +136,296 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
-            "version": "==3.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.2.0"
         },
         "colorama": {
             "hashes": [
                 "sha256:5941b2b48a20143d2267e95b1c2a7603ce057ee39fd88e7329b0c292aa16869b",
                 "sha256:9f47eda37229f68eee03b24b9748937c7dc3868f906e8ba69fbcbdd3bc5dc3e2"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.4.4"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711",
+                "sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7",
+                "sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd",
+                "sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e",
+                "sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58",
+                "sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0",
+                "sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d",
+                "sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83",
+                "sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831",
+                "sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766",
+                "sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b",
+                "sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c",
+                "sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182",
+                "sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f",
+                "sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa",
+                "sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4",
+                "sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a",
+                "sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2",
+                "sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76",
+                "sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5",
+                "sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee",
+                "sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f",
+                "sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14"
             ],
-            "version": "==39.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.2"
         },
         "docutils": {
             "hashes": [
                 "sha256:0c5b78adfbf7762415433f5515cd5c9e762339e23369dbe8000d84a4bf4ab3af",
                 "sha256:c2de3a60e9e7d07be26b7f2b00ca0309c207e06c100f9cc2a94931fc75a478fc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.16"
         },
         "globus-sdk": {
             "hashes": [
-                "sha256:2e6994f84990aa2f7c2b83689ab8f3bdfce57654abc1cfbd481a19117268395a",
-                "sha256:4945db39968cec6382ef0a44fc72ec05a8516113c9f2f6543ec0325fff47ca89"
+                "sha256:7870486a669d0a197caa7df03683b0b83801aa6e224f2a490bbbc87ada527582",
+                "sha256:d9be275d4ec18054db04732f75649c4227800c79b31fbcfb3f4f31eccfa5f4f7"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.15.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.25.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
+        "importlib-metadata": {
+            "hashes": [
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==6.8.0"
+        },
         "jmespath": {
             "hashes": [
                 "sha256:02e2e4cc71b5bcab88332eebf907519190dd9e6e82107fa7f83b1003a6252980",
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
+        "packaging": {
+            "hashes": [
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
+        },
         "pyasn1": {
             "hashes": [
-                "sha256:014c0e9976956a08139dc0712ae195324a75e142284d5f87f1a87ee1b068a359",
-                "sha256:03840c999ba71680a131cfaee6fab142e1ed9bbd9c693e285cc6aca0d555e576",
-                "sha256:0458773cfe65b153891ac249bcf1b5f8f320b7c2ce462151f8fa74de8934becf",
-                "sha256:08c3c53b75eaa48d71cf8c710312316392ed40899cb34710d092e96745a358b7",
-                "sha256:39c7e2ec30515947ff4e87fb6f456dfc6e84857d34be479c9d4a4ba4bf46aa5d",
-                "sha256:5c9414dcfede6e441f7e8f81b43b34e834731003427e5b09e4e00e3172a10f00",
-                "sha256:6e7545f1a61025a4e58bb336952c5061697da694db1cae97b116e9c46abcf7c8",
-                "sha256:78fa6da68ed2727915c4767bb386ab32cdba863caa7dbe473eaae45f9959da86",
-                "sha256:7ab8a544af125fb704feadb008c99a88805126fb525280b2270bb25cc1d78a12",
-                "sha256:99fcc3c8d804d1bc6d9a099921e39d827026409a58f2a720dcdb89374ea0c776",
-                "sha256:aef77c9fb94a3ac588e87841208bdec464471d9871bd5050a287cc9a475cd0ba",
-                "sha256:e89bf84b5437b532b0803ba5c9a5e054d21fec423a89952a74f87fa2c9b7bce2",
-                "sha256:fec3e9d8e36808a28efb59b489e4528c10ad0f480e57dcc32b4de5c9d8c9fdf3"
+                "sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57",
+                "sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde"
             ],
-            "version": "==0.4.8"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+            "version": "==0.5.0"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pyjwt": {
             "extras": [
                 "crypto"
             ],
             "hashes": [
-                "sha256:69285c7e31fc44f68a1feb309e948e0df53259d579295e6cfe2b1792329f05fd",
-                "sha256:d83c3d892a77bbb74d3e1a2cfa90afaadb60945205d1095d9221f04466f64c14"
+                "sha256:57e28d156e3d5c10088e0c68abb90bfac3df82b40a71bd0daa20c65ccd5c23de",
+                "sha256:59127c392cc44c2da5bb3192169a91f429924e17aff6534d70fdc02ab3e04320"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.0"
+            "version": "==2.8.0"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
-            "version": "==2022.7.1"
+            "version": "==2023.3"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:08682f6b72c722394747bddaf0aa62277e02557c0fd1c42cb853016a38f8dedf",
-                "sha256:0f5f5786c0e09baddcd8b4b45f20a7b5d61a7e7e99846e3c799b05c7c53fa696",
-                "sha256:129def1b7c1bf22faffd67b8f3724645203b79d8f4cc81f674654d9902cb4393",
-                "sha256:294db365efa064d00b8d1ef65d8ea2c3426ac366c0c4368d930bf1c5fb497f77",
-                "sha256:3b2b1824fe7112845700f815ff6a489360226a5609b96ec2190a45e62a9fc922",
-                "sha256:3bd0e463264cf257d1ffd2e40223b197271046d09dadf73a0fe82b9c1fc385a5",
-                "sha256:4465124ef1b18d9ace298060f4eccc64b0850899ac4ac53294547536533800c8",
-                "sha256:49d4cdd9065b9b6e206d0595fee27a96b5dd22618e7520c33204a4a3239d5b10",
-                "sha256:4e0583d24c881e14342eaf4ec5fbc97f934b999a6828693a99157fde912540cc",
-                "sha256:5accb17103e43963b80e6f837831f38d314a0495500067cb25afab2e8d7a4018",
-                "sha256:607774cbba28732bfa802b54baa7484215f530991055bb562efbed5b2f20a45e",
-                "sha256:6c78645d400265a062508ae399b60b8c167bf003db364ecb26dcab2bda048253",
-                "sha256:72a01f726a9c7851ca9bfad6fd09ca4e090a023c00945ea05ba1638c09dc3347",
-                "sha256:74c1485f7707cf707a7aef42ef6322b8f97921bd89be2ab6317fd782c2d53183",
-                "sha256:895f61ef02e8fed38159bb70f7e100e00f471eae2bc838cd0f4ebb21e28f8541",
-                "sha256:8c1be557ee92a20f184922c7b6424e8ab6691788e6d86137c5d93c1a6ec1b8fb",
-                "sha256:bb4191dfc9306777bc594117aee052446b3fa88737cd13b7188d0e7aa8162185",
-                "sha256:bfb51918d4ff3d77c1c856a9699f8492c612cde32fd3bcd344af9be34999bfdc",
-                "sha256:c20cfa2d49991c8b4147af39859b167664f2ad4561704ee74c1de03318e898db",
-                "sha256:cb333c16912324fd5f769fff6bc5de372e9e7a202247b48870bc251ed40239aa",
-                "sha256:d2d9808ea7b4af864f35ea216be506ecec180628aced0704e34aca0b040ffe46",
-                "sha256:d483ad4e639292c90170eb6f7783ad19490e7a8defb3e46f97dfe4bacae89122",
-                "sha256:dd5de0646207f053eb0d6c74ae45ba98c3395a571a2891858e87df7c9b9bd51b",
-                "sha256:e1d4970ea66be07ae37a3c2e48b5ec63f7ba6804bdddfdbd3cfd954d25a82e63",
-                "sha256:e4fac90784481d221a8e4b1162afa7c47ed953be40d31ab4629ae917510051df",
-                "sha256:fa5ae20527d8e831e8230cbffd9f8fe952815b2b7dae6ffec25318803a7528fc",
-                "sha256:fd7f6999a8070df521b6384004ef42833b9bd62cfee11a09bda1079b4b704247",
-                "sha256:fdc842473cd33f45ff6bce46aea678a54e3d21f1b61a7750ce3c498eedfe25d6",
-                "sha256:fe69978f3f768926cfa37b867e3843918e012cf83f680806599ddce33c2c68b0"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==5.4.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==6.0.1"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "rsa": {
             "hashes": [
                 "sha256:78f9a9bf4e7be0c5ded4583326e7461e3a3c5aae24073648b4bdfa797d78c9d2",
                 "sha256:9d689e6ca1b3038bc82bf8d23e944b6b6037bc02301a574935b2dd946e0353b9"
             ],
             "markers": "python_version >= '3.5' and python_version < '4'",
             "version": "==4.7.2"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
-                "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
+                "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
+                "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.6.1"
+        },
+        "setuptools": {
+            "hashes": [
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.6.0"
+            "version": "==68.0.0"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:0d4fa3743c7a453f31dae9b44fcc0c869125a323c166a6b39e20122f488addb2",
                 "sha256:2e8706b90910d66668b3f34aea9cceab3c08ba83fedd78de65ff323edc8a1414",
                 "sha256:35acc9a3be4fbd4f6f3480eecb3c637dfb5ca1812fe86baf5e6759a0133837cf",
                 "sha256:83a0cedd3449e3946307811a4c7b9d89c4b5fd464a2fb5eeccd0a5bb158ae5c8",
@@ -427,95 +441,97 @@
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
-        "typing-extensions": {
-            "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
-            ],
-            "markers": "python_version < '3.10'",
-            "version": "==4.4.0"
-        },
-        "tzlocal": {
+        "urllib3": {
             "hashes": [
-                "sha256:643c97c5294aedc737780a49d9df30889321cbe1204eac2c2ec6134035a92e44",
-                "sha256:e2cb6c6b5b604af38597403e9852872d7f534962ae2954c7f35efcb1ccacf4a4"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
-            "version": "==2.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+            "version": "==1.26.16"
         },
-        "urllib3": {
+        "zipp": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.2"
         }
     },
     "develop": {
         "coverage": {
             "hashes": [
-                "sha256:04481245ef966fbd24ae9b9e537ce899ae584d521dfbe78f89cad003c38ca2ab",
-                "sha256:0c45948f613d5d18c9ec5eaa203ce06a653334cf1bd47c783a12d0dd4fd9c851",
-                "sha256:10188fe543560ec4874f974b5305cd1a8bdcfa885ee00ea3a03733464c4ca265",
-                "sha256:218fe982371ac7387304153ecd51205f14e9d731b34fb0568181abaf7b443ba0",
-                "sha256:29571503c37f2ef2138a306d23e7270687c0efb9cab4bd8038d609b5c2393a3a",
-                "sha256:2a60d6513781e87047c3e630b33b4d1e89f39836dac6e069ffee28c4786715f5",
-                "sha256:2bf1d5f2084c3932b56b962a683074a3692bce7cabd3aa023c987a2a8e7612f6",
-                "sha256:3164d31078fa9efe406e198aecd2a02d32a62fecbdef74f76dad6a46c7e48311",
-                "sha256:32df215215f3af2c1617a55dbdfb403b772d463d54d219985ac7cd3bf124cada",
-                "sha256:33d1ae9d4079e05ac4cc1ef9e20c648f5afabf1a92adfaf2ccf509c50b85717f",
-                "sha256:33ff26d0f6cc3ca8de13d14fde1ff8efe1456b53e3f0273e63cc8b3c84a063d8",
-                "sha256:38da2db80cc505a611938d8624801158e409928b136c8916cd2e203970dde4dc",
-                "sha256:3b155caf3760408d1cb903b21e6a97ad4e2bdad43cbc265e3ce0afb8e0057e73",
-                "sha256:3b946bbcd5a8231383450b195cfb58cb01cbe7f8949f5758566b881df4b33baf",
-                "sha256:3baf5f126f30781b5e93dbefcc8271cb2491647f8283f20ac54d12161dff080e",
-                "sha256:4b14d5e09c656de5038a3f9bfe5228f53439282abcab87317c9f7f1acb280352",
-                "sha256:51b236e764840a6df0661b67e50697aaa0e7d4124ca95e5058fa3d7cbc240b7c",
-                "sha256:63ffd21aa133ff48c4dff7adcc46b7ec8b565491bfc371212122dd999812ea1c",
-                "sha256:6a43c7823cd7427b4ed763aa7fb63901ca8288591323b58c9cd6ec31ad910f3c",
-                "sha256:755e89e32376c850f826c425ece2c35a4fc266c081490eb0a841e7c1cb0d3bda",
-                "sha256:7a726d742816cb3a8973c8c9a97539c734b3a309345236cd533c4883dda05b8d",
-                "sha256:7c7c0d0827e853315c9bbd43c1162c006dd808dbbe297db7ae66cd17b07830f0",
-                "sha256:7ed681b0f8e8bcbbffa58ba26fcf5dbc8f79e7997595bf071ed5430d8c08d6f3",
-                "sha256:7ee5c9bb51695f80878faaa5598040dd6c9e172ddcf490382e8aedb8ec3fec8d",
-                "sha256:8361be1c2c073919500b6601220a6f2f98ea0b6d2fec5014c1d9cfa23dd07038",
-                "sha256:8ae125d1134bf236acba8b83e74c603d1b30e207266121e76484562bc816344c",
-                "sha256:9817733f0d3ea91bea80de0f79ef971ae94f81ca52f9b66500c6a2fea8e4b4f8",
-                "sha256:98b85dd86514d889a2e3dd22ab3c18c9d0019e696478391d86708b805f4ea0fa",
-                "sha256:9ccb092c9ede70b2517a57382a601619d20981f56f440eae7e4d7eaafd1d1d09",
-                "sha256:9d58885215094ab4a86a6aef044e42994a2bd76a446dc59b352622655ba6621b",
-                "sha256:b643cb30821e7570c0aaf54feaf0bfb630b79059f85741843e9dc23f33aaca2c",
-                "sha256:bc7c85a150501286f8b56bd8ed3aa4093f4b88fb68c0843d21ff9656f0009d6a",
-                "sha256:beeb129cacea34490ffd4d6153af70509aa3cda20fdda2ea1a2be870dfec8d52",
-                "sha256:c31b75ae466c053a98bf26843563b3b3517b8f37da4d47b1c582fdc703112bc3",
-                "sha256:c4e4881fa9e9667afcc742f0c244d9364d197490fbc91d12ac3b5de0bf2df146",
-                "sha256:c5b15ed7644ae4bee0ecf74fee95808dcc34ba6ace87e8dfbf5cb0dc20eab45a",
-                "sha256:d12d076582507ea460ea2a89a8c85cb558f83406c8a41dd641d7be9a32e1274f",
-                "sha256:d248cd4a92065a4d4543b8331660121b31c4148dd00a691bfb7a5cdc7483cfa4",
-                "sha256:d47dd659a4ee952e90dc56c97d78132573dc5c7b09d61b416a9deef4ebe01a0c",
-                "sha256:d4a5a5879a939cb84959d86869132b00176197ca561c664fc21478c1eee60d75",
-                "sha256:da9b41d4539eefd408c46725fb76ecba3a50a3367cafb7dea5f250d0653c1040",
-                "sha256:db61a79c07331e88b9a9974815c075fbd812bc9dbc4dc44b366b5368a2936063",
-                "sha256:ddb726cb861c3117a553f940372a495fe1078249ff5f8a5478c0576c7be12050",
-                "sha256:ded59300d6330be27bc6cf0b74b89ada58069ced87c48eaf9344e5e84b0072f7",
-                "sha256:e2617759031dae1bf183c16cef8fcfb3de7617f394c813fa5e8e46e9b82d4222",
-                "sha256:e5cdbb5cafcedea04924568d990e20ce7f1945a1dd54b560f879ee2d57226912",
-                "sha256:ec8e767f13be637d056f7e07e61d089e555f719b387a7070154ad80a0ff31801",
-                "sha256:ef382417db92ba23dfb5864a3fc9be27ea4894e86620d342a116b243ade5d35d",
-                "sha256:f2cba5c6db29ce991029b5e4ac51eb36774458f0a3b8d3137241b32d1bb91f06",
-                "sha256:f5b4198d85a3755d27e64c52f8c95d6333119e49fd001ae5798dac872c95e0f8",
-                "sha256:ffeeb38ee4a80a30a6877c5c4c359e5498eec095878f1581453202bfacc8fbc2"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==7.1.0"
+            "version": "==7.2.7"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
@@ -527,19 +543,19 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mock": {
             "hashes": [
-                "sha256:c41cfb1e99ba5d341fbcc5308836e7d7c9786d302f995b2c271ce2144dece9eb",
-                "sha256:e3ea505c03babf7977fd21674a69ad328053d414f05e6433c30d8fa14a534a6b"
+                "sha256:18c694e5ae8a208cdb3d2c20a993ca1a7b0efa258c247a1e565150f477f83744",
+                "sha256:5e96aad5ccda4718e0a229ed94b2024df75cc2d55575ba5762d31f5767b8767d"
             ],
             "index": "pypi",
-            "version": "==5.0.1"
+            "version": "==5.1.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
```

### Comparing `bdbag-1.6.4/README.md` & `bdbag-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
 #### Technical Papers
 
 ["I'll take that to go: Big data bags and minimal identifiers for exchange of large, complex datasets"](https://zenodo.org/record/820878) explains the motivation for BDBags and the related Minid construct, provides details on design and implementation, and gives examples of use. 
 
 ["Reproducible big data science: A case study in continuous FAIRness"](https://www.biorxiv.org/content/early/2018/02/27/268755) presents a data analysis use case in which BDBags and Minids are used to capture a transcription factor binding site analysis.
 
-### Dependencies
+### Python Dependencies
 
-* [Python 2.7](https://www.python.org/downloads/release/python-27/) is the minimum Python version required.
-* The code and dependencies are also compatible with Python 3, versions 3.5 through 3.9.
+*  Python 2.7 is the minimum Python version required. Please note however that Python 2.7 is officially end-of-life and ongoing compatibility between Python 2.7 and `bdbag` (and its dependencies) is not officially supported and cannot be guaranteed.
+*  Python 3, versions 3.7 through 3.11 are the current officially supported releases.
 
 ### Installation
 The latest `bdbag` release is available on PyPi and can be installed using `pip`:
 
 ```sh
 pip install bdbag
 ```
```

### Comparing `bdbag-1.6.4/bdbag/__init__.py` & `bdbag-1.7.0/bdbag/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,48 +17,47 @@
 import re
 import sys
 import json
 import logging
 import mimetypes
 import shutil
 from datetime import datetime
-from requests.utils import requote_uri
 from distutils.util import strtobool
-from pkg_resources import parse_version, get_distribution, DistributionNotFound
+from importlib_metadata import distribution, PackageNotFoundError
 
 logger = logging.getLogger(__name__)
 
-__version__ = "1.6.4"
+__version__ = "1.7.0"
 __bagit_version__ = "1.8.1"
 __bagit_profile_version__ = "1.3.1"
 
 if sys.version_info > (3,):  # pragma: no cover
     from urllib.parse import quote as urlquote, unquote as urlunquote, urlsplit, urlunsplit, urlparse
     from urllib.request import urlretrieve, urlopen, urlcleanup
 else:  # pragma: no cover
     from urllib import quote as urlquote, unquote as urlunquote, urlretrieve, urlopen, urlcleanup
     from urlparse import urlsplit, urlunsplit, urlparse
 
 try:
-    version = get_distribution("bdbag").version
+    version = distribution("bdbag").version
     VERSION = version + '' if not getattr(sys, 'frozen', False) else version + '-frozen'
-except DistributionNotFound:  # pragma: no cover
+except PackageNotFoundError:  # pragma: no cover
     VERSION = __version__ + '-dev' if not getattr(sys, 'frozen', False) else __version__ + '-frozen'
 PROJECT_URL = 'https://github.com/fair-research/bdbag'
 
 try:
-    version = get_distribution("bagit").version
+    version = distribution("bagit").version
     BAGIT_VERSION = version + '' if not getattr(sys, 'frozen', False) else version + '-frozen'
-except DistributionNotFound:  # pragma: no cover
+except PackageNotFoundError:  # pragma: no cover
     BAGIT_VERSION = 'unknown' if not getattr(sys, 'frozen', False) else __bagit_version__ + '-frozen'
 
 try:
-    version = get_distribution("bagit_profile").version
+    version = distribution("bagit_profile").version
     BAGIT_PROFILE_VERSION = version + '' if not getattr(sys, 'frozen', False) else version + '-frozen'
-except DistributionNotFound:  # pragma: no cover
+except PackageNotFoundError:  # pragma: no cover
     BAGIT_PROFILE_VERSION = 'unknown' if not getattr(sys, 'frozen', False) else __bagit_profile_version__ + '-frozen'
 
 BAG_PROFILE_TAG = 'BagIt-Profile-Identifier'
 BDBAG_PROFILE_ID = 'https://raw.githubusercontent.com/fair-research/bdbag/master/profiles/bdbag-profile.json'
 BDBAG_RO_PROFILE_ID = 'https://raw.githubusercontent.com/fair-research/bdbag/master/profiles/bdbag-ro-profile.json'
 
 CONTENT_DISP_REGEX = re.compile(r"^filename[*]=UTF-8''(?P<name>[-_.~A-Za-z0-9%]+)$")
```

### Comparing `bdbag-1.6.4/bdbag/bdbag_api.py` & `bdbag-1.7.0/bdbag/bdbag_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,26 +435,32 @@
         logger.info("The directory %s is a valid bag structure" % bag_path)
     except Exception as e:
         logger.error("Error while validating bag structure: %s", e)
         raise e
 
 
 def validate_bag_profile(bag_path, profile_path=None):
-
-    logger.info("Validating bag profile: %s" % bag_path)
+    logger.info("Validating bag profile: %s", bag_path)
     bag = bdbagit.BDBag(bag_path)
 
     # Instantiate a profile, supplying its URI.
-    if not profile_path:
-        profile_path = bag.info.get(BAG_PROFILE_TAG, None)
-        if not profile_path:
-            raise bdbp.ProfileValidationError("Bag does not contain a BagIt-Profile-Identifier")
+    profile_url = bag.info.get(BAG_PROFILE_TAG, None)
+    if not profile_url:
+        raise bdbp.ProfileValidationError("Bag does not contain a BagIt-Profile-Identifier")
+    logger.info("Loading profile: %s" % (profile_path if profile_path else profile_url))
+
+    profile = None
+    if profile_path:
+        try:
+            with io.open(profile_path, encoding="UTF-8") as profile_file:
+                profile = json.loads(profile_file.read())
+        except (OSError, IOError, ValueError) as exc:
+            raise bdbp.ProfileValidationError("Profile %s could not be read: %s" % (profile_path, exc))
 
-    logger.info("Retrieving profile: %s" % profile_path)
-    profile = bdbp.BDBProfile(profile_path)
+    profile = bdbp.BDBProfile(profile_url, profile)
 
     # Validate the profile.
     if profile.validate(bag):
         logger.info("Bag structure conforms to specified profile")
     else:
         raise bdbp.ProfileValidationError("Bag structure does not conform to specified profile: %s" % profile.report)
```

### Comparing `bdbag-1.6.4/bdbag/bdbag_cli.py` & `bdbag-1.7.0/bdbag/bdbag_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,20 @@
 
     validate_profile_arg = "--validate-profile"
     standard_args.add_argument(
         validate_profile_arg, const='full', nargs='?', choices=['bag-only', 'full'],
         help="Validate a bag against the profile specified by the bag's \"BagIt-Profile-Identifier\" metadata field, "
              "if present. If \"bag-only\" is specified, the bag's serialization method will not be validated.")
 
+    profile_path_arg = "--profile-path"
+    standard_args.add_argument(
+        profile_path_arg, metavar='<file>',
+        help="Optional path to local profile JSON to use for profile validation. If not specified the profile "
+             "referenced in the bag info file will be fetched and used.")
+
     config_file_arg = "--config-file"
     standard_args.add_argument(
         config_file_arg, metavar='<file>',
         help="Optional path to a configuration file. If this argument is not specified, the configuration file "
              "will be set to the value of the environment variable %s (if present) or otherwise default to: %s"
              % (DEFAULT_CONFIG_FILE_ENVAR, DEFAULT_CONFIG_FILE))
 
@@ -305,14 +311,15 @@
 
 
 def main():
 
     args, path, is_bag, is_file, is_uri = parse_cli()
 
     archive = None
+    profile = None
     temp_path = None
     error = None
     result = 0
 
     if not args.quiet:
         sys.stdout.write('\n')
 
@@ -335,15 +342,15 @@
             if not args.quiet:
                 sys.stdout.write('\n')
             return result
 
         if not is_file:
             # do not try to create or update the bag if the user just wants to validate or complete an existing bag
             if not ((args.validate or args.validate_profile or args.resolve_fetch)
-                    and not (args.update and bdb.is_bag(path))):
+                    and not (args.update and bdb.is_bag(path))) or not bdb.is_bag(path):
                 if args.checksum and 'all' in args.checksum:
                     args.checksum = ['md5', 'sha1', 'sha256', 'sha512']
                 # create or update the bag depending on the input arguments
                 bdb.make_bag(path,
                              algs=args.checksum,
                              update=args.update,
                              save_manifests=not args.skip_manifests,
@@ -370,14 +377,18 @@
                 sys.stderr.write(ASYNC_TRANSFER_VALIDATION_WARNING)
             bdb.resolve_fetch(path,
                               force=True if args.resolve_fetch == 'all' else False,
                               keychain_file=args.keychain_file,
                               config_file=args.config_file,
                               filter_expr=args.fetch_filter)
 
+        if args.validate_profile:
+            if not is_file:
+                profile = bdb.validate_bag_profile(temp_path if temp_path else path, profile_path=args.profile_path)
+
         if args.validate:
             if is_file:
                 temp_path = bdb.extract_bag(path, args.output_path, temp=True if not args.output_path else False)
             if args.validate == 'structure':
                 bdb.validate_bag_structure(temp_path if temp_path else path)
             elif args.validate == 'completeness':
                 bdb.validate_bag_structure(temp_path if temp_path else path, skip_remote=False)
@@ -388,21 +399,21 @@
 
         if args.archiver:
             archive = bdb.archive_bag(path, args.archiver)
 
         if archive is None and is_file:
             archive = path
 
-        if args.validate_profile:
+        if args.validate_profile == "full":
             if is_file:
                 if not temp_path:
-                    temp_path = bdb.extract_bag(path, args.output_path, temp=True if not args.output_path else False)
-            profile = bdb.validate_bag_profile(temp_path if temp_path else path)
-            if not args.validate_profile == "bag-only":
-                bdb.validate_bag_serialization(archive if archive else path, profile)
+                    temp_path = bdb.extract_bag(path, args.output_path, temp=args.output_path is None)
+            if not profile:
+                profile = bdb.validate_bag_profile(temp_path if temp_path else path, profile_path=args.profile_path)
+            bdb.validate_bag_serialization(archive if archive else path, profile)
 
         if args.revert:
             bdb.revert_bag(path)
 
     except Exception as e:
         result = 1
         error = "Error: %s" % get_typed_exception(e)
```

### Comparing `bdbag-1.6.4/bdbag/bdbag_config.py` & `bdbag-1.7.0/bdbag/bdbag_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # limitations under the License.
 #
 import os
 import errno
 import logging
 import json
 from collections import OrderedDict
-from bdbag import parse_version, get_typed_exception, safe_move, \
+from packaging.version import parse as parse_version
+from bdbag import get_typed_exception, safe_move, \
     DEFAULT_CONFIG_PATH, BAG_PROFILE_TAG, BDBAG_PROFILE_ID, VERSION
 from bdbag.fetch import Megabyte
 from bdbag.fetch.auth.keychain import DEFAULT_KEYCHAIN_FILE, write_keychain
 
 logger = logging.getLogger(__name__)
 
 BAG_CONFIG_TAG = "bag_config"
```

### Comparing `bdbag-1.6.4/bdbag/bdbag_ro.py` & `bdbag-1.7.0/bdbag/bdbag_ro.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/bdbag_utils.py` & `bdbag-1.7.0/bdbag/bdbag_utils.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/bdbagit.py` & `bdbag-1.7.0/bdbag/bdbagit.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/bdbagit_profile.py` & `bdbag-1.7.0/bdbag/bdbagit_profile.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/__init__.py` & `bdbag-1.7.0/bdbag/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/auth/cookies.py` & `bdbag-1.7.0/bdbag/fetch/auth/cookies.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/auth/keychain.py` & `bdbag-1.7.0/bdbag/fetch/auth/keychain.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/fetcher.py` & `bdbag-1.7.0/bdbag/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/resolvers/__init__.py` & `bdbag-1.7.0/bdbag/fetch/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/resolvers/ark_resolver.py` & `bdbag-1.7.0/bdbag/fetch/resolvers/ark_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/resolvers/base_resolver.py` & `bdbag-1.7.0/bdbag/fetch/resolvers/base_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/resolvers/dataguid_resolver.py` & `bdbag-1.7.0/bdbag/fetch/resolvers/dataguid_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/resolvers/doi_resolver.py` & `bdbag-1.7.0/bdbag/fetch/resolvers/doi_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/__init__.py` & `bdbag-1.7.0/bdbag/fetch/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/base_transport.py` & `bdbag-1.7.0/bdbag/fetch/transports/base_transport.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/fetch_boto3.py` & `bdbag-1.7.0/bdbag/fetch/transports/fetch_boto3.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/fetch_ftp.py` & `bdbag-1.7.0/bdbag/fetch/transports/fetch_ftp.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/fetch_gcs.py` & `bdbag-1.7.0/bdbag/fetch/transports/fetch_gcs.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-#
-# Copyright 2016 University of Southern California
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-import os
-import datetime
-import logging
-from importlib import import_module
-from bdbag import urlsplit, urlunsplit, stob, get_typed_exception
-from bdbag.bdbag_config import DEFAULT_CONFIG, DEFAULT_FETCH_CONFIG, FETCH_CONFIG_TAG
-from bdbag.fetch import *
-from bdbag.fetch.transports.base_transport import BaseFetchTransport
-from bdbag.fetch.auth import keychain as kc
-
-logger = logging.getLogger(__name__)
-
-GCS = None
-GSA = None
-
-
-class GCSFetchTransport(BaseFetchTransport):
-
-    def __init__(self, config, keychain, **kwargs):
-        super(GCSFetchTransport, self).__init__(config, keychain, **kwargs)
-        self.config = config or DEFAULT_FETCH_CONFIG[SCHEME_GS]
-
-    @staticmethod
-    def import_gcs():
-        # locate library
-        global GCS
-        if GCS is None:
-            gcs_module = "google.cloud.storage"
-            try:
-                GCS = import_module(gcs_module)
-            except ImportError as e:
-                raise RuntimeError(
-                    "Unable to find required module. Ensure that the Python module "
-                    "\"%s\" is installed." % gcs_module, e)
-        global GSA
-        if GSA is None:
-            gsa_module = "google.oauth2.service_account"
-            try:
-                GSA = import_module(gsa_module)
-            except ImportError as e:
-                raise RuntimeError(
-                    "Unable to find required module. Ensure that the Python module "
-                    "\"%s\" is installed." % gsa_module, e)
-
-    @staticmethod
-    def validate_auth_config(auth):
-        if not kc.has_auth_attr(auth, "auth_type"):
-            return False
-
-        return True
-
-    def get_credentials(self, url):
-        credentials = None
-        for auth in kc.get_auth_entries(url, self.keychain):
-            if not self.validate_auth_config(auth):
-                continue
-            auth_type = auth.get("auth_type")
-            auth_params = auth.get("auth_params")
-            if auth_type == "gcs-credentials":
-                credentials = auth_params
-                break
-
-        return credentials
-
-    def fetch(self, url, output_path, **kwargs):
-        success = False
-        output_path = ensure_valid_output_path(url, output_path)
-
-        self.import_gcs()
-        try:
-            credentials = self.get_credentials(url) or {}
-            project_id = credentials.get("project_id") or self.config.get("default_project_id") or None
-            service_account_creds_file = credentials.get("service_account_credentials_file")
-            storage_credentials = GSA.Credentials.from_service_account_file(service_account_creds_file) \
-                if (service_account_creds_file and os.path.isfile(service_account_creds_file)) else None
-            try:
-                gcs_client = GCS.Client(project=project_id, credentials=storage_credentials)
-            except Exception as e:
-                raise RuntimeError("Unable to create GCS storage client: %s" % get_typed_exception(e))
-
-            upr = urlsplit(url, allow_fragments=False)
-            allow_requester_pays = credentials.get("allow_requester_pays", False)
-            bucket = gcs_client.bucket(upr.netloc, user_project=project_id if allow_requester_pays else None)
-            logger.info("Attempting GET from URL: %s with project_id=%s and allow_requester_pays=%s%s" %
-                        (url, project_id, allow_requester_pays,
-                         ". Using service account credentials from file %s" % service_account_creds_file if
-                         service_account_creds_file else ""))
-            logger.debug("Transferring file %s to %s" % (url, output_path))
-            blob = bucket.blob(upr.path.lstrip("/"))
-            start = datetime.datetime.now()
-            blob.download_to_filename(output_path)
-            elapsed_time = datetime.datetime.now() - start
-            total = os.path.getsize(output_path)
-            check_transfer_size_mismatch(output_path, kwargs.get("size"), total)
-            logger.info("File [%s] transfer complete. %s" % (output_path, get_transfer_summary(total, elapsed_time)))
-            success = True
-        except Exception as e:
-            logger.error(get_typed_exception(e))
-        finally:
-            if not success:
-                logger.error("GCS GET Failed for URL: %s" % url)
-                logger.warning("File transfer failed: [%s]" % output_path)
-
-        return output_path if success else None
-
-    def cleanup(self):
-        pass
+#
+# Copyright 2016 University of Southern California
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+import os
+import datetime
+import logging
+from importlib import import_module
+from bdbag import urlsplit, urlunsplit, stob, get_typed_exception
+from bdbag.bdbag_config import DEFAULT_CONFIG, DEFAULT_FETCH_CONFIG, FETCH_CONFIG_TAG
+from bdbag.fetch import *
+from bdbag.fetch.transports.base_transport import BaseFetchTransport
+from bdbag.fetch.auth import keychain as kc
+
+logger = logging.getLogger(__name__)
+
+GCS = None
+GSA = None
+
+
+class GCSFetchTransport(BaseFetchTransport):
+
+    def __init__(self, config, keychain, **kwargs):
+        super(GCSFetchTransport, self).__init__(config, keychain, **kwargs)
+        self.config = config or DEFAULT_FETCH_CONFIG[SCHEME_GS]
+
+    @staticmethod
+    def import_gcs():
+        # locate library
+        global GCS
+        if GCS is None:
+            gcs_module = "google.cloud.storage"
+            try:
+                GCS = import_module(gcs_module)
+            except ImportError as e:
+                raise RuntimeError(
+                    "Unable to find required module. Ensure that the Python module "
+                    "\"%s\" is installed." % gcs_module, e)
+        global GSA
+        if GSA is None:
+            gsa_module = "google.oauth2.service_account"
+            try:
+                GSA = import_module(gsa_module)
+            except ImportError as e:
+                raise RuntimeError(
+                    "Unable to find required module. Ensure that the Python module "
+                    "\"%s\" is installed." % gsa_module, e)
+
+    @staticmethod
+    def validate_auth_config(auth):
+        if not kc.has_auth_attr(auth, "auth_type"):
+            return False
+
+        return True
+
+    def get_credentials(self, url):
+        credentials = None
+        for auth in kc.get_auth_entries(url, self.keychain):
+            if not self.validate_auth_config(auth):
+                continue
+            auth_type = auth.get("auth_type")
+            auth_params = auth.get("auth_params")
+            if auth_type == "gcs-credentials":
+                credentials = auth_params
+                break
+
+        return credentials
+
+    def fetch(self, url, output_path, **kwargs):
+        success = False
+        output_path = ensure_valid_output_path(url, output_path)
+
+        self.import_gcs()
+        try:
+            credentials = self.get_credentials(url) or {}
+            project_id = credentials.get("project_id") or self.config.get("default_project_id") or None
+            service_account_creds_file = credentials.get("service_account_credentials_file")
+            storage_credentials = GSA.Credentials.from_service_account_file(service_account_creds_file) \
+                if (service_account_creds_file and os.path.isfile(service_account_creds_file)) else None
+            try:
+                gcs_client = GCS.Client(project=project_id, credentials=storage_credentials)
+            except Exception as e:
+                raise RuntimeError("Unable to create GCS storage client: %s" % get_typed_exception(e))
+
+            upr = urlsplit(url, allow_fragments=False)
+            allow_requester_pays = credentials.get("allow_requester_pays", False)
+            bucket = gcs_client.bucket(upr.netloc, user_project=project_id if allow_requester_pays else None)
+            logger.info("Attempting GET from URL: %s with project_id=%s and allow_requester_pays=%s%s" %
+                        (url, project_id, allow_requester_pays,
+                         ". Using service account credentials from file %s" % service_account_creds_file if
+                         service_account_creds_file else ""))
+            logger.debug("Transferring file %s to %s" % (url, output_path))
+            blob = bucket.blob(upr.path.lstrip("/"))
+            start = datetime.datetime.now()
+            blob.download_to_filename(output_path)
+            elapsed_time = datetime.datetime.now() - start
+            total = os.path.getsize(output_path)
+            check_transfer_size_mismatch(output_path, kwargs.get("size"), total)
+            logger.info("File [%s] transfer complete. %s" % (output_path, get_transfer_summary(total, elapsed_time)))
+            success = True
+        except Exception as e:
+            logger.error(get_typed_exception(e))
+        finally:
+            if not success:
+                logger.error("GCS GET Failed for URL: %s" % url)
+                logger.warning("File transfer failed: [%s]" % output_path)
+
+        return output_path if success else None
+
+    def cleanup(self):
+        pass
```

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/fetch_globus.py` & `bdbag-1.7.0/bdbag/fetch/transports/fetch_globus.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/fetch_http.py` & `bdbag-1.7.0/bdbag/fetch/transports/fetch_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,15 @@
             redirect_status_codes = self.config.get(
                 FETCH_HTTP_REDIRECT_STATUS_CODES_TAG, DEFAULT_FETCH_HTTP_REDIRECT_STATUS_CODES)
 
             session = self.get_session(url)
             output_path = ensure_valid_output_path(url, output_path)
             allow_redirects = stob(self.config.get("allow_redirects", True))
             allow_redirects_with_token = False
+            authorization = None
             auth = self.get_auth(url) or {}
             auth_type = auth.get("auth_type")
             auth_params = auth.get("auth_params")
             if auth_type == "bearer-token":
                 allow_redirects = False
                 # Force setting the "X-Requested-With": "XMLHttpRequest" header is a workaround for some OIDC servers
                 # which on an unauthenticated request redirect to a login flow instead of responding with a 401.
@@ -216,23 +217,28 @@
                             if authorization:
                                 headers.update({"Authorization": authorization})
                             else:
                                 logger.warning(
                                     "Unable to locate Authorization header in requests session headers after redirect")
                         else:
                             logger.warning("Authorization bearer token propagation on redirect is disabled for "
-                                           "security reasons. Enable token propagation for this URL in keychain.json")
+                                           "security reasons. If necessary, you can enable token propagation for this "
+                                           "URL in keychain.json.")
                             if session.headers.get("Authorization"):
                                 del session.headers["Authorization"]
                     elif not allow_redirects:
                         logger.warning("Redirects for this scheme have been disabled via the configuration file.")
                         break
                 else:
                     break
 
+            # restore the bearer-token auth header back to the session if it exists got stripped due to redirect
+            if auth_type == "bearer-token" and authorization is not None and not session.headers.get("Authorization"):
+                session.headers.update({"Authorization": authorization})
+
             if r.status_code != 200:
                 logger.error("HTTP GET Failed for URL: %s" % url)
                 logger.error("Host %s responded:\n\n%s" % (urlsplit(url).netloc,  r.text))
                 logger.warning("File transfer failed: [%s]" % output_path)
             else:
                 total = 0
                 start = datetime.datetime.now()
```

### Comparing `bdbag-1.6.4/bdbag/fetch/transports/fetch_tag.py` & `bdbag-1.7.0/bdbag/fetch/transports/fetch_tag.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/bdbag.egg-info/SOURCES.txt` & `bdbag-1.7.0/bdbag.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .gitattributes
 .travis.yml
 CHANGELOG.md
 LICENSE
 Pipfile
 Pipfile.lock
 README.md
-pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/bdbag.yml
 bdbag/__init__.py
 bdbag/bdbag_api.py
 bdbag/bdbag_cli.py
 bdbag/bdbag_config.py
 bdbag/bdbag_ro.py
 bdbag/bdbag_utils.py
 bdbag/bdbagit.py
```

### Comparing `bdbag-1.6.4/doc/api.md` & `bdbag-1.7.0/doc/api.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/doc/cli.md` & `bdbag-1.7.0/doc/cli.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 [--skip-manifests]
 [--prune-manifests]
 [--materialize]
 [--resolve-fetch {all,missing}]
 [--fetch-filter <column><operator><value>]
 [--validate {fast,full,structure,completeness}]
 [--validate-profile {profile-only,full}]
+[--profile-path <file>]
 [--config-file <file>]
 [--keychain-file <file>]
 [--metadata-file <file>]
 [--ro-metadata-file <file>]
 [--ro-manifest-generate {overwrite, update}]
 [--remote-file-manifest <file>]
 [--quiet]
@@ -182,14 +183,20 @@
 ----
 #### `--validate-profile {bag-only, full}`
 Validate a bag against the profile specified by the bag's `BagIt-Profile-Identifier` metadata field, if present. The 
 `bag-only` argument keyword can be used to bypass the otherwise automatic bag serialization validation 
 (implied by the default value, `full`), and therefore is suitable for use on bag directories.
 
 ----
+#### `--profile-path <file>`
+Optional path to a `Bagit-Profiles-Specification` JSON file. The file format is described
+[here](https://bagit-profiles.github.io/bagit-profiles-specification/).
+If this argument is not specified, the profile specified by the bag's `BagIt-Profile-Identifier` metadata field will be used.
+
+----
 #### `--config-file <file>`
 Optional path to a *bdbag* configuration file. The configuration file format is described
 [here](./config.md#bdbag.json).
 If this argument is not specified, the configuration file will be set to the value of the environment variable `BDBAG_CONFIG_FILE` (if present) or otherwise default to `~/.bdbag/bdbag.json`.
 
 ----
 #### `--keychain-file <file>`
@@ -245,14 +252,15 @@
 |      `--prune-manifests` |                  bag dir only, update only                  | Unused manifests may only be pruned from an existing bag during an update operation.                                                                                                                                                          |
 |       `--skip-manifests` |                  bag dir only, update only                  | Skipping the recalculation of payload checksums may only be performed on an existing bag during an update operation.                                                                                                                          |
 |          `--materialize` |       bag archive, bag dir, or actionable bag URL/URI       | The `--materialze` argument cannot be combined with any other arguments except for `--config-file`, `--keychain-file`, and `--fetch-filter`.                                                                                                  |
 |        `--resolve-fetch` |              bag dir only, no create or update              | The resolution (download) of files listed in fetch.txt cannot be executed when creating or updating a bag.                                                                                                                                    |
 |         `--fetch-filter` |                  bag dir only, fetch only                   | A fetch filter is only relevant during a `--resolve-fetch`.                                                                                                                                                                                   |
 |             `--validate` |                             all                             | A bag directory or a bag archive can be validated.  If a bag archive is to be validated, it is first extracted from the archive to a temporary directory and validated, then the temporary directory is removed.                              |
 |     `--validate-profile` |                             all                             | A bag directory or a bag archive can have its profile validated.  If a bag archive is to have its profile validated, it is first extracted from the archive to a temporary directory and validated, then the temporary directory is removed.  |
+|         `--profile-path` | bag dir or bag archive, only used with `--validate-profile` | A local profile path is only valid in the context of a `--validate-profile` operation.                                                                                                                                                        |
 |          `--config-file` |             bag dir only, create or update only             | A config-file override can be specified whenever a bag is created or updated.                                                                                                                                                                 |
 |        `--keychain-file` | bag dir only, used only when `--resolve-fetch` is specified | This argument is only meaningful in the context of remote file resolution.                                                                                                                                                                    |
 |        `--metadata-file` |             bag dir only, create or update only             | A metadata config file can be specified whenever a bag is created or updated.                                                                                                                                                                 |
 |     `--ro-metadata-file` |             bag dir only, create or update only             | A Research Object metadata config file can be specified whenever a bag is created or updated.                                                                                                                                                 |
 | `--remote-file-manifest` |             bag dir only, create or update only             | A remote-file-manifest can be specified whenever a bag is created or updated.                                                                                                                                                                 |
 | `--ro-manifest-generate` |                        bag dir only                         | An RO manifest may be auto-generated on any valid bag directory.                                                                                                                                                                              |
 |    any extended argument |             bag dir only, create or update only             | Any of the standard bag metadata extended arguments, e.g., `--source-organization` or `--contact-email` may be specified during create or update of a bag directory, but not a bag archive.                                                   |
```

### Comparing `bdbag-1.6.4/doc/config.md` & `bdbag-1.7.0/doc/config.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/doc/utils.md` & `bdbag-1.7.0/doc/utils.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/bagofbags/README.md` & `bdbag-1.7.0/examples/bagofbags/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/bagofbags/bagofbags.py` & `bdbag-1.7.0/examples/bagofbags/bagofbags.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/bagofbags/images/MetaBags.png` & `bdbag-1.7.0/examples/bagofbags/images/MetaBags.png`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/bagofbags/images/MetaBags.pptx` & `bdbag-1.7.0/examples/bagofbags/images/MetaBags.pptx`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/metamanifests/README.md` & `bdbag-1.7.0/examples/metamanifests/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/metamanifests/samples/sample1/remote-files.json` & `bdbag-1.7.0/examples/metamanifests/samples/sample1/remote-files.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/examples/metamanifests/samples/sample1/ro_metadata.json` & `bdbag-1.7.0/examples/metamanifests/samples/sample1/ro_metadata.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/profiles/bdbag-profile.json` & `bdbag-1.7.0/profiles/bdbag-profile.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/profiles/bdbag-ro-profile.json` & `bdbag-1.7.0/profiles/bdbag-ro-profile.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/setup.py` & `bdbag-1.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,43 +49,47 @@
         ]
     },
     requires=[
         'pytz',
         'tzlocal',
         'requests',
         'certifi',
+        'importlib_metadata',
+        'packaging',
         'bagit',
         'bagit_profile'
     ],
     install_requires=['pytz',
-                      'tzlocal==2.1',
+                      'tzlocal<3; python_version < "3"',
+                      'tzlocal',
                       'certifi',
-                      'requests>=2.7.0,<=2.25.1; python_version == "3.5"',
+                      'packaging',
+                      'importlib-metadata',
                       'requests>=2.7.0',
                       'setuptools_scm<6.0',  # for bagit which does not properly include it in install_requires
                       'bagit==1.8.1',
                       'bagit-profile==1.3.1'
                       ],
     extras_require={
         'boto': ["boto3>=1.9.5", "botocore", "awscli"],
         'globus': ["globus_sdk>=1.6.0"],
         'gcs': ["google_cloud_storage"]
     },
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4',
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, <4',
     license='Apache 2.0',
     classifiers=[
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
+
     ]
 )
```

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag-fetch-http.zip` & `bdbag-1.7.0/test/test-data/test-archives/test-bag-fetch-http.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag-multi-parent.tgz` & `bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag-multi-parent.zip` & `bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag-no-parent.tgz` & `bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag-no-parent.zip` & `bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag.bz2` & `bdbag-1.7.0/test/test-data/test-archives/test-bag.bz2`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag.tar` & `bdbag-1.7.0/test/test-data/test-archives/test-bag.tar`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag.tgz` & `bdbag-1.7.0/test/test-data/test-archives/test-bag.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-archives/test-bag.zip` & `bdbag-1.7.0/test/test-data/test-archives/test-bag.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-empty-dirs/metadata/manifest.json` & `bdbag-1.7.0/test/test-data/test-bag-empty-dirs/metadata/manifest.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt` & `bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt` & `bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt` & `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-no-data/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bag-profile/tagmanifest-sha512.txt` & `bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg` & `bdbag-1.7.0/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg` & `bdbag-1.7.0/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg` & `bdbag-1.7.0/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg` & `bdbag-1.7.0/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-10.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-10.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-11.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-11.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-12.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-12.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-3.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-3.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-4.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-4.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-5.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-5.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-6.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-6.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-7.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-7.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-8.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-8.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-config-9.json` & `bdbag-1.7.0/test/test-data/test-config/test-config-9.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest-2.json` & `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-2.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest-encoding.json` & `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-encoding.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json` & `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-fetch-manifest.json` & `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-keychain-8.json` & `bdbag-1.7.0/test/test-data/test-config/test-keychain-8.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-keychain-9.json` & `bdbag-1.7.0/test/test-data/test-config/test-keychain-9.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test-data/test-config/test-ro-metadata.json` & `bdbag-1.7.0/test/test-data/test-config/test-ro-metadata.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test_api.py` & `bdbag-1.7.0/test/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 import mock
 import unittest
 import tarfile
 import zipfile
 from os.path import join as ospj
 from os.path import exists as ospe
 from os.path import isfile as ospif
-from bdbag import bdbag_api as bdb, bdbag_config as bdbcfg, bdbag_ro as bdbro, bdbagit as bdbagit, filter_dict, \
-    get_typed_exception, DEFAULT_CONFIG_PATH
+from bdbag import bdbag_api as bdb, bdbag_config as bdbcfg, bdbag_ro as bdbro, bdbagit as bdbagit, bdbagit_profile, \
+    filter_dict, get_typed_exception, DEFAULT_CONFIG_PATH
 from bdbag.fetch.auth import keychain
 from test.test_common import BaseTest
 
 if sys.version_info > (3,):
     from io import StringIO
 else:
     from StringIO import StringIO
@@ -889,14 +889,32 @@
             output = self.stream.getvalue()
             self.assertExpectedMessages(["The size of the local file",
                                          "does not match the size of the file",
                                          "specified in fetch.txt"], output)
         except Exception as e:
             self.fail(get_typed_exception(e))
 
+    def test_validate_profile_with_local_profile(self):
+        logger.info(self.getTestHeader('validate local profile'))
+        try:
+            profile = bdb.validate_bag_profile(self.test_bag_profile_dir, "./profiles/bdbag-profile.json")
+            self.assertIsInstance(profile, bdbagit_profile.Profile)
+        except Exception as e:
+            self.fail(get_typed_exception(e))
+
+    def test_validate_profile_with_local_bad_path_profile(self):
+        logger.info(self.getTestHeader('validate bad path local profile'))
+        try:
+            self.assertRaises(bdbagit_profile.ProfileValidationError,
+                              bdb.validate_bag_profile,
+                              self.test_bag_profile_dir,
+                              "./profiles/missing-bdbag-profile.json")
+        except Exception as e:
+            self.fail(get_typed_exception(e))
+
     def test_filter_dict(self):
         logger.info(self.getTestHeader('test filter function'))
 
         msg = "evaluating filter expression: %s"
         test_url = "http://example.com/files/examples/README.txt"
         test_length = 250624
         test_filename = "data/examples/README.txt"
```

### Comparing `bdbag-1.6.4/test/test_bdbagit.py` & `bdbag-1.7.0/test/test_bdbagit.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test_cli.py` & `bdbag-1.7.0/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,21 @@
 
     def test_validate_profile_skip_serialization(self):
         args = ARGS + [self.test_bag_dir, '--validate-profile', "bag-only"]
         logfile.writelines(self.getTestHeader('validate-profile, bag only', args))
         self._test_successful_invocation(
             args, ["Bag structure conforms to specified profile"])
 
+    def test_validate_local_profile(self):
+        args = ARGS + [self.test_bag_profile_dir, '--validate-profile', 'bag-only',
+                       '--profile-path', './profiles/bdbag-profile.json']
+        logfile.writelines(self.getTestHeader('validate-local-profile', args))
+        self._test_successful_invocation(
+            args, ["Loading profile: ./profiles/bdbag-profile.json", "Bag structure conforms to specified profile"])
+
 
 class TestCliArgParsing(BaseTest):
 
     test_type = "Arg parsing test"
 
     def setUp(self):
         super(TestCliArgParsing, self).setUp()
```

### Comparing `bdbag-1.6.4/test/test_common.py` & `bdbag-1.7.0/test/test_common.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.6.4/test/test_remote.py` & `bdbag-1.7.0/test/test_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             bdb.validate_bag_structure(bag_dir, True)
         except Exception as e:
             self.fail(bdbag.get_typed_exception(e))
 
     def test_validate_profile(self):
         logger.info(self.getTestHeader('validate profile'))
         try:
-            profile = bdb.validate_bag_profile(self.test_bag_dir)
+            profile = bdb.validate_bag_profile(self.test_bag_profile_dir)
             self.assertIsInstance(profile, bdbagit_profile.Profile)
         except Exception as e:
             self.fail(bdbag.get_typed_exception(e))
 
     def test_validate_profile_serialization_zip(self):
         logger.info(self.getTestHeader('validate profile serialization zip'))
         try:
```

