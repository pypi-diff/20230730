# Comparing `tmp/pypiserver-1.5.1.zip` & `tmp/pypiserver-1.5.2.zip`

## zipinfo {}

```diff
@@ -1,91 +1,95 @@
-Zip file size: 197212 bytes, number of entries: 89
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/bin/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/contributor_docs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/docker/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/requirements/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/.github/
--rw-r--r--  2.0 unx    14964 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver_logo.png
--rw-r--r--  2.0 unx      533 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.project.sample
--rw-r--r--  2.0 unx     5579 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bootstrap.py
--rw-r--r--  2.0 unx     2159 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/LICENSE.txt
--rw-r--r--  2.0 unx      423 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.pydevproject.sample
--rw-r--r--  2.0 unx    36669 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/README.rst
--rw-r--r--  2.0 unx      570 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.gitignore
--rw-r--r--  2.0 unx      521 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pyproject.toml
--rw-r--r--  2.0 unx      140 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.dockerignore
--rw-r--r--  2.0 unx    46300 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/PKG-INFO
--rw-r--r--  2.0 unx      649 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tox.ini
--rw-r--r--  2.0 unx      726 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/buildout.cfg
--rw-r--r--  2.0 unx      585 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/setup.cfg
--rw-r--r--  2.0 unx     2626 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/setup.py
--rw-r--r--  2.0 unx    18842 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/CHANGES.rst
--rw-r--r--  2.0 unx      632 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/Makefile
--rw-r--r--  2.0 unx       34 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.coveragerc
--rw-r--r--  2.0 unx     6795 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/docker-compose.yml
--rw-r--r--  2.0 unx     2776 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/Dockerfile
--rw-r--r--  2.0 unx      449 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/AUTHORS.rst
--rw-r--r--  2.0 unx     3236 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/pkg_helpers.py
--rw-r--r--  2.0 unx     4426 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/cache.py
--rw-r--r--  2.0 unx    10305 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/backend.py
--rw-r--r--  2.0 unx    11022 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/_app.py
--rw-r--r--  2.0 unx     6985 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/__main__.py
--rw-r--r--  2.0 unx    34170 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/config.py
--rw-r--r--  2.0 unx     1591 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/plugin.py
--rw-r--r--  2.0 unx     8441 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/__init__.py
--rw-r--r--  2.0 unx      996 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/welcome.html
--rw-r--r--  2.0 unx     5040 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/manage.py
--rw-r--r--  2.0 unx   150757 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/bottle.py
--rw-r--r--  2.0 unx     2795 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver/core.py
--rwxr-xr-x  2.0 unx     1024 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/check_readme.sh
--rwxr-xr-x  2.0 unx     7067 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/bumpver.py
--rwxr-xr-x  2.0 unx     2939 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/update_changelog.sh
--rwxr-xr-x  2.0 unx      157 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/package.sh
--rwxr-xr-x  2.0 unx     2663 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/ci_helper.py
--rw-r--r--  2.0 unx     1130 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/README.rst
--rwxr-xr-x  2.0 unx       17 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/bin/.gitignore
--rw-r--r--  2.0 unx     1016 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/contributor_docs/README.md
--rw-r--r--  2.0 unx       44 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/contributor_docs/architecture_overview.md
--rw-r--r--  2.0 unx      402 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/docker/docker-requirements.txt
--rw-r--r--  2.0 unx      304 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/docker/gunicorn.conf.py
--rwxr-xr-x  2.0 unx     3803 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/docker/entrypoint.sh
--rw-r--r--  2.0 unx      519 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/docker/README.md
--rw-r--r--  2.0 unx    18852 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/docker/test_docker.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/mypkg/
--rw-r--r--  2.0 unx       40 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/htpasswd.a.a
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/mypkg/mypkg/
--rw-r--r--  2.0 unx       83 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/mypkg/setup.cfg
--rw-r--r--  2.0 unx      191 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/mypkg/setup.py
--rw-r--r--  2.0 unx      135 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/fixtures/mypkg/mypkg/__init__.py
--rw-r--r--  2.0 unx       11 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      115 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/entry_points.txt
--rw-r--r--  2.0 unx    46300 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     1549 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/zip-safe
--rw-r--r--  2.0 unx       42 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/pypiserver.egg-info/requires.txt
--rw-r--r--  2.0 unx      212 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/requirements/dev.pip
--rw-r--r--  2.0 unx      214 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/requirements/test.pip
--rw-r--r--  2.0 unx      183 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/requirements/exe.pip
--rw-r--r--  2.0 unx     8829 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_main.py
--rw-r--r--  2.0 unx      236 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/doubles.py
--rw-r--r--  2.0 unx    21214 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_app.py
--rw-r--r--  2.0 unx       35 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test-ignorelist
--rw-r--r--  2.0 unx      459 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_docs.py
--rw-r--r--  2.0 unx     2732 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_init.py
--rw-r--r--  2.0 unx    10304 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_server.py
--rw-r--r--  2.0 unx    25551 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_config.py
--rw-r--r--  2.0 unx     4177 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_pkg_helpers.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/__init__.py
--rw-r--r--  2.0 unx     1949 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_core.py
--rw-r--r--  2.0 unx     1077 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_backend.py
--rwxr-xr-x  2.0 unx     7491 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/test_manage.py
--rw-r--r--  2.0 unx       82 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/tests/sample_msg.html
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-18 14:21 pypiserver-1.5.1/.github/workflows/
--rw-r--r--  2.0 unx     6916 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.github/workflows/ci.yml
--rw-r--r--  2.0 unx     1532 b- defN 22-Oct-18 14:21 pypiserver-1.5.1/.github/workflows/rc.yml
-89 files, 563334 bytes uncompressed, 184136 bytes compressed:  67.3%
+Zip file size: 201367 bytes, number of entries: 93
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/docker/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/requirements/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/bin/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/tests/
+-rw-r--r--  2.0 unx      585 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/setup.cfg
+-rw-r--r--  2.0 unx    19896 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/CHANGES.rst
+-rw-r--r--  2.0 unx    42772 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/README.rst
+-rw-r--r--  2.0 unx    44254 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/PKG-INFO
+-rw-r--r--  2.0 unx     6795 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docker-compose.yml
+-rw-r--r--  2.0 unx      726 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/buildout.cfg
+-rw-r--r--  2.0 unx      570 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.gitignore
+-rw-r--r--  2.0 unx     2159 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/LICENSE.txt
+-rw-r--r--  2.0 unx     2776 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/Dockerfile
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/AUTHORS.rst
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.dockerignore
+-rw-r--r--  2.0 unx      533 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.project.sample
+-rw-r--r--  2.0 unx     5617 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bootstrap.py
+-rw-r--r--  2.0 unx     2780 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/setup.py
+-rw-r--r--  2.0 unx      521 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pyproject.toml
+-rw-r--r--  2.0 unx      663 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tox.ini
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.coveragerc
+-rw-r--r--  2.0 unx      632 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/Makefile
+-rw-r--r--  2.0 unx      423 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.pydevproject.sample
+-rw-r--r--  2.0 unx    44254 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1595 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/zip-safe
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      114 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/.github/workflows/
+-rw-r--r--  2.0 unx      321 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.github/dependabot.yml
+-rw-r--r--  2.0 unx     5920 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.github/workflows/ci.yml
+-rw-r--r--  2.0 unx     1532 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/.github/workflows/rc.yml
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docker/README.md
+-rwxr-xr-x  2.0 unx     3803 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docker/entrypoint.sh
+-rw-r--r--  2.0 unx    18852 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docker/test_docker.py
+-rw-r--r--  2.0 unx      304 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docker/gunicorn.conf.py
+-rw-r--r--  2.0 unx      402 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docker/docker-requirements.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/mypkg/
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/htpasswd.a.a
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/mypkg/mypkg/
+-rw-r--r--  2.0 unx       83 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/mypkg/setup.cfg
+-rw-r--r--  2.0 unx      191 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/mypkg/setup.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/fixtures/mypkg/mypkg/__init__.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/requirements/test-requirements.txt
+-rw-r--r--  2.0 unx      212 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/requirements/dev.pip
+-rw-r--r--  2.0 unx       96 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/requirements/test.pip
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/requirements/exe.pip
+-rw-r--r--  2.0 unx     5040 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/manage.py
+-rw-r--r--  2.0 unx     2795 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/core.py
+-rw-r--r--  2.0 unx    10968 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/_app.py
+-rw-r--r--  2.0 unx     1591 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/plugin.py
+-rw-r--r--  2.0 unx     3236 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/pkg_helpers.py
+-rw-r--r--  2.0 unx    35263 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/config.py
+-rw-r--r--  2.0 unx   150757 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/bottle.py
+-rw-r--r--  2.0 unx     8969 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/__init__.py
+-rw-r--r--  2.0 unx    10305 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/backend.py
+-rw-r--r--  2.0 unx     7044 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/__main__.py
+-rw-r--r--  2.0 unx      996 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/welcome.html
+-rw-r--r--  2.0 unx     4425 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/pypiserver/cache.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/docs/__resources__/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 21:33 pypiserver-1.5.2/docs/contents/
+-rw-r--r--  2.0 unx     1421 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docs/README.md
+-rw-r--r--  2.0 unx    14964 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docs/__resources__/pypiserver_logo.png
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/docs/contents/.gitkeep
+-rw-r--r--  2.0 unx     1130 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/README.rst
+-rwxr-xr-x  2.0 unx       17 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/.gitignore
+-rwxr-xr-x  2.0 unx     7067 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/bumpver.py
+-rwxr-xr-x  2.0 unx      157 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/package.sh
+-rwxr-xr-x  2.0 unx     1024 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/check_readme.sh
+-rwxr-xr-x  2.0 unx     2663 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/ci_helper.py
+-rwxr-xr-x  2.0 unx     2939 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/bin/update_changelog.sh
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_core.py
+-rwxr-xr-x  2.0 unx     7491 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_manage.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/sample_msg.html
+-rw-r--r--  2.0 unx      236 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/doubles.py
+-rw-r--r--  2.0 unx     3353 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_init.py
+-rw-r--r--  2.0 unx    26376 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_config.py
+-rw-r--r--  2.0 unx     1077 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_backend.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_pkg_helpers.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_docs.py
+-rw-r--r--  2.0 unx    21719 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_app.py
+-rw-r--r--  2.0 unx       35 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test-ignorelist
+-rw-r--r--  2.0 unx     9379 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_main.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/__init__.py
+-rw-r--r--  2.0 unx    10304 b- defN 23-Jul-30 21:33 pypiserver-1.5.2/tests/test_server.py
+93 files, 570493 bytes uncompressed, 187721 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,268 +1,280 @@
-Filename: pypiserver-1.5.1/
+Filename: pypiserver-1.5.2/
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/
+Filename: pypiserver-1.5.2/pypiserver.egg-info/
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/
+Filename: pypiserver-1.5.2/.github/
 Comment: 
 
-Filename: pypiserver-1.5.1/contributor_docs/
+Filename: pypiserver-1.5.2/docker/
 Comment: 
 
-Filename: pypiserver-1.5.1/docker/
+Filename: pypiserver-1.5.2/fixtures/
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/
+Filename: pypiserver-1.5.2/requirements/
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/
+Filename: pypiserver-1.5.2/pypiserver/
 Comment: 
 
-Filename: pypiserver-1.5.1/requirements/
+Filename: pypiserver-1.5.2/docs/
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/
+Filename: pypiserver-1.5.2/bin/
 Comment: 
 
-Filename: pypiserver-1.5.1/.github/
+Filename: pypiserver-1.5.2/tests/
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver_logo.png
+Filename: pypiserver-1.5.2/setup.cfg
 Comment: 
 
-Filename: pypiserver-1.5.1/.project.sample
+Filename: pypiserver-1.5.2/CHANGES.rst
 Comment: 
 
-Filename: pypiserver-1.5.1/bootstrap.py
+Filename: pypiserver-1.5.2/README.rst
 Comment: 
 
-Filename: pypiserver-1.5.1/LICENSE.txt
+Filename: pypiserver-1.5.2/PKG-INFO
 Comment: 
 
-Filename: pypiserver-1.5.1/.pydevproject.sample
+Filename: pypiserver-1.5.2/docker-compose.yml
 Comment: 
 
-Filename: pypiserver-1.5.1/README.rst
+Filename: pypiserver-1.5.2/buildout.cfg
 Comment: 
 
-Filename: pypiserver-1.5.1/.gitignore
+Filename: pypiserver-1.5.2/.gitignore
 Comment: 
 
-Filename: pypiserver-1.5.1/pyproject.toml
+Filename: pypiserver-1.5.2/LICENSE.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/.dockerignore
+Filename: pypiserver-1.5.2/Dockerfile
 Comment: 
 
-Filename: pypiserver-1.5.1/PKG-INFO
+Filename: pypiserver-1.5.2/AUTHORS.rst
 Comment: 
 
-Filename: pypiserver-1.5.1/tox.ini
+Filename: pypiserver-1.5.2/.dockerignore
 Comment: 
 
-Filename: pypiserver-1.5.1/buildout.cfg
+Filename: pypiserver-1.5.2/.project.sample
 Comment: 
 
-Filename: pypiserver-1.5.1/setup.cfg
+Filename: pypiserver-1.5.2/bootstrap.py
 Comment: 
 
-Filename: pypiserver-1.5.1/setup.py
+Filename: pypiserver-1.5.2/setup.py
 Comment: 
 
-Filename: pypiserver-1.5.1/CHANGES.rst
+Filename: pypiserver-1.5.2/pyproject.toml
 Comment: 
 
-Filename: pypiserver-1.5.1/Makefile
+Filename: pypiserver-1.5.2/tox.ini
 Comment: 
 
-Filename: pypiserver-1.5.1/.coveragerc
+Filename: pypiserver-1.5.2/.coveragerc
 Comment: 
 
-Filename: pypiserver-1.5.1/docker-compose.yml
+Filename: pypiserver-1.5.2/Makefile
 Comment: 
 
-Filename: pypiserver-1.5.1/Dockerfile
+Filename: pypiserver-1.5.2/.pydevproject.sample
 Comment: 
 
-Filename: pypiserver-1.5.1/AUTHORS.rst
+Filename: pypiserver-1.5.2/pypiserver.egg-info/PKG-INFO
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/pkg_helpers.py
+Filename: pypiserver-1.5.2/pypiserver.egg-info/top_level.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/cache.py
+Filename: pypiserver-1.5.2/pypiserver.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/backend.py
+Filename: pypiserver-1.5.2/pypiserver.egg-info/zip-safe
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/_app.py
+Filename: pypiserver-1.5.2/pypiserver.egg-info/requires.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/__main__.py
+Filename: pypiserver-1.5.2/pypiserver.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/config.py
+Filename: pypiserver-1.5.2/pypiserver.egg-info/entry_points.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/plugin.py
+Filename: pypiserver-1.5.2/.github/workflows/
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/__init__.py
+Filename: pypiserver-1.5.2/.github/dependabot.yml
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/welcome.html
+Filename: pypiserver-1.5.2/.github/workflows/ci.yml
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/manage.py
+Filename: pypiserver-1.5.2/.github/workflows/rc.yml
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/bottle.py
+Filename: pypiserver-1.5.2/docker/README.md
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver/core.py
+Filename: pypiserver-1.5.2/docker/entrypoint.sh
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/check_readme.sh
+Filename: pypiserver-1.5.2/docker/test_docker.py
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/bumpver.py
+Filename: pypiserver-1.5.2/docker/gunicorn.conf.py
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/update_changelog.sh
+Filename: pypiserver-1.5.2/docker/docker-requirements.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/package.sh
+Filename: pypiserver-1.5.2/fixtures/mypkg/
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/ci_helper.py
+Filename: pypiserver-1.5.2/fixtures/htpasswd.a.a
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/README.rst
+Filename: pypiserver-1.5.2/fixtures/mypkg/mypkg/
 Comment: 
 
-Filename: pypiserver-1.5.1/bin/.gitignore
+Filename: pypiserver-1.5.2/fixtures/mypkg/setup.cfg
 Comment: 
 
-Filename: pypiserver-1.5.1/contributor_docs/README.md
+Filename: pypiserver-1.5.2/fixtures/mypkg/setup.py
 Comment: 
 
-Filename: pypiserver-1.5.1/contributor_docs/architecture_overview.md
+Filename: pypiserver-1.5.2/fixtures/mypkg/mypkg/__init__.py
 Comment: 
 
-Filename: pypiserver-1.5.1/docker/docker-requirements.txt
+Filename: pypiserver-1.5.2/requirements/test-requirements.txt
 Comment: 
 
-Filename: pypiserver-1.5.1/docker/gunicorn.conf.py
+Filename: pypiserver-1.5.2/requirements/dev.pip
 Comment: 
 
-Filename: pypiserver-1.5.1/docker/entrypoint.sh
+Filename: pypiserver-1.5.2/requirements/test.pip
 Comment: 
 
-Filename: pypiserver-1.5.1/docker/README.md
+Filename: pypiserver-1.5.2/requirements/exe.pip
 Comment: 
 
-Filename: pypiserver-1.5.1/docker/test_docker.py
+Filename: pypiserver-1.5.2/pypiserver/manage.py
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/mypkg/
+Filename: pypiserver-1.5.2/pypiserver/core.py
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/htpasswd.a.a
+Filename: pypiserver-1.5.2/pypiserver/_app.py
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/mypkg/mypkg/
+Filename: pypiserver-1.5.2/pypiserver/plugin.py
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/mypkg/setup.cfg
+Filename: pypiserver-1.5.2/pypiserver/pkg_helpers.py
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/mypkg/setup.py
+Filename: pypiserver-1.5.2/pypiserver/config.py
 Comment: 
 
-Filename: pypiserver-1.5.1/fixtures/mypkg/mypkg/__init__.py
+Filename: pypiserver-1.5.2/pypiserver/bottle.py
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/top_level.txt
+Filename: pypiserver-1.5.2/pypiserver/__init__.py
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/dependency_links.txt
+Filename: pypiserver-1.5.2/pypiserver/backend.py
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/entry_points.txt
+Filename: pypiserver-1.5.2/pypiserver/__main__.py
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/PKG-INFO
+Filename: pypiserver-1.5.2/pypiserver/welcome.html
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/SOURCES.txt
+Filename: pypiserver-1.5.2/pypiserver/cache.py
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/zip-safe
+Filename: pypiserver-1.5.2/docs/__resources__/
 Comment: 
 
-Filename: pypiserver-1.5.1/pypiserver.egg-info/requires.txt
+Filename: pypiserver-1.5.2/docs/contents/
 Comment: 
 
-Filename: pypiserver-1.5.1/requirements/dev.pip
+Filename: pypiserver-1.5.2/docs/README.md
 Comment: 
 
-Filename: pypiserver-1.5.1/requirements/test.pip
+Filename: pypiserver-1.5.2/docs/__resources__/pypiserver_logo.png
 Comment: 
 
-Filename: pypiserver-1.5.1/requirements/exe.pip
+Filename: pypiserver-1.5.2/docs/contents/.gitkeep
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_main.py
+Filename: pypiserver-1.5.2/bin/README.rst
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/doubles.py
+Filename: pypiserver-1.5.2/bin/.gitignore
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_app.py
+Filename: pypiserver-1.5.2/bin/bumpver.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test-ignorelist
+Filename: pypiserver-1.5.2/bin/package.sh
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_docs.py
+Filename: pypiserver-1.5.2/bin/check_readme.sh
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_init.py
+Filename: pypiserver-1.5.2/bin/ci_helper.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_server.py
+Filename: pypiserver-1.5.2/bin/update_changelog.sh
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_config.py
+Filename: pypiserver-1.5.2/tests/test_core.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_pkg_helpers.py
+Filename: pypiserver-1.5.2/tests/test_manage.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/__init__.py
+Filename: pypiserver-1.5.2/tests/sample_msg.html
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_core.py
+Filename: pypiserver-1.5.2/tests/doubles.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_backend.py
+Filename: pypiserver-1.5.2/tests/test_init.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/test_manage.py
+Filename: pypiserver-1.5.2/tests/test_config.py
 Comment: 
 
-Filename: pypiserver-1.5.1/tests/sample_msg.html
+Filename: pypiserver-1.5.2/tests/test_backend.py
 Comment: 
 
-Filename: pypiserver-1.5.1/.github/workflows/
+Filename: pypiserver-1.5.2/tests/test_pkg_helpers.py
 Comment: 
 
-Filename: pypiserver-1.5.1/.github/workflows/ci.yml
+Filename: pypiserver-1.5.2/tests/test_docs.py
 Comment: 
 
-Filename: pypiserver-1.5.1/.github/workflows/rc.yml
+Filename: pypiserver-1.5.2/tests/test_app.py
+Comment: 
+
+Filename: pypiserver-1.5.2/tests/test-ignorelist
+Comment: 
+
+Filename: pypiserver-1.5.2/tests/test_main.py
+Comment: 
+
+Filename: pypiserver-1.5.2/tests/__init__.py
+Comment: 
+
+Filename: pypiserver-1.5.2/tests/test_server.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pypiserver-1.5.1/pypiserver_logo.png` & `pypiserver-1.5.2/docs/__resources__/pypiserver_logo.png`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/.project.sample` & `pypiserver-1.5.2/.project.sample`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/bootstrap.py` & `pypiserver-1.5.2/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         from urllib2 import urlopen
 
     exec(urlopen("http://python-distribute.org/distribute_setup.py").read(), ez)
     setup_args = dict(to_dir=tmpeggs, download_delay=0, no_fake=True)
     ez["use_setuptools"](**setup_args)
 
     if to_reload:
+        from importlib import reload
+
         reload(pkg_resources)
     import pkg_resources
 
     # This does not (always?) update the default working set.  We will
     # do it.
     for path in sys.path:
         if path not in pkg_resources.working_set.entries:
```

## Comparing `pypiserver-1.5.1/LICENSE.txt` & `pypiserver-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/README.rst` & `pypiserver-1.5.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .. -*- mode: rst; coding: utf-8 -*-
 
-.. image:: pypiserver_logo.png
+.. image:: docs/__resources__/pypiserver_logo.png
    :width: 300 px
    :align: center
 
 ==============================================================================
 pypiserver - minimal PyPI server for use with pip/easy_install
 ==============================================================================
 |pypi-ver| |test-status| |dependencies| |python-ver| |proj-license|
 
-:Version:     1.5.1
-:Date:        2022-10-18
+:Version:     1.5.2
+:Date:        2023-07-30
 :Source:      https://github.com/pypiserver/pypiserver
 :PyPI:        https://pypi.org/project/pypiserver/
 :Tests:       https://github.com/pypiserver/pypiserver/actions
 :Maintainers: | Kostis Anagnostopoulos <ankostis@gmail.com>,
               | Matthew Planchard <mplanchard@gmail.com>,
               | Dmitrii Orlov <dmtree.dev@yahoo.com>,
               | **Someone new?** We are looking for new maintainers! 
@@ -69,15 +69,15 @@
     mkdir ~/packages                      # Copy packages into this directory.
 
    See also `Alternative Installation methods`_.
 
 2. Copy some packages into your ``~/packages`` folder and then
    get your ``pypiserver`` up and running::
 
-    pypi-server -p 8080 ~/packages &      # Will listen to all IPs.
+    pypi-server run -p 8080 ~/packages &      # Will listen to all IPs.
 
 3. From the client computer, type this::
 
     # Download and install hosted packages.
     pip install --extra-index-url http://localhost:8080/simple/ ...
 
     # or
@@ -88,132 +88,153 @@
 
     # Note that pip search does not currently work with the /simple/ endpoint.
 
    See also `Client-side configurations`_ for avoiding tedious typing.
 
 4. Enter ``pypi-server -h`` in the cmd-line to print a detailed usage message::
 
-    pypi-server [OPTIONS] [PACKAGES_DIRECTORY...]
-      start PyPI compatible package server serving packages from
-      PACKAGES_DIRECTORY. If PACKAGES_DIRECTORY is not given on the
-      command line, it uses the default ~/packages. pypiserver scans this
-      directory recursively for packages. It skips packages and
-      directories starting with a dot. Multiple package directories can be
-      specified.
-
-    pypi-server understands the following options:
-
-      -p, --port PORT
-        Listen on port PORT (default: 8080).
-
-      -i, --interface INTERFACE
-        Listen on interface INTERFACE (default: 0.0.0.0, any interface).
-
-      -a, --authenticate (update|download|list), ...
-        Comma-separated list of (case-insensitive) actions to authenticate.
-        Requires to have set the password (-P option).
-        To password-protect package downloads (in addition to uploads) while
-        leaving listings public, use:
-          -P foo/htpasswd.txt -a update,download
-        To allow unauthorized access, use:
-          -P . -a .
-        Note that when uploads are not protected, the `register` command
-        is not necessary, but `~/.pypirc` still need username and password fields,
-        even if bogus.
-        By default, only 'update' is password-protected.
-
-      -P, --passwords PASSWORD_FILE
-        Use apache htpasswd file PASSWORD_FILE to set usernames & passwords when
-        authenticating certain actions (see -a option).
-        To allow unauthorized access, use:
-          -P . -a .
-
-      --disable-fallback
-        Disable redirect to real PyPI index for packages not found in the
-        local index.
-
-      --fallback-url FALLBACK_URL
-        For packages not found in the local index, this URL will be used to
-        redirect to (default: https://pypi.org/simple/).
-
-      --server METHOD
-        Use METHOD to run the server. Valid values include paste,
-        cherrypy, twisted, gunicorn, gevent, wsgiref, auto. The
-        default is to use "auto" which chooses one of paste, cherrypy,
-        twisted or wsgiref.
-
-      -r, --root PACKAGES_DIRECTORY
-        [deprecated] Serve packages from PACKAGES_DIRECTORY.
-
-      -o, --overwrite
-        Allow overwriting existing package files.
-
-      --hash-algo ALGO
-        Any `hashlib` available algo used as fragments on package links.
-        Set one of (0, no, off, false) to disabled it (default: md5).
-
-      --welcome HTML_FILE
-        Uses the ASCII contents of HTML_FILE as welcome message response.
-
-      -v
-        Enable verbose logging; repeat for more verbosity.
-
-      --log-conf <FILE>
-        Read logging configuration from FILE.
-        By default, configuration is read from `log.conf` if found in server's dir.
-
-      --log-file <FILE>
-        Write logging info into this FILE.
-
-      --log-frmt <FILE>
-        The logging format-string (see `logging.LogRecord` class from standard python library).
-        [Default: %(asctime)s|%(name)s|%(levelname)s|%(thread)d|%(message)s]
-
-      --log-req-frmt FORMAT
-        A format-string selecting Http-Request properties to log; set to '%s' to see them all.
-        [Default: %(bottle.request)s]
-
-      --log-res-frmt FORMAT
-        A format-string selecting Http-Response properties to log; set to  '%s' to see them all.
-        [Default: %(status)s]
-
-      --log-err-frmt FORMAT
-        A format-string selecting Http-Error properties to log; set to  '%s' to see them all.
-        [Default: %(body)s: %(exception)s \n%(traceback)s]
-
-      --cache-control AGE
-        Add "Cache-Control: max-age=AGE, public" header to package downloads.
-        Pip 6+ needs this for caching.
-
-    pypi-server -h, --help
-      Show this help message.
-
-    pypi-server --version
-      Show pypi-server's version.
-
-    pypi-server -U [OPTIONS] [PACKAGES_DIRECTORY...]
-      Update packages in PACKAGES_DIRECTORY. This command searches
-      pypi.org for updates and shows a pip command line which
-      updates the package.
-
-    The following additional options can be specified with -U:
-
-      -x
-        Execute the pip commands instead of only showing them.
-
-      -d DOWNLOAD_DIRECTORY
-        Download package updates to this directory. The default is to use
-        the directory which contains the latest version of the package to
-        be updated.
-
-      -u
-        Allow updating to unstable version (alpha, beta, rc, dev versions).
-
-    Visit https://github.com/pypiserver/pypiserver for more information.
+    start PyPI compatible package server serving packages from PACKAGES_DIRECTORY. If PACKAGES_DIRECTORY is not given on the command line, it uses the default ~/packages. pypiserver scans this directory recursively for packages. It skips packages and directories starting with a dot. Multiple package directories may be specified.
 
+    positional arguments:
+      {run,update}
+        run                 Run pypiserver, serving packages from
+                            PACKAGES_DIRECTORY
+        update              Handle updates of packages managed by pypiserver. By
+                            default, a pip command to update the packages is
+                            printed to stdout for introspection or pipelining. See
+                            the `-x` option for updating packages directly.
+
+    options:
+      -h, --help            show this help message and exit
+      -v, --verbose         Enable verbose logging; repeat for more verbosity.
+      --log-file FILE       Write logging info into this FILE, as well as to
+                            stdout or stderr, if configured.
+      --log-stream STREAM   Log messages to the specified STREAM. Valid values are
+                            stdout, stderr, and none
+      --log-frmt FORMAT     The logging format-string.  (see `logging.LogRecord`
+                            class from standard python library)
+      --hash-algo HASH_ALGO
+                            Any `hashlib` available algorithm to use for
+                            generating fragments on package links. Can be disabled
+                            with one of (0, no, off, false).
+      --backend {auto,simple-dir,cached-dir}
+                            A backend implementation. Keep the default 'auto' to
+                            automatically determine whether to activate caching or
+                            not
+      --version             show program's version number and exit
+
+    Visit https://github.com/pypiserver/pypiserver for more information
+
+More details about ``pypi-server run``
+--------------------------------------
+
+Enter ``pypi-server run -h`` in the cmd-line to print a detailed usage
+message *about starting the server*::
+
+  usage: pypi-server run [-h] [-v] [--log-file FILE] [--log-stream STREAM] [--log-frmt FORMAT] [--hash-algo HASH_ALGO]
+                       [--backend {auto,simple-dir,cached-dir}] [--version] [-p PORT] [-i HOST] [-a AUTHENTICATE] [-P PASSWORD_FILE] [--disable-fallback]
+                       [--fallback-url FALLBACK_URL] [--health-endpoint HEALTH_ENDPOINT] [--server METHOD] [-o] [--welcome HTML_FILE]
+                       [--cache-control AGE] [--log-req-frmt FORMAT] [--log-res-frmt FORMAT] [--log-err-frmt FORMAT]
+                       [package_directory [package_directory ...]]
+
+  positional arguments:
+    package_directory     The directory from which to serve packages.
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -v, --verbose         Enable verbose logging; repeat for more verbosity.
+    --log-file FILE       Write logging info into this FILE, as well as to stdout or stderr, if configured.
+    --log-stream STREAM   Log messages to the specified STREAM. Valid values are stdout, stderr, and none
+    --log-frmt FORMAT     The logging format-string.  (see `logging.LogRecord` class from standard python library)
+    --hash-algo HASH_ALGO
+                          Any `hashlib` available algorithm to use for generating fragments on package links. Can be disabled with one of (0, no, off,
+                          false).
+    --backend {auto,simple-dir,cached-dir}
+                          A backend implementation. Keep the default 'auto' to automatically determine whether to activate caching or not
+    --version             show program's version number and exit
+    -p PORT, --port PORT  Listen on port PORT (default: 8080)
+    -i HOST, -H HOST, --interface HOST, --host HOST
+                          Listen on interface INTERFACE (default: 0.0.0.0)
+    -a AUTHENTICATE, --authenticate AUTHENTICATE
+                          Comma-separated list of (case-insensitive) actions to authenticate (options: download, list, update; default: update).
+                          
+                          Any actions not specified are not authenticated, so to authenticate downloads and updates, but allow unauthenticated viewing of
+                          the package list, you would use:
+                          
+                            pypi-server -a 'download, update' -P ./my_passwords.htaccess
+                          
+                          To disable authentication, use:
+                          
+                            pypi-server -a . -P .
+                          
+                          See the `-P` option for configuring users and passwords.
+                          
+                          Note that when uploads are not protected, the `register` command is not necessary, but `~/.pypirc` still needs username and
+                          password fields, even if bogus.
+    -P PASSWORD_FILE, --passwords PASSWORD_FILE
+                          Use an apache htpasswd file PASSWORD_FILE to set usernames and passwords for authentication.
+                          
+                          To allow unauthorized access, use:
+                          
+                            pypi-server -a . -P .
+                          
+    --disable-fallback    Disable the default redirect to PyPI for packages not found in the local index.
+    --fallback-url FALLBACK_URL
+                          Redirect to FALLBACK_URL for packages not found in the local index.
+    --health-endpoint HEALTH_ENDPOINT
+                          Configure a custom liveness endpoint.
+                          It always returns 200 Ok if the service is up.
+                          Otherwise, it means that the service is not responsive.
+    --server METHOD       Use METHOD to run the server. Valid values include paste, cherrypy, twisted, gunicorn, gevent, wsgiref, and auto. The default is to
+                          use "auto", which chooses one of paste, cherrypy, twisted, or wsgiref.
+    -o, --overwrite       Allow overwriting existing package files during upload.
+    --welcome HTML_FILE   Use the contents of HTML_FILE as a custom welcome message on the home page.
+    --cache-control AGE   Add "Cache-Control: max-age=AGE" header to package downloads. Pip 6+ requires this for caching. AGE is specified in seconds.
+    --log-req-frmt FORMAT
+                          A format-string selecting Http-Request properties to log; set to '%s' to see them all.
+    --log-res-frmt FORMAT
+                          A format-string selecting Http-Response properties to log; set to '%s' to see them all.
+    --log-err-frmt FORMAT
+                          A format-string selecting Http-Error properties to log; set to '%s' to see them all.
+
+More details about ``pypi-server update``
+-----------------------------------------
+
+Enter ``pypi-server update -h`` in the cmd-line to print a detailed usage
+message *about updating the managed packages*::
+
+  usage: pypi-server update [-h] [-v] [--log-file FILE] [--log-stream STREAM] [--log-frmt FORMAT] [--hash-algo HASH_ALGO]
+                            [--backend {auto,simple-dir,cached-dir}] [--version] [-x] [-d DOWNLOAD_DIRECTORY] [-u] [--blacklist-file IGNORELIST_FILE]
+                            [package_directory [package_directory ...]]
+
+  positional arguments:
+    package_directory     The directory from which to serve packages.
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -v, --verbose         Enable verbose logging; repeat for more verbosity.
+    --log-file FILE       Write logging info into this FILE, as well as to stdout or stderr, if configured.
+    --log-stream STREAM   Log messages to the specified STREAM. Valid values are stdout, stderr, and none
+    --log-frmt FORMAT     The logging format-string. (see `logging.LogRecord` class from standard python library)
+    --hash-algo HASH_ALGO
+                          Any `hashlib` available algorithm to use for generating fragments on package links. Can be disabled with one of (0, no, off,
+                          false).
+    --backend {auto,simple-dir,cached-dir}
+                          A backend implementation. Keep the default 'auto' to automatically determine whether to activate caching or not
+    --version             show program's version number and exit
+    -x, --execute         Execute the pip commands rather than printing to stdout
+    -d DOWNLOAD_DIRECTORY, --download-directory DOWNLOAD_DIRECTORY
+                          Specify a directory where packages updates will be downloaded. The default behavior is to use the directory which contains the
+                          package being updated.
+    -u, --allow-unstable  Allow updating to unstable versions (alpha, beta, rc, dev, etc.)
+    --blacklist-file IGNORELIST_FILE, --ignorelist-file IGNORELIST_FILE
+                          Don't update packages listed in this file (one package name per line, without versions, '#' comments honored). This can be useful
+                          if you upload private packages into pypiserver, but also keep a mirror of public packages that you regularly update. Attempting to
+                          pull an update of a private package from `pypi.org` might pose a security risk - e.g. a malicious user might publish a higher
+                          version of the private package, containing arbitrary code.
 
 Client-Side Configurations
 ==========================
 
 Always specifying the the pypi url on the command line is a bit
 cumbersome. Since ``pypiserver`` redirects ``pip/easy_install`` to the
 ``pypi.org`` index if it doesn't have a requested package, it is a
@@ -297,15 +318,15 @@
         pypiserver.default_config(auther=pam.authenticate)
 
       Please see `Using Ad-hoc authentication providers`_ for more information.
 
 #. You  need to restart the server with the ``-P`` option only once
    (but user/password pairs can later be added or updated on the fly)::
 
-     ./pypi-server -p 8080 -P htpasswd.txt ~/packages &
+     ./pypi-server run -p 8080 -P htpasswd.txt ~/packages &
 
 Upload with ``setuptools``
 --------------------------
 
 #. On client-side, edit or create a ``~/.pypirc`` file with a similar content::
 
      [distutils]
@@ -355,37 +376,37 @@
 ``unstable``.
 
 You can always check to see what tags are currently available at our
 `Docker Repo`_.
 
 To run the most recent release of ``pypiserver`` with Docker, simply::
 
-    docker run pypiserver/pypiserver:latest
+    docker run pypiserver/pypiserver:latest run
 
 This starts ``pypiserver`` serving packages from the ``/data/packages``
 directory inside the container, listening on the container port 8080.
 
 The container takes all the same arguments as the normal ``pypi-server``
 executable, with the exception of the internal container port (``-p``),
 which will always be 8080.
 
 Of course, just running a container isn't that interesting. To map
 port 80 on the host to port 8080 on the container::
 
-    docker run -p 80:8080 pypiserver/pypiserver:latest
+    docker run -p 80:8080 pypiserver/pypiserver:latest run
 
 You can now access your ``pypiserver`` at ``localhost:80`` in a web browser.
 
 To serve packages from a directory on the host, e.g. ``~/packages``::
 
-    docker run -p 80:8080 -v ~/packages:/data/packages pypiserver/pypiserver:latest
+    docker run -p 80:8080 -v ~/packages:/data/packages pypiserver/pypiserver:latest run
 
 To authenticate against a local ``.htpasswd`` file::
 
-    docker run -p 80:8080 -v ~/.htpasswd:/data/.htpasswd pypiserver/pypiserver:latest -P .htpasswd packages
+    docker run -p 80:8080 -v ~/.htpasswd:/data/.htpasswd pypiserver/pypiserver:latest run -P .htpasswd packages
 
 You can also specify ``pypiserver`` to run as a Docker service using a
 composefile. An example composefile is `provided <docker-compose.yml>`_.
 
 
 .. _`docker repo`: https://hub.docker.com/r/pypiserver/pypiserver/tags/
 
@@ -412,36 +433,29 @@
   pip install pypiserver --pre -I
 
 You can even install the latest ``pypiserver`` directly from *github* with the
 following command, assuming you have *git* installed on your ``PATH``::
 
   pip install git+git://github.com/pypiserver/pypiserver.git
 
-Running on Heroku/Dotcloud
---------------------------
-
-https://github.com/dexterous/pypiserver-on-the-cloud contains
-instructions on how to run ``pypiserver`` on one of the supported cloud
-service providers.
-
 
 Recipes
 =======
 
 Managing the Package Directory
 ------------------------------
 
-The ``pypi-server`` command has the ``-U`` option that searches for updates of
+The ``pypi-server`` command has the ``update`` command that searches for updates of
 available packages. It scans the package directory for available
 packages and searches on pypi.org for updates. Without further
-options ``pypi-server -U`` will just print a list of commands which must
+options ``pypi-server update`` will just print a list of commands which must
 be run in order to get the latest version of each package. Output
 looks like::
 
-    $ ./pypi-server -U
+    $ ./pypi-server update 
     checking 106 packages for newer version
 
     .........u.e...........e..u.............
     .....e..............................e...
     ..........................
 
     no releases found on pypi for PyXML, Pymacs, mercurial, setuptools
@@ -453,15 +467,15 @@
     pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror greenlet==0.3.4
 
 It first prints for each package a single character after checking the
 available versions on pypi. A dot(`.`) means the package is up-to-date, ``'u'``
 means the package can be updated and ``'e'`` means the list of releases on
 pypi is empty. After that it shows a *pip* command line which can be used
 to update a one package. Either copy and paste that or run
-``pypi-server -Ux`` in order to really execute those commands. You need
+``pypi-server update -x`` in order to really execute those commands. You need
 to have *pip* installed for that to work however.
 
 Specifying an additional ``-u`` option will also allow alpha, beta and
 release candidates to be downloaded. Without this option these
 releases won't be considered.
 
 Serving Thousands of Packages
@@ -525,15 +539,15 @@
     [Service]
     Type=simple
     # systemd requires absolute path here too.
     PIDFile=/var/run/pypiserver.pid
     User=www-data
     Group=www-data
 
-    ExecStart=/usr/local/bin/pypi-server -p 8080 -a update,download --log-file /var/log/pypiserver.log -P /etc/nginx/.htpasswd /var/www/pypi
+    ExecStart=/usr/local/bin/pypi-server run -p 8080 -a update,download --log-file /var/log/pypiserver.log -P /etc/nginx/.htpasswd /var/www/pypi
     ExecStop=/bin/kill -TERM $MAINPID
     ExecReload=/bin/kill -HUP $MAINPID
     Restart=always
 
     WorkingDirectory=/var/www/pypi
 
     TimeoutStartSec=3
@@ -553,15 +567,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 `supervisor <http://supervisord.org/>`_ has the benefit of being a pure python
 package and as such, it provides excellent cross-platform support for process
 management. An example configuration file for ``supervisor`` is given below::
 
     [program:pypi]
-    command=/home/pypi/pypi-venv/bin/pypi-server -p 7001 -P /home/pypi/.htpasswd /home/pypi/packages
+    command=/home/pypi/pypi-venv/bin/pypi-server run -p 7001 -P /home/pypi/.htpasswd /home/pypi/packages
     directory=/home/pypi
     user=pypi
     autostart=true
     autorestart=true
     stderr_logfile=/var/log/pypiserver.err.log
     stdout_logfile=/var/log/pypiserver.out.log
 
@@ -571,15 +585,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Download NSSM from https://nssm.cc unzip to a desired location such as Program Files. Decide whether you are going
 to use win32 or win64, and add that exe to environment PATH.
 
 Create a start_pypiserver.bat::
 
-    pypi-server -p 8080 C:\Path\To\Packages &
+    pypi-server run -p 8080 C:\Path\To\Packages &
 
 Test the batch file by running it first before creating the service. Make sure you can access
 the server remotely, and install packages. If you can, proceed, if not troubleshoot until you can.
 This will ensure you know the server works, before adding NSSM into the mix.
 
 From the command prompt::
 
@@ -909,14 +923,44 @@
     sta_if.active(True)
     sta_if.connect('<your ESSID>', '<your password>')
     upip.index_urls = ["http://my-server:8080"]
     upip.install("micropython-foobar")
 
 Further information on micropython-packaging can be found here: https://docs.micropython.org/en/latest/reference/packages.html
 
+Custom Health Check Endpoint
+----------------------------
+
+``pypiserver`` provides a default health endpoint at ``/health``. It always returns
+``200 Ok`` if the service is up. Otherwise, it means that the service is not responsive.
+
+In addition, ``pypiserver`` allows users to customize the health endpoint.
+Alphanumeric characters, hyphens, forward slashes and underscores are allowed
+and the endpoint should not overlap with any existing routes.
+Valid examples: ``/healthz``, ``/health/live-1``, ``/api_health``, ``/action/health``
+
+Configure a custom health endpoint by CLI arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Run pypiserver with ``--health-endpoint`` argument::
+
+    pypi-server run --health-endpoint /action/health
+
+Configure a custom health endpoint by script
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    import pypiserver
+    from pypiserver import bottle
+    app = pypiserver.app(root="./packages", health_endpoint="/action/health")
+    bottle.run(app=app, host="0.0.0.0", port=8080, server="auto")
+
+Try ``curl http://localhost:8080/action/health``
+
 
 Sources
 =======
 
 To create a copy of the repository, use::
 
     git clone https://github.com/pypiserver/pypiserver.git
@@ -1008,18 +1052,18 @@
 .. _bottle: http://bottlepy.org
 .. _PyPA: https://www.pypa.io/en/latest/
 .. _PyPI: https://pypi.org
 .. _Warehouse: https://github.com/pypa/warehouse/
 .. _twine: https://pypi.org/project/twine/
 .. _pypi-uploader: https://pypi.org/project/pypi-uploader/
 .. _python-pam: https://pypi.org/project/python-pam/
-.. |test-status| image:: https://github.com/pypiserver/pypiserver/workflows/Test/badge.svg
+.. |test-status| image:: https://github.com/pypiserver/pypiserver/actions/workflows/ci.yml/badge.svg
     :alt: test status
     :scale: 100%
-    :target: https://github.com/pypiserver/pypiserver/actions?query=workflow%3ATest
+    :target: https://github.com/pypiserver/pypiserver/actions/workflows/ci.yml
 
 .. |pypi-ver| image::  https://img.shields.io/pypi/v/pypiserver.svg
     :target: https://pypi.org/project/pypiserver/
     :alt: Latest Version in PyPI
 
 .. |python-ver| image:: https://img.shields.io/pypi/pyversions/pypiserver.svg
     :target: https://pypi.org/project/pypiserver/
```

## Comparing `pypiserver-1.5.1/.gitignore` & `pypiserver-1.5.2/.gitignore`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pyproject.toml` & `pypiserver-1.5.2/pyproject.toml`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/PKG-INFO` & `pypiserver-1.5.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,1050 +1,14 @@
 Metadata-Version: 2.1
 Name: pypiserver
-Version: 1.5.1
+Version: 1.5.2
 Summary: A minimal PyPI server for use with pip/easy_install.
 Home-page: https://github.com/pypiserver/pypiserver
 Maintainer: Kostis Anagnostopoulos <ankostis@gmail.com>Matthew Planchard <mplanchard@gmail.com>
 Maintainer-email: ankostis@gmail.com
-License: UNKNOWN
-Description: .. -*- mode: rst; coding: utf-8 -*-
-        
-        .. image:: pypiserver_logo.png
-           :width: 300 px
-           :align: center
-        
-        ==============================================================================
-        pypiserver - minimal PyPI server for use with pip/easy_install
-        ==============================================================================
-        |pypi-ver| |test-status| |dependencies| |python-ver| |proj-license|
-        
-        :Version:     1.5.1
-        :Date:        2022-10-18
-        :Source:      https://github.com/pypiserver/pypiserver
-        :PyPI:        https://pypi.org/project/pypiserver/
-        :Tests:       https://github.com/pypiserver/pypiserver/actions
-        :Maintainers: | Kostis Anagnostopoulos <ankostis@gmail.com>,
-                      | Matthew Planchard <mplanchard@gmail.com>,
-                      | Dmitrii Orlov <dmtree.dev@yahoo.com>,
-                      | **Someone new?** We are looking for new maintainers! 
-                        <https://github.com/pypiserver/pypiserver/issues/397>
-        :License:     zlib/libpng + MIT
-        :Community:   https://pypiserver.zulipchat.com
-        
-        Chat with us on `Zulip <https://pypiserver.zulipchat.com>`_!
-        
-        ``pypiserver`` is a minimal PyPI_ compatible server for ``pip`` or ``easy_install``.
-        It is based on bottle_ and serves packages from regular directories.
-        Wheels, bdists, eggs and accompanying PGP-signatures can be uploaded
-        either with ``pip``, ``setuptools``, ``twine``, ``pypi-uploader``, or simply copied
-        with ``scp``.
-        
-        .. note::
-           The official software powering PyPI_ is Warehouse_. However, Warehouse_
-           is fairly specialized to be ``pypi.org``'s own software, and should not
-           be used in other contexts. In particular, it does not officially support
-           being used as a custom package index by users wishing to serve their own
-           packages.
-        
-           ``pypiserver`` implements the same interfaces as `PyPI`_, allowing
-           standard Python packaging tooling such as ``pip`` and ``twine`` to
-           interact with it as a package index just as they would with PyPI_, while
-           making it much easier to get a running index server.
-        
-        .. contents:: Table of Contents
-          :backlinks: top
-        
-        
-        Quickstart: Installation and Usage
-        ==================================
-        
-        ``pypiserver`` works with Python 3.6+ and PyPy3.
-        
-        Older Python versions may still work, but they are not tested.
-        
-        For legacy Python versions, use ``pypiserver-1.x`` series. Note that these are
-        not officially supported, and will not receive bugfixes or new features.
-        
-        .. Tip::
-           The commands below work on a unix-like operating system with a posix shell.
-           The ``'~'`` character expands to user's home directory.
-        
-           If you're using Windows, you'll have to use their "Windows counterparts".
-           The same is true for the rest of this documentation.
-        
-        1. Install ``pypiserver`` with this command::
-        
-            pip install pypiserver                # Or: pypiserver[passlib,cache]
-            mkdir ~/packages                      # Copy packages into this directory.
-        
-           See also `Alternative Installation methods`_.
-        
-        2. Copy some packages into your ``~/packages`` folder and then
-           get your ``pypiserver`` up and running::
-        
-            pypi-server -p 8080 ~/packages &      # Will listen to all IPs.
-        
-        3. From the client computer, type this::
-        
-            # Download and install hosted packages.
-            pip install --extra-index-url http://localhost:8080/simple/ ...
-        
-            # or
-            pip install --extra-index-url http://localhost:8080 ...
-        
-            # Search hosted packages.
-            pip search --index http://localhost:8080 ...
-        
-            # Note that pip search does not currently work with the /simple/ endpoint.
-        
-           See also `Client-side configurations`_ for avoiding tedious typing.
-        
-        4. Enter ``pypi-server -h`` in the cmd-line to print a detailed usage message::
-        
-            pypi-server [OPTIONS] [PACKAGES_DIRECTORY...]
-              start PyPI compatible package server serving packages from
-              PACKAGES_DIRECTORY. If PACKAGES_DIRECTORY is not given on the
-              command line, it uses the default ~/packages. pypiserver scans this
-              directory recursively for packages. It skips packages and
-              directories starting with a dot. Multiple package directories can be
-              specified.
-        
-            pypi-server understands the following options:
-        
-              -p, --port PORT
-                Listen on port PORT (default: 8080).
-        
-              -i, --interface INTERFACE
-                Listen on interface INTERFACE (default: 0.0.0.0, any interface).
-        
-              -a, --authenticate (update|download|list), ...
-                Comma-separated list of (case-insensitive) actions to authenticate.
-                Requires to have set the password (-P option).
-                To password-protect package downloads (in addition to uploads) while
-                leaving listings public, use:
-                  -P foo/htpasswd.txt -a update,download
-                To allow unauthorized access, use:
-                  -P . -a .
-                Note that when uploads are not protected, the `register` command
-                is not necessary, but `~/.pypirc` still need username and password fields,
-                even if bogus.
-                By default, only 'update' is password-protected.
-        
-              -P, --passwords PASSWORD_FILE
-                Use apache htpasswd file PASSWORD_FILE to set usernames & passwords when
-                authenticating certain actions (see -a option).
-                To allow unauthorized access, use:
-                  -P . -a .
-        
-              --disable-fallback
-                Disable redirect to real PyPI index for packages not found in the
-                local index.
-        
-              --fallback-url FALLBACK_URL
-                For packages not found in the local index, this URL will be used to
-                redirect to (default: https://pypi.org/simple/).
-        
-              --server METHOD
-                Use METHOD to run the server. Valid values include paste,
-                cherrypy, twisted, gunicorn, gevent, wsgiref, auto. The
-                default is to use "auto" which chooses one of paste, cherrypy,
-                twisted or wsgiref.
-        
-              -r, --root PACKAGES_DIRECTORY
-                [deprecated] Serve packages from PACKAGES_DIRECTORY.
-        
-              -o, --overwrite
-                Allow overwriting existing package files.
-        
-              --hash-algo ALGO
-                Any `hashlib` available algo used as fragments on package links.
-                Set one of (0, no, off, false) to disabled it (default: md5).
-        
-              --welcome HTML_FILE
-                Uses the ASCII contents of HTML_FILE as welcome message response.
-        
-              -v
-                Enable verbose logging; repeat for more verbosity.
-        
-              --log-conf <FILE>
-                Read logging configuration from FILE.
-                By default, configuration is read from `log.conf` if found in server's dir.
-        
-              --log-file <FILE>
-                Write logging info into this FILE.
-        
-              --log-frmt <FILE>
-                The logging format-string (see `logging.LogRecord` class from standard python library).
-                [Default: %(asctime)s|%(name)s|%(levelname)s|%(thread)d|%(message)s]
-        
-              --log-req-frmt FORMAT
-                A format-string selecting Http-Request properties to log; set to '%s' to see them all.
-                [Default: %(bottle.request)s]
-        
-              --log-res-frmt FORMAT
-                A format-string selecting Http-Response properties to log; set to  '%s' to see them all.
-                [Default: %(status)s]
-        
-              --log-err-frmt FORMAT
-                A format-string selecting Http-Error properties to log; set to  '%s' to see them all.
-                [Default: %(body)s: %(exception)s \n%(traceback)s]
-        
-              --cache-control AGE
-                Add "Cache-Control: max-age=AGE, public" header to package downloads.
-                Pip 6+ needs this for caching.
-        
-            pypi-server -h, --help
-              Show this help message.
-        
-            pypi-server --version
-              Show pypi-server's version.
-        
-            pypi-server -U [OPTIONS] [PACKAGES_DIRECTORY...]
-              Update packages in PACKAGES_DIRECTORY. This command searches
-              pypi.org for updates and shows a pip command line which
-              updates the package.
-        
-            The following additional options can be specified with -U:
-        
-              -x
-                Execute the pip commands instead of only showing them.
-        
-              -d DOWNLOAD_DIRECTORY
-                Download package updates to this directory. The default is to use
-                the directory which contains the latest version of the package to
-                be updated.
-        
-              -u
-                Allow updating to unstable version (alpha, beta, rc, dev versions).
-        
-            Visit https://github.com/pypiserver/pypiserver for more information.
-        
-        
-        Client-Side Configurations
-        ==========================
-        
-        Always specifying the the pypi url on the command line is a bit
-        cumbersome. Since ``pypiserver`` redirects ``pip/easy_install`` to the
-        ``pypi.org`` index if it doesn't have a requested package, it is a
-        good idea to configure them to always use your local pypi index.
-        
-        Configuring ``pip``
-        -------------------
-        
-        For ``pip`` command this can be done by setting the environment variable
-        ``PIP_EXTRA_INDEX_URL`` in your ``.bashr/.profile/.zshrc``::
-        
-          export PIP_EXTRA_INDEX_URL=http://localhost:8080/simple/
-        
-        or by adding the following lines to ``~/.pip/pip.conf``::
-        
-          [global]
-          extra-index-url = http://localhost:8080/simple/
-        
-        .. Note::
-           If you have installed ``pypiserver`` on a remote url without *https*
-           you will receive an "untrusted" warning from *pip*, urging you to append
-           the ``--trusted-host`` option.  You can also include this option permanently
-           in your configuration-files or environment variables.
-        
-        Configuring ``easy_install``
-        ----------------------------
-        
-        For ``easy_install`` command you may set the following configuration in
-        ``~/.pydistutils.cfg``::
-        
-          [easy_install]
-          index_url = http://localhost:8080/simple/
-        
-        
-        Uploading Packages Remotely
-        ===========================
-        
-        Instead of copying packages directly to the server's folder (i.e. with ``scp``),
-        you may use python tools for the task, e.g. ``python setup.py upload``.
-        In that case, ``pypiserver`` is responsible for authenticating the upload-requests.
-        
-        .. Note::
-          We strongly advise to password-protected your uploads!
-        
-          It is possible to disable authentication for uploads (e.g. in intranets).
-          To avoid lazy security decisions, read help for ``-P`` and ``-a`` options.
-        
-        *Apache*-Like Authentication (``htpasswd``)
-        -------------------------------------------
-        
-        #. First make sure you have the *passlib* module installed (note that
-           ``passlib>=1.6`` is required), which is needed for parsing the Apache
-           *htpasswd* file specified by the ``-P``, ``--passwords`` option
-           (see next steps)::
-        
-             pip install passlib
-        
-        #. Create the Apache *htpasswd* file with at least one user/password pair
-           with this command (you'll be prompted for a password)::
-        
-             htpasswd -sc htpasswd.txt <some_username>
-        
-           .. Tip:: Read this SO question for running `htpasswd` cmd
-              under *Windows*:
-        
-                 http://serverfault.com/questions/152950/how-to-create-and-edit-htaccess-and-htpasswd-locally-on-my-computer-and-then-u
-        
-              or if you have bogus passwords that you don't care because they are for
-              an internal service (which is still "bad", from a security perspective...)
-              you may use this public service:
-        
-                 http://www.htaccesstools.com/htpasswd-generator/
-        
-           .. Tip:: When accessing pypiserver via the api, alternate authentication
-              methods are available via the ``auther`` config flag. Any callable
-              returning a boolean can be passed through to the pypiserver config in
-              order to provide custom authentication. For example, to configure
-              pypiserver to authenticate using the `python-pam`_::
-        
-                import pam
-                pypiserver.default_config(auther=pam.authenticate)
-        
-              Please see `Using Ad-hoc authentication providers`_ for more information.
-        
-        #. You  need to restart the server with the ``-P`` option only once
-           (but user/password pairs can later be added or updated on the fly)::
-        
-             ./pypi-server -p 8080 -P htpasswd.txt ~/packages &
-        
-        Upload with ``setuptools``
-        --------------------------
-        
-        #. On client-side, edit or create a ``~/.pypirc`` file with a similar content::
-        
-             [distutils]
-             index-servers =
-               pypi
-               local
-        
-             [pypi]
-             username:<your_pypi_username>
-             password:<your_pypi_passwd>
-        
-             [local]
-             repository: http://localhost:8080
-             username: <some_username>
-             password: <some_passwd>
-        
-        #. Then from within the directory of the python-project you wish to upload,
-           issue this command::
-        
-             python setup.py sdist upload -r local
-        
-        Upload with ``twine``
-        ---------------------
-        
-        To avoid storing you passwords on disk, in clear text, you may either:
-        
-        - use the ``register`` *setuptools*'s command with the ``-r`` option,
-          like that::
-        
-             python setup.py sdist register -r local upload -r local
-        
-        - use `twine`_ library, which
-          breaks the procedure in two steps.  In addition, it supports signing
-          your files with PGP-Signatures and uploading the generated `.asc` files
-          to ``pypiserver``::
-        
-             twine upload -r local --sign -identity user_name ./foo-1.zip
-        
-        
-        Using the Docker Image
-        ======================
-        
-        Starting with version 1.2.5, official Docker images will be built for each
-        push to master, each dev, alpha, or beta release, and each final release.
-        The most recent full release will always be available under the tag ``latest``,
-        and the current master branch will always be available under the tag
-        ``unstable``.
-        
-        You can always check to see what tags are currently available at our
-        `Docker Repo`_.
-        
-        To run the most recent release of ``pypiserver`` with Docker, simply::
-        
-            docker run pypiserver/pypiserver:latest
-        
-        This starts ``pypiserver`` serving packages from the ``/data/packages``
-        directory inside the container, listening on the container port 8080.
-        
-        The container takes all the same arguments as the normal ``pypi-server``
-        executable, with the exception of the internal container port (``-p``),
-        which will always be 8080.
-        
-        Of course, just running a container isn't that interesting. To map
-        port 80 on the host to port 8080 on the container::
-        
-            docker run -p 80:8080 pypiserver/pypiserver:latest
-        
-        You can now access your ``pypiserver`` at ``localhost:80`` in a web browser.
-        
-        To serve packages from a directory on the host, e.g. ``~/packages``::
-        
-            docker run -p 80:8080 -v ~/packages:/data/packages pypiserver/pypiserver:latest
-        
-        To authenticate against a local ``.htpasswd`` file::
-        
-            docker run -p 80:8080 -v ~/.htpasswd:/data/.htpasswd pypiserver/pypiserver:latest -P .htpasswd packages
-        
-        You can also specify ``pypiserver`` to run as a Docker service using a
-        composefile. An example composefile is `provided <docker-compose.yml>`_.
-        
-        
-        .. _`docker repo`: https://hub.docker.com/r/pypiserver/pypiserver/tags/
-        
-        
-        Alternative Installation Methods
-        ================================
-        
-        When trying the methods below, first use the following command to check whether
-        previous versions of ``pypiserver`` already exist, and (optionally) uninstall them::
-        
-          # VERSION-CHECK: Fails if not installed.
-          pypi-server --version
-        
-          # UNINSTALL: Invoke again until it fails.
-          pip uninstall pypiserver
-        
-        Installing the Very Latest Version
-        ----------------------------------
-        
-        In case the latest version in *pypi* is a pre-release, you have to use
-        *pip*'s `--pre` option.  And to update an existing installation combine it
-        with `--ignore-installed`::
-        
-          pip install pypiserver --pre -I
-        
-        You can even install the latest ``pypiserver`` directly from *github* with the
-        following command, assuming you have *git* installed on your ``PATH``::
-        
-          pip install git+git://github.com/pypiserver/pypiserver.git
-        
-        Running on Heroku/Dotcloud
-        --------------------------
-        
-        https://github.com/dexterous/pypiserver-on-the-cloud contains
-        instructions on how to run ``pypiserver`` on one of the supported cloud
-        service providers.
-        
-        
-        Recipes
-        =======
-        
-        Managing the Package Directory
-        ------------------------------
-        
-        The ``pypi-server`` command has the ``-U`` option that searches for updates of
-        available packages. It scans the package directory for available
-        packages and searches on pypi.org for updates. Without further
-        options ``pypi-server -U`` will just print a list of commands which must
-        be run in order to get the latest version of each package. Output
-        looks like::
-        
-            $ ./pypi-server -U
-            checking 106 packages for newer version
-        
-            .........u.e...........e..u.............
-            .....e..............................e...
-            ..........................
-        
-            no releases found on pypi for PyXML, Pymacs, mercurial, setuptools
-        
-            # update raven from 1.4.3 to 1.4.4
-            pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror raven==1.4.4
-        
-            # update greenlet from 0.3.3 to 0.3.4
-            pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror greenlet==0.3.4
-        
-        It first prints for each package a single character after checking the
-        available versions on pypi. A dot(`.`) means the package is up-to-date, ``'u'``
-        means the package can be updated and ``'e'`` means the list of releases on
-        pypi is empty. After that it shows a *pip* command line which can be used
-        to update a one package. Either copy and paste that or run
-        ``pypi-server -Ux`` in order to really execute those commands. You need
-        to have *pip* installed for that to work however.
-        
-        Specifying an additional ``-u`` option will also allow alpha, beta and
-        release candidates to be downloaded. Without this option these
-        releases won't be considered.
-        
-        Serving Thousands of Packages
-        -----------------------------
-        
-        By default, ``pypiserver`` scans the entire packages directory each time an
-        incoming HTTP request occurs. This isn't a problem for a small number of
-        packages, but causes noticeable slow-downs when serving thousands of packages.
-        
-        If you run into this problem, significant speedups can be gained by enabling
-        pypiserver's directory caching functionality. The only requirement is to
-        install the ``watchdog`` package, or it can be installed during ``pypiserver``
-        installation, by specifying the ``cache`` extras option::
-        
-            pip install pypiserver[cache]
-        
-        Additional speedups can be obtained by using your webserver's builtin
-        caching functionality. For example, if you are using `nginx` as a
-        reverse-proxy as described below in `Behind a reverse proxy`_, you can
-        easily enable caching. For example, to allow nginx to cache up to
-        10 gigabytes of data for up to 1 hour::
-        
-            proxy_cache_path /data/nginx/cache
-                             levels=1:2
-                             keys_zone=pypiserver_cache:10m
-                             max_size=10g
-                             inactive=60m
-                             use_temp_path=off;
-        
-            server {
-                # ...
-                location / {
-                    proxy_cache pypiserver_cache;
-                    proxy_pass http://localhost:8080;
-                }
-            }
-        
-        Using webserver caching is especially helpful if you have high request
-        volume. Using `nginx` caching, a real-world pypiserver installation was
-        able to easily support over 1000 package downloads/min at peak load.
-        
-        Managing Automated Startup
-        --------------------------
-        
-        There are a variety of options for handling the automated starting of
-        pypiserver upon system startup. Two of the most common are *systemd* and
-        *supervisor* for linux systems. For windows creating services with scripts isn't
-        an easy task without a third party tool such as *NSSM*.
-        
-        Running As a ``systemd`` Service
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``systemd`` is installed by default on most modern Linux systems and as such,
-        it is an excellent option for managing the pypiserver process. An example
-        config file for ``systemd`` can be seen below::
-        
-            [Unit]
-            Description=A minimal PyPI server for use with pip/easy_install.
-            After=network.target
-        
-            [Service]
-            Type=simple
-            # systemd requires absolute path here too.
-            PIDFile=/var/run/pypiserver.pid
-            User=www-data
-            Group=www-data
-        
-            ExecStart=/usr/local/bin/pypi-server -p 8080 -a update,download --log-file /var/log/pypiserver.log -P /etc/nginx/.htpasswd /var/www/pypi
-            ExecStop=/bin/kill -TERM $MAINPID
-            ExecReload=/bin/kill -HUP $MAINPID
-            Restart=always
-        
-            WorkingDirectory=/var/www/pypi
-        
-            TimeoutStartSec=3
-            RestartSec=5
-        
-            [Install]
-            WantedBy=multi-user.target
-        
-        Adjusting the paths and adding this file as ``pypiserver.service`` into your
-        ``systemd/system`` directory will allow management of the pypiserver process with
-        ``systemctl``, e.g. ``systemctl start pypiserver``.
-        
-        More useful information about *systemd* can be found at
-        https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units
-        
-        Launching through ``supervisor``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        `supervisor <http://supervisord.org/>`_ has the benefit of being a pure python
-        package and as such, it provides excellent cross-platform support for process
-        management. An example configuration file for ``supervisor`` is given below::
-        
-            [program:pypi]
-            command=/home/pypi/pypi-venv/bin/pypi-server -p 7001 -P /home/pypi/.htpasswd /home/pypi/packages
-            directory=/home/pypi
-            user=pypi
-            autostart=true
-            autorestart=true
-            stderr_logfile=/var/log/pypiserver.err.log
-            stdout_logfile=/var/log/pypiserver.out.log
-        
-        From there, the process can be managed via ``supervisord`` using ``supervisorctl``.
-        
-        Running As a service with ``NSSM`` (Windows)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Download NSSM from https://nssm.cc unzip to a desired location such as Program Files. Decide whether you are going
-        to use win32 or win64, and add that exe to environment PATH.
-        
-        Create a start_pypiserver.bat::
-        
-            pypi-server -p 8080 C:\Path\To\Packages &
-        
-        Test the batch file by running it first before creating the service. Make sure you can access
-        the server remotely, and install packages. If you can, proceed, if not troubleshoot until you can.
-        This will ensure you know the server works, before adding NSSM into the mix.
-        
-        From the command prompt::
-        
-            nssm install pypiserver
-        
-        This command will launch a NSSM gui application::
-        
-            Path: C:\Path\To\start_pypiserver.bat
-            Startup directory: Auto generates when selecting path
-            Service name: pypiserver
-        
-        There are more tabs, but that is the basic setup. If the service needs to be running with a certain
-        login credentials, make sure you enter those credentials in the logon tab.
-        
-        Start the service::
-        
-            nssm start pypiserver
-        
-        Other useful commands::
-        
-            nssm --help
-            nssm stop <servicename>
-            nssm restart <servicename>
-            nssm status <servicename>
-        
-        For detailed information please visit https://nssm.cc
-        
-        Using a Different WSGI Server
-        -----------------------------
-        
-        - The ``bottle`` web-server which supports many WSGI-servers, among others,
-          ``paste``, ``cherrypy``, ``twisted`` and ``wsgiref`` (part of Python); you select
-          them using the ``--server`` flag.
-        
-        - You may view all supported WSGI servers using the following interactive code::
-        
-            >>> from pypiserver import bottle
-            >>> list(bottle.server_names.keys())
-            ['cgi', 'gunicorn', 'cherrypy', 'eventlet', 'tornado', 'geventSocketIO',
-            'rocket', 'diesel', 'twisted', 'wsgiref', 'fapws3', 'bjoern', 'gevent',
-            'meinheld', 'auto', 'aiohttp', 'flup', 'gae', 'paste', 'waitress']
-        
-        - If none of the above servers matches your needs, invoke just the
-          ``pypiserver:app()`` method which returns the internal WSGI-app WITHOUT
-          starting-up a server - you may then send it to any WSGI server you like.
-          Read also the `Utilizing the API`_ section.
-        
-        - Some examples are given below - you may find more details in `bottle
-          site <http://bottlepy.org/docs/dev/deployment.html#switching-the-server-backend>`_.
-        
-        Apache (``mod_wsgi``)
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        To use your *Apache2* with ``pypiserver``, prefer to utilize ``mod_wsgi`` as
-        explained in `bottle's documentation <http://bottlepy.org/docs/dev/deployment.html#apache-mod-wsgi>`_.
-        
-        .. Note::
-           If you choose instead to go with ``mod_proxy``, mind that you may bump into problems
-           with the prefix-path (see `#155 <https://github.com/pypiserver/pypiserver/issues/155>`_).
-        
-        1. Adapt and place the following *Apache* configuration either into top-level scope,
-           or inside some ``<VirtualHost>`` (contributed by Thomas Waldmann)::
-        
-                WSGIScriptAlias   /     /yoursite/wsgi/pypiserver-wsgi.py
-                WSGIDaemonProcess       pypisrv user=pypisrv group=pypisrv umask=0007 \
-                                        processes=1 threads=5 maximum-requests=500 \
-                                        display-name=wsgi-pypisrv inactivity-timeout=300
-                WSGIProcessGroup        pypisrv
-                WSGIPassAuthorization On    # Required for authentication (https://github.com/pypiserver/pypiserver/issues/288)
-        
-                <Directory /yoursite/wsgi >
-                    Require all granted
-                </Directory>
-        
-           or if using older ``Apache < 2.4``, substitute the last part with this::
-        
-                <Directory /yoursite/wsgi >
-                    Order deny,allow
-                    Allow from all
-                </Directory>
-        
-        2. Then create the ``/yoursite/cfg/pypiserver.wsgi`` file and make sure that
-           the ``user`` and ``group`` of the ``WSGIDaemonProcess`` directive
-           (``pypisrv:pypisrv`` in the example) have the read permission on it::
-        
-                import pypiserver
-        
-                conf = pypiserver.default_config(
-                    root =          "/yoursite/packages",
-                    password_file = "/yoursite/htpasswd", )
-                application = pypiserver.app(**conf)
-        
-        
-           .. Tip::
-              If you have installed ``pypiserver`` in a virtualenv, follow ``mod_wsgi``'s
-              `instructions <http://modwsgi.readthedocs.io/en/develop/user-guides/virtual-environments.html>`_
-              and prepend the python code above with the following::
-        
-                    import site
-        
-                    site.addsitedir('/yoursite/venv/lib/pythonX.X/site-packages')
-        
-        .. Note::
-           For security reasons, notice that the ``Directory`` directive grants access
-           to a directory holding the ``wsgi`` start-up script, alone; nothing else.
-        
-        .. Note::
-           To enable HTTPS support on Apache, configure the directive that contains the
-           WSGI configuration to use SSL.
-        
-        ``gunicorn``
-        ~~~~~~~~~~~~
-        
-        The following command uses ``gunicorn`` to start ``pypiserver``::
-        
-          gunicorn -w4 'pypiserver:app(root="/home/ralf/packages")'
-        
-        or when using multiple roots::
-        
-          gunicorn -w4 'pypiserver:app(root=["/home/ralf/packages", "/home/ralf/experimental"])'
-        
-        ``paste``
-        ~~~~~~~~~
-        
-        `paste <http://pythonpaste.org/>`_ allows to run multiple WSGI applications
-        under different URL paths. Therefore it is possible to serve different set
-        of packages on different paths.
-        
-        The following example ``paste.ini`` could be used to serve stable and
-        unstable packages on different paths::
-        
-            [composite:main]
-            use = egg:Paste#urlmap
-            /unstable/ = unstable
-            / = stable
-        
-            [app:stable]
-            use = egg:pypiserver#main
-            root = ~/stable-packages
-        
-            [app:unstable]
-            use = egg:pypiserver#main
-            root = ~/stable-packages
-               ~/unstable-packages
-        
-            [server:main]
-            use = egg:gunicorn#main
-            host = 0.0.0.0
-            port = 9000
-            workers = 5
-            accesslog = -
-        
-        .. Note::
-           You need to install some more dependencies for this to work, like::
-        
-                pip install paste pastedeploy gunicorn pypiserver
-        
-           The server can then start with::
-        
-                gunicorn_paster paste.ini
-        
-        
-        Behind a Reverse Proxy
-        ----------------------
-        
-        You can run ``pypiserver`` behind a reverse proxy as well.
-        
-        Nginx
-        ~~~~~
-        
-        Extend your nginx configuration::
-        
-            upstream pypi {
-              server              pypiserver.example.com:12345 fail_timeout=0;
-            }
-        
-            server {
-              server_name         myproxy.example.com;
-        
-              location / {
-                proxy_set_header  Host $host:$server_port;
-                proxy_set_header  X-Forwarded-Proto $scheme;
-                proxy_set_header  X-Real-IP $remote_addr;
-                proxy_pass        http://pypi;
-              }
-            }
-        
-        As of pypiserver 1.3, you may also use the `X-Forwarded-Host` header in your
-        reverse proxy config to enable changing the base URL. For example if you
-        want to host pypiserver under a particular path on your server::
-        
-            upstream pypi {
-              server              localhost:8000;
-            }
-        
-            server {
-              location /pypi/ {
-                  proxy_set_header  X-Forwarded-Host $host:$server_port/pypi;
-                  proxy_set_header  X-Forwarded-Proto $scheme;
-                  proxy_set_header  X-Forwarded-For $proxy_add_x_forwarded_for;
-                  proxy_set_header  X-Real-IP $remote_addr;
-                  proxy_pass        http://pypi;
-              }
-            }
-        
-        Supporting HTTPS
-        ~~~~~~~~~~~~~~~~
-        
-        Using a reverse proxy is the preferred way of getting pypiserver behind
-        HTTPS. For example, to put pypiserver behind HTTPS on port 443, with
-        automatic HTTP redirection, using `nginx`::
-        
-            upstream pypi {
-              server               localhost:8000;
-            }
-        
-            server {
-              listen              80 default_server;
-              server_name         _;
-              return              301 https://$host$request_uri;
-            }
-        
-            server {
-              listen              443 ssl;
-              server_name         pypiserver.example.com;
-        
-              ssl_certificate     /etc/star.example.com.crt;
-              ssl_certificate_key /etc/star.example.com.key;
-              ssl_protocols       TLSv1 TLSv1.1 TLSv1.2;
-              ssl_ciphers         HIGH:!aNULL:!MD5;
-        
-              location / {
-                proxy_set_header  Host $host:$server_port;
-                proxy_set_header  X-Forwarded-Proto $scheme;
-                proxy_set_header  X-Real-IP $remote_addr;
-                proxy_pass        http://pypi;
-              }
-            }
-        
-        Please see `nginx's HTTPS docs for more details <http://nginx.org/en/docs/http/configuring_https_servers.html>`_.
-        
-        Getting and keeping your certificates up-to-date can be simplified using,
-        for example, using `certbot and letsencrypt <https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-18-04>`_.
-        
-        Traefik
-        ~~~~~~~
-        
-        It is also possible to use `Traefik <https://docs.traefik.io/>`_ to put pypiserver behind HTTPS on port 443, with
-        automatic HTTP redirection using Docker Compose. Please see the provided `<docker-compose.yml>`_ example for more information.
-        
-        Utilizing the API
-        -----------------
-        
-        In order to enable ad-hoc authentication-providers or to use WSGI-servers
-        not supported by *bottle* out-of-the-box, you needed to launch ``pypiserver``
-        via its API.
-        
-        - The main entry-point for configuring ``pypiserver`` is the `pypiserver:app()
-          <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L116>`_
-          function.  This function returns the internal WSGI-app that you my then
-          send to any WSGI-server you like.
-        
-        - To get all ``pypiserver:app()`` keywords and their explanations, read the
-          function `pypiserver:default_config()
-          <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L35>`_.
-        
-        - Finally, to fire-up a WSGI-server with the configured app, invoke
-          the ``bottle:run(app, host, port, server)`` function.
-          Note that ``pypiserver`` ships with it is own copy of *bottle*; to use it,
-          import it like that: ``from pypiserver import bottle``
-        
-        Using Ad-Hoc Authentication Providers
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The ``auther`` keyword of ``pypiserver:app()`` function maybe set only using
-        the API. This can be any callable that returns a boolean when passed
-        the *username* and the *password* for a given request.
-        
-        For example, to authenticate users based on the ``/etc/passwd`` file under Unix,
-        you may delegate such decisions to the `python-pam`_ library by following
-        these steps:
-        
-        1. Ensure ``python-pam`` module is installed::
-        
-            pip install python-pam
-        
-        2. Create a python-script along these lines::
-        
-            $ cat > pypiserver-start.py
-            import pypiserver
-            from pypiserver import bottle
-            import pam
-            app = pypiserver.app(root='./packages', auther=pam.authenticate)
-            bottle.run(app=app, host='0.0.0.0', port=80, server='auto')
-        
-            [Ctrl+ D]
-        
-        3. Invoke the python-script to start-up ``pypiserver``::
-        
-            $ python pypiserver-start.py
-        
-        
-        .. Note::
-           The `python-pam`_ module, requires *read* access to ``/etc/shadow`` file;
-           you may add the user under which ``pypiserver`` runs into the *shadow*
-           group, with a command like this: ``sudo usermod -a -G shadow pypy-user``.
-        
-        Use with MicroPython
-        --------------------
-        The MicroPython interpreter for embedded devices can install packages with the
-        module ``upip.py``. The module uses a specialized json-endpoint to retrieve
-        package information. This endpoint is supported by ``pypiserver``.
-        
-        It can be tested with the UNIX port of ``micropython``::
-        
-            cd micropython
-            ports/unix/micropython -m tools.upip install -i http://my-server:8080 -p /tmp/mymodules micropython-foobar
-        
-        Installing packages from the REPL of an embedded device works in this way:
-        
-        .. code-block:: python
-        
-            import network
-            import upip
-        
-            sta_if = network.WLAN(network.STA_IF)
-            sta_if.active(True)
-            sta_if.connect('<your ESSID>', '<your password>')
-            upip.index_urls = ["http://my-server:8080"]
-            upip.install("micropython-foobar")
-        
-        Further information on micropython-packaging can be found here: https://docs.micropython.org/en/latest/reference/packages.html
-        
-        
-        Sources
-        =======
-        
-        To create a copy of the repository, use::
-        
-            git clone https://github.com/pypiserver/pypiserver.git
-            cd pypiserver
-        
-        To receive any later changes, in the above folder use::
-        
-            git pull
-        
-        
-        Known Limitations
-        =================
-        
-        ``pypiserver`` does not implement the full API as seen on PyPI_. It
-        implements just enough to make ``easy_install``, ``pip install``, and
-        ``search`` work.
-        
-        The following limitations are known:
-        
-        - Command ``pypi -U`` that compares uploaded packages with *pypi* to see if
-          they are outdated, does not respect a http-proxy environment variable
-          (see `#19 <https://github.com/pypiserver/pypiserver/issues/19>`_).
-        - It accepts documentation uploads but does not save them to
-          disk (see `#47 <https://github.com/pypiserver/pypiserver/issues/47>`_ for a
-          discussion)
-        - It does not handle misspelled packages as *pypi-repo* does,
-          therefore it is suggested to use it with ``--extra-index-url`` instead
-          of ``--index-url`` (see `#38 <https://github.com/pypiserver/pypiserver/issues/38>`_).
-        
-        Please use Github's `bugtracker <https://github.com/pypiserver/pypiserver/issues>`_
-        for other bugs you find.
-        
-        
-        Similar Projects
-        ================
-        
-        There are lots of other projects, which allow you to run your own
-        PyPI server. If ``pypiserver`` doesn't work for you, the following are
-        among the most popular alternatives:
-        
-        - `devpi-server <https://pypi.org/project/devpi/>`_:
-          a reliable fast pypi.org caching server, part of
-          the comprehensive `github-style pypi index server and packaging meta tool
-          <https://pypi.org/project/devpi/>`_.
-          (version: 2.1.4, access date: 8/3/2015)
-        
-        - Check this SO question: `How to roll my own pypi
-          <http://stackoverflow.com/questions/1235331/how-to-roll-my-own-pypi>`_
-        
-        
-        Unmaintained or archived
-        ------------------------
-        
-        These projects were once alternatives to pypiserver but are now either unmaintained or archived.
-        
-        - `pip2pi <https://github.com/wolever/pip2pi>`_
-          a simple cmd-line tool that builds a PyPI-compatible local folder from pip requirements
-        
-        - `flask-pypi-proxy <http://flask-pypi-proxy.readthedocs.org/>`_
-          A proxy for PyPI that also enables also uploading custom packages.
-        
-        
-        Related Software
-        ================
-        
-        Though not direct alternatives for ``pypiserver``'s use as an index
-        server, the following is a list of related software projects that you
-        may want to familiarize with:
-        
-        - `pypi-uploader`_:
-          A command-line utility to upload packages to your ``pypiserver`` from pypi without
-          having to store them locally first.
-        
-        - `twine`_:
-          A command-line utility for interacting with PyPI or ``pypiserver``.
-        
-        - `warehouse`_:
-          the software that powers PyPI_ itself. It is not generally intended to
-          be run by end-users.
-        
-        Licensing
-        =========
-        
-        ``pypiserver`` contains a copy of bottle_ which is available under the
-        MIT license, and the remaining part is distributed under the zlib/libpng license.
-        See the ``LICENSE.txt`` file.
-        
-        
-        .. _bottle: http://bottlepy.org
-        .. _PyPA: https://www.pypa.io/en/latest/
-        .. _PyPI: https://pypi.org
-        .. _Warehouse: https://github.com/pypa/warehouse/
-        .. _twine: https://pypi.org/project/twine/
-        .. _pypi-uploader: https://pypi.org/project/pypi-uploader/
-        .. _python-pam: https://pypi.org/project/python-pam/
-        .. |test-status| image:: https://github.com/pypiserver/pypiserver/workflows/Test/badge.svg
-            :alt: test status
-            :scale: 100%
-            :target: https://github.com/pypiserver/pypiserver/actions?query=workflow%3ATest
-        
-        .. |pypi-ver| image::  https://img.shields.io/pypi/v/pypiserver.svg
-            :target: https://pypi.org/project/pypiserver/
-            :alt: Latest Version in PyPI
-        
-        .. |python-ver| image:: https://img.shields.io/pypi/pyversions/pypiserver.svg
-            :target: https://pypi.org/project/pypiserver/
-            :alt: Supported Python versions
-        
-        .. |proj-license| image:: https://img.shields.io/badge/license-BSD%2Bzlib%2Flibpng-blue.svg
-            :target: https://raw.githubusercontent.com/pypiserver/pypiserver/master/LICENSE.txt
-            :alt: Project License
-        
-        .. |dependencies| image:: https://img.shields.io/requires/github/pypiserver/pypiserver.svg
-            :target: https://requires.io/github/pypiserver/pypiserver/requirements/
-            :alt: Dependencies up-to-date?
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -1052,14 +16,1097 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Software Distribution
 Requires-Python: >=3.6
 Provides-Extra: passlib
 Provides-Extra: cache
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+.. -*- mode: rst; coding: utf-8 -*-
+
+.. image:: docs/__resources__/pypiserver_logo.png
+   :width: 300 px
+   :align: center
+
+==============================================================================
+pypiserver - minimal PyPI server for use with pip/easy_install
+==============================================================================
+|pypi-ver| |test-status| |dependencies| |python-ver| |proj-license|
+
+:Version:     1.5.2
+:Date:        2023-07-30
+:Source:      https://github.com/pypiserver/pypiserver
+:PyPI:        https://pypi.org/project/pypiserver/
+:Tests:       https://github.com/pypiserver/pypiserver/actions
+:Maintainers: | Kostis Anagnostopoulos <ankostis@gmail.com>,
+              | Matthew Planchard <mplanchard@gmail.com>,
+              | Dmitrii Orlov <dmtree.dev@yahoo.com>,
+              | **Someone new?** We are looking for new maintainers! 
+                <https://github.com/pypiserver/pypiserver/issues/397>
+:License:     zlib/libpng + MIT
+:Community:   https://pypiserver.zulipchat.com
+
+Chat with us on `Zulip <https://pypiserver.zulipchat.com>`_!
+
+``pypiserver`` is a minimal PyPI_ compatible server for ``pip`` or ``easy_install``.
+It is based on bottle_ and serves packages from regular directories.
+Wheels, bdists, eggs and accompanying PGP-signatures can be uploaded
+either with ``pip``, ``setuptools``, ``twine``, ``pypi-uploader``, or simply copied
+with ``scp``.
+
+.. note::
+   The official software powering PyPI_ is Warehouse_. However, Warehouse_
+   is fairly specialized to be ``pypi.org``'s own software, and should not
+   be used in other contexts. In particular, it does not officially support
+   being used as a custom package index by users wishing to serve their own
+   packages.
+
+   ``pypiserver`` implements the same interfaces as `PyPI`_, allowing
+   standard Python packaging tooling such as ``pip`` and ``twine`` to
+   interact with it as a package index just as they would with PyPI_, while
+   making it much easier to get a running index server.
+
+.. contents:: Table of Contents
+  :backlinks: top
+
+
+Quickstart: Installation and Usage
+==================================
+
+``pypiserver`` works with Python 3.6+ and PyPy3.
+
+Older Python versions may still work, but they are not tested.
+
+For legacy Python versions, use ``pypiserver-1.x`` series. Note that these are
+not officially supported, and will not receive bugfixes or new features.
+
+.. Tip::
+   The commands below work on a unix-like operating system with a posix shell.
+   The ``'~'`` character expands to user's home directory.
+
+   If you're using Windows, you'll have to use their "Windows counterparts".
+   The same is true for the rest of this documentation.
+
+1. Install ``pypiserver`` with this command::
+
+    pip install pypiserver                # Or: pypiserver[passlib,cache]
+    mkdir ~/packages                      # Copy packages into this directory.
+
+   See also `Alternative Installation methods`_.
+
+2. Copy some packages into your ``~/packages`` folder and then
+   get your ``pypiserver`` up and running::
+
+    pypi-server run -p 8080 ~/packages &      # Will listen to all IPs.
+
+3. From the client computer, type this::
+
+    # Download and install hosted packages.
+    pip install --extra-index-url http://localhost:8080/simple/ ...
+
+    # or
+    pip install --extra-index-url http://localhost:8080 ...
+
+    # Search hosted packages.
+    pip search --index http://localhost:8080 ...
+
+    # Note that pip search does not currently work with the /simple/ endpoint.
+
+   See also `Client-side configurations`_ for avoiding tedious typing.
+
+4. Enter ``pypi-server -h`` in the cmd-line to print a detailed usage message::
+
+    start PyPI compatible package server serving packages from PACKAGES_DIRECTORY. If PACKAGES_DIRECTORY is not given on the command line, it uses the default ~/packages. pypiserver scans this directory recursively for packages. It skips packages and directories starting with a dot. Multiple package directories may be specified.
+
+    positional arguments:
+      {run,update}
+        run                 Run pypiserver, serving packages from
+                            PACKAGES_DIRECTORY
+        update              Handle updates of packages managed by pypiserver. By
+                            default, a pip command to update the packages is
+                            printed to stdout for introspection or pipelining. See
+                            the `-x` option for updating packages directly.
+
+    options:
+      -h, --help            show this help message and exit
+      -v, --verbose         Enable verbose logging; repeat for more verbosity.
+      --log-file FILE       Write logging info into this FILE, as well as to
+                            stdout or stderr, if configured.
+      --log-stream STREAM   Log messages to the specified STREAM. Valid values are
+                            stdout, stderr, and none
+      --log-frmt FORMAT     The logging format-string.  (see `logging.LogRecord`
+                            class from standard python library)
+      --hash-algo HASH_ALGO
+                            Any `hashlib` available algorithm to use for
+                            generating fragments on package links. Can be disabled
+                            with one of (0, no, off, false).
+      --backend {auto,simple-dir,cached-dir}
+                            A backend implementation. Keep the default 'auto' to
+                            automatically determine whether to activate caching or
+                            not
+      --version             show program's version number and exit
+
+    Visit https://github.com/pypiserver/pypiserver for more information
+
+More details about ``pypi-server run``
+--------------------------------------
+
+Enter ``pypi-server run -h`` in the cmd-line to print a detailed usage
+message *about starting the server*::
+
+  usage: pypi-server run [-h] [-v] [--log-file FILE] [--log-stream STREAM] [--log-frmt FORMAT] [--hash-algo HASH_ALGO]
+                       [--backend {auto,simple-dir,cached-dir}] [--version] [-p PORT] [-i HOST] [-a AUTHENTICATE] [-P PASSWORD_FILE] [--disable-fallback]
+                       [--fallback-url FALLBACK_URL] [--health-endpoint HEALTH_ENDPOINT] [--server METHOD] [-o] [--welcome HTML_FILE]
+                       [--cache-control AGE] [--log-req-frmt FORMAT] [--log-res-frmt FORMAT] [--log-err-frmt FORMAT]
+                       [package_directory [package_directory ...]]
+
+  positional arguments:
+    package_directory     The directory from which to serve packages.
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -v, --verbose         Enable verbose logging; repeat for more verbosity.
+    --log-file FILE       Write logging info into this FILE, as well as to stdout or stderr, if configured.
+    --log-stream STREAM   Log messages to the specified STREAM. Valid values are stdout, stderr, and none
+    --log-frmt FORMAT     The logging format-string.  (see `logging.LogRecord` class from standard python library)
+    --hash-algo HASH_ALGO
+                          Any `hashlib` available algorithm to use for generating fragments on package links. Can be disabled with one of (0, no, off,
+                          false).
+    --backend {auto,simple-dir,cached-dir}
+                          A backend implementation. Keep the default 'auto' to automatically determine whether to activate caching or not
+    --version             show program's version number and exit
+    -p PORT, --port PORT  Listen on port PORT (default: 8080)
+    -i HOST, -H HOST, --interface HOST, --host HOST
+                          Listen on interface INTERFACE (default: 0.0.0.0)
+    -a AUTHENTICATE, --authenticate AUTHENTICATE
+                          Comma-separated list of (case-insensitive) actions to authenticate (options: download, list, update; default: update).
+                          
+                          Any actions not specified are not authenticated, so to authenticate downloads and updates, but allow unauthenticated viewing of
+                          the package list, you would use:
+                          
+                            pypi-server -a 'download, update' -P ./my_passwords.htaccess
+                          
+                          To disable authentication, use:
+                          
+                            pypi-server -a . -P .
+                          
+                          See the `-P` option for configuring users and passwords.
+                          
+                          Note that when uploads are not protected, the `register` command is not necessary, but `~/.pypirc` still needs username and
+                          password fields, even if bogus.
+    -P PASSWORD_FILE, --passwords PASSWORD_FILE
+                          Use an apache htpasswd file PASSWORD_FILE to set usernames and passwords for authentication.
+                          
+                          To allow unauthorized access, use:
+                          
+                            pypi-server -a . -P .
+                          
+    --disable-fallback    Disable the default redirect to PyPI for packages not found in the local index.
+    --fallback-url FALLBACK_URL
+                          Redirect to FALLBACK_URL for packages not found in the local index.
+    --health-endpoint HEALTH_ENDPOINT
+                          Configure a custom liveness endpoint.
+                          It always returns 200 Ok if the service is up.
+                          Otherwise, it means that the service is not responsive.
+    --server METHOD       Use METHOD to run the server. Valid values include paste, cherrypy, twisted, gunicorn, gevent, wsgiref, and auto. The default is to
+                          use "auto", which chooses one of paste, cherrypy, twisted, or wsgiref.
+    -o, --overwrite       Allow overwriting existing package files during upload.
+    --welcome HTML_FILE   Use the contents of HTML_FILE as a custom welcome message on the home page.
+    --cache-control AGE   Add "Cache-Control: max-age=AGE" header to package downloads. Pip 6+ requires this for caching. AGE is specified in seconds.
+    --log-req-frmt FORMAT
+                          A format-string selecting Http-Request properties to log; set to '%s' to see them all.
+    --log-res-frmt FORMAT
+                          A format-string selecting Http-Response properties to log; set to '%s' to see them all.
+    --log-err-frmt FORMAT
+                          A format-string selecting Http-Error properties to log; set to '%s' to see them all.
+
+More details about ``pypi-server update``
+-----------------------------------------
+
+Enter ``pypi-server update -h`` in the cmd-line to print a detailed usage
+message *about updating the managed packages*::
+
+  usage: pypi-server update [-h] [-v] [--log-file FILE] [--log-stream STREAM] [--log-frmt FORMAT] [--hash-algo HASH_ALGO]
+                            [--backend {auto,simple-dir,cached-dir}] [--version] [-x] [-d DOWNLOAD_DIRECTORY] [-u] [--blacklist-file IGNORELIST_FILE]
+                            [package_directory [package_directory ...]]
+
+  positional arguments:
+    package_directory     The directory from which to serve packages.
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -v, --verbose         Enable verbose logging; repeat for more verbosity.
+    --log-file FILE       Write logging info into this FILE, as well as to stdout or stderr, if configured.
+    --log-stream STREAM   Log messages to the specified STREAM. Valid values are stdout, stderr, and none
+    --log-frmt FORMAT     The logging format-string. (see `logging.LogRecord` class from standard python library)
+    --hash-algo HASH_ALGO
+                          Any `hashlib` available algorithm to use for generating fragments on package links. Can be disabled with one of (0, no, off,
+                          false).
+    --backend {auto,simple-dir,cached-dir}
+                          A backend implementation. Keep the default 'auto' to automatically determine whether to activate caching or not
+    --version             show program's version number and exit
+    -x, --execute         Execute the pip commands rather than printing to stdout
+    -d DOWNLOAD_DIRECTORY, --download-directory DOWNLOAD_DIRECTORY
+                          Specify a directory where packages updates will be downloaded. The default behavior is to use the directory which contains the
+                          package being updated.
+    -u, --allow-unstable  Allow updating to unstable versions (alpha, beta, rc, dev, etc.)
+    --blacklist-file IGNORELIST_FILE, --ignorelist-file IGNORELIST_FILE
+                          Don't update packages listed in this file (one package name per line, without versions, '#' comments honored). This can be useful
+                          if you upload private packages into pypiserver, but also keep a mirror of public packages that you regularly update. Attempting to
+                          pull an update of a private package from `pypi.org` might pose a security risk - e.g. a malicious user might publish a higher
+                          version of the private package, containing arbitrary code.
+
+Client-Side Configurations
+==========================
+
+Always specifying the the pypi url on the command line is a bit
+cumbersome. Since ``pypiserver`` redirects ``pip/easy_install`` to the
+``pypi.org`` index if it doesn't have a requested package, it is a
+good idea to configure them to always use your local pypi index.
+
+Configuring ``pip``
+-------------------
+
+For ``pip`` command this can be done by setting the environment variable
+``PIP_EXTRA_INDEX_URL`` in your ``.bashr/.profile/.zshrc``::
+
+  export PIP_EXTRA_INDEX_URL=http://localhost:8080/simple/
+
+or by adding the following lines to ``~/.pip/pip.conf``::
+
+  [global]
+  extra-index-url = http://localhost:8080/simple/
+
+.. Note::
+   If you have installed ``pypiserver`` on a remote url without *https*
+   you will receive an "untrusted" warning from *pip*, urging you to append
+   the ``--trusted-host`` option.  You can also include this option permanently
+   in your configuration-files or environment variables.
+
+Configuring ``easy_install``
+----------------------------
+
+For ``easy_install`` command you may set the following configuration in
+``~/.pydistutils.cfg``::
+
+  [easy_install]
+  index_url = http://localhost:8080/simple/
+
+
+Uploading Packages Remotely
+===========================
+
+Instead of copying packages directly to the server's folder (i.e. with ``scp``),
+you may use python tools for the task, e.g. ``python setup.py upload``.
+In that case, ``pypiserver`` is responsible for authenticating the upload-requests.
+
+.. Note::
+  We strongly advise to password-protected your uploads!
+
+  It is possible to disable authentication for uploads (e.g. in intranets).
+  To avoid lazy security decisions, read help for ``-P`` and ``-a`` options.
+
+*Apache*-Like Authentication (``htpasswd``)
+-------------------------------------------
+
+#. First make sure you have the *passlib* module installed (note that
+   ``passlib>=1.6`` is required), which is needed for parsing the Apache
+   *htpasswd* file specified by the ``-P``, ``--passwords`` option
+   (see next steps)::
+
+     pip install passlib
+
+#. Create the Apache *htpasswd* file with at least one user/password pair
+   with this command (you'll be prompted for a password)::
+
+     htpasswd -sc htpasswd.txt <some_username>
+
+   .. Tip:: Read this SO question for running `htpasswd` cmd
+      under *Windows*:
+
+         http://serverfault.com/questions/152950/how-to-create-and-edit-htaccess-and-htpasswd-locally-on-my-computer-and-then-u
+
+      or if you have bogus passwords that you don't care because they are for
+      an internal service (which is still "bad", from a security perspective...)
+      you may use this public service:
+
+         http://www.htaccesstools.com/htpasswd-generator/
+
+   .. Tip:: When accessing pypiserver via the api, alternate authentication
+      methods are available via the ``auther`` config flag. Any callable
+      returning a boolean can be passed through to the pypiserver config in
+      order to provide custom authentication. For example, to configure
+      pypiserver to authenticate using the `python-pam`_::
+
+        import pam
+        pypiserver.default_config(auther=pam.authenticate)
+
+      Please see `Using Ad-hoc authentication providers`_ for more information.
+
+#. You  need to restart the server with the ``-P`` option only once
+   (but user/password pairs can later be added or updated on the fly)::
+
+     ./pypi-server run -p 8080 -P htpasswd.txt ~/packages &
+
+Upload with ``setuptools``
+--------------------------
+
+#. On client-side, edit or create a ``~/.pypirc`` file with a similar content::
+
+     [distutils]
+     index-servers =
+       pypi
+       local
+
+     [pypi]
+     username:<your_pypi_username>
+     password:<your_pypi_passwd>
+
+     [local]
+     repository: http://localhost:8080
+     username: <some_username>
+     password: <some_passwd>
+
+#. Then from within the directory of the python-project you wish to upload,
+   issue this command::
+
+     python setup.py sdist upload -r local
+
+Upload with ``twine``
+---------------------
+
+To avoid storing you passwords on disk, in clear text, you may either:
+
+- use the ``register`` *setuptools*'s command with the ``-r`` option,
+  like that::
+
+     python setup.py sdist register -r local upload -r local
+
+- use `twine`_ library, which
+  breaks the procedure in two steps.  In addition, it supports signing
+  your files with PGP-Signatures and uploading the generated `.asc` files
+  to ``pypiserver``::
+
+     twine upload -r local --sign -identity user_name ./foo-1.zip
+
+
+Using the Docker Image
+======================
+
+Starting with version 1.2.5, official Docker images will be built for each
+push to master, each dev, alpha, or beta release, and each final release.
+The most recent full release will always be available under the tag ``latest``,
+and the current master branch will always be available under the tag
+``unstable``.
+
+You can always check to see what tags are currently available at our
+`Docker Repo`_.
+
+To run the most recent release of ``pypiserver`` with Docker, simply::
+
+    docker run pypiserver/pypiserver:latest run
+
+This starts ``pypiserver`` serving packages from the ``/data/packages``
+directory inside the container, listening on the container port 8080.
+
+The container takes all the same arguments as the normal ``pypi-server``
+executable, with the exception of the internal container port (``-p``),
+which will always be 8080.
+
+Of course, just running a container isn't that interesting. To map
+port 80 on the host to port 8080 on the container::
+
+    docker run -p 80:8080 pypiserver/pypiserver:latest run
+
+You can now access your ``pypiserver`` at ``localhost:80`` in a web browser.
+
+To serve packages from a directory on the host, e.g. ``~/packages``::
+
+    docker run -p 80:8080 -v ~/packages:/data/packages pypiserver/pypiserver:latest run
+
+To authenticate against a local ``.htpasswd`` file::
+
+    docker run -p 80:8080 -v ~/.htpasswd:/data/.htpasswd pypiserver/pypiserver:latest run -P .htpasswd packages
+
+You can also specify ``pypiserver`` to run as a Docker service using a
+composefile. An example composefile is `provided <docker-compose.yml>`_.
+
+
+.. _`docker repo`: https://hub.docker.com/r/pypiserver/pypiserver/tags/
+
+
+Alternative Installation Methods
+================================
+
+When trying the methods below, first use the following command to check whether
+previous versions of ``pypiserver`` already exist, and (optionally) uninstall them::
+
+  # VERSION-CHECK: Fails if not installed.
+  pypi-server --version
+
+  # UNINSTALL: Invoke again until it fails.
+  pip uninstall pypiserver
+
+Installing the Very Latest Version
+----------------------------------
+
+In case the latest version in *pypi* is a pre-release, you have to use
+*pip*'s `--pre` option.  And to update an existing installation combine it
+with `--ignore-installed`::
+
+  pip install pypiserver --pre -I
+
+You can even install the latest ``pypiserver`` directly from *github* with the
+following command, assuming you have *git* installed on your ``PATH``::
+
+  pip install git+git://github.com/pypiserver/pypiserver.git
+
+
+Recipes
+=======
+
+Managing the Package Directory
+------------------------------
+
+The ``pypi-server`` command has the ``update`` command that searches for updates of
+available packages. It scans the package directory for available
+packages and searches on pypi.org for updates. Without further
+options ``pypi-server update`` will just print a list of commands which must
+be run in order to get the latest version of each package. Output
+looks like::
+
+    $ ./pypi-server update 
+    checking 106 packages for newer version
+
+    .........u.e...........e..u.............
+    .....e..............................e...
+    ..........................
+
+    no releases found on pypi for PyXML, Pymacs, mercurial, setuptools
+
+    # update raven from 1.4.3 to 1.4.4
+    pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror raven==1.4.4
+
+    # update greenlet from 0.3.3 to 0.3.4
+    pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror greenlet==0.3.4
+
+It first prints for each package a single character after checking the
+available versions on pypi. A dot(`.`) means the package is up-to-date, ``'u'``
+means the package can be updated and ``'e'`` means the list of releases on
+pypi is empty. After that it shows a *pip* command line which can be used
+to update a one package. Either copy and paste that or run
+``pypi-server update -x`` in order to really execute those commands. You need
+to have *pip* installed for that to work however.
+
+Specifying an additional ``-u`` option will also allow alpha, beta and
+release candidates to be downloaded. Without this option these
+releases won't be considered.
+
+Serving Thousands of Packages
+-----------------------------
+
+By default, ``pypiserver`` scans the entire packages directory each time an
+incoming HTTP request occurs. This isn't a problem for a small number of
+packages, but causes noticeable slow-downs when serving thousands of packages.
+
+If you run into this problem, significant speedups can be gained by enabling
+pypiserver's directory caching functionality. The only requirement is to
+install the ``watchdog`` package, or it can be installed during ``pypiserver``
+installation, by specifying the ``cache`` extras option::
+
+    pip install pypiserver[cache]
+
+Additional speedups can be obtained by using your webserver's builtin
+caching functionality. For example, if you are using `nginx` as a
+reverse-proxy as described below in `Behind a reverse proxy`_, you can
+easily enable caching. For example, to allow nginx to cache up to
+10 gigabytes of data for up to 1 hour::
+
+    proxy_cache_path /data/nginx/cache
+                     levels=1:2
+                     keys_zone=pypiserver_cache:10m
+                     max_size=10g
+                     inactive=60m
+                     use_temp_path=off;
+
+    server {
+        # ...
+        location / {
+            proxy_cache pypiserver_cache;
+            proxy_pass http://localhost:8080;
+        }
+    }
+
+Using webserver caching is especially helpful if you have high request
+volume. Using `nginx` caching, a real-world pypiserver installation was
+able to easily support over 1000 package downloads/min at peak load.
+
+Managing Automated Startup
+--------------------------
+
+There are a variety of options for handling the automated starting of
+pypiserver upon system startup. Two of the most common are *systemd* and
+*supervisor* for linux systems. For windows creating services with scripts isn't
+an easy task without a third party tool such as *NSSM*.
+
+Running As a ``systemd`` Service
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``systemd`` is installed by default on most modern Linux systems and as such,
+it is an excellent option for managing the pypiserver process. An example
+config file for ``systemd`` can be seen below::
+
+    [Unit]
+    Description=A minimal PyPI server for use with pip/easy_install.
+    After=network.target
+
+    [Service]
+    Type=simple
+    # systemd requires absolute path here too.
+    PIDFile=/var/run/pypiserver.pid
+    User=www-data
+    Group=www-data
+
+    ExecStart=/usr/local/bin/pypi-server run -p 8080 -a update,download --log-file /var/log/pypiserver.log -P /etc/nginx/.htpasswd /var/www/pypi
+    ExecStop=/bin/kill -TERM $MAINPID
+    ExecReload=/bin/kill -HUP $MAINPID
+    Restart=always
+
+    WorkingDirectory=/var/www/pypi
+
+    TimeoutStartSec=3
+    RestartSec=5
+
+    [Install]
+    WantedBy=multi-user.target
+
+Adjusting the paths and adding this file as ``pypiserver.service`` into your
+``systemd/system`` directory will allow management of the pypiserver process with
+``systemctl``, e.g. ``systemctl start pypiserver``.
+
+More useful information about *systemd* can be found at
+https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units
+
+Launching through ``supervisor``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+`supervisor <http://supervisord.org/>`_ has the benefit of being a pure python
+package and as such, it provides excellent cross-platform support for process
+management. An example configuration file for ``supervisor`` is given below::
+
+    [program:pypi]
+    command=/home/pypi/pypi-venv/bin/pypi-server run -p 7001 -P /home/pypi/.htpasswd /home/pypi/packages
+    directory=/home/pypi
+    user=pypi
+    autostart=true
+    autorestart=true
+    stderr_logfile=/var/log/pypiserver.err.log
+    stdout_logfile=/var/log/pypiserver.out.log
+
+From there, the process can be managed via ``supervisord`` using ``supervisorctl``.
+
+Running As a service with ``NSSM`` (Windows)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Download NSSM from https://nssm.cc unzip to a desired location such as Program Files. Decide whether you are going
+to use win32 or win64, and add that exe to environment PATH.
+
+Create a start_pypiserver.bat::
+
+    pypi-server run -p 8080 C:\Path\To\Packages &
+
+Test the batch file by running it first before creating the service. Make sure you can access
+the server remotely, and install packages. If you can, proceed, if not troubleshoot until you can.
+This will ensure you know the server works, before adding NSSM into the mix.
+
+From the command prompt::
+
+    nssm install pypiserver
+
+This command will launch a NSSM gui application::
+
+    Path: C:\Path\To\start_pypiserver.bat
+    Startup directory: Auto generates when selecting path
+    Service name: pypiserver
+
+There are more tabs, but that is the basic setup. If the service needs to be running with a certain
+login credentials, make sure you enter those credentials in the logon tab.
+
+Start the service::
+
+    nssm start pypiserver
+
+Other useful commands::
+
+    nssm --help
+    nssm stop <servicename>
+    nssm restart <servicename>
+    nssm status <servicename>
+
+For detailed information please visit https://nssm.cc
+
+Using a Different WSGI Server
+-----------------------------
+
+- The ``bottle`` web-server which supports many WSGI-servers, among others,
+  ``paste``, ``cherrypy``, ``twisted`` and ``wsgiref`` (part of Python); you select
+  them using the ``--server`` flag.
+
+- You may view all supported WSGI servers using the following interactive code::
+
+    >>> from pypiserver import bottle
+    >>> list(bottle.server_names.keys())
+    ['cgi', 'gunicorn', 'cherrypy', 'eventlet', 'tornado', 'geventSocketIO',
+    'rocket', 'diesel', 'twisted', 'wsgiref', 'fapws3', 'bjoern', 'gevent',
+    'meinheld', 'auto', 'aiohttp', 'flup', 'gae', 'paste', 'waitress']
+
+- If none of the above servers matches your needs, invoke just the
+  ``pypiserver:app()`` method which returns the internal WSGI-app WITHOUT
+  starting-up a server - you may then send it to any WSGI server you like.
+  Read also the `Utilizing the API`_ section.
+
+- Some examples are given below - you may find more details in `bottle
+  site <http://bottlepy.org/docs/dev/deployment.html#switching-the-server-backend>`_.
+
+Apache (``mod_wsgi``)
+~~~~~~~~~~~~~~~~~~~~~
+
+To use your *Apache2* with ``pypiserver``, prefer to utilize ``mod_wsgi`` as
+explained in `bottle's documentation <http://bottlepy.org/docs/dev/deployment.html#apache-mod-wsgi>`_.
+
+.. Note::
+   If you choose instead to go with ``mod_proxy``, mind that you may bump into problems
+   with the prefix-path (see `#155 <https://github.com/pypiserver/pypiserver/issues/155>`_).
+
+1. Adapt and place the following *Apache* configuration either into top-level scope,
+   or inside some ``<VirtualHost>`` (contributed by Thomas Waldmann)::
+
+        WSGIScriptAlias   /     /yoursite/wsgi/pypiserver-wsgi.py
+        WSGIDaemonProcess       pypisrv user=pypisrv group=pypisrv umask=0007 \
+                                processes=1 threads=5 maximum-requests=500 \
+                                display-name=wsgi-pypisrv inactivity-timeout=300
+        WSGIProcessGroup        pypisrv
+        WSGIPassAuthorization On    # Required for authentication (https://github.com/pypiserver/pypiserver/issues/288)
+
+        <Directory /yoursite/wsgi >
+            Require all granted
+        </Directory>
+
+   or if using older ``Apache < 2.4``, substitute the last part with this::
+
+        <Directory /yoursite/wsgi >
+            Order deny,allow
+            Allow from all
+        </Directory>
+
+2. Then create the ``/yoursite/cfg/pypiserver.wsgi`` file and make sure that
+   the ``user`` and ``group`` of the ``WSGIDaemonProcess`` directive
+   (``pypisrv:pypisrv`` in the example) have the read permission on it::
+
+        import pypiserver
+
+        conf = pypiserver.default_config(
+            root =          "/yoursite/packages",
+            password_file = "/yoursite/htpasswd", )
+        application = pypiserver.app(**conf)
+
+
+   .. Tip::
+      If you have installed ``pypiserver`` in a virtualenv, follow ``mod_wsgi``'s
+      `instructions <http://modwsgi.readthedocs.io/en/develop/user-guides/virtual-environments.html>`_
+      and prepend the python code above with the following::
+
+            import site
+
+            site.addsitedir('/yoursite/venv/lib/pythonX.X/site-packages')
+
+.. Note::
+   For security reasons, notice that the ``Directory`` directive grants access
+   to a directory holding the ``wsgi`` start-up script, alone; nothing else.
+
+.. Note::
+   To enable HTTPS support on Apache, configure the directive that contains the
+   WSGI configuration to use SSL.
+
+``gunicorn``
+~~~~~~~~~~~~
+
+The following command uses ``gunicorn`` to start ``pypiserver``::
+
+  gunicorn -w4 'pypiserver:app(root="/home/ralf/packages")'
+
+or when using multiple roots::
+
+  gunicorn -w4 'pypiserver:app(root=["/home/ralf/packages", "/home/ralf/experimental"])'
+
+``paste``
+~~~~~~~~~
+
+`paste <http://pythonpaste.org/>`_ allows to run multiple WSGI applications
+under different URL paths. Therefore it is possible to serve different set
+of packages on different paths.
+
+The following example ``paste.ini`` could be used to serve stable and
+unstable packages on different paths::
+
+    [composite:main]
+    use = egg:Paste#urlmap
+    /unstable/ = unstable
+    / = stable
+
+    [app:stable]
+    use = egg:pypiserver#main
+    root = ~/stable-packages
+
+    [app:unstable]
+    use = egg:pypiserver#main
+    root = ~/stable-packages
+       ~/unstable-packages
+
+    [server:main]
+    use = egg:gunicorn#main
+    host = 0.0.0.0
+    port = 9000
+    workers = 5
+    accesslog = -
+
+.. Note::
+   You need to install some more dependencies for this to work, like::
+
+        pip install paste pastedeploy gunicorn pypiserver
+
+   The server can then start with::
+
+        gunicorn_paster paste.ini
+
+
+Behind a Reverse Proxy
+----------------------
+
+You can run ``pypiserver`` behind a reverse proxy as well.
+
+Nginx
+~~~~~
+
+Extend your nginx configuration::
+
+    upstream pypi {
+      server              pypiserver.example.com:12345 fail_timeout=0;
+    }
+
+    server {
+      server_name         myproxy.example.com;
+
+      location / {
+        proxy_set_header  Host $host:$server_port;
+        proxy_set_header  X-Forwarded-Proto $scheme;
+        proxy_set_header  X-Real-IP $remote_addr;
+        proxy_pass        http://pypi;
+      }
+    }
+
+As of pypiserver 1.3, you may also use the `X-Forwarded-Host` header in your
+reverse proxy config to enable changing the base URL. For example if you
+want to host pypiserver under a particular path on your server::
+
+    upstream pypi {
+      server              localhost:8000;
+    }
+
+    server {
+      location /pypi/ {
+          proxy_set_header  X-Forwarded-Host $host:$server_port/pypi;
+          proxy_set_header  X-Forwarded-Proto $scheme;
+          proxy_set_header  X-Forwarded-For $proxy_add_x_forwarded_for;
+          proxy_set_header  X-Real-IP $remote_addr;
+          proxy_pass        http://pypi;
+      }
+    }
+
+Supporting HTTPS
+~~~~~~~~~~~~~~~~
+
+Using a reverse proxy is the preferred way of getting pypiserver behind
+HTTPS. For example, to put pypiserver behind HTTPS on port 443, with
+automatic HTTP redirection, using `nginx`::
+
+    upstream pypi {
+      server               localhost:8000;
+    }
+
+    server {
+      listen              80 default_server;
+      server_name         _;
+      return              301 https://$host$request_uri;
+    }
+
+    server {
+      listen              443 ssl;
+      server_name         pypiserver.example.com;
+
+      ssl_certificate     /etc/star.example.com.crt;
+      ssl_certificate_key /etc/star.example.com.key;
+      ssl_protocols       TLSv1 TLSv1.1 TLSv1.2;
+      ssl_ciphers         HIGH:!aNULL:!MD5;
+
+      location / {
+        proxy_set_header  Host $host:$server_port;
+        proxy_set_header  X-Forwarded-Proto $scheme;
+        proxy_set_header  X-Real-IP $remote_addr;
+        proxy_pass        http://pypi;
+      }
+    }
+
+Please see `nginx's HTTPS docs for more details <http://nginx.org/en/docs/http/configuring_https_servers.html>`_.
+
+Getting and keeping your certificates up-to-date can be simplified using,
+for example, using `certbot and letsencrypt <https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-18-04>`_.
+
+Traefik
+~~~~~~~
+
+It is also possible to use `Traefik <https://docs.traefik.io/>`_ to put pypiserver behind HTTPS on port 443, with
+automatic HTTP redirection using Docker Compose. Please see the provided `<docker-compose.yml>`_ example for more information.
+
+Utilizing the API
+-----------------
+
+In order to enable ad-hoc authentication-providers or to use WSGI-servers
+not supported by *bottle* out-of-the-box, you needed to launch ``pypiserver``
+via its API.
+
+- The main entry-point for configuring ``pypiserver`` is the `pypiserver:app()
+  <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L116>`_
+  function.  This function returns the internal WSGI-app that you my then
+  send to any WSGI-server you like.
+
+- To get all ``pypiserver:app()`` keywords and their explanations, read the
+  function `pypiserver:default_config()
+  <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L35>`_.
+
+- Finally, to fire-up a WSGI-server with the configured app, invoke
+  the ``bottle:run(app, host, port, server)`` function.
+  Note that ``pypiserver`` ships with it is own copy of *bottle*; to use it,
+  import it like that: ``from pypiserver import bottle``
+
+Using Ad-Hoc Authentication Providers
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The ``auther`` keyword of ``pypiserver:app()`` function maybe set only using
+the API. This can be any callable that returns a boolean when passed
+the *username* and the *password* for a given request.
+
+For example, to authenticate users based on the ``/etc/passwd`` file under Unix,
+you may delegate such decisions to the `python-pam`_ library by following
+these steps:
+
+1. Ensure ``python-pam`` module is installed::
+
+    pip install python-pam
+
+2. Create a python-script along these lines::
+
+    $ cat > pypiserver-start.py
+    import pypiserver
+    from pypiserver import bottle
+    import pam
+    app = pypiserver.app(root='./packages', auther=pam.authenticate)
+    bottle.run(app=app, host='0.0.0.0', port=80, server='auto')
+
+    [Ctrl+ D]
+
+3. Invoke the python-script to start-up ``pypiserver``::
+
+    $ python pypiserver-start.py
+
+
+.. Note::
+   The `python-pam`_ module, requires *read* access to ``/etc/shadow`` file;
+   you may add the user under which ``pypiserver`` runs into the *shadow*
+   group, with a command like this: ``sudo usermod -a -G shadow pypy-user``.
+
+Use with MicroPython
+--------------------
+The MicroPython interpreter for embedded devices can install packages with the
+module ``upip.py``. The module uses a specialized json-endpoint to retrieve
+package information. This endpoint is supported by ``pypiserver``.
+
+It can be tested with the UNIX port of ``micropython``::
+
+    cd micropython
+    ports/unix/micropython -m tools.upip install -i http://my-server:8080 -p /tmp/mymodules micropython-foobar
+
+Installing packages from the REPL of an embedded device works in this way:
+
+.. code-block:: python
+
+    import network
+    import upip
+
+    sta_if = network.WLAN(network.STA_IF)
+    sta_if.active(True)
+    sta_if.connect('<your ESSID>', '<your password>')
+    upip.index_urls = ["http://my-server:8080"]
+    upip.install("micropython-foobar")
+
+Further information on micropython-packaging can be found here: https://docs.micropython.org/en/latest/reference/packages.html
+
+Custom Health Check Endpoint
+----------------------------
+
+``pypiserver`` provides a default health endpoint at ``/health``. It always returns
+``200 Ok`` if the service is up. Otherwise, it means that the service is not responsive.
+
+In addition, ``pypiserver`` allows users to customize the health endpoint.
+Alphanumeric characters, hyphens, forward slashes and underscores are allowed
+and the endpoint should not overlap with any existing routes.
+Valid examples: ``/healthz``, ``/health/live-1``, ``/api_health``, ``/action/health``
+
+Configure a custom health endpoint by CLI arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Run pypiserver with ``--health-endpoint`` argument::
+
+    pypi-server run --health-endpoint /action/health
+
+Configure a custom health endpoint by script
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    import pypiserver
+    from pypiserver import bottle
+    app = pypiserver.app(root="./packages", health_endpoint="/action/health")
+    bottle.run(app=app, host="0.0.0.0", port=8080, server="auto")
+
+Try ``curl http://localhost:8080/action/health``
+
+
+Sources
+=======
+
+To create a copy of the repository, use::
+
+    git clone https://github.com/pypiserver/pypiserver.git
+    cd pypiserver
+
+To receive any later changes, in the above folder use::
+
+    git pull
+
+
+Known Limitations
+=================
+
+``pypiserver`` does not implement the full API as seen on PyPI_. It
+implements just enough to make ``easy_install``, ``pip install``, and
+``search`` work.
+
+The following limitations are known:
+
+- Command ``pypi -U`` that compares uploaded packages with *pypi* to see if
+  they are outdated, does not respect a http-proxy environment variable
+  (see `#19 <https://github.com/pypiserver/pypiserver/issues/19>`_).
+- It accepts documentation uploads but does not save them to
+  disk (see `#47 <https://github.com/pypiserver/pypiserver/issues/47>`_ for a
+  discussion)
+- It does not handle misspelled packages as *pypi-repo* does,
+  therefore it is suggested to use it with ``--extra-index-url`` instead
+  of ``--index-url`` (see `#38 <https://github.com/pypiserver/pypiserver/issues/38>`_).
+
+Please use Github's `bugtracker <https://github.com/pypiserver/pypiserver/issues>`_
+for other bugs you find.
+
+
+Similar Projects
+================
+
+There are lots of other projects, which allow you to run your own
+PyPI server. If ``pypiserver`` doesn't work for you, the following are
+among the most popular alternatives:
+
+- `devpi-server <https://pypi.org/project/devpi/>`_:
+  a reliable fast pypi.org caching server, part of
+  the comprehensive `github-style pypi index server and packaging meta tool
+  <https://pypi.org/project/devpi/>`_.
+  (version: 2.1.4, access date: 8/3/2015)
+
+- Check this SO question: `How to roll my own pypi
+  <http://stackoverflow.com/questions/1235331/how-to-roll-my-own-pypi>`_
+
+
+Unmaintained or archived
+------------------------
+
+These projects were once alternatives to pypiserver but are now either unmaintained or archived.
+
+- `pip2pi <https://github.com/wolever/pip2pi>`_
+  a simple cmd-line tool that builds a PyPI-compatible local folder from pip requirements
+
+- `flask-pypi-proxy <http://flask-pypi-proxy.readthedocs.org/>`_
+  A proxy for PyPI that also enables also uploading custom packages.
+
+
+Related Software
+================
+
+Though not direct alternatives for ``pypiserver``'s use as an index
+server, the following is a list of related software projects that you
+may want to familiarize with:
+
+- `pypi-uploader`_:
+  A command-line utility to upload packages to your ``pypiserver`` from pypi without
+  having to store them locally first.
+
+- `twine`_:
+  A command-line utility for interacting with PyPI or ``pypiserver``.
+
+- `warehouse`_:
+  the software that powers PyPI_ itself. It is not generally intended to
+  be run by end-users.
+
+Licensing
+=========
+
+``pypiserver`` contains a copy of bottle_ which is available under the
+MIT license, and the remaining part is distributed under the zlib/libpng license.
+See the ``LICENSE.txt`` file.
+
+
+.. _bottle: http://bottlepy.org
+.. _PyPA: https://www.pypa.io/en/latest/
+.. _PyPI: https://pypi.org
+.. _Warehouse: https://github.com/pypa/warehouse/
+.. _twine: https://pypi.org/project/twine/
+.. _pypi-uploader: https://pypi.org/project/pypi-uploader/
+.. _python-pam: https://pypi.org/project/python-pam/
+.. |test-status| image:: https://github.com/pypiserver/pypiserver/actions/workflows/ci.yml/badge.svg
+    :alt: test status
+    :scale: 100%
+    :target: https://github.com/pypiserver/pypiserver/actions/workflows/ci.yml
+
+.. |pypi-ver| image::  https://img.shields.io/pypi/v/pypiserver.svg
+    :target: https://pypi.org/project/pypiserver/
+    :alt: Latest Version in PyPI
+
+.. |python-ver| image:: https://img.shields.io/pypi/pyversions/pypiserver.svg
+    :target: https://pypi.org/project/pypiserver/
+    :alt: Supported Python versions
+
+.. |proj-license| image:: https://img.shields.io/badge/license-BSD%2Bzlib%2Flibpng-blue.svg
+    :target: https://raw.githubusercontent.com/pypiserver/pypiserver/master/LICENSE.txt
+    :alt: Project License
+
+.. |dependencies| image:: https://img.shields.io/requires/github/pypiserver/pypiserver.svg
+    :target: https://requires.io/github/pypiserver/pypiserver/requirements/
+    :alt: Dependencies up-to-date?
```

## Comparing `pypiserver-1.5.1/tox.ini` & `pypiserver-1.5.2/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py36, py37, py38, py39, pypy3
+envlist = py36, py37, py38, py39, py310, py311, pypy3
 
 [testenv]
 deps=-r{toxinidir}/requirements/test.pip
 allowlist_externals=
     /bin/sh
 sitepackages=False
 commands=
```

## Comparing `pypiserver-1.5.1/buildout.cfg` & `pypiserver-1.5.2/buildout.cfg`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/setup.cfg` & `pypiserver-1.5.2/setup.cfg`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/setup.py` & `pypiserver-1.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from setuptools import setup
 
 tests_require = [
     "pytest>=2.3",
     "tox",
     "twine",
-    "pip>=7",
     "passlib>=1.6",
     "webtest",
 ]
 
 setup_requires = ["setuptools", "setuptools-git >= 0.3", "wheel >= 0.25.0"]
+install_requires = ["pip>=7"]
 
 
 def read_file(rel_path: str):
     return Path(__file__).parent.joinpath(rel_path).read_text()
 
 
 def get_version():
@@ -41,14 +41,15 @@
     name="pypiserver",
     description="A minimal PyPI server for use with pip/easy_install.",
     long_description=read_file("README.rst"),
     version=get_version(),
     packages=["pypiserver"],
     package_data={"pypiserver": ["welcome.html"]},
     python_requires=">=3.6",
+    install_requires=install_requires,
     setup_requires=setup_requires,
     extras_require={"passlib": ["passlib>=1.6"], "cache": ["watchdog"]},
     tests_require=tests_require,
     url="https://github.com/pypiserver/pypiserver",
     maintainer=(
         "Kostis Anagnostopoulos <ankostis@gmail.com>"
         "Matthew Planchard <mplanchard@gmail.com>"
@@ -65,14 +66,16 @@
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Build Tools",
         "Topic :: System :: Software Distribution",
     ],
     zip_safe=True,
     entry_points={
```

## Comparing `pypiserver-1.5.1/CHANGES.rst` & `pypiserver-1.5.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 Changelog
 =========
 
 2.0.0 (tbd)
 -----------
 
-1.5.1rc10-01-2022 (__rc__)
+1.5.2 (2023-07-30)
+--------------------------
+
+- 3f520cd FIX: Add missing pip dependency (#500)
+- 85e065e MAINT: Feat/dependabot (#493)
+- 73dbe15 FIX: Health endpoint usage is missing. (#481)
+- e0c9723 MAINT: Bump waitress from 1.4.4 to 2.1.2 in /docker (#454)
+- a95f456 MAINT: update docs folder (#479)
+- 8cc8e80 MAINT: Update README.rst and config.py (#470)
+- 754b0f4 MAINT: add help output for `run` and `update` to README (#478)
+- 5fd6400 MAINT: Update README to reflect run/update commands (#451)
+- abc4bfb MAINT: Upgrade to psf/black stable style 2023 (#474)
+- 383c936 MAINT: disable tests on Python3.6 (#471)
+- d716d0f FIX: explicit optional types in `config.py` (#472)
+- ae3dcf2 ENH: :stethoscope: allow customized health check endpoint (#442)
+- 2f3b997 FIX: correct 1.5.1 tag date in CHANGES (#457)
+- 4a0c6fb MAINT: from importlib import reload for Python 3 (#448)
+- 0ba44b5 FIX: force setuptools update + no duplicate runs in GH Actions (#445)
+- 530852b MAINT: Support current versions of CPython (#453)
+- 6ea316c MAINT: Upgrade GitHub Actions (#447)
+
+1.5.1 (2022-10-18)
 --------------------------
 
 - 61e4487 ENH: add extremely basic /health endpoint (#396)
 - bbd2a47 FIX: docker tests in cicd (#444)
 - 784a9a1 MAINT: Replace usage of deprecated inspect.getargspec (#436)
 - 640a748 MAINT: Add traefik/ and auth/ dirs to gitignore (#398)
 - a67829e MAINT: Fix typos in README (#431)
```

## Comparing `pypiserver-1.5.1/Makefile` & `pypiserver-1.5.2/Makefile`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/docker-compose.yml` & `pypiserver-1.5.2/docker-compose.yml`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/Dockerfile` & `pypiserver-1.5.2/Dockerfile`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/pkg_helpers.py` & `pypiserver-1.5.2/pypiserver/pkg_helpers.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/cache.py` & `pypiserver-1.5.2/pypiserver/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 try:
     from watchdog.observers import Observer
 
     ENABLE_CACHING = True
 
 except ImportError:
-
     Observer = None
 
     ENABLE_CACHING = False
 
 if t.TYPE_CHECKING:
     from pypiserver.core import PkgFile
```

## Comparing `pypiserver-1.5.1/pypiserver/backend.py` & `pypiserver-1.5.2/pypiserver/backend.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/_app.py` & `pypiserver-1.5.2/pypiserver/_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,14 @@
 
 
 @app.error
 def log_error(http_error):
     log.info(config.log_err_frmt, vars(http_error))
 
 
-@app.route("/health")
-def health():
-    return "Ok"
-
-
 @app.route("/favicon.ico")
 def favicon():
     return HTTPError(404)
 
 
 @app.route("/")
 def root():
```

## Comparing `pypiserver-1.5.1/pypiserver/__main__.py` & `pypiserver-1.5.2/pypiserver/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
     bottle._stderr = ft.partial(  # pylint: disable=protected-access
         _logwrite, logging.getLogger(bottle.__name__), logging.INFO
     )
 
     # Here `app` is a Bottle instance, which we pass to bottle.run() to run
     # the server
     app = pypiserver.app_from_config(config)
+    app = pypiserver.setup_routes_from_config(app, config)
 
     if config.server_method == "gunicorn":
         # When bottle runs gunicorn, gunicorn tries to pull its arguments from
         # sys.argv. Because pypiserver's arguments don't match gunicorn's,
         # this leads to errors.
         # Gunicorn can be configured by using a `gunicorn.conf.py` config file
         # or by specifying the `GUNICORN_CMD_ARGS` env var. See gunicorn
```

## Comparing `pypiserver-1.5.1/pypiserver/config.py` & `pypiserver-1.5.2/pypiserver/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 # Specify defaults here so that we can use them in tests &c. and not need
 # to update things in multiple places if a default changes.
 class DEFAULTS:
     """Config defaults."""
 
     AUTHENTICATE = ["update"]
     FALLBACK_URL = "https://pypi.org/simple/"
+    HEALTH_ENDPOINT = "/health"
     HASH_ALGO = "md5"
     INTERFACE = "0.0.0.0"
     LOG_FRMT = "%(asctime)s|%(name)s|%(levelname)s|%(thread)d|%(message)s"
     LOG_ERR_FRMT = "%(body)s: %(exception)s \n%(traceback)s"
     LOG_REQ_FRMT = "%(bottle.request)s"
     LOG_RES_FRMT = "%(status)s"
     LOG_STREAM = sys.stdout
@@ -130,14 +131,27 @@
     raise argparse.ArgumentTypeError(
         f"Hash algorithm '{arg}' is not available. Please select one "
         f"of {hashlib.algorithms_available}, or turn off hashing by "
         "setting --hash-algo to 'off', '0', or 'false'"
     )
 
 
+def health_endpoint_arg(arg: str) -> str:
+    """Verify the health_endpoint and raises ValueError if invalid."""
+    rule_regex = r"^/[a-z0-9/_-]+$"
+    if re.fullmatch(rule_regex, arg, re.I) is not None:
+        return arg
+
+    raise argparse.ArgumentTypeError(
+        "Invalid path for the health endpoint. Make sure that it contains only "
+        "alphanumeric characters, hyphens, forward slashes and underscores. "
+        f"In other words, make sure to match the following regex: {rule_regex}"
+    )
+
+
 def html_file_arg(arg: t.Optional[str]) -> str:
     """Parse the provided HTML file and return its contents."""
     if arg is None or arg == "pypiserver/welcome.html":
         return pkg_resources.resource_string(__name__, "welcome.html").decode(
             "utf-8"
         )
     with open(arg, "r", encoding="utf-8") as f:
@@ -379,14 +393,23 @@
         default=DEFAULTS.FALLBACK_URL,
         help=(
             "Redirect to FALLBACK_URL for packages not found in the local "
             "index."
         ),
     )
     run_parser.add_argument(
+        "--health-endpoint",
+        default=DEFAULTS.HEALTH_ENDPOINT,
+        type=health_endpoint_arg,
+        help=(
+            "Configure a custom liveness endpoint. It always returns 200 Ok if "
+            "the service is up. Otherwise, it means that the service is not responsive."
+        ),
+    )
+    run_parser.add_argument(
         "--server",
         metavar="METHOD",
         default=DEFAULTS.SERVER_METHOD,
         choices=(
             "auto",
             "cherrypy",
             "gevent",
@@ -426,14 +449,15 @@
     run_parser.add_argument(
         "--cache-control",
         metavar="AGE",
         type=int,
         help=(
             'Add "Cache-Control: max-age=AGE" header to package downloads. '
             "Pip 6+ requires this for caching."
+            "AGE is specified in seconds."
         ),
     )
     run_parser.add_argument(
         "--log-req-frmt",
         metavar="FORMAT",
         default=DEFAULTS.LOG_REQ_FRMT,
         help=(
@@ -594,15 +618,14 @@
             2: logging.DEBUG,
         }
         # Return a log-level from warning through not set (log all messages).
         # If we've specified 3 or more levels of verbosity, just return not set.
         return levels.get(self.verbosity, logging.NOTSET)
 
     def get_backend(self, arg: str) -> IBackend:
-
         available_backends: t.Dict[str, BackendFactory] = {
             "auto": get_file_backend,
             "simple-dir": SimpleFileBackend,
             "cached-dir": CachingFileBackend,
         }
 
         backend = available_backends[arg]
@@ -654,32 +677,34 @@
         self,
         port: int,
         host: str,
         authenticate: t.List[str],
         password_file: t.Optional[str],
         disable_fallback: bool,
         fallback_url: str,
+        health_endpoint: str,
         server_method: str,
         overwrite: bool,
         welcome_msg: str,
         cache_control: t.Optional[int],
         log_req_frmt: str,
         log_res_frmt: str,
         log_err_frmt: str,
-        auther: t.Callable[[str, str], bool] = None,
+        auther: t.Optional[t.Callable[[str, str], bool]] = None,
         **kwargs: t.Any,
     ) -> None:
         """Construct a RuntimeConfig."""
         super().__init__(**kwargs)
         self.port = port
         self.host = host
         self.authenticate = authenticate
         self.password_file = password_file
         self.disable_fallback = disable_fallback
         self.fallback_url = fallback_url
+        self.health_endpoint = health_endpoint
         self.server_method = server_method
         self.overwrite = overwrite
         self.welcome_msg = welcome_msg
         self.cache_control = cache_control
         self.log_req_frmt = log_req_frmt
         self.log_res_frmt = log_res_frmt
         self.log_err_frmt = log_err_frmt
@@ -696,14 +721,15 @@
             **super(RunConfig, cls).kwargs_from_namespace(namespace),
             "port": namespace.port,
             "host": namespace.host,
             "authenticate": namespace.authenticate,
             "password_file": namespace.passwords,
             "disable_fallback": namespace.disable_fallback,
             "fallback_url": namespace.fallback_url,
+            "health_endpoint": namespace.health_endpoint,
             "server_method": namespace.server,
             "overwrite": namespace.overwrite,
             "welcome_msg": namespace.welcome,
             "cache_control": namespace.cache_control,
             "log_req_frmt": namespace.log_req_frmt,
             "log_res_frmt": namespace.log_res_frmt,
             "log_err_frmt": namespace.log_err_frmt,
@@ -798,15 +824,17 @@
         of `RunConfig`.
         """
         default_config = cls.from_args(["run"])
         assert isinstance(default_config, RunConfig)
         return default_config.with_updates(**overrides)
 
     @classmethod
-    def from_args(cls, args: t.Sequence[str] = None) -> Configuration:
+    def from_args(
+        cls, args: t.Optional[t.Sequence[str]] = None
+    ) -> Configuration:
         """Construct a Config from the passed args or sys.argv."""
         # If pulling args from sys.argv (commandline arguments), argv[0] will
         # be the program name, (i.e. pypi-server), so we don't need to
         # worry about it.
         args = args if args is not None else sys.argv[1:]
         parser = get_parser()
```

## Comparing `pypiserver-1.5.1/pypiserver/plugin.py` & `pypiserver-1.5.2/pypiserver/plugin.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/__init__.py` & `pypiserver-1.5.2/pypiserver/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import re as _re
 import sys
 import typing as t
 
 from pypiserver.bottle import Bottle
 from pypiserver.config import Config, RunConfig, strtobool
 
-version = __version__ = "1.5.1"
+version = __version__ = "1.5.2"
 __version_info__ = tuple(_re.split("[.-]", __version__))
-__updated__ = "2022-10-18 16:06:16"
+__updated__ = "2023-07-30 23:18:50"
 
 __title__ = "pypiserver"
 __summary__ = "A minimal PyPI server for use with pip/easy_install."
 __uri__ = "https://github.com/pypiserver/pypiserver"
 
 
 identity = lambda x: x
@@ -117,15 +117,15 @@
 def app(**kwargs: t.Any) -> Bottle:
     """Construct a bottle app running pypiserver.
 
     :param kwds: Any overrides for defaults. Any property of RunConfig
         (or its base), defined in `pypiserver.config`, may be overridden.
     """
     config = Config.default_with_overrides(**backwards_compat_kwargs(kwargs))
-    return app_from_config(config)
+    return setup_routes_from_config(app_from_config(config), config)
 
 
 def app_from_config(config: RunConfig) -> Bottle:
     """Construct a bottle app from the provided RunConfig."""
     # The _app module instantiates a Bottle instance directly when it is
     # imported. That is `_app.app`. We directly mutate some global variables
     # on the imported `_app` module so that its endpoints will behave as
@@ -137,14 +137,28 @@
     _app.config = config
     # Add a reference to our config on the Bottle app for easy access in testing
     # and other contexts.
     _app.app._pypiserver_config = config
     return _app.app
 
 
+def setup_routes_from_config(app: Bottle, config: RunConfig) -> Bottle:
+    """Set up additional routes supplied from the config."""
+
+    def _setup_health_endpoint(app, config):
+        if config.health_endpoint in [route.rule for route in app.routes]:
+            raise RuntimeError(
+                "Provided health endpoint overlaps with existing routes"
+            )
+        app.route(config.health_endpoint, "GET", lambda: "Ok")
+
+    _setup_health_endpoint(app, config)
+    return app
+
+
 T = t.TypeVar("T")
 
 
 def paste_app_factory(_global_config, **local_conf):
     """Parse a paste config and return an app.
 
     The paste config is entirely strings, so we need to parse those
```

## Comparing `pypiserver-1.5.1/pypiserver/welcome.html` & `pypiserver-1.5.2/pypiserver/welcome.html`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/manage.py` & `pypiserver-1.5.2/pypiserver/manage.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/bottle.py` & `pypiserver-1.5.2/pypiserver/bottle.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver/core.py` & `pypiserver-1.5.2/pypiserver/core.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/bin/check_readme.sh` & `pypiserver-1.5.2/bin/check_readme.sh`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/bin/bumpver.py` & `pypiserver-1.5.2/bin/bumpver.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/bin/update_changelog.sh` & `pypiserver-1.5.2/bin/update_changelog.sh`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/bin/ci_helper.py` & `pypiserver-1.5.2/bin/ci_helper.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/bin/README.rst` & `pypiserver-1.5.2/bin/README.rst`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/docker/entrypoint.sh` & `pypiserver-1.5.2/docker/entrypoint.sh`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/docker/README.md` & `pypiserver-1.5.2/docker/README.md`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/docker/test_docker.py` & `pypiserver-1.5.2/docker/test_docker.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/pypiserver.egg-info/PKG-INFO` & `pypiserver-1.5.2/pypiserver.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,1050 +1,14 @@
 Metadata-Version: 2.1
 Name: pypiserver
-Version: 1.5.1
+Version: 1.5.2
 Summary: A minimal PyPI server for use with pip/easy_install.
 Home-page: https://github.com/pypiserver/pypiserver
 Maintainer: Kostis Anagnostopoulos <ankostis@gmail.com>Matthew Planchard <mplanchard@gmail.com>
 Maintainer-email: ankostis@gmail.com
-License: UNKNOWN
-Description: .. -*- mode: rst; coding: utf-8 -*-
-        
-        .. image:: pypiserver_logo.png
-           :width: 300 px
-           :align: center
-        
-        ==============================================================================
-        pypiserver - minimal PyPI server for use with pip/easy_install
-        ==============================================================================
-        |pypi-ver| |test-status| |dependencies| |python-ver| |proj-license|
-        
-        :Version:     1.5.1
-        :Date:        2022-10-18
-        :Source:      https://github.com/pypiserver/pypiserver
-        :PyPI:        https://pypi.org/project/pypiserver/
-        :Tests:       https://github.com/pypiserver/pypiserver/actions
-        :Maintainers: | Kostis Anagnostopoulos <ankostis@gmail.com>,
-                      | Matthew Planchard <mplanchard@gmail.com>,
-                      | Dmitrii Orlov <dmtree.dev@yahoo.com>,
-                      | **Someone new?** We are looking for new maintainers! 
-                        <https://github.com/pypiserver/pypiserver/issues/397>
-        :License:     zlib/libpng + MIT
-        :Community:   https://pypiserver.zulipchat.com
-        
-        Chat with us on `Zulip <https://pypiserver.zulipchat.com>`_!
-        
-        ``pypiserver`` is a minimal PyPI_ compatible server for ``pip`` or ``easy_install``.
-        It is based on bottle_ and serves packages from regular directories.
-        Wheels, bdists, eggs and accompanying PGP-signatures can be uploaded
-        either with ``pip``, ``setuptools``, ``twine``, ``pypi-uploader``, or simply copied
-        with ``scp``.
-        
-        .. note::
-           The official software powering PyPI_ is Warehouse_. However, Warehouse_
-           is fairly specialized to be ``pypi.org``'s own software, and should not
-           be used in other contexts. In particular, it does not officially support
-           being used as a custom package index by users wishing to serve their own
-           packages.
-        
-           ``pypiserver`` implements the same interfaces as `PyPI`_, allowing
-           standard Python packaging tooling such as ``pip`` and ``twine`` to
-           interact with it as a package index just as they would with PyPI_, while
-           making it much easier to get a running index server.
-        
-        .. contents:: Table of Contents
-          :backlinks: top
-        
-        
-        Quickstart: Installation and Usage
-        ==================================
-        
-        ``pypiserver`` works with Python 3.6+ and PyPy3.
-        
-        Older Python versions may still work, but they are not tested.
-        
-        For legacy Python versions, use ``pypiserver-1.x`` series. Note that these are
-        not officially supported, and will not receive bugfixes or new features.
-        
-        .. Tip::
-           The commands below work on a unix-like operating system with a posix shell.
-           The ``'~'`` character expands to user's home directory.
-        
-           If you're using Windows, you'll have to use their "Windows counterparts".
-           The same is true for the rest of this documentation.
-        
-        1. Install ``pypiserver`` with this command::
-        
-            pip install pypiserver                # Or: pypiserver[passlib,cache]
-            mkdir ~/packages                      # Copy packages into this directory.
-        
-           See also `Alternative Installation methods`_.
-        
-        2. Copy some packages into your ``~/packages`` folder and then
-           get your ``pypiserver`` up and running::
-        
-            pypi-server -p 8080 ~/packages &      # Will listen to all IPs.
-        
-        3. From the client computer, type this::
-        
-            # Download and install hosted packages.
-            pip install --extra-index-url http://localhost:8080/simple/ ...
-        
-            # or
-            pip install --extra-index-url http://localhost:8080 ...
-        
-            # Search hosted packages.
-            pip search --index http://localhost:8080 ...
-        
-            # Note that pip search does not currently work with the /simple/ endpoint.
-        
-           See also `Client-side configurations`_ for avoiding tedious typing.
-        
-        4. Enter ``pypi-server -h`` in the cmd-line to print a detailed usage message::
-        
-            pypi-server [OPTIONS] [PACKAGES_DIRECTORY...]
-              start PyPI compatible package server serving packages from
-              PACKAGES_DIRECTORY. If PACKAGES_DIRECTORY is not given on the
-              command line, it uses the default ~/packages. pypiserver scans this
-              directory recursively for packages. It skips packages and
-              directories starting with a dot. Multiple package directories can be
-              specified.
-        
-            pypi-server understands the following options:
-        
-              -p, --port PORT
-                Listen on port PORT (default: 8080).
-        
-              -i, --interface INTERFACE
-                Listen on interface INTERFACE (default: 0.0.0.0, any interface).
-        
-              -a, --authenticate (update|download|list), ...
-                Comma-separated list of (case-insensitive) actions to authenticate.
-                Requires to have set the password (-P option).
-                To password-protect package downloads (in addition to uploads) while
-                leaving listings public, use:
-                  -P foo/htpasswd.txt -a update,download
-                To allow unauthorized access, use:
-                  -P . -a .
-                Note that when uploads are not protected, the `register` command
-                is not necessary, but `~/.pypirc` still need username and password fields,
-                even if bogus.
-                By default, only 'update' is password-protected.
-        
-              -P, --passwords PASSWORD_FILE
-                Use apache htpasswd file PASSWORD_FILE to set usernames & passwords when
-                authenticating certain actions (see -a option).
-                To allow unauthorized access, use:
-                  -P . -a .
-        
-              --disable-fallback
-                Disable redirect to real PyPI index for packages not found in the
-                local index.
-        
-              --fallback-url FALLBACK_URL
-                For packages not found in the local index, this URL will be used to
-                redirect to (default: https://pypi.org/simple/).
-        
-              --server METHOD
-                Use METHOD to run the server. Valid values include paste,
-                cherrypy, twisted, gunicorn, gevent, wsgiref, auto. The
-                default is to use "auto" which chooses one of paste, cherrypy,
-                twisted or wsgiref.
-        
-              -r, --root PACKAGES_DIRECTORY
-                [deprecated] Serve packages from PACKAGES_DIRECTORY.
-        
-              -o, --overwrite
-                Allow overwriting existing package files.
-        
-              --hash-algo ALGO
-                Any `hashlib` available algo used as fragments on package links.
-                Set one of (0, no, off, false) to disabled it (default: md5).
-        
-              --welcome HTML_FILE
-                Uses the ASCII contents of HTML_FILE as welcome message response.
-        
-              -v
-                Enable verbose logging; repeat for more verbosity.
-        
-              --log-conf <FILE>
-                Read logging configuration from FILE.
-                By default, configuration is read from `log.conf` if found in server's dir.
-        
-              --log-file <FILE>
-                Write logging info into this FILE.
-        
-              --log-frmt <FILE>
-                The logging format-string (see `logging.LogRecord` class from standard python library).
-                [Default: %(asctime)s|%(name)s|%(levelname)s|%(thread)d|%(message)s]
-        
-              --log-req-frmt FORMAT
-                A format-string selecting Http-Request properties to log; set to '%s' to see them all.
-                [Default: %(bottle.request)s]
-        
-              --log-res-frmt FORMAT
-                A format-string selecting Http-Response properties to log; set to  '%s' to see them all.
-                [Default: %(status)s]
-        
-              --log-err-frmt FORMAT
-                A format-string selecting Http-Error properties to log; set to  '%s' to see them all.
-                [Default: %(body)s: %(exception)s \n%(traceback)s]
-        
-              --cache-control AGE
-                Add "Cache-Control: max-age=AGE, public" header to package downloads.
-                Pip 6+ needs this for caching.
-        
-            pypi-server -h, --help
-              Show this help message.
-        
-            pypi-server --version
-              Show pypi-server's version.
-        
-            pypi-server -U [OPTIONS] [PACKAGES_DIRECTORY...]
-              Update packages in PACKAGES_DIRECTORY. This command searches
-              pypi.org for updates and shows a pip command line which
-              updates the package.
-        
-            The following additional options can be specified with -U:
-        
-              -x
-                Execute the pip commands instead of only showing them.
-        
-              -d DOWNLOAD_DIRECTORY
-                Download package updates to this directory. The default is to use
-                the directory which contains the latest version of the package to
-                be updated.
-        
-              -u
-                Allow updating to unstable version (alpha, beta, rc, dev versions).
-        
-            Visit https://github.com/pypiserver/pypiserver for more information.
-        
-        
-        Client-Side Configurations
-        ==========================
-        
-        Always specifying the the pypi url on the command line is a bit
-        cumbersome. Since ``pypiserver`` redirects ``pip/easy_install`` to the
-        ``pypi.org`` index if it doesn't have a requested package, it is a
-        good idea to configure them to always use your local pypi index.
-        
-        Configuring ``pip``
-        -------------------
-        
-        For ``pip`` command this can be done by setting the environment variable
-        ``PIP_EXTRA_INDEX_URL`` in your ``.bashr/.profile/.zshrc``::
-        
-          export PIP_EXTRA_INDEX_URL=http://localhost:8080/simple/
-        
-        or by adding the following lines to ``~/.pip/pip.conf``::
-        
-          [global]
-          extra-index-url = http://localhost:8080/simple/
-        
-        .. Note::
-           If you have installed ``pypiserver`` on a remote url without *https*
-           you will receive an "untrusted" warning from *pip*, urging you to append
-           the ``--trusted-host`` option.  You can also include this option permanently
-           in your configuration-files or environment variables.
-        
-        Configuring ``easy_install``
-        ----------------------------
-        
-        For ``easy_install`` command you may set the following configuration in
-        ``~/.pydistutils.cfg``::
-        
-          [easy_install]
-          index_url = http://localhost:8080/simple/
-        
-        
-        Uploading Packages Remotely
-        ===========================
-        
-        Instead of copying packages directly to the server's folder (i.e. with ``scp``),
-        you may use python tools for the task, e.g. ``python setup.py upload``.
-        In that case, ``pypiserver`` is responsible for authenticating the upload-requests.
-        
-        .. Note::
-          We strongly advise to password-protected your uploads!
-        
-          It is possible to disable authentication for uploads (e.g. in intranets).
-          To avoid lazy security decisions, read help for ``-P`` and ``-a`` options.
-        
-        *Apache*-Like Authentication (``htpasswd``)
-        -------------------------------------------
-        
-        #. First make sure you have the *passlib* module installed (note that
-           ``passlib>=1.6`` is required), which is needed for parsing the Apache
-           *htpasswd* file specified by the ``-P``, ``--passwords`` option
-           (see next steps)::
-        
-             pip install passlib
-        
-        #. Create the Apache *htpasswd* file with at least one user/password pair
-           with this command (you'll be prompted for a password)::
-        
-             htpasswd -sc htpasswd.txt <some_username>
-        
-           .. Tip:: Read this SO question for running `htpasswd` cmd
-              under *Windows*:
-        
-                 http://serverfault.com/questions/152950/how-to-create-and-edit-htaccess-and-htpasswd-locally-on-my-computer-and-then-u
-        
-              or if you have bogus passwords that you don't care because they are for
-              an internal service (which is still "bad", from a security perspective...)
-              you may use this public service:
-        
-                 http://www.htaccesstools.com/htpasswd-generator/
-        
-           .. Tip:: When accessing pypiserver via the api, alternate authentication
-              methods are available via the ``auther`` config flag. Any callable
-              returning a boolean can be passed through to the pypiserver config in
-              order to provide custom authentication. For example, to configure
-              pypiserver to authenticate using the `python-pam`_::
-        
-                import pam
-                pypiserver.default_config(auther=pam.authenticate)
-        
-              Please see `Using Ad-hoc authentication providers`_ for more information.
-        
-        #. You  need to restart the server with the ``-P`` option only once
-           (but user/password pairs can later be added or updated on the fly)::
-        
-             ./pypi-server -p 8080 -P htpasswd.txt ~/packages &
-        
-        Upload with ``setuptools``
-        --------------------------
-        
-        #. On client-side, edit or create a ``~/.pypirc`` file with a similar content::
-        
-             [distutils]
-             index-servers =
-               pypi
-               local
-        
-             [pypi]
-             username:<your_pypi_username>
-             password:<your_pypi_passwd>
-        
-             [local]
-             repository: http://localhost:8080
-             username: <some_username>
-             password: <some_passwd>
-        
-        #. Then from within the directory of the python-project you wish to upload,
-           issue this command::
-        
-             python setup.py sdist upload -r local
-        
-        Upload with ``twine``
-        ---------------------
-        
-        To avoid storing you passwords on disk, in clear text, you may either:
-        
-        - use the ``register`` *setuptools*'s command with the ``-r`` option,
-          like that::
-        
-             python setup.py sdist register -r local upload -r local
-        
-        - use `twine`_ library, which
-          breaks the procedure in two steps.  In addition, it supports signing
-          your files with PGP-Signatures and uploading the generated `.asc` files
-          to ``pypiserver``::
-        
-             twine upload -r local --sign -identity user_name ./foo-1.zip
-        
-        
-        Using the Docker Image
-        ======================
-        
-        Starting with version 1.2.5, official Docker images will be built for each
-        push to master, each dev, alpha, or beta release, and each final release.
-        The most recent full release will always be available under the tag ``latest``,
-        and the current master branch will always be available under the tag
-        ``unstable``.
-        
-        You can always check to see what tags are currently available at our
-        `Docker Repo`_.
-        
-        To run the most recent release of ``pypiserver`` with Docker, simply::
-        
-            docker run pypiserver/pypiserver:latest
-        
-        This starts ``pypiserver`` serving packages from the ``/data/packages``
-        directory inside the container, listening on the container port 8080.
-        
-        The container takes all the same arguments as the normal ``pypi-server``
-        executable, with the exception of the internal container port (``-p``),
-        which will always be 8080.
-        
-        Of course, just running a container isn't that interesting. To map
-        port 80 on the host to port 8080 on the container::
-        
-            docker run -p 80:8080 pypiserver/pypiserver:latest
-        
-        You can now access your ``pypiserver`` at ``localhost:80`` in a web browser.
-        
-        To serve packages from a directory on the host, e.g. ``~/packages``::
-        
-            docker run -p 80:8080 -v ~/packages:/data/packages pypiserver/pypiserver:latest
-        
-        To authenticate against a local ``.htpasswd`` file::
-        
-            docker run -p 80:8080 -v ~/.htpasswd:/data/.htpasswd pypiserver/pypiserver:latest -P .htpasswd packages
-        
-        You can also specify ``pypiserver`` to run as a Docker service using a
-        composefile. An example composefile is `provided <docker-compose.yml>`_.
-        
-        
-        .. _`docker repo`: https://hub.docker.com/r/pypiserver/pypiserver/tags/
-        
-        
-        Alternative Installation Methods
-        ================================
-        
-        When trying the methods below, first use the following command to check whether
-        previous versions of ``pypiserver`` already exist, and (optionally) uninstall them::
-        
-          # VERSION-CHECK: Fails if not installed.
-          pypi-server --version
-        
-          # UNINSTALL: Invoke again until it fails.
-          pip uninstall pypiserver
-        
-        Installing the Very Latest Version
-        ----------------------------------
-        
-        In case the latest version in *pypi* is a pre-release, you have to use
-        *pip*'s `--pre` option.  And to update an existing installation combine it
-        with `--ignore-installed`::
-        
-          pip install pypiserver --pre -I
-        
-        You can even install the latest ``pypiserver`` directly from *github* with the
-        following command, assuming you have *git* installed on your ``PATH``::
-        
-          pip install git+git://github.com/pypiserver/pypiserver.git
-        
-        Running on Heroku/Dotcloud
-        --------------------------
-        
-        https://github.com/dexterous/pypiserver-on-the-cloud contains
-        instructions on how to run ``pypiserver`` on one of the supported cloud
-        service providers.
-        
-        
-        Recipes
-        =======
-        
-        Managing the Package Directory
-        ------------------------------
-        
-        The ``pypi-server`` command has the ``-U`` option that searches for updates of
-        available packages. It scans the package directory for available
-        packages and searches on pypi.org for updates. Without further
-        options ``pypi-server -U`` will just print a list of commands which must
-        be run in order to get the latest version of each package. Output
-        looks like::
-        
-            $ ./pypi-server -U
-            checking 106 packages for newer version
-        
-            .........u.e...........e..u.............
-            .....e..............................e...
-            ..........................
-        
-            no releases found on pypi for PyXML, Pymacs, mercurial, setuptools
-        
-            # update raven from 1.4.3 to 1.4.4
-            pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror raven==1.4.4
-        
-            # update greenlet from 0.3.3 to 0.3.4
-            pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror greenlet==0.3.4
-        
-        It first prints for each package a single character after checking the
-        available versions on pypi. A dot(`.`) means the package is up-to-date, ``'u'``
-        means the package can be updated and ``'e'`` means the list of releases on
-        pypi is empty. After that it shows a *pip* command line which can be used
-        to update a one package. Either copy and paste that or run
-        ``pypi-server -Ux`` in order to really execute those commands. You need
-        to have *pip* installed for that to work however.
-        
-        Specifying an additional ``-u`` option will also allow alpha, beta and
-        release candidates to be downloaded. Without this option these
-        releases won't be considered.
-        
-        Serving Thousands of Packages
-        -----------------------------
-        
-        By default, ``pypiserver`` scans the entire packages directory each time an
-        incoming HTTP request occurs. This isn't a problem for a small number of
-        packages, but causes noticeable slow-downs when serving thousands of packages.
-        
-        If you run into this problem, significant speedups can be gained by enabling
-        pypiserver's directory caching functionality. The only requirement is to
-        install the ``watchdog`` package, or it can be installed during ``pypiserver``
-        installation, by specifying the ``cache`` extras option::
-        
-            pip install pypiserver[cache]
-        
-        Additional speedups can be obtained by using your webserver's builtin
-        caching functionality. For example, if you are using `nginx` as a
-        reverse-proxy as described below in `Behind a reverse proxy`_, you can
-        easily enable caching. For example, to allow nginx to cache up to
-        10 gigabytes of data for up to 1 hour::
-        
-            proxy_cache_path /data/nginx/cache
-                             levels=1:2
-                             keys_zone=pypiserver_cache:10m
-                             max_size=10g
-                             inactive=60m
-                             use_temp_path=off;
-        
-            server {
-                # ...
-                location / {
-                    proxy_cache pypiserver_cache;
-                    proxy_pass http://localhost:8080;
-                }
-            }
-        
-        Using webserver caching is especially helpful if you have high request
-        volume. Using `nginx` caching, a real-world pypiserver installation was
-        able to easily support over 1000 package downloads/min at peak load.
-        
-        Managing Automated Startup
-        --------------------------
-        
-        There are a variety of options for handling the automated starting of
-        pypiserver upon system startup. Two of the most common are *systemd* and
-        *supervisor* for linux systems. For windows creating services with scripts isn't
-        an easy task without a third party tool such as *NSSM*.
-        
-        Running As a ``systemd`` Service
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``systemd`` is installed by default on most modern Linux systems and as such,
-        it is an excellent option for managing the pypiserver process. An example
-        config file for ``systemd`` can be seen below::
-        
-            [Unit]
-            Description=A minimal PyPI server for use with pip/easy_install.
-            After=network.target
-        
-            [Service]
-            Type=simple
-            # systemd requires absolute path here too.
-            PIDFile=/var/run/pypiserver.pid
-            User=www-data
-            Group=www-data
-        
-            ExecStart=/usr/local/bin/pypi-server -p 8080 -a update,download --log-file /var/log/pypiserver.log -P /etc/nginx/.htpasswd /var/www/pypi
-            ExecStop=/bin/kill -TERM $MAINPID
-            ExecReload=/bin/kill -HUP $MAINPID
-            Restart=always
-        
-            WorkingDirectory=/var/www/pypi
-        
-            TimeoutStartSec=3
-            RestartSec=5
-        
-            [Install]
-            WantedBy=multi-user.target
-        
-        Adjusting the paths and adding this file as ``pypiserver.service`` into your
-        ``systemd/system`` directory will allow management of the pypiserver process with
-        ``systemctl``, e.g. ``systemctl start pypiserver``.
-        
-        More useful information about *systemd* can be found at
-        https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units
-        
-        Launching through ``supervisor``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        `supervisor <http://supervisord.org/>`_ has the benefit of being a pure python
-        package and as such, it provides excellent cross-platform support for process
-        management. An example configuration file for ``supervisor`` is given below::
-        
-            [program:pypi]
-            command=/home/pypi/pypi-venv/bin/pypi-server -p 7001 -P /home/pypi/.htpasswd /home/pypi/packages
-            directory=/home/pypi
-            user=pypi
-            autostart=true
-            autorestart=true
-            stderr_logfile=/var/log/pypiserver.err.log
-            stdout_logfile=/var/log/pypiserver.out.log
-        
-        From there, the process can be managed via ``supervisord`` using ``supervisorctl``.
-        
-        Running As a service with ``NSSM`` (Windows)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Download NSSM from https://nssm.cc unzip to a desired location such as Program Files. Decide whether you are going
-        to use win32 or win64, and add that exe to environment PATH.
-        
-        Create a start_pypiserver.bat::
-        
-            pypi-server -p 8080 C:\Path\To\Packages &
-        
-        Test the batch file by running it first before creating the service. Make sure you can access
-        the server remotely, and install packages. If you can, proceed, if not troubleshoot until you can.
-        This will ensure you know the server works, before adding NSSM into the mix.
-        
-        From the command prompt::
-        
-            nssm install pypiserver
-        
-        This command will launch a NSSM gui application::
-        
-            Path: C:\Path\To\start_pypiserver.bat
-            Startup directory: Auto generates when selecting path
-            Service name: pypiserver
-        
-        There are more tabs, but that is the basic setup. If the service needs to be running with a certain
-        login credentials, make sure you enter those credentials in the logon tab.
-        
-        Start the service::
-        
-            nssm start pypiserver
-        
-        Other useful commands::
-        
-            nssm --help
-            nssm stop <servicename>
-            nssm restart <servicename>
-            nssm status <servicename>
-        
-        For detailed information please visit https://nssm.cc
-        
-        Using a Different WSGI Server
-        -----------------------------
-        
-        - The ``bottle`` web-server which supports many WSGI-servers, among others,
-          ``paste``, ``cherrypy``, ``twisted`` and ``wsgiref`` (part of Python); you select
-          them using the ``--server`` flag.
-        
-        - You may view all supported WSGI servers using the following interactive code::
-        
-            >>> from pypiserver import bottle
-            >>> list(bottle.server_names.keys())
-            ['cgi', 'gunicorn', 'cherrypy', 'eventlet', 'tornado', 'geventSocketIO',
-            'rocket', 'diesel', 'twisted', 'wsgiref', 'fapws3', 'bjoern', 'gevent',
-            'meinheld', 'auto', 'aiohttp', 'flup', 'gae', 'paste', 'waitress']
-        
-        - If none of the above servers matches your needs, invoke just the
-          ``pypiserver:app()`` method which returns the internal WSGI-app WITHOUT
-          starting-up a server - you may then send it to any WSGI server you like.
-          Read also the `Utilizing the API`_ section.
-        
-        - Some examples are given below - you may find more details in `bottle
-          site <http://bottlepy.org/docs/dev/deployment.html#switching-the-server-backend>`_.
-        
-        Apache (``mod_wsgi``)
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        To use your *Apache2* with ``pypiserver``, prefer to utilize ``mod_wsgi`` as
-        explained in `bottle's documentation <http://bottlepy.org/docs/dev/deployment.html#apache-mod-wsgi>`_.
-        
-        .. Note::
-           If you choose instead to go with ``mod_proxy``, mind that you may bump into problems
-           with the prefix-path (see `#155 <https://github.com/pypiserver/pypiserver/issues/155>`_).
-        
-        1. Adapt and place the following *Apache* configuration either into top-level scope,
-           or inside some ``<VirtualHost>`` (contributed by Thomas Waldmann)::
-        
-                WSGIScriptAlias   /     /yoursite/wsgi/pypiserver-wsgi.py
-                WSGIDaemonProcess       pypisrv user=pypisrv group=pypisrv umask=0007 \
-                                        processes=1 threads=5 maximum-requests=500 \
-                                        display-name=wsgi-pypisrv inactivity-timeout=300
-                WSGIProcessGroup        pypisrv
-                WSGIPassAuthorization On    # Required for authentication (https://github.com/pypiserver/pypiserver/issues/288)
-        
-                <Directory /yoursite/wsgi >
-                    Require all granted
-                </Directory>
-        
-           or if using older ``Apache < 2.4``, substitute the last part with this::
-        
-                <Directory /yoursite/wsgi >
-                    Order deny,allow
-                    Allow from all
-                </Directory>
-        
-        2. Then create the ``/yoursite/cfg/pypiserver.wsgi`` file and make sure that
-           the ``user`` and ``group`` of the ``WSGIDaemonProcess`` directive
-           (``pypisrv:pypisrv`` in the example) have the read permission on it::
-        
-                import pypiserver
-        
-                conf = pypiserver.default_config(
-                    root =          "/yoursite/packages",
-                    password_file = "/yoursite/htpasswd", )
-                application = pypiserver.app(**conf)
-        
-        
-           .. Tip::
-              If you have installed ``pypiserver`` in a virtualenv, follow ``mod_wsgi``'s
-              `instructions <http://modwsgi.readthedocs.io/en/develop/user-guides/virtual-environments.html>`_
-              and prepend the python code above with the following::
-        
-                    import site
-        
-                    site.addsitedir('/yoursite/venv/lib/pythonX.X/site-packages')
-        
-        .. Note::
-           For security reasons, notice that the ``Directory`` directive grants access
-           to a directory holding the ``wsgi`` start-up script, alone; nothing else.
-        
-        .. Note::
-           To enable HTTPS support on Apache, configure the directive that contains the
-           WSGI configuration to use SSL.
-        
-        ``gunicorn``
-        ~~~~~~~~~~~~
-        
-        The following command uses ``gunicorn`` to start ``pypiserver``::
-        
-          gunicorn -w4 'pypiserver:app(root="/home/ralf/packages")'
-        
-        or when using multiple roots::
-        
-          gunicorn -w4 'pypiserver:app(root=["/home/ralf/packages", "/home/ralf/experimental"])'
-        
-        ``paste``
-        ~~~~~~~~~
-        
-        `paste <http://pythonpaste.org/>`_ allows to run multiple WSGI applications
-        under different URL paths. Therefore it is possible to serve different set
-        of packages on different paths.
-        
-        The following example ``paste.ini`` could be used to serve stable and
-        unstable packages on different paths::
-        
-            [composite:main]
-            use = egg:Paste#urlmap
-            /unstable/ = unstable
-            / = stable
-        
-            [app:stable]
-            use = egg:pypiserver#main
-            root = ~/stable-packages
-        
-            [app:unstable]
-            use = egg:pypiserver#main
-            root = ~/stable-packages
-               ~/unstable-packages
-        
-            [server:main]
-            use = egg:gunicorn#main
-            host = 0.0.0.0
-            port = 9000
-            workers = 5
-            accesslog = -
-        
-        .. Note::
-           You need to install some more dependencies for this to work, like::
-        
-                pip install paste pastedeploy gunicorn pypiserver
-        
-           The server can then start with::
-        
-                gunicorn_paster paste.ini
-        
-        
-        Behind a Reverse Proxy
-        ----------------------
-        
-        You can run ``pypiserver`` behind a reverse proxy as well.
-        
-        Nginx
-        ~~~~~
-        
-        Extend your nginx configuration::
-        
-            upstream pypi {
-              server              pypiserver.example.com:12345 fail_timeout=0;
-            }
-        
-            server {
-              server_name         myproxy.example.com;
-        
-              location / {
-                proxy_set_header  Host $host:$server_port;
-                proxy_set_header  X-Forwarded-Proto $scheme;
-                proxy_set_header  X-Real-IP $remote_addr;
-                proxy_pass        http://pypi;
-              }
-            }
-        
-        As of pypiserver 1.3, you may also use the `X-Forwarded-Host` header in your
-        reverse proxy config to enable changing the base URL. For example if you
-        want to host pypiserver under a particular path on your server::
-        
-            upstream pypi {
-              server              localhost:8000;
-            }
-        
-            server {
-              location /pypi/ {
-                  proxy_set_header  X-Forwarded-Host $host:$server_port/pypi;
-                  proxy_set_header  X-Forwarded-Proto $scheme;
-                  proxy_set_header  X-Forwarded-For $proxy_add_x_forwarded_for;
-                  proxy_set_header  X-Real-IP $remote_addr;
-                  proxy_pass        http://pypi;
-              }
-            }
-        
-        Supporting HTTPS
-        ~~~~~~~~~~~~~~~~
-        
-        Using a reverse proxy is the preferred way of getting pypiserver behind
-        HTTPS. For example, to put pypiserver behind HTTPS on port 443, with
-        automatic HTTP redirection, using `nginx`::
-        
-            upstream pypi {
-              server               localhost:8000;
-            }
-        
-            server {
-              listen              80 default_server;
-              server_name         _;
-              return              301 https://$host$request_uri;
-            }
-        
-            server {
-              listen              443 ssl;
-              server_name         pypiserver.example.com;
-        
-              ssl_certificate     /etc/star.example.com.crt;
-              ssl_certificate_key /etc/star.example.com.key;
-              ssl_protocols       TLSv1 TLSv1.1 TLSv1.2;
-              ssl_ciphers         HIGH:!aNULL:!MD5;
-        
-              location / {
-                proxy_set_header  Host $host:$server_port;
-                proxy_set_header  X-Forwarded-Proto $scheme;
-                proxy_set_header  X-Real-IP $remote_addr;
-                proxy_pass        http://pypi;
-              }
-            }
-        
-        Please see `nginx's HTTPS docs for more details <http://nginx.org/en/docs/http/configuring_https_servers.html>`_.
-        
-        Getting and keeping your certificates up-to-date can be simplified using,
-        for example, using `certbot and letsencrypt <https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-18-04>`_.
-        
-        Traefik
-        ~~~~~~~
-        
-        It is also possible to use `Traefik <https://docs.traefik.io/>`_ to put pypiserver behind HTTPS on port 443, with
-        automatic HTTP redirection using Docker Compose. Please see the provided `<docker-compose.yml>`_ example for more information.
-        
-        Utilizing the API
-        -----------------
-        
-        In order to enable ad-hoc authentication-providers or to use WSGI-servers
-        not supported by *bottle* out-of-the-box, you needed to launch ``pypiserver``
-        via its API.
-        
-        - The main entry-point for configuring ``pypiserver`` is the `pypiserver:app()
-          <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L116>`_
-          function.  This function returns the internal WSGI-app that you my then
-          send to any WSGI-server you like.
-        
-        - To get all ``pypiserver:app()`` keywords and their explanations, read the
-          function `pypiserver:default_config()
-          <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L35>`_.
-        
-        - Finally, to fire-up a WSGI-server with the configured app, invoke
-          the ``bottle:run(app, host, port, server)`` function.
-          Note that ``pypiserver`` ships with it is own copy of *bottle*; to use it,
-          import it like that: ``from pypiserver import bottle``
-        
-        Using Ad-Hoc Authentication Providers
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The ``auther`` keyword of ``pypiserver:app()`` function maybe set only using
-        the API. This can be any callable that returns a boolean when passed
-        the *username* and the *password* for a given request.
-        
-        For example, to authenticate users based on the ``/etc/passwd`` file under Unix,
-        you may delegate such decisions to the `python-pam`_ library by following
-        these steps:
-        
-        1. Ensure ``python-pam`` module is installed::
-        
-            pip install python-pam
-        
-        2. Create a python-script along these lines::
-        
-            $ cat > pypiserver-start.py
-            import pypiserver
-            from pypiserver import bottle
-            import pam
-            app = pypiserver.app(root='./packages', auther=pam.authenticate)
-            bottle.run(app=app, host='0.0.0.0', port=80, server='auto')
-        
-            [Ctrl+ D]
-        
-        3. Invoke the python-script to start-up ``pypiserver``::
-        
-            $ python pypiserver-start.py
-        
-        
-        .. Note::
-           The `python-pam`_ module, requires *read* access to ``/etc/shadow`` file;
-           you may add the user under which ``pypiserver`` runs into the *shadow*
-           group, with a command like this: ``sudo usermod -a -G shadow pypy-user``.
-        
-        Use with MicroPython
-        --------------------
-        The MicroPython interpreter for embedded devices can install packages with the
-        module ``upip.py``. The module uses a specialized json-endpoint to retrieve
-        package information. This endpoint is supported by ``pypiserver``.
-        
-        It can be tested with the UNIX port of ``micropython``::
-        
-            cd micropython
-            ports/unix/micropython -m tools.upip install -i http://my-server:8080 -p /tmp/mymodules micropython-foobar
-        
-        Installing packages from the REPL of an embedded device works in this way:
-        
-        .. code-block:: python
-        
-            import network
-            import upip
-        
-            sta_if = network.WLAN(network.STA_IF)
-            sta_if.active(True)
-            sta_if.connect('<your ESSID>', '<your password>')
-            upip.index_urls = ["http://my-server:8080"]
-            upip.install("micropython-foobar")
-        
-        Further information on micropython-packaging can be found here: https://docs.micropython.org/en/latest/reference/packages.html
-        
-        
-        Sources
-        =======
-        
-        To create a copy of the repository, use::
-        
-            git clone https://github.com/pypiserver/pypiserver.git
-            cd pypiserver
-        
-        To receive any later changes, in the above folder use::
-        
-            git pull
-        
-        
-        Known Limitations
-        =================
-        
-        ``pypiserver`` does not implement the full API as seen on PyPI_. It
-        implements just enough to make ``easy_install``, ``pip install``, and
-        ``search`` work.
-        
-        The following limitations are known:
-        
-        - Command ``pypi -U`` that compares uploaded packages with *pypi* to see if
-          they are outdated, does not respect a http-proxy environment variable
-          (see `#19 <https://github.com/pypiserver/pypiserver/issues/19>`_).
-        - It accepts documentation uploads but does not save them to
-          disk (see `#47 <https://github.com/pypiserver/pypiserver/issues/47>`_ for a
-          discussion)
-        - It does not handle misspelled packages as *pypi-repo* does,
-          therefore it is suggested to use it with ``--extra-index-url`` instead
-          of ``--index-url`` (see `#38 <https://github.com/pypiserver/pypiserver/issues/38>`_).
-        
-        Please use Github's `bugtracker <https://github.com/pypiserver/pypiserver/issues>`_
-        for other bugs you find.
-        
-        
-        Similar Projects
-        ================
-        
-        There are lots of other projects, which allow you to run your own
-        PyPI server. If ``pypiserver`` doesn't work for you, the following are
-        among the most popular alternatives:
-        
-        - `devpi-server <https://pypi.org/project/devpi/>`_:
-          a reliable fast pypi.org caching server, part of
-          the comprehensive `github-style pypi index server and packaging meta tool
-          <https://pypi.org/project/devpi/>`_.
-          (version: 2.1.4, access date: 8/3/2015)
-        
-        - Check this SO question: `How to roll my own pypi
-          <http://stackoverflow.com/questions/1235331/how-to-roll-my-own-pypi>`_
-        
-        
-        Unmaintained or archived
-        ------------------------
-        
-        These projects were once alternatives to pypiserver but are now either unmaintained or archived.
-        
-        - `pip2pi <https://github.com/wolever/pip2pi>`_
-          a simple cmd-line tool that builds a PyPI-compatible local folder from pip requirements
-        
-        - `flask-pypi-proxy <http://flask-pypi-proxy.readthedocs.org/>`_
-          A proxy for PyPI that also enables also uploading custom packages.
-        
-        
-        Related Software
-        ================
-        
-        Though not direct alternatives for ``pypiserver``'s use as an index
-        server, the following is a list of related software projects that you
-        may want to familiarize with:
-        
-        - `pypi-uploader`_:
-          A command-line utility to upload packages to your ``pypiserver`` from pypi without
-          having to store them locally first.
-        
-        - `twine`_:
-          A command-line utility for interacting with PyPI or ``pypiserver``.
-        
-        - `warehouse`_:
-          the software that powers PyPI_ itself. It is not generally intended to
-          be run by end-users.
-        
-        Licensing
-        =========
-        
-        ``pypiserver`` contains a copy of bottle_ which is available under the
-        MIT license, and the remaining part is distributed under the zlib/libpng license.
-        See the ``LICENSE.txt`` file.
-        
-        
-        .. _bottle: http://bottlepy.org
-        .. _PyPA: https://www.pypa.io/en/latest/
-        .. _PyPI: https://pypi.org
-        .. _Warehouse: https://github.com/pypa/warehouse/
-        .. _twine: https://pypi.org/project/twine/
-        .. _pypi-uploader: https://pypi.org/project/pypi-uploader/
-        .. _python-pam: https://pypi.org/project/python-pam/
-        .. |test-status| image:: https://github.com/pypiserver/pypiserver/workflows/Test/badge.svg
-            :alt: test status
-            :scale: 100%
-            :target: https://github.com/pypiserver/pypiserver/actions?query=workflow%3ATest
-        
-        .. |pypi-ver| image::  https://img.shields.io/pypi/v/pypiserver.svg
-            :target: https://pypi.org/project/pypiserver/
-            :alt: Latest Version in PyPI
-        
-        .. |python-ver| image:: https://img.shields.io/pypi/pyversions/pypiserver.svg
-            :target: https://pypi.org/project/pypiserver/
-            :alt: Supported Python versions
-        
-        .. |proj-license| image:: https://img.shields.io/badge/license-BSD%2Bzlib%2Flibpng-blue.svg
-            :target: https://raw.githubusercontent.com/pypiserver/pypiserver/master/LICENSE.txt
-            :alt: Project License
-        
-        .. |dependencies| image:: https://img.shields.io/requires/github/pypiserver/pypiserver.svg
-            :target: https://requires.io/github/pypiserver/pypiserver/requirements/
-            :alt: Dependencies up-to-date?
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -1052,14 +16,1097 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Software Distribution
 Requires-Python: >=3.6
 Provides-Extra: passlib
 Provides-Extra: cache
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+.. -*- mode: rst; coding: utf-8 -*-
+
+.. image:: docs/__resources__/pypiserver_logo.png
+   :width: 300 px
+   :align: center
+
+==============================================================================
+pypiserver - minimal PyPI server for use with pip/easy_install
+==============================================================================
+|pypi-ver| |test-status| |dependencies| |python-ver| |proj-license|
+
+:Version:     1.5.2
+:Date:        2023-07-30
+:Source:      https://github.com/pypiserver/pypiserver
+:PyPI:        https://pypi.org/project/pypiserver/
+:Tests:       https://github.com/pypiserver/pypiserver/actions
+:Maintainers: | Kostis Anagnostopoulos <ankostis@gmail.com>,
+              | Matthew Planchard <mplanchard@gmail.com>,
+              | Dmitrii Orlov <dmtree.dev@yahoo.com>,
+              | **Someone new?** We are looking for new maintainers! 
+                <https://github.com/pypiserver/pypiserver/issues/397>
+:License:     zlib/libpng + MIT
+:Community:   https://pypiserver.zulipchat.com
+
+Chat with us on `Zulip <https://pypiserver.zulipchat.com>`_!
+
+``pypiserver`` is a minimal PyPI_ compatible server for ``pip`` or ``easy_install``.
+It is based on bottle_ and serves packages from regular directories.
+Wheels, bdists, eggs and accompanying PGP-signatures can be uploaded
+either with ``pip``, ``setuptools``, ``twine``, ``pypi-uploader``, or simply copied
+with ``scp``.
+
+.. note::
+   The official software powering PyPI_ is Warehouse_. However, Warehouse_
+   is fairly specialized to be ``pypi.org``'s own software, and should not
+   be used in other contexts. In particular, it does not officially support
+   being used as a custom package index by users wishing to serve their own
+   packages.
+
+   ``pypiserver`` implements the same interfaces as `PyPI`_, allowing
+   standard Python packaging tooling such as ``pip`` and ``twine`` to
+   interact with it as a package index just as they would with PyPI_, while
+   making it much easier to get a running index server.
+
+.. contents:: Table of Contents
+  :backlinks: top
+
+
+Quickstart: Installation and Usage
+==================================
+
+``pypiserver`` works with Python 3.6+ and PyPy3.
+
+Older Python versions may still work, but they are not tested.
+
+For legacy Python versions, use ``pypiserver-1.x`` series. Note that these are
+not officially supported, and will not receive bugfixes or new features.
+
+.. Tip::
+   The commands below work on a unix-like operating system with a posix shell.
+   The ``'~'`` character expands to user's home directory.
+
+   If you're using Windows, you'll have to use their "Windows counterparts".
+   The same is true for the rest of this documentation.
+
+1. Install ``pypiserver`` with this command::
+
+    pip install pypiserver                # Or: pypiserver[passlib,cache]
+    mkdir ~/packages                      # Copy packages into this directory.
+
+   See also `Alternative Installation methods`_.
+
+2. Copy some packages into your ``~/packages`` folder and then
+   get your ``pypiserver`` up and running::
+
+    pypi-server run -p 8080 ~/packages &      # Will listen to all IPs.
+
+3. From the client computer, type this::
+
+    # Download and install hosted packages.
+    pip install --extra-index-url http://localhost:8080/simple/ ...
+
+    # or
+    pip install --extra-index-url http://localhost:8080 ...
+
+    # Search hosted packages.
+    pip search --index http://localhost:8080 ...
+
+    # Note that pip search does not currently work with the /simple/ endpoint.
+
+   See also `Client-side configurations`_ for avoiding tedious typing.
+
+4. Enter ``pypi-server -h`` in the cmd-line to print a detailed usage message::
+
+    start PyPI compatible package server serving packages from PACKAGES_DIRECTORY. If PACKAGES_DIRECTORY is not given on the command line, it uses the default ~/packages. pypiserver scans this directory recursively for packages. It skips packages and directories starting with a dot. Multiple package directories may be specified.
+
+    positional arguments:
+      {run,update}
+        run                 Run pypiserver, serving packages from
+                            PACKAGES_DIRECTORY
+        update              Handle updates of packages managed by pypiserver. By
+                            default, a pip command to update the packages is
+                            printed to stdout for introspection or pipelining. See
+                            the `-x` option for updating packages directly.
+
+    options:
+      -h, --help            show this help message and exit
+      -v, --verbose         Enable verbose logging; repeat for more verbosity.
+      --log-file FILE       Write logging info into this FILE, as well as to
+                            stdout or stderr, if configured.
+      --log-stream STREAM   Log messages to the specified STREAM. Valid values are
+                            stdout, stderr, and none
+      --log-frmt FORMAT     The logging format-string.  (see `logging.LogRecord`
+                            class from standard python library)
+      --hash-algo HASH_ALGO
+                            Any `hashlib` available algorithm to use for
+                            generating fragments on package links. Can be disabled
+                            with one of (0, no, off, false).
+      --backend {auto,simple-dir,cached-dir}
+                            A backend implementation. Keep the default 'auto' to
+                            automatically determine whether to activate caching or
+                            not
+      --version             show program's version number and exit
+
+    Visit https://github.com/pypiserver/pypiserver for more information
+
+More details about ``pypi-server run``
+--------------------------------------
+
+Enter ``pypi-server run -h`` in the cmd-line to print a detailed usage
+message *about starting the server*::
+
+  usage: pypi-server run [-h] [-v] [--log-file FILE] [--log-stream STREAM] [--log-frmt FORMAT] [--hash-algo HASH_ALGO]
+                       [--backend {auto,simple-dir,cached-dir}] [--version] [-p PORT] [-i HOST] [-a AUTHENTICATE] [-P PASSWORD_FILE] [--disable-fallback]
+                       [--fallback-url FALLBACK_URL] [--health-endpoint HEALTH_ENDPOINT] [--server METHOD] [-o] [--welcome HTML_FILE]
+                       [--cache-control AGE] [--log-req-frmt FORMAT] [--log-res-frmt FORMAT] [--log-err-frmt FORMAT]
+                       [package_directory [package_directory ...]]
+
+  positional arguments:
+    package_directory     The directory from which to serve packages.
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -v, --verbose         Enable verbose logging; repeat for more verbosity.
+    --log-file FILE       Write logging info into this FILE, as well as to stdout or stderr, if configured.
+    --log-stream STREAM   Log messages to the specified STREAM. Valid values are stdout, stderr, and none
+    --log-frmt FORMAT     The logging format-string.  (see `logging.LogRecord` class from standard python library)
+    --hash-algo HASH_ALGO
+                          Any `hashlib` available algorithm to use for generating fragments on package links. Can be disabled with one of (0, no, off,
+                          false).
+    --backend {auto,simple-dir,cached-dir}
+                          A backend implementation. Keep the default 'auto' to automatically determine whether to activate caching or not
+    --version             show program's version number and exit
+    -p PORT, --port PORT  Listen on port PORT (default: 8080)
+    -i HOST, -H HOST, --interface HOST, --host HOST
+                          Listen on interface INTERFACE (default: 0.0.0.0)
+    -a AUTHENTICATE, --authenticate AUTHENTICATE
+                          Comma-separated list of (case-insensitive) actions to authenticate (options: download, list, update; default: update).
+                          
+                          Any actions not specified are not authenticated, so to authenticate downloads and updates, but allow unauthenticated viewing of
+                          the package list, you would use:
+                          
+                            pypi-server -a 'download, update' -P ./my_passwords.htaccess
+                          
+                          To disable authentication, use:
+                          
+                            pypi-server -a . -P .
+                          
+                          See the `-P` option for configuring users and passwords.
+                          
+                          Note that when uploads are not protected, the `register` command is not necessary, but `~/.pypirc` still needs username and
+                          password fields, even if bogus.
+    -P PASSWORD_FILE, --passwords PASSWORD_FILE
+                          Use an apache htpasswd file PASSWORD_FILE to set usernames and passwords for authentication.
+                          
+                          To allow unauthorized access, use:
+                          
+                            pypi-server -a . -P .
+                          
+    --disable-fallback    Disable the default redirect to PyPI for packages not found in the local index.
+    --fallback-url FALLBACK_URL
+                          Redirect to FALLBACK_URL for packages not found in the local index.
+    --health-endpoint HEALTH_ENDPOINT
+                          Configure a custom liveness endpoint.
+                          It always returns 200 Ok if the service is up.
+                          Otherwise, it means that the service is not responsive.
+    --server METHOD       Use METHOD to run the server. Valid values include paste, cherrypy, twisted, gunicorn, gevent, wsgiref, and auto. The default is to
+                          use "auto", which chooses one of paste, cherrypy, twisted, or wsgiref.
+    -o, --overwrite       Allow overwriting existing package files during upload.
+    --welcome HTML_FILE   Use the contents of HTML_FILE as a custom welcome message on the home page.
+    --cache-control AGE   Add "Cache-Control: max-age=AGE" header to package downloads. Pip 6+ requires this for caching. AGE is specified in seconds.
+    --log-req-frmt FORMAT
+                          A format-string selecting Http-Request properties to log; set to '%s' to see them all.
+    --log-res-frmt FORMAT
+                          A format-string selecting Http-Response properties to log; set to '%s' to see them all.
+    --log-err-frmt FORMAT
+                          A format-string selecting Http-Error properties to log; set to '%s' to see them all.
+
+More details about ``pypi-server update``
+-----------------------------------------
+
+Enter ``pypi-server update -h`` in the cmd-line to print a detailed usage
+message *about updating the managed packages*::
+
+  usage: pypi-server update [-h] [-v] [--log-file FILE] [--log-stream STREAM] [--log-frmt FORMAT] [--hash-algo HASH_ALGO]
+                            [--backend {auto,simple-dir,cached-dir}] [--version] [-x] [-d DOWNLOAD_DIRECTORY] [-u] [--blacklist-file IGNORELIST_FILE]
+                            [package_directory [package_directory ...]]
+
+  positional arguments:
+    package_directory     The directory from which to serve packages.
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -v, --verbose         Enable verbose logging; repeat for more verbosity.
+    --log-file FILE       Write logging info into this FILE, as well as to stdout or stderr, if configured.
+    --log-stream STREAM   Log messages to the specified STREAM. Valid values are stdout, stderr, and none
+    --log-frmt FORMAT     The logging format-string. (see `logging.LogRecord` class from standard python library)
+    --hash-algo HASH_ALGO
+                          Any `hashlib` available algorithm to use for generating fragments on package links. Can be disabled with one of (0, no, off,
+                          false).
+    --backend {auto,simple-dir,cached-dir}
+                          A backend implementation. Keep the default 'auto' to automatically determine whether to activate caching or not
+    --version             show program's version number and exit
+    -x, --execute         Execute the pip commands rather than printing to stdout
+    -d DOWNLOAD_DIRECTORY, --download-directory DOWNLOAD_DIRECTORY
+                          Specify a directory where packages updates will be downloaded. The default behavior is to use the directory which contains the
+                          package being updated.
+    -u, --allow-unstable  Allow updating to unstable versions (alpha, beta, rc, dev, etc.)
+    --blacklist-file IGNORELIST_FILE, --ignorelist-file IGNORELIST_FILE
+                          Don't update packages listed in this file (one package name per line, without versions, '#' comments honored). This can be useful
+                          if you upload private packages into pypiserver, but also keep a mirror of public packages that you regularly update. Attempting to
+                          pull an update of a private package from `pypi.org` might pose a security risk - e.g. a malicious user might publish a higher
+                          version of the private package, containing arbitrary code.
+
+Client-Side Configurations
+==========================
+
+Always specifying the the pypi url on the command line is a bit
+cumbersome. Since ``pypiserver`` redirects ``pip/easy_install`` to the
+``pypi.org`` index if it doesn't have a requested package, it is a
+good idea to configure them to always use your local pypi index.
+
+Configuring ``pip``
+-------------------
+
+For ``pip`` command this can be done by setting the environment variable
+``PIP_EXTRA_INDEX_URL`` in your ``.bashr/.profile/.zshrc``::
+
+  export PIP_EXTRA_INDEX_URL=http://localhost:8080/simple/
+
+or by adding the following lines to ``~/.pip/pip.conf``::
+
+  [global]
+  extra-index-url = http://localhost:8080/simple/
+
+.. Note::
+   If you have installed ``pypiserver`` on a remote url without *https*
+   you will receive an "untrusted" warning from *pip*, urging you to append
+   the ``--trusted-host`` option.  You can also include this option permanently
+   in your configuration-files or environment variables.
+
+Configuring ``easy_install``
+----------------------------
+
+For ``easy_install`` command you may set the following configuration in
+``~/.pydistutils.cfg``::
+
+  [easy_install]
+  index_url = http://localhost:8080/simple/
+
+
+Uploading Packages Remotely
+===========================
+
+Instead of copying packages directly to the server's folder (i.e. with ``scp``),
+you may use python tools for the task, e.g. ``python setup.py upload``.
+In that case, ``pypiserver`` is responsible for authenticating the upload-requests.
+
+.. Note::
+  We strongly advise to password-protected your uploads!
+
+  It is possible to disable authentication for uploads (e.g. in intranets).
+  To avoid lazy security decisions, read help for ``-P`` and ``-a`` options.
+
+*Apache*-Like Authentication (``htpasswd``)
+-------------------------------------------
+
+#. First make sure you have the *passlib* module installed (note that
+   ``passlib>=1.6`` is required), which is needed for parsing the Apache
+   *htpasswd* file specified by the ``-P``, ``--passwords`` option
+   (see next steps)::
+
+     pip install passlib
+
+#. Create the Apache *htpasswd* file with at least one user/password pair
+   with this command (you'll be prompted for a password)::
+
+     htpasswd -sc htpasswd.txt <some_username>
+
+   .. Tip:: Read this SO question for running `htpasswd` cmd
+      under *Windows*:
+
+         http://serverfault.com/questions/152950/how-to-create-and-edit-htaccess-and-htpasswd-locally-on-my-computer-and-then-u
+
+      or if you have bogus passwords that you don't care because they are for
+      an internal service (which is still "bad", from a security perspective...)
+      you may use this public service:
+
+         http://www.htaccesstools.com/htpasswd-generator/
+
+   .. Tip:: When accessing pypiserver via the api, alternate authentication
+      methods are available via the ``auther`` config flag. Any callable
+      returning a boolean can be passed through to the pypiserver config in
+      order to provide custom authentication. For example, to configure
+      pypiserver to authenticate using the `python-pam`_::
+
+        import pam
+        pypiserver.default_config(auther=pam.authenticate)
+
+      Please see `Using Ad-hoc authentication providers`_ for more information.
+
+#. You  need to restart the server with the ``-P`` option only once
+   (but user/password pairs can later be added or updated on the fly)::
+
+     ./pypi-server run -p 8080 -P htpasswd.txt ~/packages &
+
+Upload with ``setuptools``
+--------------------------
+
+#. On client-side, edit or create a ``~/.pypirc`` file with a similar content::
+
+     [distutils]
+     index-servers =
+       pypi
+       local
+
+     [pypi]
+     username:<your_pypi_username>
+     password:<your_pypi_passwd>
+
+     [local]
+     repository: http://localhost:8080
+     username: <some_username>
+     password: <some_passwd>
+
+#. Then from within the directory of the python-project you wish to upload,
+   issue this command::
+
+     python setup.py sdist upload -r local
+
+Upload with ``twine``
+---------------------
+
+To avoid storing you passwords on disk, in clear text, you may either:
+
+- use the ``register`` *setuptools*'s command with the ``-r`` option,
+  like that::
+
+     python setup.py sdist register -r local upload -r local
+
+- use `twine`_ library, which
+  breaks the procedure in two steps.  In addition, it supports signing
+  your files with PGP-Signatures and uploading the generated `.asc` files
+  to ``pypiserver``::
+
+     twine upload -r local --sign -identity user_name ./foo-1.zip
+
+
+Using the Docker Image
+======================
+
+Starting with version 1.2.5, official Docker images will be built for each
+push to master, each dev, alpha, or beta release, and each final release.
+The most recent full release will always be available under the tag ``latest``,
+and the current master branch will always be available under the tag
+``unstable``.
+
+You can always check to see what tags are currently available at our
+`Docker Repo`_.
+
+To run the most recent release of ``pypiserver`` with Docker, simply::
+
+    docker run pypiserver/pypiserver:latest run
+
+This starts ``pypiserver`` serving packages from the ``/data/packages``
+directory inside the container, listening on the container port 8080.
+
+The container takes all the same arguments as the normal ``pypi-server``
+executable, with the exception of the internal container port (``-p``),
+which will always be 8080.
+
+Of course, just running a container isn't that interesting. To map
+port 80 on the host to port 8080 on the container::
+
+    docker run -p 80:8080 pypiserver/pypiserver:latest run
+
+You can now access your ``pypiserver`` at ``localhost:80`` in a web browser.
+
+To serve packages from a directory on the host, e.g. ``~/packages``::
+
+    docker run -p 80:8080 -v ~/packages:/data/packages pypiserver/pypiserver:latest run
+
+To authenticate against a local ``.htpasswd`` file::
+
+    docker run -p 80:8080 -v ~/.htpasswd:/data/.htpasswd pypiserver/pypiserver:latest run -P .htpasswd packages
+
+You can also specify ``pypiserver`` to run as a Docker service using a
+composefile. An example composefile is `provided <docker-compose.yml>`_.
+
+
+.. _`docker repo`: https://hub.docker.com/r/pypiserver/pypiserver/tags/
+
+
+Alternative Installation Methods
+================================
+
+When trying the methods below, first use the following command to check whether
+previous versions of ``pypiserver`` already exist, and (optionally) uninstall them::
+
+  # VERSION-CHECK: Fails if not installed.
+  pypi-server --version
+
+  # UNINSTALL: Invoke again until it fails.
+  pip uninstall pypiserver
+
+Installing the Very Latest Version
+----------------------------------
+
+In case the latest version in *pypi* is a pre-release, you have to use
+*pip*'s `--pre` option.  And to update an existing installation combine it
+with `--ignore-installed`::
+
+  pip install pypiserver --pre -I
+
+You can even install the latest ``pypiserver`` directly from *github* with the
+following command, assuming you have *git* installed on your ``PATH``::
+
+  pip install git+git://github.com/pypiserver/pypiserver.git
+
+
+Recipes
+=======
+
+Managing the Package Directory
+------------------------------
+
+The ``pypi-server`` command has the ``update`` command that searches for updates of
+available packages. It scans the package directory for available
+packages and searches on pypi.org for updates. Without further
+options ``pypi-server update`` will just print a list of commands which must
+be run in order to get the latest version of each package. Output
+looks like::
+
+    $ ./pypi-server update 
+    checking 106 packages for newer version
+
+    .........u.e...........e..u.............
+    .....e..............................e...
+    ..........................
+
+    no releases found on pypi for PyXML, Pymacs, mercurial, setuptools
+
+    # update raven from 1.4.3 to 1.4.4
+    pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror raven==1.4.4
+
+    # update greenlet from 0.3.3 to 0.3.4
+    pip -q install --no-deps  --extra-index-url https://pypi.org/simple/ -d /home/ralf/packages/mirror greenlet==0.3.4
+
+It first prints for each package a single character after checking the
+available versions on pypi. A dot(`.`) means the package is up-to-date, ``'u'``
+means the package can be updated and ``'e'`` means the list of releases on
+pypi is empty. After that it shows a *pip* command line which can be used
+to update a one package. Either copy and paste that or run
+``pypi-server update -x`` in order to really execute those commands. You need
+to have *pip* installed for that to work however.
+
+Specifying an additional ``-u`` option will also allow alpha, beta and
+release candidates to be downloaded. Without this option these
+releases won't be considered.
+
+Serving Thousands of Packages
+-----------------------------
+
+By default, ``pypiserver`` scans the entire packages directory each time an
+incoming HTTP request occurs. This isn't a problem for a small number of
+packages, but causes noticeable slow-downs when serving thousands of packages.
+
+If you run into this problem, significant speedups can be gained by enabling
+pypiserver's directory caching functionality. The only requirement is to
+install the ``watchdog`` package, or it can be installed during ``pypiserver``
+installation, by specifying the ``cache`` extras option::
+
+    pip install pypiserver[cache]
+
+Additional speedups can be obtained by using your webserver's builtin
+caching functionality. For example, if you are using `nginx` as a
+reverse-proxy as described below in `Behind a reverse proxy`_, you can
+easily enable caching. For example, to allow nginx to cache up to
+10 gigabytes of data for up to 1 hour::
+
+    proxy_cache_path /data/nginx/cache
+                     levels=1:2
+                     keys_zone=pypiserver_cache:10m
+                     max_size=10g
+                     inactive=60m
+                     use_temp_path=off;
+
+    server {
+        # ...
+        location / {
+            proxy_cache pypiserver_cache;
+            proxy_pass http://localhost:8080;
+        }
+    }
+
+Using webserver caching is especially helpful if you have high request
+volume. Using `nginx` caching, a real-world pypiserver installation was
+able to easily support over 1000 package downloads/min at peak load.
+
+Managing Automated Startup
+--------------------------
+
+There are a variety of options for handling the automated starting of
+pypiserver upon system startup. Two of the most common are *systemd* and
+*supervisor* for linux systems. For windows creating services with scripts isn't
+an easy task without a third party tool such as *NSSM*.
+
+Running As a ``systemd`` Service
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``systemd`` is installed by default on most modern Linux systems and as such,
+it is an excellent option for managing the pypiserver process. An example
+config file for ``systemd`` can be seen below::
+
+    [Unit]
+    Description=A minimal PyPI server for use with pip/easy_install.
+    After=network.target
+
+    [Service]
+    Type=simple
+    # systemd requires absolute path here too.
+    PIDFile=/var/run/pypiserver.pid
+    User=www-data
+    Group=www-data
+
+    ExecStart=/usr/local/bin/pypi-server run -p 8080 -a update,download --log-file /var/log/pypiserver.log -P /etc/nginx/.htpasswd /var/www/pypi
+    ExecStop=/bin/kill -TERM $MAINPID
+    ExecReload=/bin/kill -HUP $MAINPID
+    Restart=always
+
+    WorkingDirectory=/var/www/pypi
+
+    TimeoutStartSec=3
+    RestartSec=5
+
+    [Install]
+    WantedBy=multi-user.target
+
+Adjusting the paths and adding this file as ``pypiserver.service`` into your
+``systemd/system`` directory will allow management of the pypiserver process with
+``systemctl``, e.g. ``systemctl start pypiserver``.
+
+More useful information about *systemd* can be found at
+https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units
+
+Launching through ``supervisor``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+`supervisor <http://supervisord.org/>`_ has the benefit of being a pure python
+package and as such, it provides excellent cross-platform support for process
+management. An example configuration file for ``supervisor`` is given below::
+
+    [program:pypi]
+    command=/home/pypi/pypi-venv/bin/pypi-server run -p 7001 -P /home/pypi/.htpasswd /home/pypi/packages
+    directory=/home/pypi
+    user=pypi
+    autostart=true
+    autorestart=true
+    stderr_logfile=/var/log/pypiserver.err.log
+    stdout_logfile=/var/log/pypiserver.out.log
+
+From there, the process can be managed via ``supervisord`` using ``supervisorctl``.
+
+Running As a service with ``NSSM`` (Windows)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Download NSSM from https://nssm.cc unzip to a desired location such as Program Files. Decide whether you are going
+to use win32 or win64, and add that exe to environment PATH.
+
+Create a start_pypiserver.bat::
+
+    pypi-server run -p 8080 C:\Path\To\Packages &
+
+Test the batch file by running it first before creating the service. Make sure you can access
+the server remotely, and install packages. If you can, proceed, if not troubleshoot until you can.
+This will ensure you know the server works, before adding NSSM into the mix.
+
+From the command prompt::
+
+    nssm install pypiserver
+
+This command will launch a NSSM gui application::
+
+    Path: C:\Path\To\start_pypiserver.bat
+    Startup directory: Auto generates when selecting path
+    Service name: pypiserver
+
+There are more tabs, but that is the basic setup. If the service needs to be running with a certain
+login credentials, make sure you enter those credentials in the logon tab.
+
+Start the service::
+
+    nssm start pypiserver
+
+Other useful commands::
+
+    nssm --help
+    nssm stop <servicename>
+    nssm restart <servicename>
+    nssm status <servicename>
+
+For detailed information please visit https://nssm.cc
+
+Using a Different WSGI Server
+-----------------------------
+
+- The ``bottle`` web-server which supports many WSGI-servers, among others,
+  ``paste``, ``cherrypy``, ``twisted`` and ``wsgiref`` (part of Python); you select
+  them using the ``--server`` flag.
+
+- You may view all supported WSGI servers using the following interactive code::
+
+    >>> from pypiserver import bottle
+    >>> list(bottle.server_names.keys())
+    ['cgi', 'gunicorn', 'cherrypy', 'eventlet', 'tornado', 'geventSocketIO',
+    'rocket', 'diesel', 'twisted', 'wsgiref', 'fapws3', 'bjoern', 'gevent',
+    'meinheld', 'auto', 'aiohttp', 'flup', 'gae', 'paste', 'waitress']
+
+- If none of the above servers matches your needs, invoke just the
+  ``pypiserver:app()`` method which returns the internal WSGI-app WITHOUT
+  starting-up a server - you may then send it to any WSGI server you like.
+  Read also the `Utilizing the API`_ section.
+
+- Some examples are given below - you may find more details in `bottle
+  site <http://bottlepy.org/docs/dev/deployment.html#switching-the-server-backend>`_.
+
+Apache (``mod_wsgi``)
+~~~~~~~~~~~~~~~~~~~~~
+
+To use your *Apache2* with ``pypiserver``, prefer to utilize ``mod_wsgi`` as
+explained in `bottle's documentation <http://bottlepy.org/docs/dev/deployment.html#apache-mod-wsgi>`_.
+
+.. Note::
+   If you choose instead to go with ``mod_proxy``, mind that you may bump into problems
+   with the prefix-path (see `#155 <https://github.com/pypiserver/pypiserver/issues/155>`_).
+
+1. Adapt and place the following *Apache* configuration either into top-level scope,
+   or inside some ``<VirtualHost>`` (contributed by Thomas Waldmann)::
+
+        WSGIScriptAlias   /     /yoursite/wsgi/pypiserver-wsgi.py
+        WSGIDaemonProcess       pypisrv user=pypisrv group=pypisrv umask=0007 \
+                                processes=1 threads=5 maximum-requests=500 \
+                                display-name=wsgi-pypisrv inactivity-timeout=300
+        WSGIProcessGroup        pypisrv
+        WSGIPassAuthorization On    # Required for authentication (https://github.com/pypiserver/pypiserver/issues/288)
+
+        <Directory /yoursite/wsgi >
+            Require all granted
+        </Directory>
+
+   or if using older ``Apache < 2.4``, substitute the last part with this::
+
+        <Directory /yoursite/wsgi >
+            Order deny,allow
+            Allow from all
+        </Directory>
+
+2. Then create the ``/yoursite/cfg/pypiserver.wsgi`` file and make sure that
+   the ``user`` and ``group`` of the ``WSGIDaemonProcess`` directive
+   (``pypisrv:pypisrv`` in the example) have the read permission on it::
+
+        import pypiserver
+
+        conf = pypiserver.default_config(
+            root =          "/yoursite/packages",
+            password_file = "/yoursite/htpasswd", )
+        application = pypiserver.app(**conf)
+
+
+   .. Tip::
+      If you have installed ``pypiserver`` in a virtualenv, follow ``mod_wsgi``'s
+      `instructions <http://modwsgi.readthedocs.io/en/develop/user-guides/virtual-environments.html>`_
+      and prepend the python code above with the following::
+
+            import site
+
+            site.addsitedir('/yoursite/venv/lib/pythonX.X/site-packages')
+
+.. Note::
+   For security reasons, notice that the ``Directory`` directive grants access
+   to a directory holding the ``wsgi`` start-up script, alone; nothing else.
+
+.. Note::
+   To enable HTTPS support on Apache, configure the directive that contains the
+   WSGI configuration to use SSL.
+
+``gunicorn``
+~~~~~~~~~~~~
+
+The following command uses ``gunicorn`` to start ``pypiserver``::
+
+  gunicorn -w4 'pypiserver:app(root="/home/ralf/packages")'
+
+or when using multiple roots::
+
+  gunicorn -w4 'pypiserver:app(root=["/home/ralf/packages", "/home/ralf/experimental"])'
+
+``paste``
+~~~~~~~~~
+
+`paste <http://pythonpaste.org/>`_ allows to run multiple WSGI applications
+under different URL paths. Therefore it is possible to serve different set
+of packages on different paths.
+
+The following example ``paste.ini`` could be used to serve stable and
+unstable packages on different paths::
+
+    [composite:main]
+    use = egg:Paste#urlmap
+    /unstable/ = unstable
+    / = stable
+
+    [app:stable]
+    use = egg:pypiserver#main
+    root = ~/stable-packages
+
+    [app:unstable]
+    use = egg:pypiserver#main
+    root = ~/stable-packages
+       ~/unstable-packages
+
+    [server:main]
+    use = egg:gunicorn#main
+    host = 0.0.0.0
+    port = 9000
+    workers = 5
+    accesslog = -
+
+.. Note::
+   You need to install some more dependencies for this to work, like::
+
+        pip install paste pastedeploy gunicorn pypiserver
+
+   The server can then start with::
+
+        gunicorn_paster paste.ini
+
+
+Behind a Reverse Proxy
+----------------------
+
+You can run ``pypiserver`` behind a reverse proxy as well.
+
+Nginx
+~~~~~
+
+Extend your nginx configuration::
+
+    upstream pypi {
+      server              pypiserver.example.com:12345 fail_timeout=0;
+    }
+
+    server {
+      server_name         myproxy.example.com;
+
+      location / {
+        proxy_set_header  Host $host:$server_port;
+        proxy_set_header  X-Forwarded-Proto $scheme;
+        proxy_set_header  X-Real-IP $remote_addr;
+        proxy_pass        http://pypi;
+      }
+    }
+
+As of pypiserver 1.3, you may also use the `X-Forwarded-Host` header in your
+reverse proxy config to enable changing the base URL. For example if you
+want to host pypiserver under a particular path on your server::
+
+    upstream pypi {
+      server              localhost:8000;
+    }
+
+    server {
+      location /pypi/ {
+          proxy_set_header  X-Forwarded-Host $host:$server_port/pypi;
+          proxy_set_header  X-Forwarded-Proto $scheme;
+          proxy_set_header  X-Forwarded-For $proxy_add_x_forwarded_for;
+          proxy_set_header  X-Real-IP $remote_addr;
+          proxy_pass        http://pypi;
+      }
+    }
+
+Supporting HTTPS
+~~~~~~~~~~~~~~~~
+
+Using a reverse proxy is the preferred way of getting pypiserver behind
+HTTPS. For example, to put pypiserver behind HTTPS on port 443, with
+automatic HTTP redirection, using `nginx`::
+
+    upstream pypi {
+      server               localhost:8000;
+    }
+
+    server {
+      listen              80 default_server;
+      server_name         _;
+      return              301 https://$host$request_uri;
+    }
+
+    server {
+      listen              443 ssl;
+      server_name         pypiserver.example.com;
+
+      ssl_certificate     /etc/star.example.com.crt;
+      ssl_certificate_key /etc/star.example.com.key;
+      ssl_protocols       TLSv1 TLSv1.1 TLSv1.2;
+      ssl_ciphers         HIGH:!aNULL:!MD5;
+
+      location / {
+        proxy_set_header  Host $host:$server_port;
+        proxy_set_header  X-Forwarded-Proto $scheme;
+        proxy_set_header  X-Real-IP $remote_addr;
+        proxy_pass        http://pypi;
+      }
+    }
+
+Please see `nginx's HTTPS docs for more details <http://nginx.org/en/docs/http/configuring_https_servers.html>`_.
+
+Getting and keeping your certificates up-to-date can be simplified using,
+for example, using `certbot and letsencrypt <https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-18-04>`_.
+
+Traefik
+~~~~~~~
+
+It is also possible to use `Traefik <https://docs.traefik.io/>`_ to put pypiserver behind HTTPS on port 443, with
+automatic HTTP redirection using Docker Compose. Please see the provided `<docker-compose.yml>`_ example for more information.
+
+Utilizing the API
+-----------------
+
+In order to enable ad-hoc authentication-providers or to use WSGI-servers
+not supported by *bottle* out-of-the-box, you needed to launch ``pypiserver``
+via its API.
+
+- The main entry-point for configuring ``pypiserver`` is the `pypiserver:app()
+  <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L116>`_
+  function.  This function returns the internal WSGI-app that you my then
+  send to any WSGI-server you like.
+
+- To get all ``pypiserver:app()`` keywords and their explanations, read the
+  function `pypiserver:default_config()
+  <https://github.com/pypiserver/pypiserver/blob/master/pypiserver/__init__.py#L35>`_.
+
+- Finally, to fire-up a WSGI-server with the configured app, invoke
+  the ``bottle:run(app, host, port, server)`` function.
+  Note that ``pypiserver`` ships with it is own copy of *bottle*; to use it,
+  import it like that: ``from pypiserver import bottle``
+
+Using Ad-Hoc Authentication Providers
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The ``auther`` keyword of ``pypiserver:app()`` function maybe set only using
+the API. This can be any callable that returns a boolean when passed
+the *username* and the *password* for a given request.
+
+For example, to authenticate users based on the ``/etc/passwd`` file under Unix,
+you may delegate such decisions to the `python-pam`_ library by following
+these steps:
+
+1. Ensure ``python-pam`` module is installed::
+
+    pip install python-pam
+
+2. Create a python-script along these lines::
+
+    $ cat > pypiserver-start.py
+    import pypiserver
+    from pypiserver import bottle
+    import pam
+    app = pypiserver.app(root='./packages', auther=pam.authenticate)
+    bottle.run(app=app, host='0.0.0.0', port=80, server='auto')
+
+    [Ctrl+ D]
+
+3. Invoke the python-script to start-up ``pypiserver``::
+
+    $ python pypiserver-start.py
+
+
+.. Note::
+   The `python-pam`_ module, requires *read* access to ``/etc/shadow`` file;
+   you may add the user under which ``pypiserver`` runs into the *shadow*
+   group, with a command like this: ``sudo usermod -a -G shadow pypy-user``.
+
+Use with MicroPython
+--------------------
+The MicroPython interpreter for embedded devices can install packages with the
+module ``upip.py``. The module uses a specialized json-endpoint to retrieve
+package information. This endpoint is supported by ``pypiserver``.
+
+It can be tested with the UNIX port of ``micropython``::
+
+    cd micropython
+    ports/unix/micropython -m tools.upip install -i http://my-server:8080 -p /tmp/mymodules micropython-foobar
+
+Installing packages from the REPL of an embedded device works in this way:
+
+.. code-block:: python
+
+    import network
+    import upip
+
+    sta_if = network.WLAN(network.STA_IF)
+    sta_if.active(True)
+    sta_if.connect('<your ESSID>', '<your password>')
+    upip.index_urls = ["http://my-server:8080"]
+    upip.install("micropython-foobar")
+
+Further information on micropython-packaging can be found here: https://docs.micropython.org/en/latest/reference/packages.html
+
+Custom Health Check Endpoint
+----------------------------
+
+``pypiserver`` provides a default health endpoint at ``/health``. It always returns
+``200 Ok`` if the service is up. Otherwise, it means that the service is not responsive.
+
+In addition, ``pypiserver`` allows users to customize the health endpoint.
+Alphanumeric characters, hyphens, forward slashes and underscores are allowed
+and the endpoint should not overlap with any existing routes.
+Valid examples: ``/healthz``, ``/health/live-1``, ``/api_health``, ``/action/health``
+
+Configure a custom health endpoint by CLI arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Run pypiserver with ``--health-endpoint`` argument::
+
+    pypi-server run --health-endpoint /action/health
+
+Configure a custom health endpoint by script
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    import pypiserver
+    from pypiserver import bottle
+    app = pypiserver.app(root="./packages", health_endpoint="/action/health")
+    bottle.run(app=app, host="0.0.0.0", port=8080, server="auto")
+
+Try ``curl http://localhost:8080/action/health``
+
+
+Sources
+=======
+
+To create a copy of the repository, use::
+
+    git clone https://github.com/pypiserver/pypiserver.git
+    cd pypiserver
+
+To receive any later changes, in the above folder use::
+
+    git pull
+
+
+Known Limitations
+=================
+
+``pypiserver`` does not implement the full API as seen on PyPI_. It
+implements just enough to make ``easy_install``, ``pip install``, and
+``search`` work.
+
+The following limitations are known:
+
+- Command ``pypi -U`` that compares uploaded packages with *pypi* to see if
+  they are outdated, does not respect a http-proxy environment variable
+  (see `#19 <https://github.com/pypiserver/pypiserver/issues/19>`_).
+- It accepts documentation uploads but does not save them to
+  disk (see `#47 <https://github.com/pypiserver/pypiserver/issues/47>`_ for a
+  discussion)
+- It does not handle misspelled packages as *pypi-repo* does,
+  therefore it is suggested to use it with ``--extra-index-url`` instead
+  of ``--index-url`` (see `#38 <https://github.com/pypiserver/pypiserver/issues/38>`_).
+
+Please use Github's `bugtracker <https://github.com/pypiserver/pypiserver/issues>`_
+for other bugs you find.
+
+
+Similar Projects
+================
+
+There are lots of other projects, which allow you to run your own
+PyPI server. If ``pypiserver`` doesn't work for you, the following are
+among the most popular alternatives:
+
+- `devpi-server <https://pypi.org/project/devpi/>`_:
+  a reliable fast pypi.org caching server, part of
+  the comprehensive `github-style pypi index server and packaging meta tool
+  <https://pypi.org/project/devpi/>`_.
+  (version: 2.1.4, access date: 8/3/2015)
+
+- Check this SO question: `How to roll my own pypi
+  <http://stackoverflow.com/questions/1235331/how-to-roll-my-own-pypi>`_
+
+
+Unmaintained or archived
+------------------------
+
+These projects were once alternatives to pypiserver but are now either unmaintained or archived.
+
+- `pip2pi <https://github.com/wolever/pip2pi>`_
+  a simple cmd-line tool that builds a PyPI-compatible local folder from pip requirements
+
+- `flask-pypi-proxy <http://flask-pypi-proxy.readthedocs.org/>`_
+  A proxy for PyPI that also enables also uploading custom packages.
+
+
+Related Software
+================
+
+Though not direct alternatives for ``pypiserver``'s use as an index
+server, the following is a list of related software projects that you
+may want to familiarize with:
+
+- `pypi-uploader`_:
+  A command-line utility to upload packages to your ``pypiserver`` from pypi without
+  having to store them locally first.
+
+- `twine`_:
+  A command-line utility for interacting with PyPI or ``pypiserver``.
+
+- `warehouse`_:
+  the software that powers PyPI_ itself. It is not generally intended to
+  be run by end-users.
+
+Licensing
+=========
+
+``pypiserver`` contains a copy of bottle_ which is available under the
+MIT license, and the remaining part is distributed under the zlib/libpng license.
+See the ``LICENSE.txt`` file.
+
+
+.. _bottle: http://bottlepy.org
+.. _PyPA: https://www.pypa.io/en/latest/
+.. _PyPI: https://pypi.org
+.. _Warehouse: https://github.com/pypa/warehouse/
+.. _twine: https://pypi.org/project/twine/
+.. _pypi-uploader: https://pypi.org/project/pypi-uploader/
+.. _python-pam: https://pypi.org/project/python-pam/
+.. |test-status| image:: https://github.com/pypiserver/pypiserver/actions/workflows/ci.yml/badge.svg
+    :alt: test status
+    :scale: 100%
+    :target: https://github.com/pypiserver/pypiserver/actions/workflows/ci.yml
+
+.. |pypi-ver| image::  https://img.shields.io/pypi/v/pypiserver.svg
+    :target: https://pypi.org/project/pypiserver/
+    :alt: Latest Version in PyPI
+
+.. |python-ver| image:: https://img.shields.io/pypi/pyversions/pypiserver.svg
+    :target: https://pypi.org/project/pypiserver/
+    :alt: Supported Python versions
+
+.. |proj-license| image:: https://img.shields.io/badge/license-BSD%2Bzlib%2Flibpng-blue.svg
+    :target: https://raw.githubusercontent.com/pypiserver/pypiserver/master/LICENSE.txt
+    :alt: Project License
+
+.. |dependencies| image:: https://img.shields.io/requires/github/pypiserver/pypiserver.svg
+    :target: https://requires.io/github/pypiserver/pypiserver/requirements/
+    :alt: Dependencies up-to-date?
```

## Comparing `pypiserver-1.5.1/pypiserver.egg-info/SOURCES.txt` & `pypiserver-1.5.2/pypiserver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,36 @@
 Dockerfile
 LICENSE.txt
 Makefile
 README.rst
 bootstrap.py
 buildout.cfg
 docker-compose.yml
-pypiserver_logo.png
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/rc.yml
 bin/.gitignore
 bin/README.rst
 bin/bumpver.py
 bin/check_readme.sh
 bin/ci_helper.py
 bin/package.sh
 bin/update_changelog.sh
-contributor_docs/README.md
-contributor_docs/architecture_overview.md
 docker/README.md
 docker/docker-requirements.txt
 docker/entrypoint.sh
 docker/gunicorn.conf.py
 docker/test_docker.py
+docs/README.md
+docs/__resources__/pypiserver_logo.png
+docs/contents/.gitkeep
 fixtures/htpasswd.a.a
 fixtures/mypkg/setup.cfg
 fixtures/mypkg/setup.py
 fixtures/mypkg/mypkg/__init__.py
 pypiserver/__init__.py
 pypiserver/__main__.py
 pypiserver/_app.py
@@ -54,14 +55,15 @@
 pypiserver.egg-info/dependency_links.txt
 pypiserver.egg-info/entry_points.txt
 pypiserver.egg-info/requires.txt
 pypiserver.egg-info/top_level.txt
 pypiserver.egg-info/zip-safe
 requirements/dev.pip
 requirements/exe.pip
+requirements/test-requirements.txt
 requirements/test.pip
 tests/__init__.py
 tests/doubles.py
 tests/sample_msg.html
 tests/test-ignorelist
 tests/test_app.py
 tests/test_backend.py
```

## Comparing `pypiserver-1.5.1/tests/test_main.py` & `pypiserver-1.5.2/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         # other passed args.
         __main__.main([str(THIS_DIR)] + argv)
         return self.run_kwargs
 
 
 @pytest.fixture()
 def main(monkeypatch):
-
     main = main_wrapper()
 
     def run(**kwargs):
         sys.stdout.write(f"RUN: {kwargs}\n")
         app = kwargs.pop("app")
         main.app = app
         main.run_kwargs = kwargs
@@ -290,7 +289,24 @@
     assert len(our_check_order) == len(bottle_adapters)
 
     # And the order should be the same
     assert all(
         us.name.lower() in them
         for us, them in zip(our_check_order, bottle_adapters)
     )
+
+
+def test_health_endpoint_default(main):
+    main([])
+    assert main.app._pypiserver_config.health_endpoint == "/health"
+    assert "/health" in (route.rule for route in main.app.routes)
+
+
+def test_health_endpoint_customized(main):
+    main(["--health-endpoint", "/healthz"])
+    assert main.app._pypiserver_config.health_endpoint == "/healthz"
+    assert "/healthz" in (route.rule for route in main.app.routes)
+
+
+def test_health_endpoint_invalid_customized(main):
+    with pytest.raises(SystemExit):
+        main(["--health-endpoint", "/health!"])
```

## Comparing `pypiserver-1.5.1/tests/test_app.py` & `pypiserver-1.5.2/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,20 +184,37 @@
 
 
 def test_packages_empty(testapp):
     resp = testapp.get("/packages/")
     assert len(resp.html("a")) == 0
 
 
-def test_health(testapp):
+def test_health_default_endpoint(testapp):
     resp = testapp.get("/health")
     assert resp.status_int == 200
     assert "Ok" in resp
 
 
+def test_health_customized_endpoint(root):
+    from pypiserver import app
+
+    _app = app(root=root.strpath, health_endpoint="/healthz")
+    testapp = webtest.TestApp(_app)
+    resp = testapp.get("/healthz")
+    assert resp.status_int == 200
+    assert "Ok" in resp
+
+
+def test_health_invalid_customized_endpoint(root):
+    from pypiserver import app
+
+    with pytest.raises(RuntimeError, match="overlaps with existing routes"):
+        app(root=root.strpath, health_endpoint="/simple")
+
+
 def test_favicon(testapp):
     testapp.get("/favicon.ico", status=404)
 
 
 def test_fallback(testapp):
     assert not testapp.app._pypiserver_config.disable_fallback
     resp = testapp.get("/simple/pypiserver/", status=302)
```

## Comparing `pypiserver-1.5.1/tests/test_init.py` & `pypiserver-1.5.2/tests/test_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # Third party imports
 import pytest
 
 
 # Local imports
 import pypiserver
+from pypiserver.config import Config
 
 logger = logging.getLogger(__name__)
 
 TEST_DIR = pathlib.Path(__file__).parent
 HTPASS_FILE = TEST_DIR / "../fixtures/htpasswd.a.a"
 WELCOME_FILE = TEST_DIR / "sample_msg.html"
 
@@ -99,7 +100,23 @@
 def test_backwards_compat_kwargs_duplicate_check(
     kwargs: t.Dict[str, t.Any]
 ) -> None:
     """Duplicate legacy and modern kwargs cause an error."""
     with pytest.raises(ValueError) as err:
         pypiserver.backwards_compat_kwargs(kwargs)
     assert "('redirect_to_fallback', 'disable_fallback')" in str(err.value)
+
+
+def test_setup_routes_from_config_customized_endpoint() -> None:
+    _app = pypiserver.setup_routes_from_config(
+        pypiserver.app(),
+        Config.default_with_overrides(health_endpoint="/healthz"),
+    )
+    assert "/healthz" in (route.rule for route in _app.routes)
+
+
+def test_setup_routes_from_config_invalid_customized_endpoint() -> None:
+    with pytest.raises(RuntimeError, match="overlaps with existing routes"):
+        pypiserver.setup_routes_from_config(
+            pypiserver.app(),
+            Config.default_with_overrides(health_endpoint="/simple"),
+        )
```

## Comparing `pypiserver-1.5.1/tests/test_server.py` & `pypiserver-1.5.2/tests/test_server.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/tests/test_config.py` & `pypiserver-1.5.2/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -365,14 +365,29 @@
     ConfigTestCase(
         case="Run: fallback-url specified",
         args=["run", "--fallback-url", "foobar.com"],
         legacy_args=["--fallback-url", "foobar.com"],
         exp_config_type=RunConfig,
         exp_config_values={"fallback_url": "foobar.com"},
     ),
+    # health-endpoint
+    ConfigTestCase(
+        case="Run: health-endpoint unspecified",
+        args=["run"],
+        legacy_args=[],
+        exp_config_type=RunConfig,
+        exp_config_values={"health_endpoint": DEFAULTS.HEALTH_ENDPOINT},
+    ),
+    ConfigTestCase(
+        case="Run: health-endpoint specified",
+        args=["run", "--health-endpoint", "/healthz"],
+        legacy_args=["--health-endpoint", "/healthz"],
+        exp_config_type=RunConfig,
+        exp_config_values={"health_endpoint": "/healthz"},
+    ),
     # server method
     ConfigTestCase(
         case="Run: server method unspecified",
         args=["run"],
         legacy_args=[],
         exp_config_type=RunConfig,
         exp_config_values={"server_method": DEFAULTS.SERVER_METHOD},
@@ -679,14 +694,22 @@
         ConfigErrorCase(
             case=f"Invalid hash algo: {val}",
             args=["run", "--hash-algo", val],
             exp_txt=f"Hash algorithm '{val}' is not available",
         )
         for val in ("true", "foo", "1", "md6")
     ),
+    *(
+        ConfigErrorCase(
+            case=f"Invalid health endpoint: {val}",
+            args=["run", "--health-endpoint", val],
+            exp_txt="Invalid path for the health endpoint",
+        )
+        for val in ("/", "health", "/health!", "/:health", "/health?check=True")
+    ),
 )
 # pylint: disable=unsubscriptable-object
 CONFIG_ERROR_PARAMS = (i[1:] for i in _CONFIG_ERROR_CASES)
 # pylint: enable=unsubscriptable-object
 CONFIG_ERROR_IDS = (i.case for i in _CONFIG_ERROR_CASES)
 
 
@@ -721,15 +744,15 @@
 
     assert conf == conf_legacy
 
 
 @pytest.mark.parametrize(
     "args, exp_txt",
     CONFIG_ERROR_PARAMS,
-    ids=CONFIG_TEST_IDS,
+    ids=CONFIG_ERROR_IDS,
 )
 def test_config_error(
     args: t.List[str],
     exp_txt: t.Optional[str],
     capsys,
 ) -> None:
     """Validate error cases."""
```

## Comparing `pypiserver-1.5.1/tests/test_pkg_helpers.py` & `pypiserver-1.5.2/tests/test_pkg_helpers.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/tests/test_core.py` & `pypiserver-1.5.2/tests/test_core.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/tests/test_backend.py` & `pypiserver-1.5.2/tests/test_backend.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/tests/test_manage.py` & `pypiserver-1.5.2/tests/test_manage.py`

 * *Files identical despite different names*

## Comparing `pypiserver-1.5.1/.github/workflows/ci.yml` & `pypiserver-1.5.2/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,53 @@
 # Run tests
 
 name: CI
 
 on:
   # This will run when any branch or tag is pushed
   push:
-    # standalone is an old branch containing a fully functional pypiserver
-    # executable, from back in the day before docker & a better pip.
-    branches-ignore:
-      - standalone
+    branches:
+      - "master"
     tags:
       - "v**"
-  # Allowing to run on fork pull requests
+  # Allowing to run on fork and other pull requests
   pull_request:
 
 jobs:
-  test-cpython:
+  test-python:
     runs-on: ubuntu-latest
     strategy:
+      fail-fast: false
       matrix:
-        # Commented out as tests with tox on python3.9 fail with updated dependencies.
-        # See https://github.com/pypiserver/pypiserver/issues/406.
-        # uncomment when the issue #406 is resolved.
-        # python-version: ["3.6", "3.7", "3.8", "3.9"]
-        python-version: ["3.6", "3.7", "3.8"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "pypy3.9", "3.11"] # "3.12-dev"
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
-        run: pip install tox
-      - name: Run tests
-        # Create a tox env specification by stripping the dot out of the version
-        # specification and appending it to "py"
         run: |
-          tox -e "py$(echo ${{ matrix.python-version }} | tr -d .)"
-
-  test-pypy:
-    # Run a a separate job so we don't need to mess with conditionally
-    # splitting the python version from the build matrix. Also the pypy
-    # tests take freaking forever.
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v2
-      - name: Set up Python
-        uses: actions/setup-python@v2
-        with:
-          python-version: pypy3
-      - name: Install dependencies
-        run: pip install tox
+          pip install --upgrade setuptools
+          pip install tox==3.27.*
       - name: Run tests
-        run: tox -e pypy3
+        run: tox -e py
 
   check:
-    # These checks only need to be done once, not for every python version we s
-    # upport
+    # These checks only need to be done once, not for every python version we
+    # support
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          # Pretty much any python version will do
-          python-version: "3.9"
+          # Use the current version of Python
+          python-version: "3.x"
       - name: Install dependencies
         run: |
           pip install -r "requirements/dev.pip"
           pip install types-pkg_resources # one of mypy required stubs
       - name: Check types
         # individual mypy files for now, until we get the rest
         # of the project typechecking
@@ -88,34 +66,33 @@
   # installed. I'm going to say for now probably 99% of people using
   # the docker image will be doing so from a linux system, e.g. for
   # a k8s deploy, and I've verified manually that things work on
   # MacOS, so /shrug.
   test-docker:
     runs-on: "ubuntu-latest"
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          # Pretty much any python version will do
-          python-version: "3.9"
+          # Use the current version of Python
+          python-version: "3.x"
       - name: Install test dependencies
         run: pip install -r "requirements/test.pip"
       - name: Install package
         run: pip install -r "requirements/exe.pip"
       - name: Run tests
         run: "pytest docker/test_docker.py"
 
   tests:
     runs-on: "ubuntu-latest"
     needs:
       - "check"
       - "test-docker"
-      - "test-cpython"
-      - "test-pypy"
+      - "test-python"
     steps:
       - name: "Everything is good!"
         run: "echo true"
 
   # RELEASES
 
   ## PYPI
@@ -124,18 +101,18 @@
     runs-on: ubuntu-latest
     needs:
       - "tests"
     # only if a tag is pushed
     if: startsWith(github.event.ref, 'refs/tags/v')
     steps:
       - uses: actions/checkout@master
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v1
+      - name: Set up Python
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: 3.x
 
       - name: Build distribution _wheel_.
         run: |
           ./bin/package.sh
 
       - name: Publish distribution 📦 to PyPI.
         uses: pypa/gh-action-pypi-publish@master
@@ -147,19 +124,19 @@
 
   # figure out which docker tags we need to push
   docker-determine-tags:
     runs-on: "ubuntu-latest"
     needs:
       - "tests"
     steps:
-      - uses: "actions/checkout@v2"
+      - uses: "actions/checkout@v3"
 
-      - uses: "actions/setup-python@v2"
+      - uses: "actions/setup-python@v4"
         with:
-          python-version: "3.9"
+          python-version: "3.x"
 
         # This script prints a JSON array of needed docker tags, depending on the
         # ref. That array is then used to construct the matrix of the
         # deploy-docker job
       - name: "Get expected docker tags"
         id: "tags"
         run: >-
@@ -184,18 +161,18 @@
     needs:
       - "docker-determine-tags"
     if: "${{ fromJson(needs.docker-determine-tags.outputs.has_tags) }}"
     strategy:
       matrix:
         tag: "${{ fromJson(needs.docker-determine-tags.outputs.tags) }}"
     steps:
-      - uses: "actions/checkout@v2"
+      - uses: "actions/checkout@v3"
 
       - name: "Cache Docker layers"
-        uses: "actions/cache@v2"
+        uses: "actions/cache@v3"
         with:
           path: "/tmp/.buildx-cache"
           key: "${{ runner.os }}-buildx-${{ github.sha }}"
           restore-keys: |
             ${{ runner.os }}-buildx-
 
       - name: "Login to Docker Hub"
```

## Comparing `pypiserver-1.5.1/.github/workflows/rc.yml` & `pypiserver-1.5.2/.github/workflows/rc.yml`

 * *Files identical despite different names*

