# Comparing `tmp/scikit_build_core-0.4.7.tar.gz` & `tmp/scikit_build_core-0.4.8.tar.gz`

## Comparing `scikit_build_core-0.4.7.tar` & `scikit_build_core-0.4.8.tar`

### file list

```diff
@@ -1,267 +1,268 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.gitattributes
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.packit.yaml
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.readthedocs.yml
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/noxfile.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.fmf/version
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/packit.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/examples.fmf
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/smoke.fmf
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/tests/rpmlint.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/tests/smoke.fmf
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/changelog.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/cmakelists.md
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/conf.py
--rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/configuration.md
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/getting_started.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/index.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/man.md
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/migration_guide.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/main.fmf
--rwxr-xr-x   0        0        0      865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/test.sh
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/LICENSE
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/README.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/pyproject.toml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/tests/test_basic.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/LICENSE
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/README.md
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/src/main.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/tests/test_basic.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/main.fmf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/main.fmf
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/main.fmf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/main.fmf
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/nanobind/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/nanobind/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/main.fmf
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7032 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_cmake_config.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_file_processor.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_fileapi.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_get_requires.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_shutil.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_simplest_c.py
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/LICENSE
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/README.md
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    14490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.gitattributes
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.packit.yaml
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.readthedocs.yml
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/noxfile.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.fmf/version
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/plans/examples.fmf
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/distro/tests/smoke.fmf
+-rw-r--r--   0        0        0    19389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/changelog.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/cmakelists.md
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/conf.py
+-rw-r--r--   0        0        0    11449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/configuration.md
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/getting_started.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/index.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/man.md
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/migration_guide.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/main.fmf
+-rwxr-xr-x   0        0        0      903 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/test.sh
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/abi3/main.fmf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/c/main.fmf
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/cython/main.fmf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/fortran/main.fmf
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/nanobind/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/nanobind/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/pybind11/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/swig/main.fmf
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/docs/ext/conftabs.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    10983 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_get_requires.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_shutil.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    14376 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/LICENSE
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/README.md
+-rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0    14706 2020-02-02 00:00:00.000000 scikit_build_core-0.4.8/PKG-INFO
```

### Comparing `scikit_build_core-0.4.7/.packit.yaml` & `scikit_build_core-0.4.8/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/.pre-commit-config.yaml` & `scikit_build_core-0.4.8/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -25,46 +25,46 @@
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.14.0
+    rev: 1.15.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.3.0]
 
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
     hooks:
       - id: cmake-format
         exclude: ^src/scikit_build_core/resources/find_python
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.275
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         exclude: |
           (?x)^(
             tests/packages/simplest_c/src/simplest/__init__.py|
             tests/packages/dynamic_metadata/src/dynamic/__init__.py|
             tests/packages/.*/setup.py
```

### Comparing `scikit_build_core-0.4.7/noxfile.py` & `scikit_build_core-0.4.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.8/.github/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 ```bash
 nox -s downstream -- https://github.com/...
 ```
 
 # Setting up for development
 
-See the [Scikit-HEP Developer introduction][skhep-dev-intro] for a detailed
-description of best practices for developing packages.
+See the [Scientific-Python Development Guide][skdev] for a detailed description
+of best practices for developing packages.
 
-[skhep-dev-intro]: https://scikit-hep.org/developer/intro
+[skdev]: https://learn.scientific-python.org/development
 
 ## Quick development
 
 The fastest way to start with development is to use nox. If you don't have nox,
 you can use `pipx run nox` to run it without installing, or `pipx install nox`.
 If you don't have pipx (pip for applications), then you can install with with
 `pip install pipx` (the only case were installing an application with regular
```

### Comparing `scikit_build_core-0.4.7/.github/matchers/pylint.json` & `scikit_build_core-0.4.8/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/.github/workflows/cd.yml` & `scikit_build_core-0.4.8/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/.github/workflows/ci.yml` & `scikit_build_core-0.4.8/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,15 @@
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v1
 
   docs:
     name: Docs on ${{ matrix.runs-on }}
     strategy:
+      fail-fast: false
       matrix:
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.runs-on }}
     timeout-minutes: 15
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `scikit_build_core-0.4.7/distro/python-scikit-build-core.spec` & `scikit_build_core-0.4.8/distro/python-scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/changelog.md` & `scikit_build_core-0.4.8/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,44 @@
 # Changelog
 
+## Version 0.4.8
+
+This release focus on two fixes that correct some interference issues with other
+setuptools plugins. A few new features were added (opt-in only): the ability to
+select build targets, install components, and opt-in `--strip` (will be opt-out
+in 0.5 if the minimum-version is set to 0.5+ or unset).
+
+Features:
+
+- Add build target support by @henryiii in #432
+- Add component support and strip support by @henryiii in #430
+
+Fixes:
+
+- (setuptools) Avoid instantiating build too soon by @henryiii in #443
+- (setuptools) Avoid interfering with other setuptools plugins by @henryiii in
+  #414
+- Only link to valid module paths (not things like gitignore) in editable
+  installs by @henryiii in #444
+
+Docs:
+
+- Fix typo and invalid Markdown in `getting_started.md` by @0xTowel in #439
+- Conf tabs as extension by @henryiii in #433
+- Fix `nanobind`/`pybind11` `src` & sp-dev by @henryiii in #429
+- Link to source by @henryiii in #431
+- Small suggestions for docs by @rebecca-burwei in #428
+
+Tests and other:
+
+- Fix fedora downstream tests by @LecrisUT in #416
+- Ruff moved to astral-sh by @henryiii in #418
+- `target-version` no longer needed by Black or Ruff by @henryiii in #419
+- Use `get_origin`/`get_args` by @henryiii in #423
+
 ## Version 0.4.7
 
 This version fixes a unused variable message in 0.4.6, along with a debug
 logging improvement, and a few test fixes, including a regression in the recent
 noxfile reworking.
 
 - fix: remove `SKBUILD_STATE` unused message when building by @henryiii in #401
```

### Comparing `scikit_build_core-0.4.7/docs/cmakelists.md` & `scikit_build_core-0.4.8/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/configuration.md` & `scikit_build_core-0.4.8/docs/configuration.md`

 * *Files 14% similar despite different names*

```diff
@@ -223,65 +223,34 @@
 historic compatibility if you'd like:
 
 ```toml
 [tool.scikit-build]
 wheel.expand-macos-universal-tags = false
 ```
 
-## Configuring CMake arguments and defines
-
-You can select a different build type, such as `Debug`:
-
-````{tab} pyproject.toml
-
-```toml
-[tool.scikit-build]
-cmake.build-type = "Debug"
-```
-
-````
-
-`````{tab} config-settings
-
+You can select only specific components to install:
 
-````{tab} pip
-
-```console
-$ pip install . --config-settings=cmake.build-type=Debug
-```
-
-````
-
-````{tab} build
+```{conftabs} install.components ["python"]
 
-```console
-$ pipx run build --wheel -Ccmake.build-type=Debug
 ```
 
-````
+And you can turn off binary stripping:
 
-````{tab} cibuildwheel
+```{conftabs} install.strip False
 
-```toml
-[tool.cibuildwheel.config-settings]
-"cmake.build-type" = "Debug"
 ```
 
-````
+## Configuring CMake arguments and defines
 
-`````
+You can select a different build type, such as `Debug`:
 
-````{tab} Environment
+```{conftabs} cmake.build-type "Debug"
 
-```yaml
-SKBUILD_CMAKE_BUILD_TYPE: Debug
 ```
 
-````
-
 You can specify CMake defines:
 
 ````{tab} pyproject.toml
 
 ```toml
 [tool.scikit-build.cmake.define]
 SOME_DEFINE = "ON"
@@ -292,16 +261,14 @@
 `````{tab} config-settings
 
 
 ````{tab} pip
 
 ```console
 $ pip install . --config-settings=cmake.define.SOME_DEFINE=ON
-$ # NEXT VERSION OF PIP ONLY
-$ pip install . -Ccmake.define.SOME_DEFINE=ON
 ```
 
 ````
 
 ````{tab} build
 
 ```console
@@ -325,79 +292,47 @@
 
 ```yaml
 SKBUILD_CMAKE_DEFINES: SOME_DEFINE=ON
 ```
 
 ````
 
-You can also manually specify the exact cmake args. Beyond the normal
+You can also manually specify the exact CMake args. Beyond the normal
 `SKBUILD_CMAKE_ARGS`, the `CMAKE_ARGS` space-separated environment variable is
 also supported (with some filtering for options scikit-build-core doesn't
 support overriding).
 
-````{tab} pyproject.toml
-
-```toml
-[tool.scikit-build]
-cmake.args = ["-DSOME_DEFINE=ON", "-DOTHER=OFF"]
-```
-
-````
-
-`````{tab} config-settings
-
-
-````{tab} pip
-
-```console
-$ pip install . --config-settings=cmake.args="-DSOME_DEFINE=ON;-DOTHER=OFF"
-$ # NEXT VERSION OF PIP ONLY
-$ pip install . -Ccmake.args=-SOME_DEFINE=ON -Ccmake.args=-DOTHER=OFF
-```
-
-````
+```{conftabs} cmake.args ["-DSOME_DEFINE=ON", "-DOTHER=OFF"]
 
-````{tab} build
-
-```console
-$ pipx run build -Ccmake.args="-DSOME_DEFINE=ON;-DOTHER=OFF"
-$ pipx run build -Ccmake.args=-DSOME_DEFINE=ON -Ccmake.args=-DOTHER=OFF
 ```
 
-````
+You can also specify this using CMAKE_ARGS, spae separated:
 
-````{tab} cibuildwheel
-
-```toml
-[tool.cibuildwheel.config-settings]
-"cmake.args" = ["-DSOME_DEFINE=ON", "-DOTHER=OFF"]
+```yaml
+CMAKE_ARGS: -DSOME_DEFINE=ON -DOTHER=OFF
 ```
 
-````
-
-`````
+You can also specify only specific targets to build (leaving this off builds the
+default targets):
 
-````{tab} Environment
+```{conftabs} cmake.targets ["python"]
 
-```yaml
-SKBUILD_CMAKE_ARGS: -DSOME_DEFINE=ON;-DOTHER=OFF
-CMAKE_ARGS: -DSOME_DEFINE=ON -DOTHER=OFF
 ```
 
-````
-
 ## Dynamic metadata
 
 Scikit-build-core 0.3.0 supports dynamic metadata with two built-in plugins.
 
 :::{warning}
 
 This is not ready for plugin development outside of scikit-build-core;
 `tool.scikit-build.experimental=true` is required to use plugins that are not
-shipped with scikit-build-core, since the interface is provisional. :::
+shipped with scikit-build-core, since the interface is provisional.
+
+:::
 
 :::{tab} Setuptools-scm
 
 You can use [setuptools-scm](https://github.com/pypa/setuptools_scm) to pull the
 version from VCS:
 
 ```toml
@@ -492,61 +427,18 @@
 
 ## Other options
 
 You can select a custom build dir; by default scikit-build-core will use a
 temporary dir. If you select a persistent one, you can get major rebuild
 speedups.
 
-````{tab} pyproject.toml
+```{conftabs} build-dir "build/{wheel_tag}"
 
-```toml
-[tool.scikit-build]
-build-dir = "build/{wheel_tag}"
 ```
 
-````
-
-`````{tab} config-settings
-
-
-````{tab} pip
-
-```console
-$ pip install . --config-settings='build-dir=build/{wheel_tag}'
-```
-
-````
-
-````{tab} build
-
-```console
-$ pipx run build --wheel -Cbuild-dir='build/{wheel_tag}'
-```
-
-````
-
-````{tab} cibuildwheel
-
-```toml
-[tool.cibuildwheel.config-settings]
-build-dir = "build/{wheel_tag}"
-```
-
-````
-
-`````
-
-````{tab} Environment
-
-```yaml
-SKBUILD_BUILD_DIR: "build/{wheel_tag}"
-```
-
-````
-
 Scikit-build-core also strictly validates configuration; if you need to disable
 this, you can:
 
 ```toml
 [tool.scikit-build]
 strict-config = false
 ```
```

### Comparing `scikit_build_core-0.4.7/docs/getting_started.md` & `scikit_build_core-0.4.8/docs/getting_started.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 # Getting started
 
 If you've never made a Python package before,
 [packaging.python.org's tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 is a great place to start. It walks you through creating a simple package in
-pure Python using modern tooling and configuration.
+pure Python using modern tooling and configuration. Another great resource is
+the
+[Scientific Python Developer Guide](https://learn.scientific-python.org/development).
 
 ## Writing an extension
 
 We will be writing these files:
 
-````{tab} C
+````{tab} pybind11
 
 ```
 example-project
-├── example.c
+├── example.cpp
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
-````{tab} ABI3
+````{tab} nanobind
 
 ```
 example-project
-├── example.c
+├── example.cpp
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
-````{tab} pybind11
+````{tab} SWIG
 
 ```
 example-project
-├── example.cpp
+├── example.c
+├── example.i
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
-````{tab} nanobind
+````{tab} Cython
 
 ```
 example-project
-├── example.cpp
+├── example.pyx
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
-````{tab} SWIG
+````{tab} C
 
 ```
 example-project
 ├── example.c
-├── example.i
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
-````{tab} Cython
+````{tab} ABI3
 
 ```
 example-project
-├── example.pyx
+├── example.c
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
 ````{tab} Fortran
@@ -88,30 +90,14 @@
 ````
 
 ### Source code
 
 For this tutorial, you can either write a C extension yourself, or you can use
 pybind11 and C++. Select your preferred version using the tabs - compare them!
 
-````{tab} C
-
-```{literalinclude} examples/getting_started/c/example.c
-:language: c
-```
-
-````
-
-````{tab} ABI3
-
-```{literalinclude} examples/getting_started/abi3/example.c
-:language: c
-```
-
-````
-
 ````{tab} pybind11
 
 ```{literalinclude} examples/getting_started/pybind11/example.cpp
 :language: cpp
 ```
 
 ````
@@ -140,42 +126,42 @@
 
 ```{literalinclude} examples/getting_started/cython/example.pyx
 :language: cython
 ```
 
 ````
 
-````{tab} Fortran
+````{tab} C
 
-```{literalinclude} examples/getting_started/fortran/example.f
-:language: fortran
+```{literalinclude} examples/getting_started/c/example.c
+:language: c
 ```
 
 ````
 
-### Python package configuration
-
-To create your first compiled package, start with a pyproject.toml like this:
-
-````{tab} C
+````{tab} ABI3
 
-```{literalinclude} examples/getting_started/c/pyproject.toml
-:language: toml
+```{literalinclude} examples/getting_started/abi3/example.c
+:language: c
 ```
 
 ````
 
-````{tab} ABI3
+````{tab} Fortran
 
-```{literalinclude} examples/getting_started/abi3/pyproject.toml
-:language: toml
+```{literalinclude} examples/getting_started/fortran/example.f
+:language: fortran
 ```
 
 ````
 
+### Python package configuration
+
+To create your first compiled package, start with a pyproject.toml like this:
+
 ````{tab} pybind11
 
 ```{literalinclude} examples/getting_started/pybind11/pyproject.toml
 :language: toml
 ```
 
 ````
@@ -190,23 +176,37 @@
 
 ````{tab} SWIG
 
 ```{literalinclude} examples/getting_started/swig/pyproject.toml
 :language: toml
 ```
 
-
 ````
 
 ````{tab} Cython
 
 ```{literalinclude} examples/getting_started/cython/pyproject.toml
 :language: toml
 ```
 
+````
+
+````{tab} C
+
+```{literalinclude} examples/getting_started/c/pyproject.toml
+:language: toml
+```
+
+````
+
+````{tab} ABI3
+
+```{literalinclude} examples/getting_started/abi3/pyproject.toml
+:language: toml
+```
 
 ````
 
 ````{tab} Fortran
 
 ```{literalinclude} examples/getting_started/fortran/pyproject.toml
 :language: toml
@@ -231,143 +231,143 @@
 tools installed. Setuptools is not used by scikit-build-core's native builder,
 and wheel should never be in this list.
 
 There are other keys you should include under `[project]` if you plan to publish
 a package, but this is enough to start for now. The
 [project metadata specification](https://packaging.python.org/en/latest/specifications/declaring-project-metadata)
 page covers what keys are available. Another example is available at
-[the Scikit-HEP Developer Pages](https://scikit-hep.org/developer/pep621).
+[the Scientific Python Library Development Guide](https://learn.scientific-python.org/development/guides/).
 
 ### CMake file
 
-Now, you'll need a CMake file. This one will do:
+Now, you'll need a file called `CMakeLists.txt`. This one will do:
 
-````{tab} C
+````{tab} pybind11
 
-```{literalinclude} examples/getting_started/c/CMakeLists.txt
+```{literalinclude} examples/getting_started/pybind11/CMakeLists.txt
 :language: cmake
 ```
 
 Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
 
 The project line can optionally use `SKBUILD_PROJECT_NAME` and
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
-`find_package(Python ...)` should always include the `Development.Module`
-component instead of `Developement`; the latter breaks if the embedding
-components are missing, such as when you are building redistributable wheels on
-Linux.
+If you place find Python first, pybind11 will respect it instead of the classic
+FindPythonInterp/FindPythonLibs mechanisms, which work, but are not as modern.
+Here we set `PYBIND11_NEWPYTHON` to `ON` instead of doing the find Python
+ourselves. Pybind11 places its config file such that CMake can find it from
+site-packages.
 
-You'll want `WITH_SOABI` when you make the module to ensure the full extension
-is included on Unix systems (PyPy won't even be able to open the extension
-without it).
+You can either use `pybind11_add_module` or `python_add_library` and then link
+to `pybind11::module`, your choice.
 
 ````
 
-````{tab} ABI3
+````{tab} nanobind
 
-```{literalinclude} examples/getting_started/abi3/CMakeLists.txt
+```{literalinclude} examples/getting_started/nanobind/CMakeLists.txt
 :language: cmake
 ```
 
-Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
+Scikit-build and nanobind require CMake 3.15, so there's no need to set it
+lower than 3.15.
 
 The project line can optionally use `SKBUILD_PROJECT_NAME` and
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
-`find_package(Python ...)` needs `Development.SABIModule` for ABI3 extensions.
-
-You'll want `WITH_SOABI` when you make the module. You'll also need to set the `USE_SABI`
-argument to the minimum version to build with. This will also add a proper
-PRIVATE define of `Py_LIMITED_API` for you.
-
-```{note}
-This will not support pypy, so you'll want to provide an alternative if you
-support PyPy).
-```
-
+Nanobind places its config file such that CMake can find it from site-packages.
 ````
 
-````{tab} pybind11
+````{tab} SWIG
 
-```{literalinclude} examples/getting_started/pybind11/CMakeLists.txt
+```{literalinclude} examples/getting_started/swig/CMakeLists.txt
 :language: cmake
 ```
 
 Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
 
 The project line can optionally use `SKBUILD_PROJECT_NAME` and
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
-If you place find Python first, pybind11 will resepct it instead of the classic
-FindPythonInterp/FindPythonLibs mechanisms, which work, but are not as modern.
-Here we set `PYBIND11_NEWPYTHON` to `ON` instead of doing the find Python
-ourselves. Pybind11 places its config file such that CMake can find it from
-site-packages.
-
-You can either use `pybind11_add_module` or `python_add_library` and then link
-to `pybind11::module`, your choice.
+You'll need to handle the generation of files by SWIG directly.
 
 ````
 
-````{tab} nanobind
+````{tab} Cython
 
-```{literalinclude} examples/getting_started/pybind11/CMakeLists.txt
+```{literalinclude} examples/getting_started/cython/CMakeLists.txt
 :language: cmake
 ```
 
-Scikit-build and nanobind require CMake 3.15, so there's no need to set it
-lower than 3.15.
+Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
 
 The project line can optionally use `SKBUILD_PROJECT_NAME` and
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
-Nanobind places its config file such that CMake can find it from site-packages.
+You'll need to handle the generation of files by Cython directly at the moment.
+A helper (similar to scikit-build classic) might be added in the future.
+
 ````
 
-````{tab} SWIG
+````{tab} C
 
-```{literalinclude} examples/getting_started/swig/CMakeLists.txt
+```{literalinclude} examples/getting_started/c/CMakeLists.txt
 :language: cmake
 ```
 
 Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
 
 The project line can optionally use `SKBUILD_PROJECT_NAME` and
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
-You'll need to handle the generation of files by SWIG directly.
+`find_package(Python ...)` should always include the `Development.Module`
+component instead of `Developement`; the latter breaks if the embedding
+components are missing, such as when you are building redistributable wheels on
+Linux.
+
+You'll want `WITH_SOABI` when you make the module to ensure the full extension
+is included on Unix systems (PyPy won't even be able to open the extension
+without it).
 
 ````
 
-````{tab} Cython
+````{tab} ABI3
 
-```{literalinclude} examples/getting_started/cython/CMakeLists.txt
+```{literalinclude} examples/getting_started/abi3/CMakeLists.txt
 :language: cmake
 ```
 
 Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
 
 The project line can optionally use `SKBUILD_PROJECT_NAME` and
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
-You'll need to handle the generation of files by Cython directly at the moment.
-A helper (similar to scikti-build classic) might be added in the future.
+`find_package(Python ...)` needs `Development.SABIModule` for ABI3 extensions.
+
+You'll want `WITH_SOABI` when you make the module. You'll also need to set the `USE_SABI`
+argument to the minimum version to build with. This will also add a proper
+PRIVATE define of `Py_LIMITED_API` for you.
+
+```{note}
+This will not support pypy, so you'll want to provide an alternative if you
+support PyPy).
+```
 
 ````
 
 ````{tab} Fortran
 
 ```{literalinclude} examples/getting_started/fortran/CMakeLists.txt
 :language: cmake
@@ -394,14 +394,17 @@
 
 That's it! You can try building it:
 
 ```console
 $ pipx run build
 ```
 
+[pipx](https://pypa.github.io/pipx/) allows you to install and run Python
+applications in isolated environments.
+
 Or installing it (in a virtualenv, ideally):
 
 ```console
 $ pip install .
 ```
 
 That's it for a basic package!
```

### Comparing `scikit_build_core-0.4.7/docs/index.md` & `scikit_build_core-0.4.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/migration_guide.md` & `scikit_build_core-0.4.8/docs/migration_guide.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.8/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/test.sh` & `scikit_build_core-0.4.8/docs/examples/test.sh`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # vim: dict+=/usr/share/beakerlib/dictionary.vim cpt=.,w,b,u,t,i,k
 # shellcheck disable=all
 source /usr/share/beakerlib/beakerlib.sh || exit 1
 
 rlJournalStart
     rlPhaseStartSetup
         rlRun "tmp=\$(mktemp -d)" 0 "Create tmp directory"
-		    rlRun "rsync -r $TMT_TREE$TMT_TEST_NAME/ $tmp" 0 "Copy example project"
-		    rlRun "rsync -r $TMT_TREE$TMT_TEST_NAME/../test.py $tmp" 0 "Copy test.py file"
+		    rlRun "rsync -r ${TMT_SOURCE_DIR:-$TMT_TREE}$TMT_TEST_NAME/ $tmp" 0 "Copy example project"
+		    rlRun "rsync -r ${TMT_SOURCE_DIR:-$TMT_TREE}$TMT_TEST_NAME/../test.py $tmp" 0 "Copy test.py file"
         rlRun "pushd $tmp"
         rlRun "tree" 0 "Show directory tree"
         rlRun "set -o pipefail"
     rlPhaseEnd
 
     rlPhaseStartTest
         rlRun "pip install . --config-settings=cmake.verbose=true" 0 "Build the python project"
```

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/CMakeLists.txt` & `scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/LICENSE` & `scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/README.md` & `scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/pyproject.toml` & `scikit_build_core-0.4.8/docs/examples/downstream/nanobind_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/LICENSE` & `scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/README.md` & `scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/pyproject.toml` & `scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/src/main.cpp` & `scikit_build_core-0.4.8/docs/examples/downstream/pybind11_example/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.8/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.8/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.8/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.8/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.8/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.8/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.4.8/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.8/src/scikit_build_core/cmake.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,34 +205,58 @@
     ) -> Generator[str, None, None]:
         if verbose:
             yield "-v"
         if self.build_type and not self.single_config:
             yield "--config"
             yield self.build_type
 
-    def build(self, build_args: Sequence[str] = (), *, verbose: bool = False) -> None:
+    def build(
+        self,
+        build_args: Sequence[str] = (),
+        *,
+        targets: Sequence[str] = (),
+        verbose: bool = False,
+    ) -> None:
         local_args = self._compute_build_args(verbose=verbose)
+        if not targets:
+            self._build(*local_args, *build_args)
+            return
 
+        for target in targets:
+            self._build(*local_args, "--target", target, *build_args)
+
+    def _build(self, *args: str) -> None:
         try:
-            Run(env=self.env).live(
-                self.cmake, "--build", self.build_dir, *build_args, *local_args
-            )
+            Run(env=self.env).live(self.cmake, "--build", self.build_dir, *args)
         except subprocess.CalledProcessError:
             msg = "CMake build failed"
             raise FailedLiveProcessError(msg) from None
 
-    def install(self, prefix: Path) -> None:
-        opts: list[str] = []
+    def install(
+        self, prefix: Path, *, strip: bool = False, components: Sequence[str] = ()
+    ) -> None:
+        opts = ["--prefix", str(prefix)]
         if not self.single_config and self.build_type:
             opts += ["--config", self.build_type]
+        if strip:
+            opts.append("--strip")
+
+        if not components:
+            self._install(opts)
+            return
+
+        for comp in components:
+            opts_with_comp = [*opts, "--component", comp]
+            logger.info("Installing component {}", comp)
+            self._install(opts_with_comp)
+
+    def _install(self, opts: Sequence[str]) -> None:
         try:
             Run(env=self.env).live(
                 self.cmake,
                 "--install",
                 self.build_dir,
-                "--prefix",
-                prefix,
                 *opts,
             )
         except subprocess.CalledProcessError:
             msg = "CMake install failed"
             raise FailedLiveProcessError(msg) from None
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.8/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.8/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.8/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/_pathutil.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from collections.abc import Generator, Sequence
 from pathlib import Path
 
 from ._file_processor import each_unignored_file
 
-__all__ = ["scantree", "path_to_module", "packages_to_file_mapping"]
+__all__ = ["scantree", "path_to_module", "packages_to_file_mapping", "is_valid_module"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 def scantree(path: Path) -> Generator[Path, None, None]:
@@ -46,7 +46,15 @@
             exclude=exclude,
         ):
             package_dir = platlib_dir / filepath.relative_to(base_path)
             if not package_dir.is_file():
                 mapping[str(filepath)] = str(package_dir)
 
     return mapping
+
+
+def is_valid_module(path: Path) -> bool:
+    parts = path.parts
+    return (
+        all(p.isidentifier() for p in parts[:-1])
+        and parts[-1].split(".", 1)[0].isidentifier()
+    )
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/sdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             gzip.GzipFile(sdist_dir / filename, mode="wb", mtime=timestamp)
         )
         tar = stack.enter_context(
             tarfile.TarFile(fileobj=gzip_container, mode="w", format=tarfile.PAX_FORMAT)
         )
         paths = sorted(
             each_unignored_file(
-                Path("."),
+                Path(),
                 include=settings.sdist.include,
                 exclude=settings.sdist.exclude,
             )
         )
         for filepath in paths:
             tar.add(
                 filepath,
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.8/src/scikit_build_core/build/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 from ..builder.builder import Builder, archs_to_tags, get_archs
 from ..builder.wheel_tag import WheelTag
 from ..cmake import CMake, CMaker
 from ..resources import resources
 from ..settings.metadata import get_standard_metadata
 from ..settings.skbuild_read_settings import SettingsReader
 from ._init import setup_logging
-from ._pathutil import packages_to_file_mapping, path_to_module, scantree
+from ._pathutil import (
+    is_valid_module,
+    packages_to_file_mapping,
+    path_to_module,
+    scantree,
+)
 from ._scripts import process_script_dir
 from ._wheelfile import WheelWriter
 
 __all__: list[str] = ["_build_wheel_impl"]
 
 
 def __dir__() -> list[str]:
@@ -39,15 +44,15 @@
     name: str,
 ) -> list[str]:
     if packages is not None:
         return list(packages)
 
     # Auto package discovery
     packages = []
-    for base_path in (Path("src"), Path(".")):
+    for base_path in (Path("src"), Path()):
         path = base_path / name
         if path.is_dir() and (
             (path / "__init__.py").is_file() or (path / "__init__.pyi").is_file()
         ):
             logger.info("Discovered Python package at {}", path)
             packages += [str(path)]
             break
@@ -252,14 +257,15 @@
 
             if editable:
                 modules = {
                     path_to_module(Path(v).relative_to(wheel_dirs["platlib"])): str(
                         Path(k).resolve()
                     )
                     for k, v in mapping.items()
+                    if is_valid_module(Path(v).relative_to(wheel_dirs["platlib"]))
                 }
                 installed = {
                     path_to_module(v.relative_to(wheel_dirs["platlib"])): str(
                         v.relative_to(wheel_dirs["platlib"])
                     )
                     for v in scantree(wheel_dirs["platlib"])
                 }
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.8/src/scikit_build_core/builder/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,11 +184,18 @@
 
         self.config.configure(
             defines=cmake_defines,
             cmake_args=[*self.get_cmake_args(), *configure_args],
         )
 
     def build(self, build_args: list[str]) -> None:
-        self.config.build(build_args=build_args, verbose=self.settings.cmake.verbose)
+        self.config.build(
+            build_args=build_args,
+            targets=self.settings.cmake.targets,
+            verbose=self.settings.cmake.verbose,
+        )
 
     def install(self, install_dir: Path) -> None:
-        self.config.install(install_dir)
+        components = self.settings.install.components
+        strip = self.settings.install.strip
+        assert strip is not None
+        self.config.install(install_dir, strip=strip, components=components)
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.8/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.8/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.8/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.8/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.8/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/reply.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dataclasses
 import json
 import sys
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Type, TypeVar, Union  # noqa: TID251
 
 from .._compat.builtins import ExceptionGroup
+from .._compat.typing import get_args, get_origin
 from .model.cache import Cache
 from .model.cmakefiles import CMakeFiles
 from .model.codemodel import CodeModel, Target
 from .model.directory import Directory
 from .model.index import Index
 
 __all__ = ["load_reply_dir"]
@@ -84,19 +85,20 @@
 
         return target(**input_dict)
 
     def _convert_any(self, item: Any, target: Type[T]) -> T:
         if dataclasses.is_dataclass(target):
             # We don't have DataclassInstance exposed in typing yet
             return self.make_class(item, target)  # type: ignore[return-value]
-        if hasattr(target, "__origin__"):
-            if target.__origin__ == list:  # type: ignore[attr-defined]
-                return [self._convert_any(i, target.__args__[0]) for i in item]  # type: ignore[return-value,attr-defined]
-            if target.__origin__ == Union:  # type: ignore[attr-defined]
-                return self._convert_any(item, target.__args__[0])  # type: ignore[no-any-return,attr-defined]
+        origin = get_origin(target)
+        if origin is not None:
+            if origin == list:
+                return [self._convert_any(i, get_args(target)[0]) for i in item]  # type: ignore[return-value]
+            if origin == Union:
+                return self._convert_any(item, get_args(target)[0])  # type: ignore[no-any-return]
 
         return target(item)  # type: ignore[call-arg]
 
 
 def load_reply_dir(path: Path) -> Index:
     return Converter(path).load()
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.8/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.8/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.8/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.8/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.8/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.8/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.8/src/scikit_build_core/settings/skbuild_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 from typing import Any, Dict, List, Optional
 
 __all__ = [
     "BackportSettings",
     "CMakeSettings",
     "EditableSettings",
+    "InstallSettings",
     "LoggingSettings",
     "NinjaSettings",
     "SDistSettings",
     "ScikitBuildSettings",
     "WheelSettings",
 ]
 
@@ -43,18 +44,22 @@
     verbose: bool = False
 
     #: The build type to use when building the project.
     #: Valid options are: "Debug", "Release", "RelWithDebInfo", "MinSizeRel",
     #: "", etc.
     build_type: str = "Release"
 
-    #: The source directory to use when building the project. Currently only affects
-    #: the native builder (not the setuptools plugin).
+    #: The source directory to use when building the project. Currently only
+    #: affects the native builder (not the setuptools plugin).
     source_dir: str = ""
 
+    #: The build targets to use when building the project. Empty builds the
+    #: default target.
+    targets: List[str] = dataclasses.field(default_factory=list)
+
 
 @dataclasses.dataclass
 class LoggingSettings:
     #: The logging level to display.
     level: str = "WARNING"
 
 
@@ -122,23 +127,33 @@
 
     #: Rebuild the project when the package is imported.
     #: The build-directory must be set.
     rebuild: bool = False
 
 
 @dataclasses.dataclass
+class InstallSettings:
+    #: The components to install. If empty, the default is used.
+    components: List[str] = dataclasses.field(default_factory=list)
+
+    #: Whether to strip the binaries. True for scikit-build-core 0.5+.
+    strip: Optional[bool] = None
+
+
+@dataclasses.dataclass
 class ScikitBuildSettings:
     cmake: CMakeSettings = dataclasses.field(default_factory=CMakeSettings)
     ninja: NinjaSettings = dataclasses.field(default_factory=NinjaSettings)
     logging: LoggingSettings = dataclasses.field(default_factory=LoggingSettings)
     sdist: SDistSettings = dataclasses.field(default_factory=SDistSettings)
     wheel: WheelSettings = dataclasses.field(default_factory=WheelSettings)
     backport: BackportSettings = dataclasses.field(default_factory=BackportSettings)
     metadata: Dict[str, Dict[str, Any]] = dataclasses.field(default_factory=dict)
     editable: EditableSettings = dataclasses.field(default_factory=EditableSettings)
+    install: InstallSettings = dataclasses.field(default_factory=InstallSettings)
 
     #: Strictly check all config options. If False, warnings will be
     #: printed for unknown options. If True, an error will be raised.
     strict_config: bool = True
 
     #: Enable early previews of features not finalized yet.
     experimental: bool = False
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.8/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,20 @@
 
         if self.settings.editable.rebuild and not self.settings.build_dir:
             rich_print(
                 "[red][bold]ERROR:[/bold] editable mode with rebuild requires build_dir"
             )
             raise SystemExit(7)
 
+        install_policy = self.settings.minimum_version is None or Version(
+            self.settings.minimum_version
+        ) >= Version("0.5")
+        if self.settings.install.strip is None:
+            self.settings.install.strip = install_policy
+
     def unrecognized_options(self) -> Generator[str, None, None]:
         return self.sources.unrecognized_options(ScikitBuildSettings)
 
     def suggestions(self, index: int) -> dict[str, list[str]]:
         all_options = list(self.sources[index].all_option_names(ScikitBuildSettings))
         result: dict[str, list[str]] = {
             k: [] for k in self.sources[index].unrecognized_options(ScikitBuildSettings)
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.8/src/scikit_build_core/settings/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import dataclasses
 import os
 import typing
 from collections.abc import Generator, Iterator, Mapping, Sequence
 from typing import Any, TypeVar, Union
 
 from .._compat.builtins import ExceptionGroup
-from .._compat.typing import Protocol, runtime_checkable
+from .._compat.typing import Protocol, get_args, get_origin
 
 T = TypeVar("T")
 
 __all__ = ["Source", "SourceChain", "ConfSource", "EnvSource", "TOMLSource"]
 
 
 def __dir__() -> list[str]:
@@ -68,40 +68,28 @@
         if len(types) != 1:
             msg = f"Could not access {'.'.join(names)}"
             raise KeyError(msg)
         (__opt,) = types
     return __opt
 
 
-@runtime_checkable
-class TypeLike(Protocol):
-    @property
-    def __origin__(self) -> Any:
-        ...
-
-    @property
-    def __args__(self) -> list[Any]:
-        ...
-
-
 def _process_union(target: type[Any]) -> Any:
     """
     Selects the non-None item in an Optional or Optional-like Union. Passes
     through non-Unions.
     """
 
-    if (
-        not isinstance(target, TypeLike)
-        or not hasattr(target, "__origin__")
-        or target.__origin__ is not Union
-    ):
+    origin = get_origin(target)
+
+    if origin is None or origin is not Union:
         return target
 
-    if len(target.__args__) == 2:
-        items = list(target.__args__)
+    args = get_args(target)
+    if len(args) == 2:
+        items = list(args)
         if type(None) not in items:
             msg = f"None must be in union, got {items}"
             raise AssertionError(msg)
         items.remove(type(None))
         return items[0]
 
     msg = "Only Unions with None supported"
@@ -111,34 +99,30 @@
 def _get_target_raw_type(target: type[Any]) -> type[Any]:
     """
     Takes a type like ``Optional[str]`` and returns str,
     or ``Optional[Dict[str, int]]`` and returns dict.
     """
 
     target = _process_union(target)
-    # The hasattr is required for Python 3.7, though not quite sure why
-    if isinstance(target, TypeLike) and hasattr(target, "__origin__"):
-        return target.__origin__
-    return target
+    origin = get_origin(target)
+    return origin or target
 
 
 def _get_inner_type(__target: type[Any]) -> type[Any]:
     """
     Takes a types like ``List[str]`` and returns str,
     or ``Dict[str, int]`` and returns int.
     """
 
     raw_target = _get_target_raw_type(__target)
     target = _process_union(__target)
     if raw_target == list:
-        assert isinstance(__target, TypeLike)
-        return target.__args__[0]
+        return get_args(target)[0]  # type: ignore[no-any-return]
     if raw_target == dict:
-        assert isinstance(__target, TypeLike)
-        return target.__args__[1]
+        return get_args(target)[1]  # type: ignore[no-any-return]
     msg = f"Expected a list or dict, got {target!r}"
     raise AssertionError(msg)
 
 
 def _nested_dataclass_to_names(__target: type[Any], *inner: str) -> Iterator[list[str]]:
     """
     Yields each entry, like ``("a", "b", "c")`` for ``a.b.c``.
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.4.8/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,29 +178,30 @@
         or getattr(dist, "cmake_source_dir", None) is not None
     )
 
 
 def _prepare_extension_detection(dist: Distribution) -> None:
     # Setuptools needs to know that it has extensions modules
 
-    dist.has_ext_modules = lambda: type(dist).has_ext_modules(dist) or _has_cmake(dist)  # type: ignore[method-assign]
+    orig_has_ext_modules = dist.has_ext_modules
+    dist.has_ext_modules = lambda: orig_has_ext_modules() or _has_cmake(dist)  # type: ignore[method-assign]
 
     # Hack for stdlib distutils
     if not setuptools.distutils.__package__.startswith("setuptools"):  # type: ignore[attr-defined]
 
         class EvilList(list):  # type: ignore[type-arg]
             def __len__(self) -> int:
                 return super().__len__() or int(_has_cmake(dist))
 
         dist.ext_modules = getattr(dist, "ext_modules", []) or EvilList()
 
 
 def _prepare_build_cmake_command(dist: Distribution) -> None:
     # Prepare new build_cmake command and make sure build calls it
-    build = dist.get_command_obj("build")
+    build = dist.get_command_class("build")
     assert build is not None
     if "build_cmake" not in {x for x, _ in build.sub_commands}:
         build.sub_commands.append(
             ("build_cmake", lambda cmd: _has_cmake(cmd.distribution))  # type: ignore[arg-type]
         )
```

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.8/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.4.8/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/conftest.py` & `scikit_build_core-0.4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_builder.py` & `scikit_build_core-0.4.8/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_cmake_config.py` & `scikit_build_core-0.4.8/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_custom_modules.py` & `scikit_build_core-0.4.8/tests/test_custom_modules.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.8/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_file_processor.py` & `scikit_build_core-0.4.8/tests/test_file_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,13 +41,13 @@
     if (
         sys.platform.startswith("win")
         and not exposed_symlink.joinpath("file2").is_file()
     ):
         pytest.skip("Windows symlink support not available")
 
     # Test that each_unignored_file() follows the symlink
-    assert sorted(each_unignored_file(Path("."))) == [
+    assert sorted(each_unignored_file(Path())) == [
         gitignore,
         exposed_symlink / "file2",
         file1,
         file2,
     ]
```

### Comparing `scikit_build_core-0.4.7/tests/test_fileapi.py` & `scikit_build_core-0.4.8/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_fortran.py` & `scikit_build_core-0.4.8/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_generator_default.py` & `scikit_build_core-0.4.8/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_get_requires.py` & `scikit_build_core-0.4.8/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_logging.py` & `scikit_build_core-0.4.8/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_module_dir.py` & `scikit_build_core-0.4.8/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_name_main.py` & `scikit_build_core-0.4.8/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.8/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_process_scripts.py` & `scikit_build_core-0.4.8/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_program_search.py` & `scikit_build_core-0.4.8/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.8/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.8/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.8/tests/test_pyproject_pep517.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.usefixtures("package_simple_pyproject_ext")
 def test_pep517_wheel(virtualenv):
     dist = Path("dist")
-    out = build_wheel("dist")
+    out = build_wheel("dist", {"cmake.targets": ["cmake_example"]})  # Could leave empty
     (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
     assert wheel == dist / out
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
```

### Comparing `scikit_build_core-0.4.7/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.8/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.8/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_settings.py` & `scikit_build_core-0.4.8/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.8/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.8/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.8/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_shutil.py` & `scikit_build_core-0.4.8/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_simple_pure.py` & `scikit_build_core-0.4.8/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/test_simplest_c.py` & `scikit_build_core-0.4.8/tests/test_simplest_c.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,44 +42,57 @@
                 "PKG-INFO",
             )
         }
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
-def test_pep517_wheel(tmp_path, monkeypatch, virtualenv):
+@pytest.mark.parametrize(
+    "component", [[], ["PythonModule"], ["PythonModule", "Generated"]]
+)
+def test_pep517_wheel(tmp_path, monkeypatch, virtualenv, component):
     dist = tmp_path / "dist"
     dist.mkdir()
     monkeypatch.chdir(SIMPLEST)
     if Path("dist").is_dir():
         shutil.rmtree("dist")
-    out = build_wheel(str(dist))
+    out = build_wheel(str(dist), config_settings={"install.components": component})
     (wheel,) = dist.glob("simplest-0.0.1-*.whl")
     assert wheel == dist / out
 
     virtualenv.install(wheel)
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = {x.name for x in p.iterdir()}
             simplest_pkg = {x.name for x in p.joinpath("simplest").iterdir()}
 
         filtered_pkg = {x for x in simplest_pkg if not x.startswith("_module")}
+        if not component or "PythonModule" in component:
+            assert filtered_pkg != simplest_pkg
+        else:
+            assert filtered_pkg == simplest_pkg
 
-        assert len(filtered_pkg) == len(simplest_pkg) - 2
-        assert {"simplest-0.0.1.dist-info", "simplest"} == file_names
-        assert {
+        expected_wheel_files = {
             "__init__.py",
             "data.txt",
             "excluded.txt",
-            "generated.txt",
             "sdist_only.txt",
-            "generated_ignored.txt",
-        } == filtered_pkg
+        }
+
+        if not component:
+            expected_wheel_files.add("generated_ignored.txt")
+
+        if not component or "Generated" in component:
+            expected_wheel_files.add("generated.txt")
+
+        assert len(filtered_pkg) == len(simplest_pkg) - 2
+        assert {"simplest-0.0.1.dist-info", "simplest"} == file_names
+        assert expected_wheel_files == filtered_pkg
         # Note that generated_ignored.txt is here because all CMake installed files are
         # present, CMake has the final say.
 
     version = virtualenv.execute("from simplest import square; print(square(2))")
     assert version == "4.0"
```

### Comparing `scikit_build_core-0.4.7/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.8/tests/test_skbuild_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     assert settings.ninja.make_fallback
     assert settings.cmake.minimum_version == "3.15"
     assert settings.cmake.args == []
     assert settings.cmake.define == {}
     assert not settings.cmake.verbose
     assert settings.cmake.build_type == "Release"
     assert not settings.cmake.source_dir
+    assert settings.cmake.targets == []
     assert settings.logging.level == "WARNING"
     assert settings.sdist.include == []
     assert settings.sdist.exclude == []
     assert settings.sdist.reproducible
     assert settings.wheel.packages is None
     assert settings.wheel.py_api == ""
     assert not settings.wheel.expand_macos_universal_tags
@@ -48,28 +49,31 @@
     assert not settings.experimental
     assert settings.minimum_version is None
     assert settings.build_dir == ""
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
     assert not settings.editable.rebuild
     assert settings.editable.verbose
+    assert settings.install.components == []
+    assert settings.install.strip
 
 
 def test_skbuild_settings_envvar(tmp_path, monkeypatch):
     monkeypatch.setattr(
         scikit_build_core.settings.skbuild_read_settings, "__version__", "0.1.0"
     )
 
     monkeypatch.setenv("SKBUILD_NINJA_MINIMUM_VERSION", "1.1")
     monkeypatch.setenv("SKBUILD_NINJA_MAKE_FALLBACK", "0")
     monkeypatch.setenv("SKBUILD_CMAKE_MINIMUM_VERSION", "3.16")
     monkeypatch.setenv("SKBUILD_CMAKE_ARGS", "-DFOO=BAR;-DBAR=FOO")
     monkeypatch.setenv("SKBUILD_CMAKE_DEFINE", "a=1;b=2")
     monkeypatch.setenv("SKBUILD_CMAKE_BUILD_TYPE", "Debug")
     monkeypatch.setenv("SKBUILD_CMAKE_SOURCE_DIR", "a/b/c")
+    monkeypatch.setenv("SKBUILD_CMAKE_TARGETS", "a;b;c")
     monkeypatch.setenv("SKBUILD_LOGGING_LEVEL", "DEBUG")
     monkeypatch.setenv("SKBUILD_SDIST_INCLUDE", "a;b; c")
     monkeypatch.setenv("SKBUILD_SDIST_EXCLUDE", "d;e;f")
     monkeypatch.setenv("SKBUILD_SDIST_REPRODUCIBLE", "OFF")
     monkeypatch.setenv("SKBUILD_WHEEL_PACKAGES", "j; k; l")
     monkeypatch.setenv("SKBUILD_WHEEL_PY_API", "cp39")
     monkeypatch.setenv("SKBUILD_WHEEL_EXPAND_MACOS_UNIVERSAL_TAGS", "True")
@@ -78,14 +82,16 @@
     monkeypatch.setenv("SKBUILD_STRICT_CONFIG", "0")
     monkeypatch.setenv("SKBUILD_EXPERIMENTAL", "1")
     monkeypatch.setenv("SKBUILD_MINIMUM_VERSION", "0.1")
     monkeypatch.setenv("SKBUILD_CMAKE_VERBOSE", "TRUE")
     monkeypatch.setenv("SKBUILD_BUILD_DIR", "a/b/c")
     monkeypatch.setenv("SKBUILD_EDITABLE_REBUILD", "True")
     monkeypatch.setenv("SKBUILD_EDITABLE_VERBOSE", "False")
+    monkeypatch.setenv("SKBUILD_INSTALL_COMPONENTS", "a;b;c")
+    monkeypatch.setenv("SKBUILD_INSTALL_STRIP", "False")
 
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text("", encoding="utf-8")
 
     config_settings: dict[str, list[str] | str] = {}
 
     settings_reader = SettingsReader.from_file(pyproject_toml, config_settings)
@@ -95,14 +101,15 @@
     assert settings.ninja.minimum_version == "1.1"
     assert settings.cmake.minimum_version == "3.16"
     assert settings.cmake.args == ["-DFOO=BAR", "-DBAR=FOO"]
     assert settings.cmake.define == {"a": "1", "b": "2"}
     assert settings.cmake.verbose
     assert settings.cmake.build_type == "Debug"
     assert settings.cmake.source_dir == "a/b/c"
+    assert settings.cmake.targets == ["a", "b", "c"]
     assert not settings.ninja.make_fallback
     assert settings.logging.level == "DEBUG"
     assert settings.sdist.include == ["a", "b", "c"]
     assert settings.sdist.exclude == ["d", "e", "f"]
     assert not settings.sdist.reproducible
     assert settings.wheel.packages == ["j", "k", "l"]
     assert settings.wheel.py_api == "cp39"
@@ -113,14 +120,16 @@
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
     assert settings.editable.rebuild
     assert not settings.editable.verbose
+    assert settings.install.components == ["a", "b", "c"]
+    assert not settings.install.strip
 
 
 def test_skbuild_settings_config_settings(tmp_path, monkeypatch):
     monkeypatch.setattr(
         scikit_build_core.settings.skbuild_read_settings, "__version__", "0.1.0"
     )
 
@@ -133,14 +142,15 @@
         "cmake.minimum-version": "3.17",
         "cmake.args": ["-DFOO=BAR", "-DBAR=FOO"],
         "cmake.define.a": "1",
         "cmake.define.b": "2",
         "cmake.verbose": "true",
         "cmake.build-type": "Debug",
         "cmake.source-dir": "a/b/c",
+        "cmake.targets": ["a", "b", "c"],
         "logging.level": "INFO",
         "sdist.include": ["a", "b", "c"],
         "sdist.exclude": "d;e;f",
         "sdist.reproducible": "false",
         "wheel.packages": ["j", "k", "l"],
         "wheel.py-api": "cp39",
         "wheel.expand-macos-universal-tags": "True",
@@ -149,28 +159,31 @@
         "strict-config": "false",
         "experimental": "1",
         "minimum-version": "0.1",
         "build-dir": "a/b/c",
         "editable.mode": "redirect",
         "editable.rebuild": "True",
         "editable.verbose": "False",
+        "install.components": ["a", "b", "c"],
+        "install.strip": "True",
     }
 
     settings_reader = SettingsReader.from_file(pyproject_toml, config_settings)
     settings = settings_reader.settings
     assert list(settings_reader.unrecognized_options()) == []
 
     assert settings.ninja.minimum_version == "1.2"
     assert not settings.ninja.make_fallback
     assert settings.cmake.minimum_version == "3.17"
     assert settings.cmake.args == ["-DFOO=BAR", "-DBAR=FOO"]
     assert settings.cmake.define == {"a": "1", "b": "2"}
     assert settings.cmake.verbose
     assert settings.cmake.build_type == "Debug"
     assert settings.cmake.source_dir == "a/b/c"
+    assert settings.cmake.targets == ["a", "b", "c"]
     assert settings.logging.level == "INFO"
     assert settings.sdist.include == ["a", "b", "c"]
     assert settings.sdist.exclude == ["d", "e", "f"]
     assert not settings.sdist.reproducible
     assert settings.wheel.packages == ["j", "k", "l"]
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
@@ -180,14 +193,16 @@
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
     assert settings.editable.rebuild
     assert not settings.editable.verbose
+    assert settings.install.components == ["a", "b", "c"]
+    assert settings.install.strip
 
 
 def test_skbuild_settings_pyproject_toml(tmp_path, monkeypatch):
     monkeypatch.setattr(
         scikit_build_core.settings.skbuild_read_settings, "__version__", "0.1.0"
     )
     pyproject_toml = tmp_path / "pyproject.toml"
@@ -199,14 +214,15 @@
             ninja.make-fallback = false
             cmake.minimum-version = "3.18"
             cmake.args = ["-DFOO=BAR", "-DBAR=FOO"]
             cmake.define = {a = "1", b = "2"}
             cmake.build-type = "Debug"
             cmake.verbose = true
             cmake.source-dir = "a/b/c"
+            cmake.targets = ["a", "b", "c"]
             logging.level = "ERROR"
             sdist.include = ["a", "b", "c"]
             sdist.exclude = ["d", "e", "f"]
             sdist.reproducible = false
             wheel.packages = ["j", "k", "l"]
             wheel.py-api = "cp39"
             wheel.expand-macos-universal-tags = true
@@ -216,14 +232,16 @@
             experimental = true
             minimum-version = "0.1"
             build-dir = "a/b/c"
             metadata.version.provider = "a"
             editable.mode = "redirect"
             editable.rebuild = true
             editable.verbose = false
+            install.components = ["a", "b", "c"]
+            install.strip = true
             """
         ),
         encoding="utf-8",
     )
 
     config_settings: dict[str, list[str] | str] = {}
 
@@ -235,14 +253,15 @@
     assert not settings.ninja.make_fallback
     assert settings.cmake.minimum_version == "3.18"
     assert settings.cmake.args == ["-DFOO=BAR", "-DBAR=FOO"]
     assert settings.cmake.define == {"a": "1", "b": "2"}
     assert settings.cmake.verbose
     assert settings.cmake.build_type == "Debug"
     assert settings.cmake.source_dir == "a/b/c"
+    assert settings.cmake.targets == ["a", "b", "c"]
     assert settings.logging.level == "ERROR"
     assert settings.sdist.include == ["a", "b", "c"]
     assert settings.sdist.exclude == ["d", "e", "f"]
     assert not settings.sdist.reproducible
     assert settings.wheel.packages == ["j", "k", "l"]
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
@@ -252,14 +271,16 @@
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {"version": {"provider": "a"}}
     assert settings.editable.mode == "redirect"
     assert settings.editable.rebuild
     assert not settings.editable.verbose
+    assert settings.install.components == ["a", "b", "c"]
+    assert settings.install.strip
 
 
 def test_skbuild_settings_pyproject_toml_broken(tmp_path, capsys):
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(
         textwrap.dedent(
             """\
@@ -323,7 +344,28 @@
         ex.split()
         == """\
       ERROR: Unrecognized options in config-settings:
         cmake.minimum-verison -> Did you mean: cmake.minimum-version, minimum-version, ninja.minimum-version?
         logger -> Did you mean: logging?
       """.split()
     )
+
+
+def test_skbuild_settings_min_version_defaults(tmp_path, monkeypatch):
+    monkeypatch.setattr(
+        scikit_build_core.settings.skbuild_read_settings, "__version__", "0.5.0"
+    )
+
+    pyproject_toml = tmp_path / "pyproject.toml"
+    pyproject_toml.write_text("", encoding="utf-8")
+
+    settings_reader = SettingsReader.from_file(
+        pyproject_toml, {"minimum-version": "0.4"}
+    )
+    settings = settings_reader.settings
+    assert not settings.install.strip
+
+    settings_reader = SettingsReader.from_file(
+        pyproject_toml, {"minimum-version": "0.5"}
+    )
+    settings = settings_reader.settings
+    assert settings.install.strip
```

### Comparing `scikit_build_core-0.4.7/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.8/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.8/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.8/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.8/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.8/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.8/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.8/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.8/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.4.8/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.4.8/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.8/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.4.8/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.4.8/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.8/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.8/tests/packages/simplest_c/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,22 @@
   LANGUAGES C
   VERSION ${SKBUILD_PROJECT_VERSION})
 
 find_package(Python COMPONENTS Interpreter Development.Module)
 
 python_add_library(_module MODULE src/module.c WITH_SOABI)
 
-install(TARGETS _module DESTINATION ${SKBUILD_PROJECT_NAME})
+install(
+  TARGETS _module
+  DESTINATION ${SKBUILD_PROJECT_NAME}
+  COMPONENT PythonModule)
 
 # Testing artifacts
 file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/generated.txt "Testing")
-install(FILES ${CMAKE_CURRENT_BINARY_DIR}/generated.txt
-        DESTINATION ${SKBUILD_PROJECT_NAME})
+install(
+  FILES ${CMAKE_CURRENT_BINARY_DIR}/generated.txt
+  DESTINATION ${SKBUILD_PROJECT_NAME}
+  COMPONENT Generated)
 
 file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/generated_ignored.txt "Testing")
 install(FILES ${CMAKE_CURRENT_BINARY_DIR}/generated_ignored.txt
         DESTINATION ${SKBUILD_PROJECT_NAME})
```

### Comparing `scikit_build_core-0.4.7/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.8/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/.gitignore` & `scikit_build_core-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/LICENSE` & `scikit_build_core-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.7/README.md` & `scikit_build_core-0.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,19 +105,19 @@
 (so you will usually prefix everything by the package name).
 
 More examples are in the
 [tests/packages](https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages).
 
 ## Configuration
 
-All configuration options can be placed in `pyproject.toml`, passed via `-C` or
-`--config-setting` in build or `--config-settings` in `pip` (warning: pip
-doesn't support list options), or set as environment variables.
-`tool.scikit-build` is used in toml, `skbuild.` for `-C` options, or `SKBUILD_*`
-for environment variables. The defaults are listed below:
+All configuration options can be placed in `pyproject.toml`, passed via
+`-C`/`--config-setting` in build or `-C`/`--config-settings` in `pip` , or set
+as environment variables. `tool.scikit-build` is used in toml, `skbuild.` for
+`-C` options, or `SKBUILD_*` for environment variables. The defaults are listed
+below:
 
 ```toml
 [tool.scikit-build]
 # The PEP 517 build hooks will add ninja and/or cmake if the versions on the
 # system are not at least these versions. Disabled by an empty string.
 cmake.minimum-version = "3.15"
 ninja.minimum-version = "1.5"
@@ -133,14 +133,17 @@
 
 # This activates verbose builds
 cmake.verbose = false
 
 # This controls the CMake build type
 cmake.build-type = "Release"
 
+# The targets to build - empty builds all default targets.
+cmake.targets = []
+
 # Display logs at or above this level.
 logging.level = "WARNING"
 
 # Include and exclude patterns, in gitignore syntax. Include overrides exclude.
 # Wheels include packages included in the sdist; CMake has the final say.
 sdist.include = []
 sdist.exclude = []
@@ -167,14 +170,20 @@
 # original dir is still at SKBUILD_PLATLIB_DIR (also SKBUILD_DATA_DIR, etc. are
 # available)
 wheel.install-dir = "."
 
 # The licence file(s) to include in the wheel metadata directory.
 wheel.license-files = ["LICEN[CS]E*", "COPYING*", "NOTICE*", "AUTHORS*"]
 
+# Strip the binaries. Defaults to True for scikit-build-core 0.5+.
+install.strip = true
+
+# Components to install. Leave empty to install all components.
+install.components = []
+
 # This will backport an internal copy of FindPython if CMake is less than this
 # value. Set to 0 or the empty string to disable. The default will be kept in
 # sync with the version of FindPython stored in scikit-build-core.
 backport.find-python = "3.26.1"
 
 # This is the only editable mode currently
 editable.mode = "redirect"
```

### Comparing `scikit_build_core-0.4.7/pyproject.toml` & `scikit_build_core-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,14 @@
 extend-ignore = [
     "PLR",     # Design rules for pylint
     "PLE1205", # Format check doesn't work with our custom logger
     "E501",    # Line too long
     "PT004",   # Incorrect, just usefixtures instead.
     "RUF009",  # Too easy to get a false positive
 ]
-target-version = "py37"
 typing-modules = ["scikit_build_core._compat.typing"]
 src = ["src"]
 unfixable = ["T20", "F841"]
 exclude = []
 
 [tool.ruff.flake8-tidy-imports.banned-api]
 "typing.Callable".msg = "Use collections.abc.Callable instead."
@@ -231,15 +230,15 @@
 "typing.Mapping".msg = "Use collections.abc.Mapping instead."
 "typing.Sequence".msg = "Use collections.abc.Sequence instead."
 "typing.Set".msg = "Use collections.abc.Set instead."
 "typing.Literal".msg = "Use scikit_build_core._compat.typing.Literal instead."
 "typing.Protocol".msg = "Use scikit_build_core._compat.typing.Protocol instead."
 "typing.Self".msg = "Use scikit_build_core._compat.typing.Self instead."
 "typing_extensions.Self".msg = "Use scikit_build_core._compat.typing.Self instead."
-"typing.runtime_checkable".msg = "Use scikit_build_core._compat.typing.runtime_checkable instead."
+"typing.runtime_checkable".msg = "Add and use scikit_build_core._compat.typing.runtime_checkable instead."
 "typing.Final".msg = "Add scikit_build_core._compat.typing.Final instead."
 "typing.NotRequired".msg = "Add scikit_build_core._compat.typing.NotRequired instead."
 "typing.OrderedDict".msg = "Add scikit_build_core._compat.typing.OrderedDict instead."
 "typing.TypedDict".msg = "Add scikit_build_core._compat.typing.TypedDict instead."
 "typing.assert_never".msg = "Add scikit_build_core._compat.typing.assert_never instead."
 "tomli".msg = "Use scikit_build_core._compat.tomllib instead."
 "tomllib".msg = "Use scikit_build_core._compat.tomllib instead."
```

### Comparing `scikit_build_core-0.4.7/PKG-INFO` & `scikit_build_core-0.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.4.7
+Version: 0.4.8
 Summary: Build backend for CMake based projects
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -178,19 +178,19 @@
 (so you will usually prefix everything by the package name).
 
 More examples are in the
 [tests/packages](https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages).
 
 ## Configuration
 
-All configuration options can be placed in `pyproject.toml`, passed via `-C` or
-`--config-setting` in build or `--config-settings` in `pip` (warning: pip
-doesn't support list options), or set as environment variables.
-`tool.scikit-build` is used in toml, `skbuild.` for `-C` options, or `SKBUILD_*`
-for environment variables. The defaults are listed below:
+All configuration options can be placed in `pyproject.toml`, passed via
+`-C`/`--config-setting` in build or `-C`/`--config-settings` in `pip` , or set
+as environment variables. `tool.scikit-build` is used in toml, `skbuild.` for
+`-C` options, or `SKBUILD_*` for environment variables. The defaults are listed
+below:
 
 ```toml
 [tool.scikit-build]
 # The PEP 517 build hooks will add ninja and/or cmake if the versions on the
 # system are not at least these versions. Disabled by an empty string.
 cmake.minimum-version = "3.15"
 ninja.minimum-version = "1.5"
@@ -206,14 +206,17 @@
 
 # This activates verbose builds
 cmake.verbose = false
 
 # This controls the CMake build type
 cmake.build-type = "Release"
 
+# The targets to build - empty builds all default targets.
+cmake.targets = []
+
 # Display logs at or above this level.
 logging.level = "WARNING"
 
 # Include and exclude patterns, in gitignore syntax. Include overrides exclude.
 # Wheels include packages included in the sdist; CMake has the final say.
 sdist.include = []
 sdist.exclude = []
@@ -240,14 +243,20 @@
 # original dir is still at SKBUILD_PLATLIB_DIR (also SKBUILD_DATA_DIR, etc. are
 # available)
 wheel.install-dir = "."
 
 # The licence file(s) to include in the wheel metadata directory.
 wheel.license-files = ["LICEN[CS]E*", "COPYING*", "NOTICE*", "AUTHORS*"]
 
+# Strip the binaries. Defaults to True for scikit-build-core 0.5+.
+install.strip = true
+
+# Components to install. Leave empty to install all components.
+install.components = []
+
 # This will backport an internal copy of FindPython if CMake is less than this
 # value. Set to 0 or the empty string to disable. The default will be kept in
 # sync with the version of FindPython stored in scikit-build-core.
 backport.find-python = "3.26.1"
 
 # This is the only editable mode currently
 editable.mode = "redirect"
```

