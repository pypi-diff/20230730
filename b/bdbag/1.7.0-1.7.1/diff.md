# Comparing `tmp/bdbag-1.7.0.tar.gz` & `tmp/bdbag-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdbag-1.7.0.tar", last modified: Sun Jul 30 00:27:25 2023, max compression
+gzip compressed data, was "bdbag-1.7.1.tar", last modified: Sun Jul 30 02:54:08 2023, max compression
```

## Comparing `bdbag-1.7.0.tar` & `bdbag-1.7.1.tar`

### file list

```diff
@@ -1,467 +1,467 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/
--rw-rw-rw-   0        0        0       18 2022-01-11 18:46:35.000000 bdbag-1.7.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.138764 bdbag-1.7.0/.github/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.223412 bdbag-1.7.0/.github/workflows/
--rw-rw-rw-   0        0        0     1599 2023-07-21 21:19:21.000000 bdbag-1.7.0/.github/workflows/bdbag.yml
--rw-rw-rw-   0        0        0      750 2022-05-27 21:39:45.000000 bdbag-1.7.0/.travis.yml
--rw-rw-rw-   0        0        0    19388 2023-07-24 19:38:50.000000 bdbag-1.7.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    11357 2022-01-11 18:46:35.000000 bdbag-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     7193 2023-07-30 00:27:25.909708 bdbag-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      197 2022-05-26 23:02:23.000000 bdbag-1.7.0/Pipfile
--rw-rw-rw-   0        0        0    36425 2023-07-21 21:50:32.000000 bdbag-1.7.0/Pipfile.lock
--rw-rw-rw-   0        0        0     5771 2023-07-24 19:32:43.000000 bdbag-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.285920 bdbag-1.7.0/bdbag/
--rw-rw-rw-   0        0        0     9985 2023-07-25 18:36:01.000000 bdbag-1.7.0/bdbag/__init__.py
--rw-rw-rw-   0        0        0    26658 2023-07-24 18:23:35.000000 bdbag-1.7.0/bdbag/bdbag_api.py
--rw-rw-rw-   0        0        0    20001 2023-07-25 16:48:58.000000 bdbag-1.7.0/bdbag/bdbag_cli.py
--rw-rw-rw-   0        0        0     9578 2023-07-20 18:46:39.000000 bdbag-1.7.0/bdbag/bdbag_config.py
--rw-rw-rw-   0        0        0    13883 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/bdbag_ro.py
--rw-rw-rw-   0        0        0    27410 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/bdbag_utils.py
--rw-rw-rw-   0        0        0    24599 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/bdbagit.py
--rw-rw-rw-   0        0        0     2357 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/bdbagit_profile.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.323696 bdbag-1.7.0/bdbag/fetch/
--rw-rw-rw-   0        0        0     2233 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.339326 bdbag-1.7.0/bdbag/fetch/auth/
--rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/auth/__init__.py
--rw-rw-rw-   0        0        0     3282 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/auth/cookies.py
--rw-rw-rw-   0        0        0     6159 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/auth/keychain.py
--rw-rw-rw-   0        0        0     4980 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/fetcher.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.354944 bdbag-1.7.0/bdbag/fetch/resolvers/
--rw-rw-rw-   0        0        0     2486 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/__init__.py
--rw-rw-rw-   0        0        0     2802 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/ark_resolver.py
--rw-rw-rw-   0        0        0     3142 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/base_resolver.py
--rw-rw-rw-   0        0        0     2271 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/dataguid_resolver.py
--rw-rw-rw-   0        0        0     2600 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/resolvers/doi_resolver.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.423979 bdbag-1.7.0/bdbag/fetch/transports/
--rw-rw-rw-   0        0        0     2701 2022-11-15 21:11:09.000000 bdbag-1.7.0/bdbag/fetch/transports/__init__.py
--rw-rw-rw-   0        0        0     1057 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/transports/base_transport.py
--rw-rw-rw-   0        0        0     7061 2022-05-26 21:34:05.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_boto3.py
--rw-rw-rw-   0        0        0     3348 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_ftp.py
--rw-rw-rw-   0        0        0     5193 2023-02-02 22:20:48.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_gcs.py
--rw-rw-rw-   0        0        0     5133 2022-02-11 20:26:50.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_globus.py
--rw-rw-rw-   0        0        0    12755 2023-07-19 21:57:14.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_http.py
--rw-rw-rw-   0        0        0     1389 2022-01-11 18:46:35.000000 bdbag-1.7.0/bdbag/fetch/transports/fetch_tag.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.308055 bdbag-1.7.0/bdbag.egg-info/
--rw-rw-rw-   0        0        0     7193 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19233 2023-07-30 00:27:25.000000 bdbag-1.7.0/bdbag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      247 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-30 00:27:24.000000 bdbag-1.7.0/bdbag.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.470859 bdbag-1.7.0/doc/
--rw-rw-rw-   0        0        0    38271 2023-02-02 23:26:13.000000 bdbag-1.7.0/doc/api.md
--rw-rw-rw-   0        0        0    39553 2023-07-25 19:26:55.000000 bdbag-1.7.0/doc/cli.md
--rw-rw-rw-   0        0        0    30574 2023-02-02 23:26:13.000000 bdbag-1.7.0/doc/config.md
--rw-rw-rw-   0        0        0    10987 2022-01-11 18:46:35.000000 bdbag-1.7.0/doc/utils.md
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.138764 bdbag-1.7.0/examples/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.486484 bdbag-1.7.0/examples/bagofbags/
--rw-rw-rw-   0        0        0     1519 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/README.md
--rw-rw-rw-   0        0        0     7342 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/bagofbags.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.502105 bdbag-1.7.0/examples/bagofbags/images/
--rw-rw-rw-   0        0        0   127142 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/images/MetaBags.png
--rw-rw-rw-   0        0        0    48632 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/bagofbags/images/MetaBags.pptx
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.508616 bdbag-1.7.0/examples/metamanifests/
--rw-rw-rw-   0        0        0      840 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.138764 bdbag-1.7.0/examples/metamanifests/samples/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.524260 bdbag-1.7.0/examples/metamanifests/samples/sample1/
--rw-rw-rw-   0        0        0      236 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/samples/sample1/metadata.json
--rw-rw-rw-   0        0        0      741 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/samples/sample1/remote-files.json
--rw-rw-rw-   0        0        0     4729 2022-01-11 18:46:35.000000 bdbag-1.7.0/examples/metamanifests/samples/sample1/ro_metadata.json
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.539884 bdbag-1.7.0/profiles/
--rw-rw-rw-   0        0        0      940 2022-01-11 18:46:35.000000 bdbag-1.7.0/profiles/bdbag-profile.json
--rw-rw-rw-   0        0        0     1091 2022-01-11 18:46:35.000000 bdbag-1.7.0/profiles/bdbag-ro-profile.json
--rw-rw-rw-   0        0        0      539 2023-07-30 00:27:25.909708 bdbag-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     3216 2023-07-24 19:44:55.000000 bdbag-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.555509 bdbag-1.7.0/test/
--rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.170015 bdbag-1.7.0/test/test-data/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.555509 bdbag-1.7.0/test/test-data/test-archives/
--rw-rw-rw-   0        0        0     2355 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-fetch-http.zip
--rw-rw-rw-   0        0        0     2460 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.tgz
--rw-rw-rw-   0        0        0     5253 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.zip
--rw-rw-rw-   0        0        0     2369 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.tgz
--rw-rw-rw-   0        0        0     4596 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.zip
--rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.7z
--rw-rw-rw-   0        0        0     2319 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.bz2
--rw-rw-rw-   0        0        0    20480 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.tar
--rw-rw-rw-   0        0        0     2370 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.tgz
--rw-rw-rw-   0        0        0     5257 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-archives/test-bag.zip
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.571127 bdbag-1.7.0/test/test-data/test-bag/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/data/test2/test2.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.586753 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/
--rw-rw-rw-   0        0        0      351 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/bagit.txt
--rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/fetch.txt
--rw-rw-rw-   0        0        0      124 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-md5.txt
--rw-rw-rw-   0        0        0      140 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-sha1.txt
--rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-sha256.txt
--rw-rw-rw-   0        0        0      316 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/manifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.586753 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/metadata/
--rw-rw-rw-   0        0        0     1207 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/metadata/manifest.json
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      459 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      651 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1163 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.586753 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/data/README.txt
--rw-rw-rw-   0        0        0       53 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/data/README.txt
--rw-rw-rw-   0        0        0       44 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark-bad/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.608887 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/data/README.txt
--rw-rw-rw-   0        0        0       62 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ark2/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/data/README.txt
--rw-rw-rw-   0        0        0       90 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-dataguid/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.624522 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/data/README.txt
--rw-rw-rw-   0        0        0       59 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/fetch.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-doi/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.640148 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/
--rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/data/
--rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/data/1KB.zip
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/data/README.txt
--rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/fetch.txt
--rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/manifest-md5.txt
--rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/
--rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/data/
--rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/data/1KB.zip
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/data/README.txt
--rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/fetch.txt
--rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/manifest-md5.txt
--rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.655773 bdbag-1.7.0/test/test-data/test-bag-fetch-http/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.702648 bdbag-1.7.0/test/test-data/test-bag-fetch-http/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/data/README.txt
--rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.671413 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.671413 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/data/README.txt
--rw-rw-rw-   0        0        0      409 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/fetch.txt
--rw-rw-rw-   0        0        0      232 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/manifest-md5.txt
--rw-rw-rw-   0        0        0      360 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-bad/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.671413 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.687024 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/data/README.txt
--rw-rw-rw-   0        0        0      153 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/fetch.txt
--rw-rw-rw-   0        0        0      111 2022-01-11 18:46:35.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/manifest-md5.txt
--rw-rw-rw-   0        0        0      175 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.687024 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.687024 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/data/README.txt
--rw-rw-rw-   0        0        0      269 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.702648 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.702648 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/data/README.txt
--rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.709161 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.709161 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/data/README.txt
--rw-rw-rw-   0        0        0       48 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/fetch.txt
--rw-rw-rw-   0        0        0      115 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-minid/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.709161 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.724798 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/data/README.txt
--rw-rw-rw-   0        0        0      113 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/fetch.txt
--rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/manifest-md5.txt
--rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-fetch-tag/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.724798 bdbag-1.7.0/test/test-data/test-bag-incomplete/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/data/test2/test2.txt
--rw-rw-rw-   0        0        0      188 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/fetch.txt
--rw-rw-rw-   0        0        0      219 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-sha1.txt
--rw-rw-rw-   0        0        0      444 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/manifest-sha512.txt
--rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/
--rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.740424 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/data/README.txt
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      282 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/fetch.txt
--rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-incomplete-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.756049 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.756049 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/README.txt
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      284 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.756049 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.771674 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/README.txt
--rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-identifier.txt
--rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/fetch.txt
--rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.771674 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/
--rw-rw-rw-   0        0        0      320 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.771674 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/data/README.txt
--rw-rw-rw-   0        0        0       50 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      192 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-state-manifest-fetch/tagmanifest-md5.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.787298 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/data/test2/test2.txt
--rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/fetch.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/manifest-sha512.txt
--rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/data/test2/test2.txt
--rw-rw-rw-   0        0        0      105 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-md5.txt
--rw-rw-rw-   0        0        0      121 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha1.txt
--rw-rw-rw-   0        0        0      169 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha256.txt
--rw-rw-rw-   0        0        0      297 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.809435 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.825072 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/data/test1/test1.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.825072 bdbag-1.7.0/test/test-data/test-bag-no-data/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/bagit.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/
--rw-rw-rw-   0        0        0      294 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/data/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/data/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.840697 bdbag-1.7.0/test/test-data/test-bag-profile/data/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/data/test2/test2.txt
--rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/
--rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/data/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/data/README.txt
--rw-rw-rw-   0        0        0      135 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/fetch.txt
--rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bag-update-invalid-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bdbagit/
--rw-rw-rw-   0        0        0      221 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/README
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.856322 bdbag-1.7.0/test/test-data/test-bdbagit/loc/
--rw-rw-rw-   0        0        0   139367 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg
--rw-rw-rw-   0        0        0   143435 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.871947 bdbag-1.7.0/test/test-data/test-bdbagit/si/
--rw-rw-rw-   0        0        0   381813 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg
--rw-rw-rw-   0        0        0   326929 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-config/
--rw-rw-rw-   0        0        0      415 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/base-config.json
--rw-rw-rw-   0        0        0      806 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-10.json
--rw-rw-rw-   0        0        0      513 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-11.json
--rw-rw-rw-   0        0        0      576 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-12.json
--rw-rw-rw-   0        0        0      401 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-2.json
--rw-rw-rw-   0        0        0     2773 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-3.json
--rw-rw-rw-   0        0        0     1243 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-4.json
--rw-rw-rw-   0        0        0     1199 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-5.json
--rw-rw-rw-   0        0        0     1052 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-6.json
--rw-rw-rw-   0        0        0      825 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-7.json
--rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-8.json
--rw-rw-rw-   0        0        0      828 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config-9.json
--rw-rw-rw-   0        0        0      354 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-config.json
--rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-cookies-1.txt
--rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-cookies-2.txt
--rw-rw-rw-   0        0        0       83 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-cookies-bad.txt
--rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-2.json
--rw-rw-rw-   0        0        0     1574 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-encoding.json
--rw-rw-rw-   0        0        0      616 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json
--rw-rw-rw-   0        0        0      944 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest.json
--rw-rw-rw-   0        0        0      312 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-invalid-fetch-manifest-1.json
--rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-invalid-fetch-manifest-2.json
--rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-1.json
--rw-rw-rw-   0        0        0      233 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-2.json
--rw-rw-rw-   0        0        0      288 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-3.json
--rw-rw-rw-   0        0        0      212 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-4.json
--rw-rw-rw-   0        0        0      191 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-5.json
--rw-rw-rw-   0        0        0      278 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-6.json
--rw-rw-rw-   0        0        0      279 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-7.json
--rw-rw-rw-   0        0        0      704 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-8.json
--rw-rw-rw-   0        0        0      672 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-9.json
--rw-rw-rw-   0        0        0      146 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-keychain-bad-1.json
--rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-metadata.json
--rw-rw-rw-   0        0        0     1259 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-config/test-ro-metadata.json
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-dir/
--rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-dir/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-dir/test1/
--rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-dir/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-dir/test2/
--rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-dir/test2/test2.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-http/
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-http/test-fetch-http.txt
--rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-http/test-fetch-identifier.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 00:27:25.909708 bdbag-1.7.0/test/test-data/test-http-encoded/
--rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.0/test/test-data/test-http-encoded/test fetch%http®.txt
--rw-rw-rw-   0        0        0    51544 2023-07-21 22:52:04.000000 bdbag-1.7.0/test/test_api.py
--rw-rw-rw-   0        0        0    49471 2022-05-26 22:19:59.000000 bdbag-1.7.0/test/test_bdbagit.py
--rw-rw-rw-   0        0        0    13183 2023-07-24 18:49:12.000000 bdbag-1.7.0/test/test_cli.py
--rw-rw-rw-   0        0        0     8155 2022-05-27 21:25:14.000000 bdbag-1.7.0/test/test_common.py
--rw-rw-rw-   0        0        0    57435 2023-03-29 18:38:57.000000 bdbag-1.7.0/test/test_remote.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.811457 bdbag-1.7.1/
+-rw-rw-rw-   0        0        0       18 2022-01-11 18:46:35.000000 bdbag-1.7.1/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:07.946648 bdbag-1.7.1/.github/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.040421 bdbag-1.7.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1599 2023-07-21 21:19:21.000000 bdbag-1.7.1/.github/workflows/bdbag.yml
+-rw-rw-rw-   0        0        0      750 2022-05-27 21:39:45.000000 bdbag-1.7.1/.travis.yml
+-rw-rw-rw-   0        0        0    20147 2023-07-30 02:46:11.000000 bdbag-1.7.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11357 2022-01-11 18:46:35.000000 bdbag-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     7193 2023-07-30 02:54:08.811457 bdbag-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2022-05-26 23:02:23.000000 bdbag-1.7.1/Pipfile
+-rw-rw-rw-   0        0        0    36425 2023-07-21 21:50:32.000000 bdbag-1.7.1/Pipfile.lock
+-rw-rw-rw-   0        0        0     5771 2023-07-24 19:32:43.000000 bdbag-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.093839 bdbag-1.7.1/bdbag/
+-rw-rw-rw-   0        0        0     9919 2023-07-30 02:16:33.000000 bdbag-1.7.1/bdbag/__init__.py
+-rw-rw-rw-   0        0        0    26658 2023-07-24 18:23:35.000000 bdbag-1.7.1/bdbag/bdbag_api.py
+-rw-rw-rw-   0        0        0    20001 2023-07-25 16:48:58.000000 bdbag-1.7.1/bdbag/bdbag_cli.py
+-rw-rw-rw-   0        0        0     9801 2023-07-30 02:47:49.000000 bdbag-1.7.1/bdbag/bdbag_config.py
+-rw-rw-rw-   0        0        0    13883 2022-05-26 21:34:05.000000 bdbag-1.7.1/bdbag/bdbag_ro.py
+-rw-rw-rw-   0        0        0    27410 2022-05-26 21:34:05.000000 bdbag-1.7.1/bdbag/bdbag_utils.py
+-rw-rw-rw-   0        0        0    24599 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/bdbagit.py
+-rw-rw-rw-   0        0        0     2357 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/bdbagit_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.147232 bdbag-1.7.1/bdbag/fetch/
+-rw-rw-rw-   0        0        0     2233 2022-05-26 21:34:05.000000 bdbag-1.7.1/bdbag/fetch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.162871 bdbag-1.7.1/bdbag/fetch/auth/
+-rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/auth/__init__.py
+-rw-rw-rw-   0        0        0     3282 2022-05-26 21:34:05.000000 bdbag-1.7.1/bdbag/fetch/auth/cookies.py
+-rw-rw-rw-   0        0        0     6159 2022-05-26 21:34:05.000000 bdbag-1.7.1/bdbag/fetch/auth/keychain.py
+-rw-rw-rw-   0        0        0     4980 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.209752 bdbag-1.7.1/bdbag/fetch/resolvers/
+-rw-rw-rw-   0        0        0     2486 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/resolvers/__init__.py
+-rw-rw-rw-   0        0        0     2802 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/resolvers/ark_resolver.py
+-rw-rw-rw-   0        0        0     3142 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/resolvers/base_resolver.py
+-rw-rw-rw-   0        0        0     2271 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/resolvers/dataguid_resolver.py
+-rw-rw-rw-   0        0        0     2600 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/resolvers/doi_resolver.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.278778 bdbag-1.7.1/bdbag/fetch/transports/
+-rw-rw-rw-   0        0        0     2701 2022-11-15 21:11:09.000000 bdbag-1.7.1/bdbag/fetch/transports/__init__.py
+-rw-rw-rw-   0        0        0     1057 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/transports/base_transport.py
+-rw-rw-rw-   0        0        0     7061 2022-05-26 21:34:05.000000 bdbag-1.7.1/bdbag/fetch/transports/fetch_boto3.py
+-rw-rw-rw-   0        0        0     3348 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/transports/fetch_ftp.py
+-rw-rw-rw-   0        0        0     5193 2023-02-02 22:20:48.000000 bdbag-1.7.1/bdbag/fetch/transports/fetch_gcs.py
+-rw-rw-rw-   0        0        0     5133 2022-02-11 20:26:50.000000 bdbag-1.7.1/bdbag/fetch/transports/fetch_globus.py
+-rw-rw-rw-   0        0        0    12755 2023-07-19 21:57:14.000000 bdbag-1.7.1/bdbag/fetch/transports/fetch_http.py
+-rw-rw-rw-   0        0        0     1389 2022-01-11 18:46:35.000000 bdbag-1.7.1/bdbag/fetch/transports/fetch_tag.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.125094 bdbag-1.7.1/bdbag.egg-info/
+-rw-rw-rw-   0        0        0     7193 2023-07-30 02:54:07.000000 bdbag-1.7.1/bdbag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19233 2023-07-30 02:54:07.000000 bdbag-1.7.1/bdbag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 02:54:07.000000 bdbag-1.7.1/bdbag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-07-30 02:54:07.000000 bdbag-1.7.1/bdbag.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      247 2023-07-30 02:54:07.000000 bdbag-1.7.1/bdbag.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-30 02:54:07.000000 bdbag-1.7.1/bdbag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.325656 bdbag-1.7.1/doc/
+-rw-rw-rw-   0        0        0    38271 2023-02-02 23:26:13.000000 bdbag-1.7.1/doc/api.md
+-rw-rw-rw-   0        0        0    39553 2023-07-25 19:26:55.000000 bdbag-1.7.1/doc/cli.md
+-rw-rw-rw-   0        0        0    30574 2023-02-02 23:26:13.000000 bdbag-1.7.1/doc/config.md
+-rw-rw-rw-   0        0        0    10987 2022-01-11 18:46:35.000000 bdbag-1.7.1/doc/utils.md
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:07.962289 bdbag-1.7.1/examples/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.341274 bdbag-1.7.1/examples/bagofbags/
+-rw-rw-rw-   0        0        0     1519 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/bagofbags/README.md
+-rw-rw-rw-   0        0        0     7342 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/bagofbags/bagofbags.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.347789 bdbag-1.7.1/examples/bagofbags/images/
+-rw-rw-rw-   0        0        0   127142 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/bagofbags/images/MetaBags.png
+-rw-rw-rw-   0        0        0    48632 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/bagofbags/images/MetaBags.pptx
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.347789 bdbag-1.7.1/examples/metamanifests/
+-rw-rw-rw-   0        0        0      840 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/metamanifests/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:07.962289 bdbag-1.7.1/examples/metamanifests/samples/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.379058 bdbag-1.7.1/examples/metamanifests/samples/sample1/
+-rw-rw-rw-   0        0        0      236 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/metamanifests/samples/sample1/metadata.json
+-rw-rw-rw-   0        0        0      741 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/metamanifests/samples/sample1/remote-files.json
+-rw-rw-rw-   0        0        0     4729 2022-01-11 18:46:35.000000 bdbag-1.7.1/examples/metamanifests/samples/sample1/ro_metadata.json
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.379058 bdbag-1.7.1/profiles/
+-rw-rw-rw-   0        0        0      940 2022-01-11 18:46:35.000000 bdbag-1.7.1/profiles/bdbag-profile.json
+-rw-rw-rw-   0        0        0     1091 2022-01-11 18:46:35.000000 bdbag-1.7.1/profiles/bdbag-ro-profile.json
+-rw-rw-rw-   0        0        0      539 2023-07-30 02:54:08.811457 bdbag-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     3216 2023-07-24 19:44:55.000000 bdbag-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.448082 bdbag-1.7.1/test/
+-rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:07.993545 bdbag-1.7.1/test/test-data/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.448082 bdbag-1.7.1/test/test-data/test-archives/
+-rw-rw-rw-   0        0        0     2355 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag-fetch-http.zip
+-rw-rw-rw-   0        0        0     2460 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag-multi-parent.tgz
+-rw-rw-rw-   0        0        0     5253 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag-multi-parent.zip
+-rw-rw-rw-   0        0        0     2369 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag-no-parent.tgz
+-rw-rw-rw-   0        0        0     4596 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag-no-parent.zip
+-rw-rw-rw-   0        0        0        0 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag.7z
+-rw-rw-rw-   0        0        0     2319 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag.bz2
+-rw-rw-rw-   0        0        0    20480 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag.tar
+-rw-rw-rw-   0        0        0     2370 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag.tgz
+-rw-rw-rw-   0        0        0     5257 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-archives/test-bag.zip
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.463724 bdbag-1.7.1/test/test-data/test-bag/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bag/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bag/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bag/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.479354 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/
+-rw-rw-rw-   0        0        0      351 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/bagit.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/fetch.txt
+-rw-rw-rw-   0        0        0      124 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/manifest-md5.txt
+-rw-rw-rw-   0        0        0      140 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      316 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/manifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.479354 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/metadata/
+-rw-rw-rw-   0        0        0     1207 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/metadata/manifest.json
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      459 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      651 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1163 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.479354 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.510597 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/data/README.txt
+-rw-rw-rw-   0        0        0       53 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.494976 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.494976 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/data/README.txt
+-rw-rw-rw-   0        0        0       44 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark-bad/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.510597 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.510597 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/data/README.txt
+-rw-rw-rw-   0        0        0       62 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ark2/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.510597 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.510597 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/data/README.txt
+-rw-rw-rw-   0        0        0       90 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-dataguid/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.526229 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.526229 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/data/README.txt
+-rw-rw-rw-   0        0        0       59 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/fetch.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-doi/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.526229 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/
+-rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.548365 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/data/
+-rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/data/1KB.zip
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/data/README.txt
+-rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/fetch.txt
+-rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/manifest-md5.txt
+-rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.548365 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/
+-rw-rw-rw-   0        0        0      349 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.548365 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/data/
+-rw-rw-rw-   0        0        0     1024 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/data/1KB.zip
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/data/README.txt
+-rw-rw-rw-   0        0        0       52 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/fetch.txt
+-rw-rw-rw-   0        0        0       97 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/manifest-md5.txt
+-rw-rw-rw-   0        0        0      161 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.548365 bdbag-1.7.1/test/test-data/test-bag-fetch-http/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.595263 bdbag-1.7.1/test/test-data/test-bag-fetch-http/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/data/README.txt
+-rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.564006 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.564006 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/data/README.txt
+-rw-rw-rw-   0        0        0      409 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/fetch.txt
+-rw-rw-rw-   0        0        0      232 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/manifest-md5.txt
+-rw-rw-rw-   0        0        0      360 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-bad/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.564006 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.564006 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/data/README.txt
+-rw-rw-rw-   0        0        0      153 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/fetch.txt
+-rw-rw-rw-   0        0        0      111 2022-01-11 18:46:35.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/manifest-md5.txt
+-rw-rw-rw-   0        0        0      175 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.579635 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.579635 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/data/README.txt
+-rw-rw-rw-   0        0        0      269 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.595263 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.595263 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/data/README.txt
+-rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.595263 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.595263 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/data/README.txt
+-rw-rw-rw-   0        0        0       48 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/fetch.txt
+-rw-rw-rw-   0        0        0      115 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-minid/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.610884 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.610884 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/data/README.txt
+-rw-rw-rw-   0        0        0      113 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/fetch.txt
+-rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/manifest-md5.txt
+-rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-fetch-tag/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.626505 bdbag-1.7.1/test/test-data/test-bag-incomplete/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.642134 bdbag-1.7.1/test/test-data/test-bag-incomplete/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.642134 bdbag-1.7.1/test/test-data/test-bag-incomplete/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.642134 bdbag-1.7.1/test/test-data/test-bag-incomplete/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      188 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/fetch.txt
+-rw-rw-rw-   0        0        0      219 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      444 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.626505 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/
+-rw-rw-rw-   0        0        0      348 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.626505 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      282 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-incomplete-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.648648 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.648648 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      284 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.648648 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.664291 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/data/README.txt
+-rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-identifier.txt
+-rw-rw-rw-   0        0        0      280 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/fetch.txt
+-rw-rw-rw-   0        0        0      174 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.664291 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/
+-rw-rw-rw-   0        0        0      320 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.664291 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/data/README.txt
+-rw-rw-rw-   0        0        0       50 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      192 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-state-manifest-fetch/tagmanifest-md5.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.679916 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.679916 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.679916 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.679916 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      339 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      563 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1011 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.695541 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.695541 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.695541 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.695541 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      105 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/manifest-md5.txt
+-rw-rw-rw-   0        0        0      121 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      169 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      297 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.711166 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.711166 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.711166 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/data/test1/test1.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.726791 bdbag-1.7.1/test/test-data/test-bag-no-data/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/bagit.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-no-data/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.726791 bdbag-1.7.1/test/test-data/test-bag-profile/
+-rw-rw-rw-   0        0        0      294 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.742415 bdbag-1.7.1/test/test-data/test-bag-profile/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/data/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.742415 bdbag-1.7.1/test/test-data/test-bag-profile/data/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.742415 bdbag-1.7.1/test/test-data/test-bag-profile/data/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      160 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-profile/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/
+-rw-rw-rw-   0        0        0      321 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/data/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      135 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      109 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bag-update-invalid-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bdbagit/
+-rw-rw-rw-   0        0        0      221 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bdbagit/README
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bdbagit/loc/
+-rw-rw-rw-   0        0        0   139367 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg
+-rw-rw-rw-   0        0        0   143435 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.748932 bdbag-1.7.1/test/test-data/test-bdbagit/si/
+-rw-rw-rw-   0        0        0   381813 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg
+-rw-rw-rw-   0        0        0   326929 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.795829 bdbag-1.7.1/test/test-data/test-config/
+-rw-rw-rw-   0        0        0      415 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/base-config.json
+-rw-rw-rw-   0        0        0      806 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-10.json
+-rw-rw-rw-   0        0        0      513 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-11.json
+-rw-rw-rw-   0        0        0      576 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-12.json
+-rw-rw-rw-   0        0        0      401 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-2.json
+-rw-rw-rw-   0        0        0     2773 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-3.json
+-rw-rw-rw-   0        0        0     1243 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-4.json
+-rw-rw-rw-   0        0        0     1199 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-5.json
+-rw-rw-rw-   0        0        0     1052 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-6.json
+-rw-rw-rw-   0        0        0      825 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-7.json
+-rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-8.json
+-rw-rw-rw-   0        0        0      828 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config-9.json
+-rw-rw-rw-   0        0        0      354 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-config.json
+-rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-cookies-1.txt
+-rw-rw-rw-   0        0        0      244 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-cookies-2.txt
+-rw-rw-rw-   0        0        0       83 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-cookies-bad.txt
+-rw-rw-rw-   0        0        0      861 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest-2.json
+-rw-rw-rw-   0        0        0     1574 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest-encoding.json
+-rw-rw-rw-   0        0        0      616 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json
+-rw-rw-rw-   0        0        0      944 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest.json
+-rw-rw-rw-   0        0        0      312 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-invalid-fetch-manifest-1.json
+-rw-rw-rw-   0        0        0      187 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-invalid-fetch-manifest-2.json
+-rw-rw-rw-   0        0        0      199 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-1.json
+-rw-rw-rw-   0        0        0      233 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-2.json
+-rw-rw-rw-   0        0        0      288 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-3.json
+-rw-rw-rw-   0        0        0      212 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-4.json
+-rw-rw-rw-   0        0        0      191 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-5.json
+-rw-rw-rw-   0        0        0      278 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-6.json
+-rw-rw-rw-   0        0        0      279 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-7.json
+-rw-rw-rw-   0        0        0      704 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-8.json
+-rw-rw-rw-   0        0        0      672 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-9.json
+-rw-rw-rw-   0        0        0      146 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-keychain-bad-1.json
+-rw-rw-rw-   0        0        0      173 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-metadata.json
+-rw-rw-rw-   0        0        0     1259 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-config/test-ro-metadata.json
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.795829 bdbag-1.7.1/test/test-data/test-dir/
+-rw-rw-rw-   0        0        0       66 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-dir/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.795829 bdbag-1.7.1/test/test-data/test-dir/test1/
+-rw-rw-rw-   0        0        0       45 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-dir/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.795829 bdbag-1.7.1/test/test-data/test-dir/test2/
+-rw-rw-rw-   0        0        0       56 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-dir/test2/test2.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.795829 bdbag-1.7.1/test/test-data/test-http/
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-http/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      223 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-http/test-fetch-identifier.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:54:08.795829 bdbag-1.7.1/test/test-data/test-http-encoded/
+-rw-rw-rw-   0        0        0      201 2022-01-11 18:46:36.000000 bdbag-1.7.1/test/test-data/test-http-encoded/test fetch%http®.txt
+-rw-rw-rw-   0        0        0    51544 2023-07-21 22:52:04.000000 bdbag-1.7.1/test/test_api.py
+-rw-rw-rw-   0        0        0    49471 2022-05-26 22:19:59.000000 bdbag-1.7.1/test/test_bdbagit.py
+-rw-rw-rw-   0        0        0    13183 2023-07-24 18:49:12.000000 bdbag-1.7.1/test/test_cli.py
+-rw-rw-rw-   0        0        0     8155 2022-05-27 21:25:14.000000 bdbag-1.7.1/test/test_common.py
+-rw-rw-rw-   0        0        0    57435 2023-03-29 18:38:57.000000 bdbag-1.7.1/test/test_remote.py
```

### Comparing `bdbag-1.7.0/.github/workflows/bdbag.yml` & `bdbag-1.7.1/.github/workflows/bdbag.yml`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/.travis.yml` & `bdbag-1.7.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/CHANGELOG.md` & `bdbag-1.7.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # CHANGE LOG
 
+## 1.7.1
+Fix issue with `packaging.parse` throwing `InvalidVersion` in the `upgrade_config()` function when trying to parse the 
+informational version string `VERSION` set by `bdbag` when it is running in a "frozen" (e.g., with `cx_Freeze`) environment.
+In such cases, `VERSION` is set to something like `1.7.1-frozen`, which is not `PEP-440` compliant.
+This was not an issue in previous releases due to the fact that the implementation used `pkg_resources.parse_version` which was not as strict.
+
+The code in `upgrade_config()` has been changed to parse the `PEP-440` compliant version returned by `packaging.parse` 
+rather than use the global string `VERSION`, which can still be (and is) used elsewhere for purely informational and descriptive purposes. 
+
 ## 1.7.0
 * PR: [#54](https://github.com/fair-research/bdbag/pull/54): Add support for passing a local profile path for profile validation. Thanks to [Bernhard Hampel-Waffenthal](https://github.com/prettybits) for the contribution.
 * [#40](https://github.com/fair-research/bdbag/issues/40): Replace deprecated use of `pkg_resources` with `importlib-metadata` and `packaging`.
 * Fix issue with HTTP fetch transport where bearer-token auth gets stripped from the session on a legitimate redirect but not restored for any potential new request on that same URL-bound session.
 * Unpin `tzlocal` unless Python<3.
 * Support for Python 3.5 and 3.6 has been dropped. Python 3.7 compatibility is deprecated but still officially supported in this release.
```

### Comparing `bdbag-1.7.0/LICENSE` & `bdbag-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/PKG-INFO` & `bdbag-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdbag
-Version: 1.7.0
+Version: 1.7.1
 Summary: Big Data Bag Utilities
 Home-page: https://github.com/fair-research/bdbag/
 Author: Mike D'Arcy
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bdbag-1.7.0/Pipfile.lock` & `bdbag-1.7.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/README.md` & `bdbag-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/__init__.py` & `bdbag-1.7.1/bdbag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 import shutil
 from datetime import datetime
 from distutils.util import strtobool
 from importlib_metadata import distribution, PackageNotFoundError
 
 logger = logging.getLogger(__name__)
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 __bagit_version__ = "1.8.1"
 __bagit_profile_version__ = "1.3.1"
 
 if sys.version_info > (3,):  # pragma: no cover
     from urllib.parse import quote as urlquote, unquote as urlunquote, urlsplit, urlunsplit, urlparse
     from urllib.request import urlretrieve, urlopen, urlcleanup
 else:  # pragma: no cover
     from urllib import quote as urlquote, unquote as urlunquote, urlretrieve, urlopen, urlcleanup
     from urlparse import urlsplit, urlunsplit, urlparse
 
 try:
     version = distribution("bdbag").version
     VERSION = version + '' if not getattr(sys, 'frozen', False) else version + '-frozen'
 except PackageNotFoundError:  # pragma: no cover
-    VERSION = __version__ + '-dev' if not getattr(sys, 'frozen', False) else __version__ + '-frozen'
+    VERSION = __version__ + '.dev'
 PROJECT_URL = 'https://github.com/fair-research/bdbag'
 
 try:
     version = distribution("bagit").version
     BAGIT_VERSION = version + '' if not getattr(sys, 'frozen', False) else version + '-frozen'
 except PackageNotFoundError:  # pragma: no cover
     BAGIT_VERSION = 'unknown' if not getattr(sys, 'frozen', False) else __bagit_version__ + '-frozen'
```

### Comparing `bdbag-1.7.0/bdbag/bdbag_api.py` & `bdbag-1.7.1/bdbag/bdbag_api.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/bdbag_cli.py` & `bdbag-1.7.1/bdbag/bdbag_cli.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/bdbag_config.py` & `bdbag-1.7.1/bdbag/bdbag_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 #
 import os
 import errno
 import logging
 import json
 from collections import OrderedDict
 from packaging.version import parse as parse_version
+from importlib_metadata import distribution, PackageNotFoundError
 from bdbag import get_typed_exception, safe_move, \
-    DEFAULT_CONFIG_PATH, BAG_PROFILE_TAG, BDBAG_PROFILE_ID, VERSION
+    DEFAULT_CONFIG_PATH, BAG_PROFILE_TAG, BDBAG_PROFILE_ID, VERSION, __version__
 from bdbag.fetch import Megabyte
 from bdbag.fetch.auth.keychain import DEFAULT_KEYCHAIN_FILE, write_keychain
 
 logger = logging.getLogger(__name__)
 
 BAG_CONFIG_TAG = "bag_config"
 BAG_SPEC_VERSION_TAG = "bagit_spec_version"
@@ -128,15 +129,15 @@
             "handler": "bdbag.fetch.resolvers.dataguid_resolver.DataGUIDResolverHandler",
             ID_RESOLVER_TAG: ["n2t.net"]
         }
     ]
 }
 
 DEFAULT_CONFIG = {
-    CONFIG_VERSION_TAG: VERSION,
+    CONFIG_VERSION_TAG: __version__,
     BAG_CONFIG_TAG:
         {
             BAG_SPEC_VERSION_TAG: DEFAULT_BAG_SPEC_VERSION,
             BAG_ALGORITHMS_TAG: DEFAULT_BAG_ALGORITHMS,
             BAG_PROCESSES_TAG: 1,
             BAG_METADATA_TAG:
                 {
@@ -211,24 +212,28 @@
         return
 
     updated = False
     with open(config_file) as cf:
         config = json.loads(cf.read(), object_pairs_hook=OrderedDict)
 
     new_config = None
-    if parse_version(VERSION) > parse_version(config.get(CONFIG_VERSION_TAG, "0")):
+    try:
+        version = distribution("bdbag").version
+    except PackageNotFoundError:  # pragma: no cover
+        version = __version__
+    if parse_version(version) > parse_version(config.get(CONFIG_VERSION_TAG, "0")):
         new_config = DEFAULT_CONFIG.copy()
         config_items = [BAG_CONFIG_TAG, FETCH_CONFIG_TAG, RESOLVER_CONFIG_TAG, ID_RESOLVER_TAG]
         copy_config_items(config, new_config, config_items)
         updated = True
 
     if updated and new_config:
         safe_move(config_file)
         write_config(new_config, config_file)
-        print("Updated configuration file [%s] to current version format: %s" % (config_file, str(VERSION)))
+        print("Updated configuration file [%s] to current version format: %s" % (config_file, str(version)))
 
 
 def copy_config_items(old_config, new_config, key_names):
     for key_name in key_names:
         if key_name in get_deprecated_config_keys(old_config):
             continue
         item = old_config.get(key_name)
```

### Comparing `bdbag-1.7.0/bdbag/bdbag_ro.py` & `bdbag-1.7.1/bdbag/bdbag_ro.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/bdbag_utils.py` & `bdbag-1.7.1/bdbag/bdbag_utils.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/bdbagit.py` & `bdbag-1.7.1/bdbag/bdbagit.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/bdbagit_profile.py` & `bdbag-1.7.1/bdbag/bdbagit_profile.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/__init__.py` & `bdbag-1.7.1/bdbag/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/auth/cookies.py` & `bdbag-1.7.1/bdbag/fetch/auth/cookies.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/auth/keychain.py` & `bdbag-1.7.1/bdbag/fetch/auth/keychain.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/fetcher.py` & `bdbag-1.7.1/bdbag/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/resolvers/__init__.py` & `bdbag-1.7.1/bdbag/fetch/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/resolvers/ark_resolver.py` & `bdbag-1.7.1/bdbag/fetch/resolvers/ark_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/resolvers/base_resolver.py` & `bdbag-1.7.1/bdbag/fetch/resolvers/base_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/resolvers/dataguid_resolver.py` & `bdbag-1.7.1/bdbag/fetch/resolvers/dataguid_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/resolvers/doi_resolver.py` & `bdbag-1.7.1/bdbag/fetch/resolvers/doi_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/__init__.py` & `bdbag-1.7.1/bdbag/fetch/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/base_transport.py` & `bdbag-1.7.1/bdbag/fetch/transports/base_transport.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/fetch_boto3.py` & `bdbag-1.7.1/bdbag/fetch/transports/fetch_boto3.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/fetch_ftp.py` & `bdbag-1.7.1/bdbag/fetch/transports/fetch_ftp.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/fetch_gcs.py` & `bdbag-1.7.1/bdbag/fetch/transports/fetch_gcs.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/fetch_globus.py` & `bdbag-1.7.1/bdbag/fetch/transports/fetch_globus.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/fetch_http.py` & `bdbag-1.7.1/bdbag/fetch/transports/fetch_http.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag/fetch/transports/fetch_tag.py` & `bdbag-1.7.1/bdbag/fetch/transports/fetch_tag.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/bdbag.egg-info/PKG-INFO` & `bdbag-1.7.1/bdbag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdbag
-Version: 1.7.0
+Version: 1.7.1
 Summary: Big Data Bag Utilities
 Home-page: https://github.com/fair-research/bdbag/
 Author: Mike D'Arcy
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bdbag-1.7.0/bdbag.egg-info/SOURCES.txt` & `bdbag-1.7.1/bdbag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/doc/api.md` & `bdbag-1.7.1/doc/api.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/doc/cli.md` & `bdbag-1.7.1/doc/cli.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/doc/config.md` & `bdbag-1.7.1/doc/config.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/doc/utils.md` & `bdbag-1.7.1/doc/utils.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/bagofbags/README.md` & `bdbag-1.7.1/examples/bagofbags/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/bagofbags/bagofbags.py` & `bdbag-1.7.1/examples/bagofbags/bagofbags.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/bagofbags/images/MetaBags.png` & `bdbag-1.7.1/examples/bagofbags/images/MetaBags.png`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/bagofbags/images/MetaBags.pptx` & `bdbag-1.7.1/examples/bagofbags/images/MetaBags.pptx`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/metamanifests/README.md` & `bdbag-1.7.1/examples/metamanifests/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/metamanifests/samples/sample1/remote-files.json` & `bdbag-1.7.1/examples/metamanifests/samples/sample1/remote-files.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/examples/metamanifests/samples/sample1/ro_metadata.json` & `bdbag-1.7.1/examples/metamanifests/samples/sample1/ro_metadata.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/profiles/bdbag-profile.json` & `bdbag-1.7.1/profiles/bdbag-profile.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/profiles/bdbag-ro-profile.json` & `bdbag-1.7.1/profiles/bdbag-ro-profile.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/setup.cfg` & `bdbag-1.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/setup.py` & `bdbag-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag-fetch-http.zip` & `bdbag-1.7.1/test/test-data/test-archives/test-bag-fetch-http.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.tgz` & `bdbag-1.7.1/test/test-data/test-archives/test-bag-multi-parent.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag-multi-parent.zip` & `bdbag-1.7.1/test/test-data/test-archives/test-bag-multi-parent.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.tgz` & `bdbag-1.7.1/test/test-data/test-archives/test-bag-no-parent.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag-no-parent.zip` & `bdbag-1.7.1/test/test-data/test-archives/test-bag-no-parent.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag.bz2` & `bdbag-1.7.1/test/test-data/test-archives/test-bag.bz2`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag.tar` & `bdbag-1.7.1/test/test-data/test-archives/test-bag.tar`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag.tgz` & `bdbag-1.7.1/test/test-data/test-archives/test-bag.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-archives/test-bag.zip` & `bdbag-1.7.1/test/test-data/test-archives/test-bag.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-empty-dirs/metadata/manifest.json` & `bdbag-1.7.1/test/test-data/test-bag-empty-dirs/metadata/manifest.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt` & `bdbag-1.7.1/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt` & `bdbag-1.7.1/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt` & `bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-no-data/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-no-data/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bag-profile/tagmanifest-sha512.txt` & `bdbag-1.7.1/test/test-data/test-bag-profile/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg` & `bdbag-1.7.1/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg` & `bdbag-1.7.1/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg` & `bdbag-1.7.1/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg` & `bdbag-1.7.1/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-10.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-10.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-11.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-11.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-12.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-12.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-3.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-3.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-4.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-4.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-5.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-5.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-6.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-6.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-7.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-7.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-8.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-8.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-config-9.json` & `bdbag-1.7.1/test/test-data/test-config/test-config-9.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-2.json` & `bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest-2.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-encoding.json` & `bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest-encoding.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json` & `bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-fetch-manifest.json` & `bdbag-1.7.1/test/test-data/test-config/test-fetch-manifest.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-keychain-8.json` & `bdbag-1.7.1/test/test-data/test-config/test-keychain-8.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-keychain-9.json` & `bdbag-1.7.1/test/test-data/test-config/test-keychain-9.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test-data/test-config/test-ro-metadata.json` & `bdbag-1.7.1/test/test-data/test-config/test-ro-metadata.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test_api.py` & `bdbag-1.7.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test_bdbagit.py` & `bdbag-1.7.1/test/test_bdbagit.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test_cli.py` & `bdbag-1.7.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test_common.py` & `bdbag-1.7.1/test/test_common.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.0/test/test_remote.py` & `bdbag-1.7.1/test/test_remote.py`

 * *Files identical despite different names*

