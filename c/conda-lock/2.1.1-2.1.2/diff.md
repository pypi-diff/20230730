# Comparing `tmp/conda_lock-2.1.1.tar.gz` & `tmp/conda_lock-2.1.2.tar.gz`

## Comparing `conda_lock-2.1.1.tar` & `conda_lock-2.1.2.tar`

### file list

```diff
@@ -1,557 +1,559 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.flake8
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.gitattributes
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 conda_lock-2.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 conda_lock-2.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.1/Dockerfile
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 conda_lock-2.1.1/DockerfileTest
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 conda_lock-2.1.1/codecov.yml
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 conda_lock-2.1.1/mkdocs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 conda_lock-2.1.1/mypy.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 conda_lock-2.1.1/pyrightconfig.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 conda_lock-2.1.1/renovate.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 conda_lock-2.1.1/requirements-dev.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/update-lockfile.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/__main__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/click_helpers.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/common.py
--rw-r--r--   0        0        0    50388 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/conda_lock.py
--rw-r--r--   0        0        0    20109 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/conda_solver.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/errors.py
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/invoke_conda.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lookup.py
--rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/pypi_solver.py
--rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/virtual_package.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/LICENSES.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo.LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo.pyi
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda.pyi
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry-core.LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry.LICENSE
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry.pyi
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/vendor.txt
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo/LICENSE
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo/io/io_mixin.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/.version
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE.txt
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/__main__.py
--rw-r--r--   0        0        0    47200 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/activate.py
--rw-r--r--   0        0        0    17270 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/api.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/appdirs.LICENSE.txt
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/distro.LICENSE.txt
--rw-r--r--   0        0        0    53998 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/exceptions.py
--rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/exports.py
--rw-r--r--   0        0        0    15475 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/history.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/instructions.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/lock.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/misc.py
--rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/plan.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/py-cpuinfo.LICENSE
--rw-r--r--   0        0        0    66502 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/resolve.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/six.LICENSE
--rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/utils.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/__init__.py
--rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/appdirs.py
--rw-r--r--   0        0        0    39759 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/distro.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/six.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/__init__.py
--rw-r--r--   0        0        0    33620 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/setutils.py
--rw-r--r--   0        0        0    20478 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/cpuinfo/__init__.py
--rw-r--r--   0        0        0    83718 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py
--rw-r--r--   0        0        0    25343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/recipes.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/utils.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/__main__.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_main.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_tqdm.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/auto.py
--rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/cli.py
--rw-r--r--   0        0        0    57572 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/std.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/utils.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/version.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/LICENSE
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/collection.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/compat.py
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/decorators.py
--rw-r--r--   0        0        0    33324 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/entity.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/exceptions.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/ish.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/logz.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/packaging.py
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/type_coercion.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/__init__.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/constants.py
--rw-r--r--   0        0        0    75564 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/context.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/exceptions.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/__init__.py
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/common.py
--rw-r--r--   0        0        0    59153 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/conda_argparse.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/find_commands.py
--rw-r--r--   0        0        0    16609 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/install.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main.py
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_clean.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_compare.py
--rw-r--r--   0        0        0    16627 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_config.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_create.py
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_info.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_init.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_install.py
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_notices.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_package.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_pip.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_remove.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_rename.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_run.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_search.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_update.py
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/python_api.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/__init__.py
--rw-r--r--   0        0        0    26678 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_logic.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/compat.py
--rw-r--r--   0        0        0    58130 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/configuration.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/constants.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/cuda.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/decorators.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/disk.py
--rw-r--r--   0        0        0    21968 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/io.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/logic.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/path.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/serialize.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/signals.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/toposort.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/url.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/__init__.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/linux.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/unix.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/windows.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/pkg_formats/__init__.py
--rw-r--r--   0        0        0    45704 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/pkg_formats/python.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/__init__.py
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/envs_manager.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/index.py
--rw-r--r--   0        0        0    61517 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/initialize.py
--rw-r--r--   0        0        0    58045 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/link.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/package_cache.py
--rw-r--r--   0        0        0    32215 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/package_cache_data.py
--rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/path_actions.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/portability.py
--rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/prefix_data.py
--rw-r--r--   0        0        0    71861 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/solve.py
--rw-r--r--   0        0        0    30211 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/subdir_data.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/__init__.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/anaconda_client.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/logging.py
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/subprocess.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/__init__.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/download.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/session.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/__init__.py
--rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/__init__.py
--rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/create.py
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/delete.py
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/link.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/permissions.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/read.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/test.py
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/update.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/__init__.py
--rw-r--r--   0        0        0    18571 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/channel.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/dist.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/enums.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/leased_path_entry.py
--rw-r--r--   0        0        0    35276 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/match_spec.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/package_info.py
--rw-r--r--   0        0        0    16650 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/prefix_graph.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/records.py
--rw-r--r--   0        0        0    24971 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/version.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/__init__.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/cache.py
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/core.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/http.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/types.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/views.py
--rw-r--r--   0        0        0    40960 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-32.exe
--rw-r--r--   0        0        0    41984 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-64.exe
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda.xsh
--rw-r--r--   0        0        0   126355 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda_icon.ico
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/Library/bin/conda.bat
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/Scripts/activate.bat
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/bin/activate
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/bin/conda
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/bin/deactivate
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/Conda.psm1
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/activate.bat
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda-hook.ps1
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda.bat
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/deactivate.bat
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/rename_tmp.bat
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/cases.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/decorators.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/fixtures.py
--rw-r--r--   0        0        0    29666 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/helpers.py
--rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/integration.py
--rw-r--r--   0        0        0    46730 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/solver_helpers.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/gateways/__init__.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/gateways/fixtures.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/__init__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/fixtures.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/helpers.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/trust/__init__.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/trust/constants.py
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/trust/signature_verification.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/LICENSE
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/__version__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/exceptions.py
--rwxr-xr-x   0        0        0     5366 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/factory.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/locations.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/poetry.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/_vendor/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/__init__.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/config.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/config_source.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/dict_config_source.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/file_config_source.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/__init__.py
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/factory.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/poetry.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/_pyrsistent_version.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE
--rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/vendor.txt
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py
--rw-r--r--   0        0        0    88313 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/py.typed
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__main__.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py
--rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py
--rw-r--r--   0        0        0    29400 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__init__.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/common.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py
--rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py
--rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py
--rw-r--r--   0        0        0    35346 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py
--rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py
--rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/__init__.py
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py
--rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/__init__.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py
--rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py
--rw-r--r--   0        0        0    14643 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py
--rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/py.typed
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py
--rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py
--rw-r--r--   0        0        0    33853 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py
--rw-r--r--   0        0        0    42075 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_document.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/exceptions/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/exceptions/base.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/__init__.py
--rw-r--r--   0        0        0    20976 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/api.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builder.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/metadata.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/__init__.py
--rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/builder.py
--rw-r--r--   0        0        0    14530 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py
--rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/include.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/module.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/__init__.py
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/dependency.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/directory_dependency.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/file_dependency.py
--rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/package.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/project_package.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/specification.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/url_dependency.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/__init__.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/link.py
--rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/utils.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/exceptions.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/tables.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/toml.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/__init__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/empty_constraint.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/exceptions.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/patterns.py
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_constraint.py
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_range.py
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_union.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/__init__.py
--rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/license.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/updater.py
--rw-r--r--   0        0        0    30162 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/data/licenses.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/exceptions.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/_compat.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/helpers.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/patterns.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/toml_file.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/__init__.py
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/git.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/base.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/exceptions.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/helpers.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/legacy_version.py
--rw-r--r--   0        0        0    22972 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/markers.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/requirements.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/utils.py
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/__init__.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/markers.lark
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/inspection/__init__.py
--rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/inspection/info.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/__init__.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/authenticator.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/base_installer.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chef.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chooser.py
--rw-r--r--   0        0        0    24842 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/executor.py
--rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/installer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/noop_installer.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/pip_installer.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/install.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/operation.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/uninstall.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/update.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/io/__init__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/io/null_io.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/json/__init__.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/__init__.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/layout.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/src.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/standard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/api.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/builders/__init__.py
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/builders/editable.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/__init__.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/assignment.py
--rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/failure.py
--rw-r--r--   0        0        0    16149 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py
--rwxr-xr-x   0        0        0     7506 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/partial_solution.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/result.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/set_relation.py
--rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/term.py
--rwxr-xr-x   0        0        0    18984 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/version_solver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/__init__.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/dependency_package.py
--rw-r--r--   0        0        0    22709 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/locker.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/package_collection.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/exceptions.py
--rwxr-xr-x   0        0        0    29291 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/provider.py
--rw-r--r--   0        0        0    16301 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/solver.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/__init__.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/base_repository.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/exceptions.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/installed_repository.py
--rwxr-xr-x   0        0        0    12943 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/legacy_repository.py
--rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pool.py
--rwxr-xr-x   0        0        0    16575 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pypi_repository.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/remote_repository.py
--rwxr-xr-x   0        0        0     3408 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/_compat.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/appdirs.py
--rw-r--r--   0        0        0    54820 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/env.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/exporter.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/extras.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/helpers.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/password_manager.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/patterns.py
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/setup_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/version/__init__.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/version/version_selector.py
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lockfile/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lockfile/v1/models.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lockfile/v2prelim/models.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/models/__init__.py
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/models/channel.py
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/models/lock_spec.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/README.md
--rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/migration.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/requirements.txt
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/vendor_helpers.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry.patch
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/aggregation.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/conda_common.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/environment_yaml.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/meta_yaml.py
--rw-r--r--   0        0        0    20022 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/pyproject_toml.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/selectors.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/authenticated_channels.md
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/docker.md
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/flags.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/getting_started.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/index.md
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/output.md
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/pip.md
--rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/scipy-2023.md
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/src_environment_yml.md
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/src_meta_yaml.md
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/src_pyproject.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/cli/gen.md
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/flags/strip-auth.md
--rw-r--r--   0        0        0   305465 2020-02-02 00:00:00.000000 conda_lock-2.1.1/environments/conda-lock.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 conda_lock-2.1.1/environments/dev-environment.yaml
--rw-r--r--   0        0        0   324897 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/pangeo/conda-lock.yml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/pangeo/environment.yml
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/zlib/conda-lock.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/zlib/environment.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.gitignore
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 conda_lock-2.1.1/LICENSE
--rw-r--r--   0        0        0    15293 2020-02-02 00:00:00.000000 conda_lock-2.1.1/README.md
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 conda_lock-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    17290 2020-02-02 00:00:00.000000 conda_lock-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.flake8
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.gitattributes
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 conda_lock-2.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 conda_lock-2.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.2/Dockerfile
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 conda_lock-2.1.2/DockerfileTest
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 conda_lock-2.1.2/codecov.yml
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 conda_lock-2.1.2/mkdocs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 conda_lock-2.1.2/mypy.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 conda_lock-2.1.2/pyrightconfig.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 conda_lock-2.1.2/renovate.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 conda_lock-2.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.github/workflows/update-lockfile.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/__main__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/click_helpers.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/common.py
+-rw-r--r--   0        0        0    50716 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/conda_lock.py
+-rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/conda_solver.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/errors.py
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/invoke_conda.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/lookup.py
+-rw-r--r--   0        0        0    13495 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/pypi_solver.py
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/virtual_package.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/LICENSES.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/cleo.LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/cleo.pyi
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda.pyi
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry-core.LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry.LICENSE
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry.pyi
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/vendor.txt
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/cleo/LICENSE
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/cleo/io/io_mixin.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/.version
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/LICENSE
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/LICENSE.txt
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/__main__.py
+-rw-r--r--   0        0        0    47200 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/activate.py
+-rw-r--r--   0        0        0    17270 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/api.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/appdirs.LICENSE.txt
+-rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/distro.LICENSE.txt
+-rw-r--r--   0        0        0    53998 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/exceptions.py
+-rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/exports.py
+-rw-r--r--   0        0        0    15475 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/history.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/instructions.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/lock.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/misc.py
+-rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/plan.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/py-cpuinfo.LICENSE
+-rw-r--r--   0        0        0    66502 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/resolve.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/six.LICENSE
+-rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/utils.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/__init__.py
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/appdirs.py
+-rw-r--r--   0        0        0    39759 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/distro.py
+-rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/six.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/__init__.py
+-rw-r--r--   0        0        0    33620 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/setutils.py
+-rw-r--r--   0        0        0    20478 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/cpuinfo/__init__.py
+-rw-r--r--   0        0        0    83718 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py
+-rw-r--r--   0        0        0    25343 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/recipes.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/utils.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/__main__.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/_main.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/_tqdm.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/auto.py
+-rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/cli.py
+-rw-r--r--   0        0        0    57572 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/std.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/utils.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/version.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/LICENSE
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/collection.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/compat.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/decorators.py
+-rw-r--r--   0        0        0    33324 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/entity.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/exceptions.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/ish.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/logz.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/packaging.py
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/type_coercion.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/base/__init__.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/base/constants.py
+-rw-r--r--   0        0        0    75564 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/base/context.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/base/exceptions.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/__init__.py
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/common.py
+-rw-r--r--   0        0        0    59153 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/conda_argparse.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/find_commands.py
+-rw-r--r--   0        0        0    16609 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/install.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main.py
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_clean.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_compare.py
+-rw-r--r--   0        0        0    16627 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_config.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_create.py
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_info.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_init.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_install.py
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_notices.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_package.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_pip.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_remove.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_rename.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_run.py
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_search.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_update.py
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/cli/python_api.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/__init__.py
+-rw-r--r--   0        0        0    26678 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/_logic.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/compat.py
+-rw-r--r--   0        0        0    58130 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/configuration.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/constants.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/cuda.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/decorators.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/disk.py
+-rw-r--r--   0        0        0    21968 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/io.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/logic.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/path.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/serialize.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/signals.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/toposort.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/url.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/__init__.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/linux.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/unix.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/windows.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/pkg_formats/__init__.py
+-rw-r--r--   0        0        0    45704 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/common/pkg_formats/python.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/__init__.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/envs_manager.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/index.py
+-rw-r--r--   0        0        0    61517 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/initialize.py
+-rw-r--r--   0        0        0    58045 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/link.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/package_cache.py
+-rw-r--r--   0        0        0    32215 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/package_cache_data.py
+-rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/path_actions.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/portability.py
+-rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/prefix_data.py
+-rw-r--r--   0        0        0    71861 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/solve.py
+-rw-r--r--   0        0        0    30211 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/core/subdir_data.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/__init__.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/anaconda_client.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/logging.py
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/subprocess.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/__init__.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/download.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/session.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/__init__.py
+-rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/__init__.py
+-rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/create.py
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/delete.py
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/link.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/permissions.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/read.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/test.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/update.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/__init__.py
+-rw-r--r--   0        0        0    18571 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/channel.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/dist.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/enums.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/leased_path_entry.py
+-rw-r--r--   0        0        0    35276 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/match_spec.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/package_info.py
+-rw-r--r--   0        0        0    16650 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/prefix_graph.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/records.py
+-rw-r--r--   0        0        0    24971 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/models/version.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/notices/__init__.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/notices/cache.py
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/notices/core.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/notices/http.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/notices/types.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/notices/views.py
+-rw-r--r--   0        0        0    40960 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/cli-32.exe
+-rw-r--r--   0        0        0    41984 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/cli-64.exe
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/conda.xsh
+-rw-r--r--   0        0        0   126355 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/conda_icon.ico
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/Library/bin/conda.bat
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/Scripts/activate.bat
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/bin/activate
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/bin/conda
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/bin/deactivate
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/Conda.psm1
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/activate.bat
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda-hook.ps1
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda.bat
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/deactivate.bat
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/rename_tmp.bat
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/cases.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/decorators.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/fixtures.py
+-rw-r--r--   0        0        0    29666 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/helpers.py
+-rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/integration.py
+-rw-r--r--   0        0        0    46730 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/solver_helpers.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/gateways/__init__.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/gateways/fixtures.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/notices/__init__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/notices/fixtures.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/testing/notices/helpers.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/trust/__init__.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/trust/constants.py
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/conda/trust/signature_verification.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/LICENSE
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/__version__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/exceptions.py
+-rwxr-xr-x   0        0        0     5366 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/factory.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/locations.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/poetry.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/_vendor/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/config/__init__.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/config/config.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/config/config_source.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/config/dict_config_source.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/config/file_config_source.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/__init__.py
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/factory.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/poetry.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/_pyrsistent_version.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE
+-rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/vendor.txt
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py
+-rw-r--r--   0        0        0    88313 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/py.typed
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__main__.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py
+-rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py
+-rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py
+-rw-r--r--   0        0        0    29400 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/__init__.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/common.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py
+-rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py
+-rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py
+-rw-r--r--   0        0        0    35346 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py
+-rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/__init__.py
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py
+-rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/__init__.py
+-rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py
+-rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py
+-rw-r--r--   0        0        0    14643 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py
+-rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/py.typed
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py
+-rw-r--r--   0        0        0    33853 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py
+-rw-r--r--   0        0        0    42075 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_document.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/exceptions/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/exceptions/base.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/json/__init__.py
+-rw-r--r--   0        0        0    20976 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/api.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builder.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/metadata.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/__init__.py
+-rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/builder.py
+-rw-r--r--   0        0        0    14530 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py
+-rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/include.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/module.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/__init__.py
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/dependency.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/directory_dependency.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/file_dependency.py
+-rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/package.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/project_package.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/specification.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/url_dependency.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/utils/__init__.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/utils/link.py
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/utils/utils.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/pyproject/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/pyproject/exceptions.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/pyproject/tables.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/pyproject/toml.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/__init__.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/empty_constraint.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/exceptions.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/patterns.py
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version_constraint.py
+-rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version_range.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version_union.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/__init__.py
+-rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/license.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/updater.py
+-rw-r--r--   0        0        0    30162 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/data/licenses.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/toml/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/toml/exceptions.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/toml/file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/_compat.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/helpers.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/patterns.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/toml_file.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/vcs/__init__.py
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/vcs/git.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/base.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/exceptions.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/helpers.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/legacy_version.py
+-rw-r--r--   0        0        0    22972 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/markers.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/requirements.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/utils.py
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/grammars/__init__.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/grammars/markers.lark
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/inspection/__init__.py
+-rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/inspection/info.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/__init__.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/authenticator.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/base_installer.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/chef.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/chooser.py
+-rw-r--r--   0        0        0    24842 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/executor.py
+-rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/installer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/noop_installer.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/pip_installer.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/install.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/operation.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/uninstall.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/update.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/io/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/io/null_io.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/json/__init__.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/layouts/__init__.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/layouts/layout.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/layouts/src.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/layouts/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/masonry/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/masonry/api.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/masonry/builders/__init__.py
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/masonry/builders/editable.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/__init__.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/assignment.py
+-rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/failure.py
+-rw-r--r--   0        0        0    16149 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/incompatibility.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py
+-rwxr-xr-x   0        0        0     7506 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/partial_solution.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/result.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/set_relation.py
+-rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/term.py
+-rwxr-xr-x   0        0        0    18984 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/version_solver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/__init__.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/dependency_package.py
+-rw-r--r--   0        0        0    22709 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/locker.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/package_collection.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/puzzle/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/puzzle/exceptions.py
+-rwxr-xr-x   0        0        0    29291 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/puzzle/provider.py
+-rw-r--r--   0        0        0    16301 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/puzzle/solver.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/__init__.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/base_repository.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/exceptions.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/installed_repository.py
+-rwxr-xr-x   0        0        0    12943 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/legacy_repository.py
+-rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/pool.py
+-rwxr-xr-x   0        0        0    16575 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/pypi_repository.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/remote_repository.py
+-rwxr-xr-x   0        0        0     3408 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/_compat.py
+-rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/appdirs.py
+-rw-r--r--   0        0        0    54820 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/env.py
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/exporter.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/extras.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/helpers.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/password_manager.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/patterns.py
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/setup_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/version/__init__.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/_vendor/poetry/version/version_selector.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/interfaces/vendored_conda.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/interfaces/vendored_poetry.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/lockfile/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/lockfile/v1/models.py
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/lockfile/v2prelim/models.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/models/__init__.py
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/models/channel.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/models/lock_spec.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/README.md
+-rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/migration.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/requirements.txt
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/vendor_helpers.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/patches/poetry.patch
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/aggregation.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/conda_common.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/environment_yaml.py
+-rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/meta_yaml.py
+-rw-r--r--   0        0        0    20236 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/pyproject_toml.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 conda_lock-2.1.2/conda_lock/src_parser/selectors.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/authenticated_channels.md
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/docker.md
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/flags.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/getting_started.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/index.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/output.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/pip.md
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/scipy-2023.md
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/src_environment_yml.md
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/src_meta_yaml.md
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/src_pyproject.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/cli/gen.md
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.2/docs/flags/strip-auth.md
+-rw-r--r--   0        0        0   309705 2020-02-02 00:00:00.000000 conda_lock-2.1.2/environments/conda-lock.yml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 conda_lock-2.1.2/environments/dev-environment.yaml
+-rw-r--r--   0        0        0   324897 2020-02-02 00:00:00.000000 conda_lock-2.1.2/example/pangeo/conda-lock.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 conda_lock-2.1.2/example/pangeo/environment.yml
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 conda_lock-2.1.2/example/zlib/conda-lock.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 conda_lock-2.1.2/example/zlib/environment.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 conda_lock-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 conda_lock-2.1.2/LICENSE
+-rw-r--r--   0        0        0    15293 2020-02-02 00:00:00.000000 conda_lock-2.1.2/README.md
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 conda_lock-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    17258 2020-02-02 00:00:00.000000 conda_lock-2.1.2/PKG-INFO
```

### Comparing `conda_lock-2.1.1/.pre-commit-config.yaml` & `conda_lock-2.1.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   rev: v4.4.0
   hooks:
     - id: trailing-whitespace
       exclude: "^.*\\.patch$"
     - id: check-ast
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/pycqa/flake8
   rev: 6.0.0
   hooks:
```

### Comparing `conda_lock-2.1.1/CODE_OF_CONDUCT.md` & `conda_lock-2.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/CONTRIBUTING.md` & `conda_lock-2.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/mkdocs.yml` & `conda_lock-2.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/mypy.ini` & `conda_lock-2.1.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/.github/workflows/mkdocs.yml` & `conda_lock-2.1.2/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/.github/workflows/release.yaml` & `conda_lock-2.1.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/.github/workflows/test.yml` & `conda_lock-2.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/.github/workflows/update-lockfile.yaml` & `conda_lock-2.1.2/.github/workflows/update-lockfile.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 name: Run conda-lock to update dependencies
 
 on:
   push:
+    branches:
+    - main
   workflow_dispatch:
   schedule:
   # At 5:28am UTC Monday and Thursday
   - cron: 28 5 * * MON,THU
 
 jobs:
   conda-lock:
@@ -45,11 +47,12 @@
         # # This PAT should have read-write permissions for "Pull Requests"
         # # and read-write permissions for "Contents".
         # token: ${{ secrets.GH_PAT_FOR_PR }}
         commit-message: Relock dependencies
         title: Relock dependencies
         body: >
           This pull request relocks the dependencies with conda-lock.
+          It is triggered by [update-lockfile](https://github.com/conda/conda-lock/blob/main/.github/workflows/update-lockfile.yaml).
         branch: relock-deps
         labels: conda-lock
         reviewers: maresb
         delete-branch: true
```

### Comparing `conda_lock-2.1.1/conda_lock/click_helpers.py` & `conda_lock-2.1.2/conda_lock/click_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/common.py` & `conda_lock-2.1.2/conda_lock/common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/conda_lock.py` & `conda_lock-2.1.2/conda_lock/conda_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import posixpath
 import re
 import sys
 import tempfile
 
 from contextlib import contextmanager
 from functools import partial
+from importlib.metadata import distribution
 from types import TracebackType
 from typing import (
     AbstractSet,
     Any,
     Dict,
     Iterator,
     List,
@@ -28,15 +29,14 @@
     Tuple,
     Type,
     Union,
 )
 from urllib.parse import urlsplit
 
 import click
-import pkg_resources
 import yaml
 
 from ensureconda.api import ensureconda
 from typing_extensions import Literal
 
 from conda_lock.click_helpers import OrderedGroup
 from conda_lock.common import (
@@ -255,14 +255,15 @@
     filename_template: Optional[str] = None,
     filter_categories: bool = False,
     extras: Optional[AbstractSet[str]] = None,
     check_input_hash: bool = False,
     metadata_choices: AbstractSet[MetadataOption] = frozenset(),
     metadata_yamls: Sequence[pathlib.Path] = (),
     with_cuda: Optional[str] = None,
+    strip_auth: bool = False,
 ) -> None:
     """
     Generate a lock file from the src files provided
 
     Parameters
     ----------
     conda :
@@ -381,14 +382,15 @@
                 conda=conda,
                 spec=lock_spec,
                 platforms=platforms_to_lock,
                 lockfile_path=lockfile_path,
                 update_spec=update_spec,
                 metadata_choices=metadata_choices,
                 metadata_yamls=metadata_yamls,
+                strip_auth=strip_auth,
             )
 
             if "lock" in kinds:
                 write_conda_lock_file(
                     lock_content,
                     lockfile_path,
                     metadata_choices=metadata_choices,
@@ -478,15 +480,15 @@
     for plat in platforms:
         for kind in kinds:
             if filename_template:
                 context = {
                     "platform": plat,
                     "dev-dependencies": str(include_dev_dependencies).lower(),
                     "input-hash": lockfile.metadata.content_hash,
-                    "version": pkg_resources.get_distribution("conda_lock").version,
+                    "version": distribution("conda_lock").version,
                     "timestamp": datetime.datetime.utcnow().strftime("%Y%m%dT%H%M%SZ"),
                 }
 
                 filename = filename_template.format(**context)
             else:
                 filename = f"conda-{plat}.lock"
 
@@ -681,14 +683,15 @@
 
 def _solve_for_arch(
     conda: PathLike,
     spec: LockSpecification,
     platform: str,
     channels: List[Channel],
     update_spec: Optional[UpdateSpecification] = None,
+    strip_auth: bool = False,
 ) -> List[LockedDependency]:
     """
     Solve specification for a single platform
     """
     if update_spec is None:
         update_spec = UpdateSpecification()
 
@@ -721,14 +724,15 @@
             pip_locked={
                 dep.name: dep for dep in update_spec.locked if dep.manager == "pip"
             },
             conda_locked={dep.name: dep for dep in conda_deps.values()},
             python_version=conda_deps["python"].version,
             platform=platform,
             allow_pypi_requests=spec.allow_pypi_requests,
+            strip_auth=strip_auth,
         )
     else:
         pip_deps = {}
 
     return list(conda_deps.values()) + list(pip_deps.values())
 
 
@@ -765,14 +769,15 @@
     conda: PathLike,
     spec: LockSpecification,
     platforms: List[str] = [],
     lockfile_path: pathlib.Path,
     update_spec: Optional[UpdateSpecification] = None,
     metadata_choices: AbstractSet[MetadataOption] = frozenset(),
     metadata_yamls: Sequence[pathlib.Path] = (),
+    strip_auth: bool = False,
 ) -> Lockfile:
     """
     Solve or update specification
     """
     assert spec.virtual_package_repo is not None
     virtual_package_channel = spec.virtual_package_repo.channel
 
@@ -781,14 +786,15 @@
     for platform in platforms or spec.platforms:
         deps = _solve_for_arch(
             conda=conda,
             spec=spec,
             platform=platform,
             channels=[*spec.channels, virtual_package_channel],
             update_spec=update_spec,
+            strip_auth=strip_auth,
         )
 
         for dep in deps:
             locked[(dep.manager, dep.name, dep.platform)] = dep
 
     meta_sources: Dict[str, pathlib.Path] = {}
     for source in spec.sources:
@@ -992,14 +998,15 @@
     extras: Optional[AbstractSet[str]] = None,
     virtual_package_spec: Optional[pathlib.Path] = None,
     with_cuda: Optional[str] = None,
     update: Optional[List[str]] = None,
     filter_categories: bool = False,
     metadata_choices: AbstractSet[MetadataOption] = frozenset(),
     metadata_yamls: Sequence[pathlib.Path] = (),
+    strip_auth: bool = False,
 ) -> None:
     if environment_files == DEFAULT_FILES:
         if lockfile_path.exists():
             lock_content = parse_conda_lock_file(lockfile_path)
             # reconstruct native paths
             locked_environment_files = [
                 pathlib.Path(p)
@@ -1043,14 +1050,15 @@
         filename_template=filename_template,
         include_dev_dependencies=include_dev_dependencies,
         extras=extras,
         check_input_hash=check_input_hash,
         filter_categories=filter_categories,
         metadata_choices=metadata_choices,
         metadata_yamls=metadata_yamls,
+        strip_auth=strip_auth,
     )
 
 
 @click.group(cls=OrderedGroup, default="lock", default_if_no_args=True)
 @click.version_option()
 def main() -> None:
     """To get help for subcommands, use the conda-lock <SUBCOMMAND> --help"""
@@ -1305,24 +1313,25 @@
         extras=extras_,
         virtual_package_spec=virtual_package_spec,
         with_cuda=with_cuda,
         update=update,
         filter_categories=filter_categories,
         metadata_choices=metadata_enum_choices,
         metadata_yamls=metadata_yamls,
+        strip_auth=strip_auth,
     )
     if strip_auth:
         with tempfile.TemporaryDirectory() as tempdir:
             filename_template_temp = f"{tempdir}/{filename_template.split('/')[-1]}"
             lock_func(filename_template=filename_template_temp)
             filename_template_dir = "/".join(filename_template.split("/")[:-1])
             for file in os.listdir(tempdir):
-                lockfile = read_file(os.path.join(tempdir, file))
-                lockfile = _strip_auth_from_lockfile(lockfile)
-                write_file(lockfile, os.path.join(filename_template_dir, file))
+                lockfile_content = read_file(os.path.join(tempdir, file))
+                lockfile_content = _strip_auth_from_lockfile(lockfile_content)
+                write_file(lockfile_content, os.path.join(filename_template_dir, file))
     else:
         lock_func(
             filename_template=filename_template, check_input_hash=check_input_hash
         )
 
 
 @main.command("install")
```

### Comparing `conda_lock-2.1.1/conda_lock/conda_solver.py` & `conda_lock-2.1.2/conda_lock/conda_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Dict, Iterable, Iterator, List, MutableSequence, Optional, Sequence
 from urllib.parse import urlsplit, urlunsplit
 
 import yaml
 
 from typing_extensions import TypedDict
 
-from conda_lock._vendor.conda.models.match_spec import MatchSpec
+from conda_lock.interfaces.vendored_conda import MatchSpec
 from conda_lock.invoke_conda import (
     PathLike,
     _get_conda_flags,
     conda_env_override,
     conda_pkgs_dir,
     is_micromamba,
 )
@@ -573,14 +573,15 @@
                 "channel": channel,
                 "url": dep.url,
                 "md5": dep.hash.md5,
                 "build": build,
                 "build_number": build_number,
                 "version": dep.version,
                 "subdir": path.parent.name,
+                "fn": path.name,
                 "depends": [f"{k} {v}".strip() for k, v in dep.dependencies.items()],
             }
             # mamba requires these to be stringlike so null are not allowed here
             if dep.hash.sha256 is not None:
                 entry["sha256"] = dep.hash.sha256
 
             with open(conda_meta / (path.name + ".json"), "w") as f:
```

### Comparing `conda_lock-2.1.1/conda_lock/invoke_conda.py` & `conda_lock-2.1.2/conda_lock/invoke_conda.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/lookup.py` & `conda_lock-2.1.2/conda_lock/lookup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from functools import cached_property
 from typing import Dict
 
 import requests
 import yaml
 
+from packaging.utils import NormalizedName, canonicalize_name
 from typing_extensions import TypedDict
 
 
 class MappingEntry(TypedDict):
     conda_name: str
     # legacy field, generally not used by anything anymore
     conda_forge: str
-    pypi_name: str
+    pypi_name: NormalizedName
 
 
 class _LookupLoader:
     _mapping_url: str = "https://raw.githubusercontent.com/regro/cf-graph-countyfair/master/mappings/pypi/grayskull_pypi_mapping.yaml"
 
     @property
     def mapping_url(self) -> str:
@@ -24,34 +25,34 @@
     @mapping_url.setter
     def mapping_url(self, value: str) -> None:
         del self.pypi_lookup
         del self.conda_lookup
         self._mapping_url = value
 
     @cached_property
-    def pypi_lookup(self) -> Dict[str, MappingEntry]:
+    def pypi_lookup(self) -> Dict[NormalizedName, MappingEntry]:
         res = requests.get(self._mapping_url)
         res.raise_for_status()
         lookup = yaml.safe_load(res.content)
         # lowercase and kebabcase the pypi names
         assert lookup is not None
-        lookup = {k.lower().replace("_", "-"): v for k, v in lookup.items()}
+        lookup = {canonicalize_name(k): v for k, v in lookup.items()}
         for v in lookup.values():
-            v["pypi_name"] = v["pypi_name"].lower().replace("_", "-")
+            v["pypi_name"] = canonicalize_name(v["pypi_name"])
         return lookup
 
     @cached_property
     def conda_lookup(self) -> Dict[str, MappingEntry]:
         return {record["conda_name"]: record for record in self.pypi_lookup.values()}
 
 
 LOOKUP_OBJECT = _LookupLoader()
 
 
-def get_forward_lookup() -> Dict[str, MappingEntry]:
+def get_forward_lookup() -> Dict[NormalizedName, MappingEntry]:
     global LOOKUP_OBJECT
     return LOOKUP_OBJECT.pypi_lookup
 
 
 def get_lookup() -> Dict[str, MappingEntry]:
     """
     Reverse grayskull name mapping to map conda names onto PyPI
@@ -61,16 +62,18 @@
 
 
 def set_lookup_location(lookup_url: str) -> None:
     global LOOKUP_OBJECT
     LOOKUP_OBJECT.mapping_url = lookup_url
 
 
-def conda_name_to_pypi_name(name: str) -> str:
+def conda_name_to_pypi_name(name: str) -> NormalizedName:
     """return the pypi name for a conda package"""
     lookup = get_lookup()
-    return lookup.get(name, {"pypi_name": name})["pypi_name"]
+    cname = canonicalize_name(name)
+    return lookup.get(cname, {"pypi_name": cname})["pypi_name"]
 
 
 def pypi_name_to_conda_name(name: str) -> str:
     """return the conda name for a pypi package"""
-    return get_forward_lookup().get(name, {"conda_name": name})["conda_name"]
+    cname = canonicalize_name(name)
+    return get_forward_lookup().get(cname, {"conda_name": cname})["conda_name"]
```

### Comparing `conda_lock-2.1.1/conda_lock/pypi_solver.py` & `conda_lock-2.1.2/conda_lock/pypi_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import re
 import sys
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional
-from urllib.parse import urldefrag
+from urllib.parse import urldefrag, urlsplit, urlunsplit
 
 from clikit.api.io.flags import VERY_VERBOSE
 from clikit.io import ConsoleIO, NullIO
 from packaging.tags import compatible_tags, cpython_tags, mac_platforms
 
-from conda_lock._vendor.poetry.core.packages import Dependency as PoetryDependency
-from conda_lock._vendor.poetry.core.packages import Package as PoetryPackage
-from conda_lock._vendor.poetry.core.packages import (
-    ProjectPackage as PoetryProjectPackage,
+from conda_lock.interfaces.vendored_poetry import (
+    Chooser,
+    Env,
+    Factory,
+    PoetryDependency,
+    PoetryPackage,
+    PoetryProjectPackage,
+    PoetrySolver,
+    PoetryURLDependency,
+    PoetryVCSDependency,
+    Pool,
+    PyPiRepository,
+    Repository,
+    Uninstall,
 )
-from conda_lock._vendor.poetry.core.packages import URLDependency as PoetryURLDependency
-from conda_lock._vendor.poetry.core.packages import VCSDependency as PoetryVCSDependency
-from conda_lock._vendor.poetry.factory import Factory
-from conda_lock._vendor.poetry.installation.chooser import Chooser
-from conda_lock._vendor.poetry.installation.operations.uninstall import Uninstall
-from conda_lock._vendor.poetry.puzzle import Solver as PoetrySolver
-from conda_lock._vendor.poetry.repositories.pool import Pool
-from conda_lock._vendor.poetry.repositories.pypi_repository import PyPiRepository
-from conda_lock._vendor.poetry.repositories.repository import Repository
-from conda_lock._vendor.poetry.utils.env import Env
 from conda_lock.lockfile import apply_categories
 from conda_lock.lockfile.v2prelim.models import (
     DependencySource,
     HashModel,
     LockedDependency,
 )
 from conda_lock.lookup import conda_name_to_pypi_name
@@ -184,14 +184,15 @@
 
 
 def get_requirements(
     result: List,
     platform: str,
     pool: Pool,
     env: Env,
+    strip_auth: bool = False,
 ) -> List[LockedDependency]:
     """Extract distributions from Poetry package plan, ignoring uninstalls
     (usually: conda package with no pypi equivalent) and skipped ops
     (already installed)
     """
     chooser = Chooser(pool, env=env)
     requirements: List[LockedDependency] = []
@@ -226,15 +227,15 @@
                     version=str(op.package.version),
                     manager="pip",
                     source=source,
                     platform=platform,
                     dependencies={
                         dep.name: str(dep.constraint) for dep in op.package.requires
                     },
-                    url=url,
+                    url=url if not strip_auth else _strip_auth(url),
                     hash=hash,
                 )
             )
     return requirements
 
 
 def solve_pypi(
@@ -242,14 +243,15 @@
     use_latest: List[str],
     pip_locked: Dict[str, LockedDependency],
     conda_locked: Dict[str, LockedDependency],
     python_version: str,
     platform: str,
     allow_pypi_requests: bool = True,
     verbose: bool = False,
+    strip_auth: bool = False,
 ) -> Dict[str, LockedDependency]:
     """
     Solve pip dependencies for the given platform
 
     Parameters
     ----------
     conda :
@@ -266,14 +268,16 @@
         Version of Python in conda_locked
     platform :
         Target platform
     allow_pypi_requests :
         Add pypi.org to the list of repositories (pip packages only)
     verbose :
         Print chatter from solver
+    strip_auth :
+        Whether to strip HTTP Basic auth from URLs.
 
     """
     dummy_package = PoetryProjectPackage("_dummy_package_", "0.0.0")
     dependencies: List[PoetryDependency] = [
         get_dependency(spec) for spec in pip_specs.values()
     ]
     for dep in dependencies:
@@ -326,15 +330,15 @@
         {spec.name for spec in pip_locked.values()}.intersection(use_latest)
     )
     env = PlatformEnv(python_version, platform)
     # find platform-specific solution (e.g. dependencies conditioned on markers)
     with s.use_environment(env):
         result = s.solve(use_latest=to_update)
 
-    requirements = get_requirements(result, platform, pool, env)
+    requirements = get_requirements(result, platform, pool, env, strip_auth=strip_auth)
 
     # use PyPI names of conda packages to walking the dependency tree and propagate
     # categories from explicit to transitive dependencies
     planned = {
         **{dep.name: [dep] for dep in requirements},
     }
 
@@ -342,15 +346,15 @@
     # may have multiple conda packages that map to it. One example is the `dask`
     # pip package; on the Conda side, there are two packages `dask` and `dask-core`
     # that map to it.
     # We use the pip names for the packages for everything so that planned
     # is essentially a dictionary of:
     #  - pip package name -> list of LockedDependency that are needed for this package
     for conda_name, locked_dep in conda_locked.items():
-        pypi_name = conda_name_to_pypi_name(conda_name).lower()
+        pypi_name = conda_name_to_pypi_name(conda_name)
         if pypi_name in planned:
             planned[pypi_name].append(locked_dep)
         else:
             planned[pypi_name] = [locked_dep]
 
     apply_categories(requested=pip_specs, planned=planned, convert_to_pip_names=True)
 
@@ -373,7 +377,16 @@
             {"name": source[0], "url": source[1]["url"]}, config
         )
         for source in config.get("repositories", {}).items()
     ]
     if allow_pypi_requests:
         repos.append(PyPiRepository())
     return Pool(repositories=[*repos])
+
+
+def _strip_auth(url: str) -> str:
+    """Strip HTTP Basic authentication from a URL."""
+    parts = urlsplit(url, allow_fragments=True)
+    # Remove everything before and including the last '@' character in the part
+    # between 'scheme://' and the subsequent '/'.
+    netloc = parts.netloc.split("@")[-1]
+    return urlunsplit((parts.scheme, netloc, parts.path, parts.query, parts.fragment))
```

### Comparing `conda_lock-2.1.1/conda_lock/virtual_package.py` & `conda_lock-2.1.2/conda_lock/virtual_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from collections import defaultdict
 from types import TracebackType
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Type
 
 from pydantic import BaseModel, Field, validator
 
-from conda_lock._vendor.conda.models.match_spec import MatchSpec
+from conda_lock.interfaces.vendored_conda import MatchSpec
 from conda_lock.models.channel import Channel
 
 
 logger = logging.getLogger(__name__)
 
 # datetime.datetime(2020, 1, 1).timestamp()
 DEFAULT_TIME = 1577854800000
```

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/LICENSES.md` & `conda_lock-2.1.2/conda_lock/_vendor/LICENSES.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/cleo.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/cleo.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry-core.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry-core.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/cleo/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/cleo/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/cleo/io/io_mixin.py` & `conda_lock-2.1.2/conda_lock/_vendor/cleo/io/io_mixin.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/conda/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE.txt` & `conda_lock-2.1.2/conda_lock/_vendor/conda/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/activate.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/activate.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/api.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/appdirs.LICENSE.txt` & `conda_lock-2.1.2/conda_lock/_vendor/conda/appdirs.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/distro.LICENSE.txt` & `conda_lock-2.1.2/conda_lock/_vendor/conda/distro.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/exceptions.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/exports.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/exports.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/history.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/history.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/instructions.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/instructions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/lock.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/lock.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/misc.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/misc.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/plan.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/plan.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/py-cpuinfo.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/conda/py-cpuinfo.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/resolve.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/resolve.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/six.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/conda/six.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/appdirs.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/distro.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/six.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/setutils.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/setutils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/recipes.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/cli.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/cli.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/std.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/_vendor/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/collection.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/collection.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/decorators.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/decorators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/entity.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/entity.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/exceptions.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/ish.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/ish.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/logz.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/logz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/packaging.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/packaging.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/type_coercion.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/auxlib/type_coercion.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/base/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/base/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/base/constants.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/base/constants.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/base/context.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/base/context.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/common.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/conda_argparse.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/conda_argparse.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/find_commands.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/find_commands.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/install.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/install.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_clean.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_clean.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_compare.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_compare.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_config.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_config.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_create.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_create.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_info.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_init.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_init.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_install.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_install.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_list.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_list.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_package.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_pip.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_pip.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_remove.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_remove.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_rename.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_rename.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_run.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_search.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_search.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_update.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/main_update.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/python_api.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/cli/python_api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_logic.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/_logic.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/configuration.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/configuration.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/constants.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/constants.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/cuda.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/cuda.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/decorators.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/decorators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/disk.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/disk.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/io.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/io.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/logic.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/logic.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/path.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/path.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/serialize.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/serialize.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/signals.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/signals.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/toposort.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/toposort.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/url.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/url.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/linux.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/linux.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/windows.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/_os/windows.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/common/pkg_formats/python.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/common/pkg_formats/python.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/envs_manager.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/envs_manager.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/index.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/index.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/initialize.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/initialize.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/link.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/link.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/package_cache_data.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/package_cache_data.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/path_actions.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/path_actions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/portability.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/portability.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/prefix_data.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/prefix_data.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/solve.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/solve.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/core/subdir_data.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/core/subdir_data.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/anaconda_client.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/anaconda_client.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/logging.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/logging.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/subprocess.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/subprocess.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/download.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/download.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/session.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/session.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/create.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/create.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/delete.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/delete.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/link.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/link.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/permissions.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/permissions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/read.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/read.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/test.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/test.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/update.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/gateways/disk/update.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/channel.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/channel.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/dist.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/dist.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/enums.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/enums.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/leased_path_entry.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/leased_path_entry.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/match_spec.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/match_spec.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/package_info.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/package_info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/prefix_graph.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/prefix_graph.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/records.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/records.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/models/version.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/models/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/cache.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/notices/cache.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/core.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/notices/core.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/http.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/notices/http.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/types.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/notices/types.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/views.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/notices/views.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-32.exe` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/cli-32.exe`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-64.exe` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/cli-64.exe`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda.xsh` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/conda.xsh`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda_icon.ico` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/conda_icon.ico`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/Scripts/activate.bat` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/Conda.psm1` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/Conda.psm1`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda.bat` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh` & `conda_lock-2.1.2/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/decorators.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/fixtures.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/integration.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/integration.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/solver_helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/solver_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/gateways/fixtures.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/gateways/fixtures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/fixtures.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/notices/fixtures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/testing/notices/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/trust/constants.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/trust/constants.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/conda/trust/signature_verification.py` & `conda_lock-2.1.2/conda_lock/_vendor/conda/trust/signature_verification.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/factory.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/factory.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/locations.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/locations.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/poetry.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/poetry.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/config/config.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/config/config.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/config/dict_config_source.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/config/dict_config_source.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/config/file_config_source.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/config/file_config_source.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/factory.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/factory.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/poetry.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/poetry.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/vendor.txt` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/vendor.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/common.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/json/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/api.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builder.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builder.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/metadata.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/metadata.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/builder.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/builder.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/include.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/include.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/module.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/module.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/dependency.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/directory_dependency.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/directory_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/file_dependency.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/file_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/package.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/project_package.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/project_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/specification.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/specification.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/url_dependency.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/url_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/link.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/utils/link.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/packages/utils/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/tables.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/pyproject/tables.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/toml.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/pyproject/toml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/empty_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/patterns.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/patterns.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_constraint.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_range.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version_range.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_union.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/semver/version_union.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/license.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/license.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/updater.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/updater.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/data/licenses.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/spdx/data/licenses.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/file.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/toml/file.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/_compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/toml_file.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/utils/toml_file.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/git.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/vcs/git.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/base.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/base.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/legacy_version.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/legacy_version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/markers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/markers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/requirements.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/requirements.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/utils.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/version.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/markers.lark` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/grammars/markers.lark`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/inspection/info.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/inspection/info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/authenticator.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/authenticator.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chef.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/chef.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chooser.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/chooser.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/executor.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/executor.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/installer.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/installer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/noop_installer.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/noop_installer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/pip_installer.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/pip_installer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/install.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/install.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/operation.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/operation.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/uninstall.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/uninstall.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/update.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/installation/operations/update.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/json/__init__.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/json/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/layout.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/api.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/masonry/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/builders/editable.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/masonry/builders/editable.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/assignment.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/failure.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/partial_solution.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/term.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/term.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/version_solver.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/dependency_package.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/dependency_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/locker.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/locker.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/package_collection.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/packages/package_collection.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/provider.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/puzzle/provider.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/solver.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/puzzle/solver.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/installed_repository.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/installed_repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/legacy_repository.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/legacy_repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pool.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/pool.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pypi_repository.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/pypi_repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/repository.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/_compat.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/appdirs.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/env.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/env.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/exporter.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/exporter.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/extras.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/extras.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/helpers.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/password_manager.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/password_manager.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/setup_reader.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/utils/setup_reader.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/_vendor/poetry/version/version_selector.py` & `conda_lock-2.1.2/conda_lock/_vendor/poetry/version/version_selector.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/lockfile/__init__.py` & `conda_lock-2.1.2/conda_lock/lockfile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             if dep_name(item.manager, item.name) not in deps
         ]
 
     def dep_name(manager: str, dep: str) -> str:
         # If we operate on lists of pip names and this is a conda dependency, we
         # convert the name to a pip name.
         if convert_to_pip_names and manager == "conda":
-            return conda_name_to_pypi_name(dep).lower()
+            return conda_name_to_pypi_name(dep)
         return dep
 
     for name, request in requested.items():
         todo: List[str] = list()
         deps: Set[str] = set()
         item = name
```

### Comparing `conda_lock-2.1.1/conda_lock/lockfile/v1/models.py` & `conda_lock-2.1.2/conda_lock/lockfile/v1/models.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/lockfile/v2prelim/models.py` & `conda_lock-2.1.2/conda_lock/lockfile/v2prelim/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         package: List[LockedDependency], update: bool = False
     ) -> List[LockedDependency]:
         platforms = {d.platform for d in package}
 
         # Resort the conda packages topologically
         final_package: List[LockedDependency] = []
         for platform in sorted(platforms):
-            from conda_lock._vendor.conda.common.toposort import toposort
+            from conda_lock.interfaces.vendored_conda import toposort
 
             # Add the remaining non-conda packages in the order in which they appeared.
             # Order the pip packages topologically ordered (might be not 100% perfect if they depend on
             # other conda packages, but good enough
             for manager in ["conda", "pip"]:
                 lookup = defaultdict(set)
                 packages: Dict[str, LockedDependency] = {}
```

### Comparing `conda_lock-2.1.1/conda_lock/models/channel.py` & `conda_lock-2.1.2/conda_lock/models/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import re
 import typing
 
 from posixpath import expandvars
 from typing import FrozenSet, List, Optional, cast
 from urllib.parse import unquote, urlparse, urlunparse
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 
 if typing.TYPE_CHECKING:
     from pydantic.typing import ReprArgs
 
 
 logger = logging.getLogger(__name__)
@@ -86,23 +86,22 @@
     """Repr helper that hides falsely values"""
 
     def __repr_args__(self: BaseModel) -> "ReprArgs":
         return [(key, value) for key, value in self.__dict__.items() if value]
 
 
 class Channel(ZeroValRepr, BaseModel):
+    model_config = ConfigDict(frozen=True)  # type: ignore
+
     url: str
     used_env_vars: FrozenSet[str] = Field(default=frozenset())
 
     def __lt__(self, other: "Channel") -> bool:
         return tuple(self.dict().values()) < tuple(other.dict().values())
 
-    class Config:
-        frozen = True
-
     @classmethod
     def from_string(cls, value: str) -> "Channel":
         if "://" in value:
             # url like string
             return cls.from_conda_url(CondaUrl.from_string(value))
         else:
             # this is a simple url
```

### Comparing `conda_lock-2.1.1/conda_lock/models/lock_spec.py` & `conda_lock-2.1.2/conda_lock/models/lock_spec.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/migration.py` & `conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/migration.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/vendor_helpers.py` & `conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/vendor_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch` & `conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry.patch` & `conda_lock-2.1.2/conda_lock/scripts/vendor_poetry/patches/poetry.patch`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/__init__.py` & `conda_lock-2.1.2/conda_lock/src_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/aggregation.py` & `conda_lock-2.1.2/conda_lock/src_parser/aggregation.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/conda_common.py` & `conda_lock-2.1.2/conda_lock/src_parser/conda_common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/environment_yaml.py` & `conda_lock-2.1.2/conda_lock/src_parser/environment_yaml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/meta_yaml.py` & `conda_lock-2.1.2/conda_lock/src_parser/meta_yaml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/pyproject_toml.py` & `conda_lock-2.1.2/conda_lock/src_parser/pyproject_toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 
 if sys.version_info >= (3, 11):
     from tomllib import load as toml_load
 else:
     from tomli import load as toml_load
 
-from pkg_resources import Requirement
+from packaging.requirements import Requirement
+from packaging.utils import canonicalize_name as canonicalize_pypi_name
 from typing_extensions import Literal
 
 from conda_lock.common import get_in
 from conda_lock.lookup import get_forward_lookup as get_lookup
 from conda_lock.models.lock_spec import (
     Dependency,
     LockSpecification,
@@ -69,25 +70,27 @@
 
 
 def join_version_components(pieces: Sequence[Union[str, int]]) -> str:
     return ".".join(str(p) for p in pieces)
 
 
 def normalize_pypi_name(name: str) -> str:
-    name = name.replace("_", "-").lower()
-    if name in get_lookup():
-        lookup = get_lookup()[name]
+    cname = canonicalize_pypi_name(name)
+    if cname in get_lookup():
+        lookup = get_lookup()[cname]
         res = lookup.get("conda_name") or lookup.get("conda_forge")
         if res is not None:
             return res
         else:
-            logging.warning(f"Could not find conda name for {name}. Assuming identity.")
-            return name
+            logging.warning(
+                f"Could not find conda name for {cname}. Assuming identity."
+            )
+            return cname
     else:
-        return name
+        return cname
 
 
 def poetry_version_to_conda_version(version_string: Optional[str]) -> Optional[str]:
     if version_string is None:
         return None
     components = [c.replace(" ", "").strip() for c in version_string.split(",")]
     output_components = []
@@ -364,27 +367,28 @@
     return spec
 
 
 def parse_requirement_specifier(
     requirement: str,
 ) -> Requirement:
     """Parse a url requirement to a conda spec"""
-    requirement_specifier = requirement.split(";")[0].strip()
-
     if (
-        requirement_specifier.startswith("git+")
-        or requirement_specifier.startswith("https://")
-        or requirement_specifier.startswith("ssh://")
+        requirement.startswith("git+")
+        or requirement.startswith("https://")
+        or requirement.startswith("ssh://")
     ):
-        parsed_req = Requirement.parse(
-            requirement_specifier.split("/")[-1].replace("@", "==")
-        )
-        parsed_req.url = requirement_specifier
-        return parsed_req
-    return Requirement.parse(requirement_specifier)
+        # Handle the case where only the URL is specified without a package name
+        repo_name_and_maybe_tag = requirement.split("/")[-1]
+        repo_name = repo_name_and_maybe_tag.split("@")[0]
+        if repo_name.endswith(".git"):
+            repo_name = repo_name[:-4]
+        # Use the repo name as a placeholder for the package name
+        return Requirement(f"{repo_name} @ {requirement}")
+    else:
+        return Requirement(requirement)
 
 
 def unpack_git_url(url: str) -> Tuple[str, Optional[str]]:
     if url.endswith(".git"):
         url = url[:-4]
     if url.startswith("git+"):
         url = url[4:]
@@ -403,16 +407,16 @@
     requirement: str,
     manager: Literal["conda", "pip"] = "conda",
     category: str = "main",
     normalize_name: bool = True,
 ) -> Dependency:
     """Parse a requirements.txt like requirement to a conda spec"""
     parsed_req = parse_requirement_specifier(requirement)
-    name = parsed_req.unsafe_name.lower()
-    collapsed_version = ",".join("".join(spec) for spec in parsed_req.specs)
+    name = canonicalize_pypi_name(parsed_req.name)
+    collapsed_version = str(parsed_req.specifier)
     conda_version = poetry_version_to_conda_version(collapsed_version)
     if conda_version:
         conda_version = ",".join(sorted(conda_version.split(",")))
 
     if normalize_name:
         conda_dep_name = normalize_pypi_name(name)
     else:
```

### Comparing `conda_lock-2.1.1/conda_lock/src_parser/selectors.py` & `conda_lock-2.1.2/conda_lock/src_parser/selectors.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/authenticated_channels.md` & `conda_lock-2.1.2/docs/authenticated_channels.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/docker.md` & `conda_lock-2.1.2/docs/docker.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/flags.md` & `conda_lock-2.1.2/docs/flags.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/index.md` & `conda_lock-2.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/output.md` & `conda_lock-2.1.2/docs/output.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/pip.md` & `conda_lock-2.1.2/docs/pip.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/scipy-2023.md` & `conda_lock-2.1.2/docs/scipy-2023.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/src_environment_yml.md` & `conda_lock-2.1.2/docs/src_environment_yml.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/src_meta_yaml.md` & `conda_lock-2.1.2/docs/src_meta_yaml.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/src_pyproject.md` & `conda_lock-2.1.2/docs/src_pyproject.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/docs/flags/strip-auth.md` & `conda_lock-2.1.2/docs/flags/strip-auth.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/environments/conda-lock.yml` & `conda_lock-2.1.2/environments/conda-lock.yml`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # To update a single package to the latest version compatible with the version constraints in the source:
 #     conda-lock lock  --lockfile conda-lock.yml --update PACKAGE
 # To re-solve the entire environment, e.g. after changing a version constraint in the source file:
 #     conda-lock -f dev-environment.yaml -f ../pyproject.toml --lockfile conda-lock.yml
 version: 1
 metadata:
   content_hash:
-    linux-64: b6e455b8b0e03f338acef5a91853bdf4b53521fb69f388755b38f39d2d7e4898
-    osx-64: ac01a58e8589deb7c1dc47c4c8d7e65f7e11dd71f005fc369c031debb972eb22
-    osx-arm64: 211518777b5ac7d4cd01085197c568f0d1b03f6d0fd02d0fc2bd65fb443fcd80
-    win-64: b86d024b78d0f2adc187cc955262791f3235d3e803da03719114396961c75236
-    linux-aarch64: 543992163b3f2120bbdf616115d1869f55235af636cc16df2acaa8f30c68d7ad
+    linux-64: 004d5fe1e2914905f8968024db52b93a2eaac88ccefd31f56fa9822e6489eb46
+    osx-64: 1e54101be819c268095e8d9cc55be440b7b18815fbd856c518e67172ece321b3
+    osx-arm64: 17950d7ede473d00c724747ba649f8e6731ddd7327819481d847e6129c4cb5dd
+    win-64: b3a3fd1ef25295ab6728c64a21ed13862db56d5fbf55dda340a02d9ecab46bdb
+    linux-aarch64: 5ad5f97e0be6b3d16bf561ebdde3d52300b205244642436ae1d0bdd85d6d3caa
   channels:
   - url: conda-forge
     used_env_vars: []
   platforms:
   - linux-64
   - osx-64
   - osx-arm64
@@ -235,18 +235,18 @@
   optional: false
 - name: libzlib
   version: 1.2.13
   manager: conda
   platform: linux-64
   dependencies:
     libgcc-ng: '>=12'
-  url: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
   hash:
-    md5: f3f9de449d32ca9b9c66a22863c96f41
-    sha256: 22f3663bcf294d349327e60e464a51cd59664a71b8ed70c28a9f512d10bc77dd
+    md5: f36c115f1ee199da648e0597ec2047ad
+    sha256: 370c7c5893b737596fd6ca0d9190c9715d89d888b8c88537ae1ef168c25e82e4
   category: main
   optional: false
 - name: ncurses
   version: '6.4'
   manager: conda
   platform: linux-64
   dependencies:
@@ -357,56 +357,56 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2
   hash:
     md5: 5b8c42eb62e9fc961af70bdd6a26e168
     sha256: 032fd769aad9d4cad40ba261ab222675acb7ec951a8832455fce18ef33fa8df0
   category: main
   optional: false
 - name: libglib
-  version: 2.76.3
+  version: 2.76.4
   manager: conda
   platform: linux-64
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     libffi: '>=3.4,<4.0a0'
     libgcc-ng: '>=12'
     libiconv: '>=1.17,<2.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     pcre2: '>=10.40,<10.41.0a0'
-  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.4-hebfc3b9_0.conda
   hash:
-    md5: a64f11b244b2c112cd3fa1cbe9493999
-    sha256: 6a34c6b123f06fcee7e28e981ec0daad09bce35616ad8e9e61ef84be7fad4d92
+    md5: c6f951789c888f7bbd2dd6858eab69de
+    sha256: e909b5e648d1ace172aac2ddf9d755f72429b134155a9b07156acb58a77ceee1
   category: main
   optional: false
 - name: python
-  version: 3.11.3
+  version: 3.11.4
   manager: conda
   platform: linux-64
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     ld_impl_linux-64: '>=2.36.1'
     libexpat: '>=2.5.0,<3.0a0'
     libffi: '>=3.4,<4.0a0'
     libgcc-ng: '>=12'
     libnsl: '>=2.0.0,<2.1.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libuuid: '>=2.38.1,<3.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    ncurses: '>=6.4,<7.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     readline: '>=8.2,<9.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     xz: '>=5.2.6,<6.0a0'
     pip: ''
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda
   hash:
-    md5: 37005ea5f68df6a8a381b70cf4d4a160
-    sha256: 5013c65e922895baa6f60fba4ec84ee13b9a53e1fb9aa66804c33f74ea236024
+    md5: 1c628861a2a126b9fc9363ca1b7d014e
+    sha256: 04422f10d5bcb251fd254d6a9b0659dcde55e900d48cca159cb1fef637b0050c
   category: main
   optional: false
 - name: appdirs
   version: 1.4.4
   manager: conda
   platform: linux-64
   dependencies:
@@ -450,36 +450,36 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: ebb5f5f7dc4f1a3780ef7ea7738db08c
     sha256: fbc03537a27ef756162c49b1d0608bf7ab12fa5e38ceb8563d6f4859e835ac5c
   category: dev
   optional: true
 - name: charset-normalizer
-  version: 3.1.0
+  version: 3.2.0
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   category: main
   optional: false
 - name: click
-  version: 8.1.3
+  version: 8.1.5
   manager: conda
   platform: linux-64
   dependencies:
     __unix: ''
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.5-unix_pyh707e725_0.conda
   hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+    md5: 4f63f3e01a26e7058eabfa5f984cd6f3
+    sha256: fa46a7053309ff3f4b90b9c32b3c2a7353e3cf1e9807c08e75aed480630848b7
   category: main
   optional: false
 - name: colorama
   version: 0.4.6
   manager: conda
   platform: linux-64
   dependencies:
@@ -550,47 +550,47 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda
   hash:
     md5: 207175b7d514d42f977ec505800d6824
     sha256: 4d3d05138bccdf694ac61a4d483df674684c9e057c2cceeb1fee70181b36a334
   category: dev
   optional: true
 - name: exceptiongroup
-  version: 1.1.1
+  version: 1.1.2
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   category: dev
   optional: true
 - name: execnet
-  version: 1.9.0
+  version: 2.0.2
   manager: conda
   platform: linux-64
   dependencies:
-    python: 2.7|>=3.5
-  url: https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/execnet-2.0.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 0e521f7a5e60d508b121d38b04874fb2
-    sha256: 1900bbc1764d01405e55be2e369d1b830fb435eb0f27c57033372c60f34c675c
+    md5: 67de0d8241e1060a479e3c37793e26f9
+    sha256: 88ea68a360198af39368beecf057af6b31f0ae38071b2bdb2aa961b6ae5427c0
   category: dev
   optional: true
 - name: filelock
-  version: 3.12.1
+  version: 3.12.2
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1f262528bc0ca9d410b98c02d09de3ac
-    sha256: dbb815b1f9c893cdf9a17360148509c439ed83e23128eb6d0be2a9459371c0f2
+    md5: 53522ec72e6adae42bd373ef58357230
+    sha256: 1cbae9f05860f2e566e2977f14dfcd5494beb22c028b0a853ade4ec381d9de71
   category: main
   optional: false
 - name: flaky
   version: 3.7.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -821,23 +821,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
   hash:
     md5: be1e9f1c65a1ed0f2ae9352fec99db64
     sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
   category: main
   optional: false
 - name: pluggy
-  version: 1.0.0
+  version: 1.2.0
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   category: dev
   optional: true
 - name: psutil
   version: 5.9.5
   manager: conda
   platform: linux-64
   dependencies:
@@ -988,23 +988,23 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py311h2582759_1.conda
   hash:
     md5: 5e997292429a22ad50c11af0a2cb0f08
     sha256: 0d5f4dd130796304eab2b48b51d08729acc7d40313e7d8124070490b3a53392c
   category: main
   optional: false
 - name: setuptools
-  version: 67.7.2
+  version: 68.0.0
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 3b68bc43ec6baa48f7354a446267eefe
-    sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
+    md5: 5a7739d0f57ee64133c9d32e6507c46d
+    sha256: 083a0913f5b56644051f31ac40b4eeea762a88c00aa12437817191b85a753cec
   category: main
   optional: false
 - name: six
   version: 1.16.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1072,23 +1072,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 92facfec94bc02d6ccf42e7173831a36
     sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
   category: main
   optional: false
 - name: typing_extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   category: main
   optional: false
 - name: webencodings
   version: 0.5.1
   manager: conda
   platform: linux-64
   dependencies:
@@ -1096,23 +1096,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   category: main
   optional: false
 - name: websocket-client
-  version: 1.5.3
+  version: 1.6.1
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.3-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   hash:
-    md5: 9beb712a1de20fea4e339a2d62851564
-    sha256: 5176f7157b3152535e11c360b089d45d7eaf4c6c0e2116952138ab2ae195419f
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   category: dev
   optional: true
 - name: wheel
   version: 0.40.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1134,38 +1134,38 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/wrapt-1.15.0-py311h2582759_0.conda
   hash:
     md5: 15565d8602a78c6a994e4d9fcb391920
     sha256: 6a169c6822097ca262f824b15bf86371be3f89264d3aefbca92544c4c5535d81
   category: dev
   optional: true
 - name: zipp
-  version: 3.15.0
+  version: 3.16.2
   manager: conda
   platform: linux-64
   dependencies:
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   category: main
   optional: false
 - name: astroid
-  version: 2.15.5
+  version: 2.15.6
   manager: conda
   platform: linux-64
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     wrapt: <2,>=1.14
-  url: https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.5-py311h38be061_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.6-py311h38be061_0.conda
   hash:
-    md5: bc99014b1cb98221bc4a0f4dc889d26f
-    sha256: 4434cc86c7c84847c9382b0a9e41ba6ccb01a8a6b6ccc75ebe8736f99e1f22ff
+    md5: 28b1d4a493fb6acd24cc299d77fed871
+    sha256: 90cbd291d82ffe9aac735a0e543e802d5292d772389f7c8846e744aaf2df5310
   category: dev
   optional: true
 - name: bleach
   version: 6.0.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1277,24 +1277,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
   hash:
     md5: b2355343d6315c892543200231d7154a
     sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
   category: main
   optional: false
 - name: importlib-metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
   hash:
-    md5: f91a5d5175fb7ff2a91952ec7da59cb9
-    sha256: 33d49065756a73fbb92277c756fa00a41891408528eb90ae05ff3367a401ae6e
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   category: main
   optional: false
 - name: isort
   version: 5.12.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1303,24 +1303,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/isort-5.12.0-pyhd8ed1ab_1.conda
   hash:
     md5: 07ed3421bad60867234c7a9282ea39d4
     sha256: d34a62e33ac7acc8fd3167ceb0e2aee4e7974b94de263f52d752716429d95bcb
   category: dev
   optional: true
 - name: jaraco.classes
-  version: 3.2.3
+  version: 3.3.0
   manager: conda
   platform: linux-64
   dependencies:
     more-itertools: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
   category: main
   optional: false
 - name: jinja2
   version: 3.1.2
   manager: conda
   platform: linux-64
   dependencies:
@@ -1329,43 +1329,42 @@
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
   category: main
   optional: false
 - name: markdown-it-py
-  version: 2.2.0
+  version: 3.0.0
   manager: conda
   platform: linux-64
   dependencies:
     mdurl: '>=0.1,<1'
-    python: '>=3.7'
-    typing_extensions: '>=3.7.4'
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: b2928a6c6d52d7e3562b4a59c3214e3a
-    sha256: 65ed439862c1851463f03a9bc5109992ce3e3e025e9a2d76d13ca19f576eee9f
+    md5: 93a8e71256479c62074356ef6ebf501b
+    sha256: c041b0eaf7a6af3344d5dd452815cdc148d6284fec25a4fa3f4263b3a021e962
   category: dev
   optional: true
 - name: mypy
-  version: 1.3.0
+  version: 1.4.1
   manager: conda
   platform: linux-64
   dependencies:
     libgcc-ng: '>=12'
     mypy_extensions: '>=0.4.3'
     psutil: '>=4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     tomli: '>=1.1.0'
     typing_extensions: '>=3.10'
-  url: https://conda.anaconda.org/conda-forge/linux-64/mypy-1.3.0-py311h459d7ec_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/mypy-1.4.1-py311h459d7ec_0.conda
   hash:
-    md5: 20a0e6f8cee024e4f07f2a2f3020f3c2
-    sha256: 9932e63e7d642a543270ef37d4c8d70b78db8dbc29cf2fc58d13174e1ed7821a
+    md5: 70099a5eee9a60f4bd52e388b77b3378
+    sha256: 235514c25d96fe726403893509c573aa1071fba49a57dcfa88ae37d87ba317c8
   category: dev
   optional: true
 - name: nodeenv
   version: 1.8.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1374,25 +1373,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
   hash:
     md5: 2a75b296096adabbabadd5e9782e5fcc
     sha256: 1320306234552717149f36f825ddc7e27ea295f24829e9db4cc6ceaff0b032bd
   category: dev
   optional: true
 - name: pip
-  version: 23.1.2
+  version: '23.2'
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
     setuptools: ''
     wheel: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7288da0d36821349cf1126e8670292df
-    sha256: 4fe1f47f6eac5b2635a622b6f985640bf835843c1d8d7ccbbae0f7d27cadec92
+    md5: fb90dfe13ce16c0a3374e3d34e3291c5
+    sha256: 31e71fc25dbc411c1595661c8eb2c2491e71895ce6954ea2d0e9a585d39eed57
   category: dev
   optional: true
 - name: pyproject_hooks
   version: 1.0.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1400,14 +1399,32 @@
     tomli: '>=1.1.0'
   url: https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda
   hash:
     md5: 21de50391d584eb7f4441b9de1ad773f
     sha256: 016340837fcfef57b351febcbe855eedf0c1f0ecfc910ed48c7fbd20535f9847
   category: dev
   optional: true
+- name: pytest
+  version: 7.4.0
+  manager: conda
+  platform: linux-64
+  dependencies:
+    colorama: ''
+    exceptiongroup: '>=1.0.0rc8'
+    iniconfig: ''
+    packaging: ''
+    pluggy: '>=0.12,<2.0'
+    python: '>=3.7'
+    tomli: '>=1.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3cfe9b9e958e7238a386933c75d190db
+    sha256: 52b2eb4e8d0380d92d45643d0c9706725e691ce8404dab4c2db4aaf58e48a23c
+  category: dev
+  optional: true
 - name: python-dateutil
   version: 2.8.2
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.6'
     six: '>=1.5'
@@ -1427,39 +1444,39 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 626ed9060ddeb681ddc42bcad89156ab
     sha256: 900319483135730d9836855a807822f0500b1a239520749103e9ef9b7ba9f246
   category: dev
   optional: true
 - name: ruamel.yaml
-  version: 0.17.31
+  version: 0.17.32
   manager: conda
   platform: linux-64
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     ruamel.yaml.clib: '>=0.1.2'
     setuptools: ''
-  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.31-py311h459d7ec_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py311h459d7ec_0.conda
   hash:
-    md5: f0fc1409f49257fe5ec2d86d0595d9bc
-    sha256: a5d8d5b290c055301fbf9e5dfb0250df5cd7fa97cd7333e933926958782b32ab
+    md5: 628868dc17f9bd39a2eb77846e35980c
+    sha256: 5439baf06577b6de47047282343b5fc45324f84f3bf0517784f405e0a011a466
   category: main
   optional: false
 - name: typing-extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: linux-64
   dependencies:
-    typing_extensions: 4.6.3
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
+    typing_extensions: 4.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   category: main
   optional: false
 - name: watchdog
   version: 3.0.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1468,14 +1485,27 @@
     pyyaml: '>=3.10'
   url: https://conda.anaconda.org/conda-forge/linux-64/watchdog-3.0.0-py311h38be061_0.conda
   hash:
     md5: a3e24b38169e66795f7af4779ea337b3
     sha256: 02c19cf52bd5209ff4afe779b0a58e9781d528b30868739f0a72ec881e7f9393
   category: dev
   optional: true
+- name: annotated-types
+  version: 0.5.0
+  manager: conda
+  platform: linux-64
+  dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  category: main
+  optional: false
 - name: bcrypt
   version: 3.2.2
   manager: conda
   platform: linux-64
   dependencies:
     cffi: '>=1.1'
     libgcc-ng: '>=12'
@@ -1516,27 +1546,27 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/cmarkgfm-0.8.0-py311hd4cff14_2.tar.bz2
   hash:
     md5: ed1a2dba3b53fcd450f2fe867af0ba3f
     sha256: 1256bf87376f3e8dfad69a5df39536e5f601eed3a2fd1eae28330296fb1910c8
   category: dev
   optional: true
 - name: cryptography
-  version: 41.0.1
+  version: 41.0.2
   manager: conda
   platform: linux-64
   dependencies:
     cffi: '>=1.12'
     libgcc-ng: '>=12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py311h63ff55d_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.2-py311h63ff55d_0.conda
   hash:
-    md5: 69ad01f66b8efff535d341ba5b283c2c
-    sha256: 7e8c5469d96b08ef1acd4cc2fc41d40ae76c30e08372cfe9f7a5a236bec2eb65
+    md5: 90e9e96dd807c2613a163c197192da6c
+    sha256: bb6dd1cf13023b311c9a740f5d77ede6d121d56c0754ca581bcf4a63089f0dcb
   category: main
   optional: false
 - name: flake8-builtins
   version: 2.1.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1584,37 +1614,37 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   category: dev
   optional: true
 - name: gitpython
-  version: 3.1.31
+  version: 3.1.32
   manager: conda
   platform: linux-64
   dependencies:
     gitdb: '>=4.0.1,<5'
     python: '>=3.7'
     typing_extensions: '>=3.7.4.3'
-  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda
   hash:
-    md5: f6e6b482110246a81c3f03e81c68752d
-    sha256: 77c531def610089bc190508fcf304cf96c085c5fe977ab8f7d7c1641769592ac
+    md5: 5809a12901d57388444c3293c975d0bb
+    sha256: 07008a94189e570fcabe003b99bd50b8263f60c824f36f81a8819bb7cf7eab1b
   category: main
   optional: false
 - name: importlib_metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: linux-64
   dependencies:
-    importlib-metadata: '>=6.6.0,<6.6.1.0a0'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
   hash:
-    md5: 3cbc9615f10a3d471532b83e4250b971
-    sha256: 5de35d3c019d8a36e0a0deeb04a62689837bd68234a0a73a3355b860b442eca4
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   category: main
   optional: false
 - name: markdown
   version: 3.3.7
   manager: conda
   platform: linux-64
   dependencies:
@@ -1623,39 +1653,39 @@
   url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.3.7-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 0a0bed31742342688a8570b3b8a50f36
     sha256: 4af5d3f376295753d787be5013900ebca572bd8f30d59e34fbae512ec414eb5e
   category: dev
   optional: true
 - name: platformdirs
-  version: 3.5.1
+  version: 3.8.1
   manager: conda
   platform: linux-64
   dependencies:
     python: '>=3.7'
-    typing-extensions: '>=4.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda
+    typing-extensions: '>=4.6.3'
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda
   hash:
-    md5: e2be672aece1f060adf7154f76531a35
-    sha256: d7845c01a9ee5a224cc9242782befed7d12dc6aac1103650ec87917b20f3579e
+    md5: e76070baecfaca6ecdb5fbd5af7c9309
+    sha256: b5012d6fd30f2462b6ca595539cfdae9aaf61b3b7a56e51ab94aef0fd9efcd3d
   category: main
   optional: false
-- name: pydantic
-  version: 1.10.9
+- name: pydantic-core
+  version: 2.3.0
   manager: conda
   platform: linux-64
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-    typing-extensions: '>=4.2.0'
-  url: https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.9-py311h459d7ec_0.conda
+    typing-extensions: '>=4.6.0'
+  url: https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.3.0-py311h46250e7_0.conda
   hash:
-    md5: 1d8d643ba4e4fcf3e95ce787261798da
-    sha256: 008a91072f7402d03c6ae2ef90873c60d8122ce9defcbe97143daa963f15e5b7
+    md5: 99ca132ca705de6765df5e3c4c346572
+    sha256: 263149c465df875858a8cd5cf85362e3466d03862900ca0fa4570daf29826e0d
   category: main
   optional: false
 - name: pynacl
   version: 1.5.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1667,31 +1697,68 @@
     six: ''
   url: https://conda.anaconda.org/conda-forge/linux-64/pynacl-1.5.0-py311hd4cff14_2.tar.bz2
   hash:
     md5: 8557e0732900a008d8b72e3effbd8521
     sha256: e247c650393f9f7b4fa3e587f50bf89f29872899dddf7e598c782874f88ea25c
   category: dev
   optional: true
-- name: pytest
-  version: 7.3.1
+- name: pytest-cov
+  version: 4.1.0
   manager: conda
   platform: linux-64
   dependencies:
-    colorama: ''
-    exceptiongroup: ''
-    importlib-metadata: '>=0.12'
-    iniconfig: ''
-    packaging: ''
-    pluggy: '>=0.12,<2.0'
-    python: '>=3.8'
-    tomli: '>=1.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.1-pyhd8ed1ab_0.conda
+    coverage: '>=5.2.1'
+    pytest: '>=4.6'
+    python: '>=3.7'
+    toml: ''
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 547c7de697ec99b494a28ddde185b5a4
-    sha256: 42f89db577266b9dc195d09189b92f3af3354fb50c98b1f996c580322dffa8b5
+    md5: 06eb685a3a0b146347a58dda979485da
+    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
+  category: dev
+  optional: true
+- name: pytest-flake8
+  version: 1.1.1
+  manager: conda
+  platform: linux-64
+  dependencies:
+    flake8: '>=4.0'
+    pytest: '>=7.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
+  hash:
+    md5: d717971066d534fd18dfe80a79146f38
+    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
+  category: dev
+  optional: true
+- name: pytest-timeout
+  version: 2.1.0
+  manager: conda
+  platform: linux-64
+  dependencies:
+    pytest: '>=5.0.0'
+    python: '>=3.6'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 2b23b25991cbc6886b95942704fc5c62
+    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
+  category: dev
+  optional: true
+- name: pytest-xdist
+  version: 3.3.1
+  manager: conda
+  platform: linux-64
+  dependencies:
+    execnet: '>=1.1'
+    pytest: '>=6.2.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 816073bb54ef59f33f0f26c14f88311b
+    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
   category: dev
   optional: true
 - name: python-build
   version: 0.10.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1704,26 +1771,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda
   hash:
     md5: 0ab47ce574f6a8bcb9f2076436e7fedb
     sha256: 4c2cd519c85aa8b8e584723ca5f452aa5941d18374470adebfe73bf30fd27573
   category: dev
   optional: true
 - name: rich
-  version: 13.4.1
+  version: 13.4.2
   manager: conda
   platform: linux-64
   dependencies:
-    markdown-it-py: '>=2.2.0,<3.0.0'
+    markdown-it-py: '>=2.2.0'
     pygments: '>=2.13.0,<3.0.0'
     python: '>=3.7.0'
     typing_extensions: '>=4.0.0,<5.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: c3bcbe0d086f15e5918568d3865e4dbf
-    sha256: 312f2628e06a591096a851bf678833fe670ecb16e9b15517ce8e03d7c9d9e600
+    md5: f993baacc175e83fafd6b846e9c4c8a2
+    sha256: d0f6506b0bf1f5563b6b42cf018002b7007bd49e62ad4a178c2a50bf3a7fe45f
   category: dev
   optional: true
 - name: ukkonen
   version: 1.0.1
   manager: conda
   platform: linux-64
   dependencies:
@@ -1735,29 +1802,29 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py311h4dd048b_3.tar.bz2
   hash:
     md5: dbfea4376856bf7bd2121e719cf816e5
     sha256: 41d7b9ab6414ce61496dd001e98a49d73d6cf61e5c051c22df35e218c72de1f1
   category: dev
   optional: true
 - name: black
-  version: 23.3.0
+  version: 23.7.0
   manager: conda
   platform: linux-64
   dependencies:
     click: '>=8.0.0'
     mypy_extensions: '>=0.4.3'
     packaging: '>=22.0'
     pathspec: '>=0.9'
     platformdirs: '>=2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/linux-64/black-23.3.0-py311h38be061_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/black-23.7.0-py311h38be061_1.conda
   hash:
-    md5: b0d621848bfba5aacbdfc43dfdeabfec
-    sha256: c729ebbdca2ca7286305ad51cc3beea6b85e68cd02794fb9895f3d5e16540b86
+    md5: 9dc54d30b15760b58706ac840803f6b4
+    sha256: bb03f67cb1b242ef59d9b80a8d9e99bc1e4725230473ceb59b9a6d0fb989cf9f
   category: dev
   optional: true
 - name: check-manifest
   version: '0.49'
   manager: conda
   platform: linux-64
   dependencies:
@@ -1768,25 +1835,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/check-manifest-0.49-pyhd8ed1ab_0.conda
   hash:
     md5: 65b3059f2f0807433ee3c2673a886123
     sha256: f8d03ad89aacf5278b74f73f6720588cfa41481c959206147fd58d54f7974487
   category: dev
   optional: true
 - name: flake8-comprehensions
-  version: 3.12.0
+  version: 3.13.0
   manager: conda
   platform: linux-64
   dependencies:
     flake8: '>=3.0,!=3.2.0'
     importlib_metadata: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.12.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.13.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 18c6bc2bb3cd3950029569362cca2e33
-    sha256: c825986cf7a2f617b61373e421d74e9383696d48def52e4619af2bea1b747e8d
+    md5: f1fca1448e90eaa8fc5a3676813b4c0c
+    sha256: 3fd60ba3cfedd29fcceea147141aea74763483e3491e32afdeaa4357cf8eb92e
   category: dev
   optional: true
 - name: identify
   version: 2.5.24
   manager: conda
   platform: linux-64
   dependencies:
@@ -1847,14 +1914,31 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/paramiko-3.2.0-pyhd8ed1ab_0.conda
   hash:
     md5: f212c7eb95e909df4795297f73690993
     sha256: e425a03e5e2ef2ec5a78711686c59cfceeeeec3a98165fbc7d186bd6a5cb78de
   category: dev
   optional: true
+- name: pydantic
+  version: 2.0.3
+  manager: conda
+  platform: linux-64
+  dependencies:
+    annotated-types: '>=0.4.0'
+    libgcc-ng: '>=12'
+    pydantic-core: 2.3.0
+    python: '>=3.11,<3.12.0a0'
+    python_abi: 3.11.*
+    typing-extensions: '>=4.6.1'
+  url: https://conda.anaconda.org/conda-forge/linux-64/pydantic-2.0.3-py311h459d7ec_0.conda
+  hash:
+    md5: 2a4ec2f1b4110a562a7c5434a8f88e99
+    sha256: 85d0434238307e89f2472042ddc8f7292dce193440e41f742fe57b5096d7fb3e
+  category: main
+  optional: false
 - name: pylint
   version: 2.17.4
   manager: conda
   platform: linux-64
   dependencies:
     astroid: '>=2.15.4,<2.17.0-dev0'
     colorama: '>=0.4.5'
@@ -1869,25 +1953,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pylint-2.17.4-pyhd8ed1ab_0.conda
   hash:
     md5: a9d97fe4617aba393d90ea81576b6b46
     sha256: dec2a299b39212fc311771faec9d5cd854a18f8655d04930b8d69139c9d8a546
   category: dev
   optional: true
 - name: pymdown-extensions
-  version: 10.0.1
+  version: 10.1.0
   manager: conda
   platform: linux-64
   dependencies:
     markdown: '>=3.2'
     python: '>=3.7'
     pyyaml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.0.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.1.0-pyhd8ed1ab_0.conda
   hash:
-    md5: c97339cff97ae0c82dcfd7ccf72cb3d1
-    sha256: fac9ac7e236925056e69bcdec34b219a2fa860bf9434d4391986dad6afd22859
+    md5: ab329864b9f57210f3d2f9c6cd30b921
+    sha256: 892c9409b5d3d8329c8b435d91f9075df271f06bde4ed04ec23fb19831502b02
   category: dev
   optional: true
 - name: pyopenssl
   version: 23.2.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -1895,84 +1979,28 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   category: main
   optional: false
-- name: pytest-cov
-  version: 4.1.0
-  manager: conda
-  platform: linux-64
-  dependencies:
-    coverage: '>=5.2.1'
-    pytest: '>=4.6'
-    python: '>=3.7'
-    toml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
-  hash:
-    md5: 06eb685a3a0b146347a58dda979485da
-    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
-  category: dev
-  optional: true
-- name: pytest-flake8
-  version: 1.1.1
-  manager: conda
-  platform: linux-64
-  dependencies:
-    flake8: '>=4.0'
-    pytest: '>=7.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
-  hash:
-    md5: d717971066d534fd18dfe80a79146f38
-    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
-  category: dev
-  optional: true
-- name: pytest-timeout
-  version: 2.1.0
-  manager: conda
-  platform: linux-64
-  dependencies:
-    pytest: '>=5.0.0'
-    python: '>=3.6'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
-  hash:
-    md5: 2b23b25991cbc6886b95942704fc5c62
-    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
-  category: dev
-  optional: true
-- name: pytest-xdist
-  version: 3.3.1
-  manager: conda
-  platform: linux-64
-  dependencies:
-    execnet: '>=1.1'
-    pytest: '>=6.2.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
-  hash:
-    md5: 816073bb54ef59f33f0f26c14f88311b
-    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
-  category: dev
-  optional: true
 - name: readme_renderer
-  version: '37.3'
+  version: '40.0'
   manager: conda
   platform: linux-64
   dependencies:
     bleach: '>=2.1.0'
     cmarkgfm: '>=0.8.0'
     docutils: '>=0.13.1'
     pygments: '>=2.5.1'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 82e8ab317fe8f1d2a944688438dce868
-    sha256: 3f6d5ffe4c07bbddfcc7d108d01a1cbd78d38e9b860de46f16ca617bd4f42cd1
+    md5: 9ba2b509f6fe88364512caa9089ea886
+    sha256: 37a3b585fab825fb737ff0b2c1d2b9446ffb27b0ec42529ef7102558cafe331f
   category: dev
   optional: true
 - name: secretstorage
   version: 3.3.3
   manager: conda
   platform: linux-64
   dependencies:
@@ -1984,60 +2012,60 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py311h38be061_1.tar.bz2
   hash:
     md5: ec745aaae03cc47120c1f11ac7b7bcf5
     sha256: eb3c992e3ab0ed8b2aabe99030b58bd90413eff13246ade769bdc8add29174cb
   category: main
   optional: false
 - name: virtualenv
-  version: 20.23.0
+  version: 20.24.0
   manager: conda
   platform: linux-64
   dependencies:
     distlib: <1,>=0.3.6
-    filelock: <4,>=3.11
-    platformdirs: <4,>=3.2
+    filelock: <4,>=3.12
+    platformdirs: <4,>=3.5.1
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.0-pyhd8ed1ab_0.conda
   hash:
-    md5: a920e114c4c2ced2280e266da65ab5e6
-    sha256: 13d667887ea08b6d1fe2eb09d2d737f9af7343735d3bfa5ffaa3f67eec8eaff7
+    md5: 1b4a286252e336bef9ef8fa589eefdd1
+    sha256: d8b3a1badec92e81aed61d24fa33268ead568eae02372333d95bc38fce296330
   category: main
   optional: false
 - name: keyring
-  version: 23.13.1
+  version: 24.2.0
   manager: conda
   platform: linux-64
   dependencies:
     importlib_metadata: '>=4.11.4'
     jaraco.classes: ''
     jeepney: '>=0.4.2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     secretstorage: '>=3.2'
-  url: https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py311h38be061_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/keyring-24.2.0-py311h38be061_0.conda
   hash:
-    md5: 0dc0127b1daefefa5e2caa49dde5c230
-    sha256: f3bf1f96a2d577a8ae8f023cba8301dc82b44a91afb0c370d70c90c205a39710
+    md5: b8eedb6181eff2dfeb34182330db1240
+    sha256: 0cca007d39351cada97570660505e4a5be09eda7b1a9fa4027707f4304dda98e
   category: main
   optional: false
 - name: pre-commit
-  version: 3.3.2
+  version: 3.3.3
   manager: conda
   platform: linux-64
   dependencies:
     cfgv: '>=2.0.0'
     identify: '>=1.0.0'
     nodeenv: '>=0.11.1'
     python: '>=3.8'
     pyyaml: '>=5.1'
     virtualenv: '>=20.10.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.2-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.3-pyha770c72_0.conda
   hash:
-    md5: dbb0111b18ea5c9983fb8db0aef6000b
-    sha256: a55d8a19bb00c2c5bf8a074c94d5ac1ffed8d63c53c9df4cee76f3764ad7a304
+    md5: dd64a0e440754ed97610b3e6b502b6b1
+    sha256: 3df1434057ce827d88cdd84578732030b3d4b5a0bc6c58bff12b7f8001c1be5b
   category: dev
   optional: true
 - name: urllib3
   version: 1.26.15
   manager: conda
   platform: linux-64
   dependencies:
@@ -2081,29 +2109,29 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda
   hash:
     md5: 9f0b2eb5f5dd2cec36d5342a80adfec0
     sha256: 894e2f4c59221b9633c60281a17fefe09ba0bf5d996992cebeb504d0585dd0dd
   category: main
   optional: false
 - name: docker-py
-  version: 6.1.0
+  version: 6.1.3
   manager: conda
   platform: linux-64
   dependencies:
     packaging: '>=14.0'
     paramiko: '>=2.4.3'
     python: '>=3.7'
     pywin32-on-windows: ''
     requests: '>=2.26.0'
     urllib3: '>=1.26.0'
     websocket-client: '>=0.32.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.3-pyhd8ed1ab_0.conda
   hash:
-    md5: 543336c6aa9516cfb29c51d5c162b177
-    sha256: 5e01e15e20ee573c99b530633a0d5c71fd515e4ac6d2f5f5f57baece8b915cc3
+    md5: c95d23d8bae7e21491868cc7772d7c73
+    sha256: 7c3031602e92fd7682302ef98a45bdf7374d48a849cdd3900b7c68a32d162177
   category: dev
   optional: true
 - name: doctr
   version: 1.9.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -2130,32 +2158,32 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: c99ae3abf501990769047b4b40a98f17
     sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
   category: main
   optional: false
 - name: mkdocs-material
-  version: 9.1.15
+  version: 9.1.18
   manager: conda
   platform: linux-64
   dependencies:
     colorama: '>=0.4'
     jinja2: '>=3.0'
     markdown: '>=3.2'
     mkdocs: '>=1.4.2'
     mkdocs-material-extensions: '>=1.1'
     pygments: '>=2.14'
-    pymdown-extensions: '>=9.9'
+    pymdown-extensions: '>=9.9.1'
     python: '>=3.7'
     regex: '>=2022.4.24'
     requests: '>=2.26'
-  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.15-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.18-pyhd8ed1ab_0.conda
   hash:
-    md5: 11383355f8c54b2a89ffd689c0cc5276
-    sha256: 445cacaa27a2c96fdb852b0d0d281e196fba89b6879ac4dd1988fa75270af04a
+    md5: 8fca138f1f46db013daf43d342169612
+    sha256: b23684c0774d7c9a08e265f97c0411d8d1737f27b94e484d37bf161c2ca52f4b
   category: dev
   optional: true
 - name: requests-toolbelt
   version: 1.0.0
   manager: conda
   platform: linux-64
   dependencies:
@@ -2390,18 +2418,18 @@
   optional: false
 - name: libzlib
   version: 1.2.13
   manager: conda
   platform: linux-aarch64
   dependencies:
     libgcc-ng: '>=12'
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h4e544f5_4.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
   hash:
-    md5: 88596b6277fe6d39f046983aae6044db
-    sha256: 9803ac96dbdbc27df9c149e06d4436b778c468bd0e6e023fbcb49a6fe9c404b4
+    md5: b213aa87eea9491ef7b129179322e955
+    sha256: aeeefbb61e5e8227e53566d5e42dbb49e120eb99109996bf0dbfde8f180747a7
   category: main
   optional: false
 - name: ncurses
   version: '6.4'
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -2512,56 +2540,56 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.12-hd8af866_0.tar.bz2
   hash:
     md5: 7894e82ff743bd96c76585ddebe28e2a
     sha256: d659316c9e502fb0e1b9a284fb0f0c00e273bff787e9385ab14be9af13dcd0d2
   category: main
   optional: false
 - name: libglib
-  version: 2.76.3
+  version: 2.76.4
   manager: conda
   platform: linux-aarch64
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     libffi: '>=3.4,<4.0a0'
     libgcc-ng: '>=12'
     libiconv: '>=1.17,<2.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     pcre2: '>=10.40,<10.41.0a0'
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.76.3-h0464669_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.76.4-h0464669_0.conda
   hash:
-    md5: 8af0b99551d0d5cd020b5368b15c458a
-    sha256: 70ab257be48124ed4f3cc830f07c43443c2b56881be1572b80bea5a39b4e022c
+    md5: 9841a8bff458f50ce8b41f386c57db02
+    sha256: 67ebafd87306e6b08c015b76226deee3f9e975a51151c6a28e89d999e4bbfbf4
   category: main
   optional: false
 - name: python
-  version: 3.11.3
+  version: 3.11.4
   manager: conda
   platform: linux-aarch64
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     ld_impl_linux-aarch64: '>=2.36.1'
     libexpat: '>=2.5.0,<3.0a0'
     libffi: '>=3.4,<4.0a0'
     libgcc-ng: '>=12'
     libnsl: '>=2.0.0,<2.1.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libuuid: '>=2.38.1,<3.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    ncurses: '>=6.4,<7.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     readline: '>=8.2,<9.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     xz: '>=5.2.6,<6.0a0'
     pip: ''
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.11.3-h07235ee_0_cpython.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.11.4-h43d1f9e_0_cpython.conda
   hash:
-    md5: c674dc74adf86554b366331c6a882e68
-    sha256: d7d5be6979227106d7b1ef970e17eac64d3ce2515e49e9613f192deb3b7ee6b0
+    md5: c8fc93307c88656b8138af853a1b653d
+    sha256: 9d1d6339fb54c5fe0c7f367e075e846cb337e2dcc275543de461ff4449a64ea7
   category: main
   optional: false
 - name: appdirs
   version: 1.4.4
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -2605,36 +2633,36 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: ebb5f5f7dc4f1a3780ef7ea7738db08c
     sha256: fbc03537a27ef756162c49b1d0608bf7ab12fa5e38ceb8563d6f4859e835ac5c
   category: dev
   optional: true
 - name: charset-normalizer
-  version: 3.1.0
+  version: 3.2.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   category: main
   optional: false
 - name: click
-  version: 8.1.3
+  version: 8.1.5
   manager: conda
   platform: linux-aarch64
   dependencies:
     __unix: ''
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.5-unix_pyh707e725_0.conda
   hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+    md5: 4f63f3e01a26e7058eabfa5f984cd6f3
+    sha256: fa46a7053309ff3f4b90b9c32b3c2a7353e3cf1e9807c08e75aed480630848b7
   category: main
   optional: false
 - name: colorama
   version: 0.4.6
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -2705,47 +2733,47 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/docutils-0.20.1-py311hfecb2dc_0.conda
   hash:
     md5: b7a59668b152f36fbcbd5e34e12b5b35
     sha256: c0e3e87d6321b8ff814eea15eb7f110c14fb97742e9bc5b782bd14bd77e63e22
   category: dev
   optional: true
 - name: exceptiongroup
-  version: 1.1.1
+  version: 1.1.2
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   category: dev
   optional: true
 - name: execnet
-  version: 1.9.0
+  version: 2.0.2
   manager: conda
   platform: linux-aarch64
   dependencies:
-    python: 2.7|>=3.5
-  url: https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/execnet-2.0.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 0e521f7a5e60d508b121d38b04874fb2
-    sha256: 1900bbc1764d01405e55be2e369d1b830fb435eb0f27c57033372c60f34c675c
+    md5: 67de0d8241e1060a479e3c37793e26f9
+    sha256: 88ea68a360198af39368beecf057af6b31f0ae38071b2bdb2aa961b6ae5427c0
   category: dev
   optional: true
 - name: filelock
-  version: 3.12.1
+  version: 3.12.2
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1f262528bc0ca9d410b98c02d09de3ac
-    sha256: dbb815b1f9c893cdf9a17360148509c439ed83e23128eb6d0be2a9459371c0f2
+    md5: 53522ec72e6adae42bd373ef58357230
+    sha256: 1cbae9f05860f2e566e2977f14dfcd5494beb22c028b0a853ade4ec381d9de71
   category: main
   optional: false
 - name: flaky
   version: 3.7.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -2976,23 +3004,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
   hash:
     md5: be1e9f1c65a1ed0f2ae9352fec99db64
     sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
   category: main
   optional: false
 - name: pluggy
-  version: 1.0.0
+  version: 1.2.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   category: dev
   optional: true
 - name: psutil
   version: 5.9.5
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3143,23 +3171,23 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/ruamel.yaml.clib-0.2.7-py311h1d6c08a_1.conda
   hash:
     md5: ab27bf4e2dc92321211cd2977220a3f0
     sha256: 5631c85035068e5ba01c35ef8c67899d93344a3211c1a18d8ddcbd926b8e72b1
   category: main
   optional: false
 - name: setuptools
-  version: 67.7.2
+  version: 68.0.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 3b68bc43ec6baa48f7354a446267eefe
-    sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
+    md5: 5a7739d0f57ee64133c9d32e6507c46d
+    sha256: 083a0913f5b56644051f31ac40b4eeea762a88c00aa12437817191b85a753cec
   category: main
   optional: false
 - name: six
   version: 1.16.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3227,23 +3255,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 92facfec94bc02d6ccf42e7173831a36
     sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
   category: main
   optional: false
 - name: typing_extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   category: main
   optional: false
 - name: webencodings
   version: 0.5.1
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3251,23 +3279,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   category: main
   optional: false
 - name: websocket-client
-  version: 1.5.3
+  version: 1.6.1
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.3-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   hash:
-    md5: 9beb712a1de20fea4e339a2d62851564
-    sha256: 5176f7157b3152535e11c360b089d45d7eaf4c6c0e2116952138ab2ae195419f
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   category: dev
   optional: true
 - name: wheel
   version: 0.40.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3289,38 +3317,38 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/wrapt-1.15.0-py311h1d6c08a_0.conda
   hash:
     md5: 015597e497555da65d7fef7edaa60abf
     sha256: daf6b1a22731b34922f9f17e88709dd553e2b5f9091fa64ceb646aafb4d97cab
   category: dev
   optional: true
 - name: zipp
-  version: 3.15.0
+  version: 3.16.2
   manager: conda
   platform: linux-aarch64
   dependencies:
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   category: main
   optional: false
 - name: astroid
-  version: 2.15.5
+  version: 2.15.6
   manager: conda
   platform: linux-aarch64
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     wrapt: <2,>=1.14
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/astroid-2.15.5-py311hec3470c_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/astroid-2.15.6-py311hec3470c_0.conda
   hash:
-    md5: 4fe7a6f1cb1dd4ead75365972d5c7d4f
-    sha256: 8b6c66e4c2a1df79fd247138de35ae7f40d8bd8607e5798da762e1dd93277fc7
+    md5: f5ffeb7e72b7a52b776a1f8bd9a93d23
+    sha256: e480ce49e28cc9e5feb736fdcaf965aa273263df81eef5149319a7380057cd2d
   category: dev
   optional: true
 - name: bleach
   version: 6.0.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3432,24 +3460,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
   hash:
     md5: b2355343d6315c892543200231d7154a
     sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
   category: main
   optional: false
 - name: importlib-metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
   hash:
-    md5: f91a5d5175fb7ff2a91952ec7da59cb9
-    sha256: 33d49065756a73fbb92277c756fa00a41891408528eb90ae05ff3367a401ae6e
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   category: main
   optional: false
 - name: isort
   version: 5.12.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3458,24 +3486,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/isort-5.12.0-pyhd8ed1ab_1.conda
   hash:
     md5: 07ed3421bad60867234c7a9282ea39d4
     sha256: d34a62e33ac7acc8fd3167ceb0e2aee4e7974b94de263f52d752716429d95bcb
   category: dev
   optional: true
 - name: jaraco.classes
-  version: 3.2.3
+  version: 3.3.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     more-itertools: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
   category: main
   optional: false
 - name: jinja2
   version: 3.1.2
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3484,43 +3512,42 @@
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
   category: main
   optional: false
 - name: markdown-it-py
-  version: 2.2.0
+  version: 3.0.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     mdurl: '>=0.1,<1'
-    python: '>=3.7'
-    typing_extensions: '>=3.7.4'
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: b2928a6c6d52d7e3562b4a59c3214e3a
-    sha256: 65ed439862c1851463f03a9bc5109992ce3e3e025e9a2d76d13ca19f576eee9f
+    md5: 93a8e71256479c62074356ef6ebf501b
+    sha256: c041b0eaf7a6af3344d5dd452815cdc148d6284fec25a4fa3f4263b3a021e962
   category: dev
   optional: true
 - name: mypy
-  version: 1.3.0
+  version: 1.4.1
   manager: conda
   platform: linux-aarch64
   dependencies:
     libgcc-ng: '>=12'
     mypy_extensions: '>=0.4.3'
     psutil: '>=4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     tomli: '>=1.1.0'
     typing_extensions: '>=3.10'
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/mypy-1.3.0-py311hcd402e7_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/mypy-1.4.1-py311hcd402e7_0.conda
   hash:
-    md5: d03449605f5f5c5b15dc7704fff236b1
-    sha256: 31743f18ffa1bba2b70900a35b1b7b84fd7ad3e92bf2864c657bf0b2ceb4bea6
+    md5: 5aa11df4d3c9009dcbbf31cee9a3ad8b
+    sha256: 017cc7e9b2f807dad76a1d3ee239d9d22cf32f9aeeb892b179355913ff75cfec
   category: dev
   optional: true
 - name: nodeenv
   version: 1.8.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3529,25 +3556,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
   hash:
     md5: 2a75b296096adabbabadd5e9782e5fcc
     sha256: 1320306234552717149f36f825ddc7e27ea295f24829e9db4cc6ceaff0b032bd
   category: dev
   optional: true
 - name: pip
-  version: 23.1.2
+  version: '23.2'
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
     setuptools: ''
     wheel: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7288da0d36821349cf1126e8670292df
-    sha256: 4fe1f47f6eac5b2635a622b6f985640bf835843c1d8d7ccbbae0f7d27cadec92
+    md5: fb90dfe13ce16c0a3374e3d34e3291c5
+    sha256: 31e71fc25dbc411c1595661c8eb2c2491e71895ce6954ea2d0e9a585d39eed57
   category: dev
   optional: true
 - name: pyproject_hooks
   version: 1.0.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3555,14 +3582,32 @@
     tomli: '>=1.1.0'
   url: https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda
   hash:
     md5: 21de50391d584eb7f4441b9de1ad773f
     sha256: 016340837fcfef57b351febcbe855eedf0c1f0ecfc910ed48c7fbd20535f9847
   category: dev
   optional: true
+- name: pytest
+  version: 7.4.0
+  manager: conda
+  platform: linux-aarch64
+  dependencies:
+    colorama: ''
+    exceptiongroup: '>=1.0.0rc8'
+    iniconfig: ''
+    packaging: ''
+    pluggy: '>=0.12,<2.0'
+    python: '>=3.7'
+    tomli: '>=1.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3cfe9b9e958e7238a386933c75d190db
+    sha256: 52b2eb4e8d0380d92d45643d0c9706725e691ce8404dab4c2db4aaf58e48a23c
+  category: dev
+  optional: true
 - name: python-dateutil
   version: 2.8.2
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.6'
     six: '>=1.5'
@@ -3582,39 +3627,39 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 626ed9060ddeb681ddc42bcad89156ab
     sha256: 900319483135730d9836855a807822f0500b1a239520749103e9ef9b7ba9f246
   category: dev
   optional: true
 - name: ruamel.yaml
-  version: 0.17.31
+  version: 0.17.32
   manager: conda
   platform: linux-aarch64
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     ruamel.yaml.clib: '>=0.1.2'
     setuptools: ''
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/ruamel.yaml-0.17.31-py311hcd402e7_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/ruamel.yaml-0.17.32-py311hcd402e7_0.conda
   hash:
-    md5: 34c050532ef52e45f92c79907644fbcc
-    sha256: 7cdcad982a6bce34b2a2af93a06973baf6986f8088834d787e4bef68926688cf
+    md5: 160b89258ba007591e5630197bf241d0
+    sha256: e8b0e67b90f38c85c96721bd1ced2ebbdf647b3289a4f3564e054dc5733fefc1
   category: main
   optional: false
 - name: typing-extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: linux-aarch64
   dependencies:
-    typing_extensions: 4.6.3
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
+    typing_extensions: 4.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   category: main
   optional: false
 - name: watchdog
   version: 3.0.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3623,14 +3668,27 @@
     pyyaml: '>=3.10'
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/watchdog-3.0.0-py311hfecb2dc_0.conda
   hash:
     md5: 2554c4674b21c7863a11734a60b48903
     sha256: 8225659eb773bbd2cff0cf229baa68195e192b8f6d6e529c20e48d1de6a7e29f
   category: dev
   optional: true
+- name: annotated-types
+  version: 0.5.0
+  manager: conda
+  platform: linux-aarch64
+  dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  category: main
+  optional: false
 - name: bcrypt
   version: 3.2.2
   manager: conda
   platform: linux-aarch64
   dependencies:
     cffi: '>=1.1'
     libgcc-ng: '>=12'
@@ -3671,27 +3729,27 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/cmarkgfm-0.8.0-py311hdfa8b44_2.tar.bz2
   hash:
     md5: a0384090e0cd470dbf59ba8314103986
     sha256: 711b771bec0458e1fb9e8598d8312fdec48454a4a3a8eff5dfc821555495d6e5
   category: dev
   optional: true
 - name: cryptography
-  version: 41.0.1
+  version: 41.0.2
   manager: conda
   platform: linux-aarch64
   dependencies:
     cffi: '>=1.12'
     libgcc-ng: '>=12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/cryptography-41.0.1-py311hd42d77a_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/cryptography-41.0.2-py311hd42d77a_0.conda
   hash:
-    md5: c893e800b4530e416a84fa6c22b506d8
-    sha256: d4754db5d3a89dcc573fa3586a66218b59a99944ddd50abefa60f7e97d741976
+    md5: 6c662efe3125dcf9e15824b1940d2bed
+    sha256: f007111d58fcca8e15f799d54a9be6f485bbbe7b6e2299f881b1dc92ed0882b6
   category: main
   optional: false
 - name: flake8-builtins
   version: 2.1.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3739,37 +3797,37 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   category: dev
   optional: true
 - name: gitpython
-  version: 3.1.31
+  version: 3.1.32
   manager: conda
   platform: linux-aarch64
   dependencies:
     gitdb: '>=4.0.1,<5'
     python: '>=3.7'
     typing_extensions: '>=3.7.4.3'
-  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda
   hash:
-    md5: f6e6b482110246a81c3f03e81c68752d
-    sha256: 77c531def610089bc190508fcf304cf96c085c5fe977ab8f7d7c1641769592ac
+    md5: 5809a12901d57388444c3293c975d0bb
+    sha256: 07008a94189e570fcabe003b99bd50b8263f60c824f36f81a8819bb7cf7eab1b
   category: main
   optional: false
 - name: importlib_metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: linux-aarch64
   dependencies:
-    importlib-metadata: '>=6.6.0,<6.6.1.0a0'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
   hash:
-    md5: 3cbc9615f10a3d471532b83e4250b971
-    sha256: 5de35d3c019d8a36e0a0deeb04a62689837bd68234a0a73a3355b860b442eca4
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   category: main
   optional: false
 - name: markdown
   version: 3.3.7
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3778,39 +3836,39 @@
   url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.3.7-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 0a0bed31742342688a8570b3b8a50f36
     sha256: 4af5d3f376295753d787be5013900ebca572bd8f30d59e34fbae512ec414eb5e
   category: dev
   optional: true
 - name: platformdirs
-  version: 3.5.1
+  version: 3.8.1
   manager: conda
   platform: linux-aarch64
   dependencies:
     python: '>=3.7'
-    typing-extensions: '>=4.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda
+    typing-extensions: '>=4.6.3'
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda
   hash:
-    md5: e2be672aece1f060adf7154f76531a35
-    sha256: d7845c01a9ee5a224cc9242782befed7d12dc6aac1103650ec87917b20f3579e
+    md5: e76070baecfaca6ecdb5fbd5af7c9309
+    sha256: b5012d6fd30f2462b6ca595539cfdae9aaf61b3b7a56e51ab94aef0fd9efcd3d
   category: main
   optional: false
-- name: pydantic
-  version: 1.10.9
+- name: pydantic-core
+  version: 2.3.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-    typing-extensions: '>=4.2.0'
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pydantic-1.10.9-py311hcd402e7_0.conda
+    typing-extensions: '>=4.6.0'
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pydantic-core-2.3.0-py311h2bdde80_0.conda
   hash:
-    md5: d4ad60a6df4512316019bd35e4c7d4fd
-    sha256: 2e7b1ee0caedbb1c30da72a0ef888faeaed25a92270897f67c58b6cc300e462f
+    md5: 2373c6117c5b60ea238eb56ecec4ae62
+    sha256: d0f4568335c3bbe4c3f1b2e9ded8a623e8ab1dea8e60b5891ae717274f6646f0
   category: main
   optional: false
 - name: pynacl
   version: 1.5.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3822,31 +3880,68 @@
     six: ''
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/pynacl-1.5.0-py311hdfa8b44_2.tar.bz2
   hash:
     md5: 4fce9c3e11fe331f40d14c64367a37f9
     sha256: 5f0eda2da18af1c644530e002b3b5d9bca36eb4054a1a5db04e5b62f793c034e
   category: dev
   optional: true
-- name: pytest
-  version: 7.3.1
+- name: pytest-cov
+  version: 4.1.0
   manager: conda
   platform: linux-aarch64
   dependencies:
-    colorama: ''
-    exceptiongroup: ''
-    importlib-metadata: '>=0.12'
-    iniconfig: ''
-    packaging: ''
-    pluggy: '>=0.12,<2.0'
-    python: '>=3.8'
-    tomli: '>=1.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.1-pyhd8ed1ab_0.conda
+    coverage: '>=5.2.1'
+    pytest: '>=4.6'
+    python: '>=3.7'
+    toml: ''
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 06eb685a3a0b146347a58dda979485da
+    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
+  category: dev
+  optional: true
+- name: pytest-flake8
+  version: 1.1.1
+  manager: conda
+  platform: linux-aarch64
+  dependencies:
+    flake8: '>=4.0'
+    pytest: '>=7.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
   hash:
-    md5: 547c7de697ec99b494a28ddde185b5a4
-    sha256: 42f89db577266b9dc195d09189b92f3af3354fb50c98b1f996c580322dffa8b5
+    md5: d717971066d534fd18dfe80a79146f38
+    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
+  category: dev
+  optional: true
+- name: pytest-timeout
+  version: 2.1.0
+  manager: conda
+  platform: linux-aarch64
+  dependencies:
+    pytest: '>=5.0.0'
+    python: '>=3.6'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 2b23b25991cbc6886b95942704fc5c62
+    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
+  category: dev
+  optional: true
+- name: pytest-xdist
+  version: 3.3.1
+  manager: conda
+  platform: linux-aarch64
+  dependencies:
+    execnet: '>=1.1'
+    pytest: '>=6.2.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 816073bb54ef59f33f0f26c14f88311b
+    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
   category: dev
   optional: true
 - name: python-build
   version: 0.10.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3859,26 +3954,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda
   hash:
     md5: 0ab47ce574f6a8bcb9f2076436e7fedb
     sha256: 4c2cd519c85aa8b8e584723ca5f452aa5941d18374470adebfe73bf30fd27573
   category: dev
   optional: true
 - name: rich
-  version: 13.4.1
+  version: 13.4.2
   manager: conda
   platform: linux-aarch64
   dependencies:
-    markdown-it-py: '>=2.2.0,<3.0.0'
+    markdown-it-py: '>=2.2.0'
     pygments: '>=2.13.0,<3.0.0'
     python: '>=3.7.0'
     typing_extensions: '>=4.0.0,<5.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: c3bcbe0d086f15e5918568d3865e4dbf
-    sha256: 312f2628e06a591096a851bf678833fe670ecb16e9b15517ce8e03d7c9d9e600
+    md5: f993baacc175e83fafd6b846e9c4c8a2
+    sha256: d0f6506b0bf1f5563b6b42cf018002b7007bd49e62ad4a178c2a50bf3a7fe45f
   category: dev
   optional: true
 - name: ukkonen
   version: 1.0.1
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3890,29 +3985,29 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/ukkonen-1.0.1-py311hc04b03c_3.tar.bz2
   hash:
     md5: 07831574cdc6f96b7f5c882f69afe189
     sha256: f26f8bffd42e5758299dc81e909966d41478db90b45f42901cdd4b2888d3ddeb
   category: dev
   optional: true
 - name: black
-  version: 23.3.0
+  version: 23.7.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     click: '>=8.0.0'
     mypy_extensions: '>=0.4.3'
     packaging: '>=22.0'
     pathspec: '>=0.9'
     platformdirs: '>=2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/black-23.3.0-py311hec3470c_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/black-23.7.0-py311hec3470c_1.conda
   hash:
-    md5: 473d677e53810464458ad083e47e97e6
-    sha256: 4727ff1d75b44004cf0f213882ded5cd50f4a4118734823595e36afc19b9805b
+    md5: 9ae157cafb93525f2dfc6b96a4b6951f
+    sha256: b1f575fd6f2b739db5f5a0da4209a54af496054129eb03f7b89dcab0c25941db
   category: dev
   optional: true
 - name: check-manifest
   version: '0.49'
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -3923,25 +4018,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/check-manifest-0.49-pyhd8ed1ab_0.conda
   hash:
     md5: 65b3059f2f0807433ee3c2673a886123
     sha256: f8d03ad89aacf5278b74f73f6720588cfa41481c959206147fd58d54f7974487
   category: dev
   optional: true
 - name: flake8-comprehensions
-  version: 3.12.0
+  version: 3.13.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     flake8: '>=3.0,!=3.2.0'
     importlib_metadata: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.12.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.13.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 18c6bc2bb3cd3950029569362cca2e33
-    sha256: c825986cf7a2f617b61373e421d74e9383696d48def52e4619af2bea1b747e8d
+    md5: f1fca1448e90eaa8fc5a3676813b4c0c
+    sha256: 3fd60ba3cfedd29fcceea147141aea74763483e3491e32afdeaa4357cf8eb92e
   category: dev
   optional: true
 - name: identify
   version: 2.5.24
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -4002,14 +4097,31 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/paramiko-3.2.0-pyhd8ed1ab_0.conda
   hash:
     md5: f212c7eb95e909df4795297f73690993
     sha256: e425a03e5e2ef2ec5a78711686c59cfceeeeec3a98165fbc7d186bd6a5cb78de
   category: dev
   optional: true
+- name: pydantic
+  version: 2.0.3
+  manager: conda
+  platform: linux-aarch64
+  dependencies:
+    annotated-types: '>=0.4.0'
+    libgcc-ng: '>=12'
+    pydantic-core: 2.3.0
+    python: '>=3.11,<3.12.0a0'
+    python_abi: 3.11.*
+    typing-extensions: '>=4.6.1'
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pydantic-2.0.3-py311hcd402e7_0.conda
+  hash:
+    md5: 4bf55f474124da80b4d2df64059d59da
+    sha256: 7899a403dec6cb7ae49c8498a91d8180b12fbf0e88935ccfb275564025dc8816
+  category: main
+  optional: false
 - name: pylint
   version: 2.17.4
   manager: conda
   platform: linux-aarch64
   dependencies:
     astroid: '>=2.15.4,<2.17.0-dev0'
     colorama: '>=0.4.5'
@@ -4024,25 +4136,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pylint-2.17.4-pyhd8ed1ab_0.conda
   hash:
     md5: a9d97fe4617aba393d90ea81576b6b46
     sha256: dec2a299b39212fc311771faec9d5cd854a18f8655d04930b8d69139c9d8a546
   category: dev
   optional: true
 - name: pymdown-extensions
-  version: 10.0.1
+  version: 10.1.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     markdown: '>=3.2'
     python: '>=3.7'
     pyyaml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.0.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.1.0-pyhd8ed1ab_0.conda
   hash:
-    md5: c97339cff97ae0c82dcfd7ccf72cb3d1
-    sha256: fac9ac7e236925056e69bcdec34b219a2fa860bf9434d4391986dad6afd22859
+    md5: ab329864b9f57210f3d2f9c6cd30b921
+    sha256: 892c9409b5d3d8329c8b435d91f9075df271f06bde4ed04ec23fb19831502b02
   category: dev
   optional: true
 - name: pyopenssl
   version: 23.2.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -4050,84 +4162,28 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   category: main
   optional: false
-- name: pytest-cov
-  version: 4.1.0
-  manager: conda
-  platform: linux-aarch64
-  dependencies:
-    coverage: '>=5.2.1'
-    pytest: '>=4.6'
-    python: '>=3.7'
-    toml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
-  hash:
-    md5: 06eb685a3a0b146347a58dda979485da
-    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
-  category: dev
-  optional: true
-- name: pytest-flake8
-  version: 1.1.1
-  manager: conda
-  platform: linux-aarch64
-  dependencies:
-    flake8: '>=4.0'
-    pytest: '>=7.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
-  hash:
-    md5: d717971066d534fd18dfe80a79146f38
-    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
-  category: dev
-  optional: true
-- name: pytest-timeout
-  version: 2.1.0
-  manager: conda
-  platform: linux-aarch64
-  dependencies:
-    pytest: '>=5.0.0'
-    python: '>=3.6'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
-  hash:
-    md5: 2b23b25991cbc6886b95942704fc5c62
-    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
-  category: dev
-  optional: true
-- name: pytest-xdist
-  version: 3.3.1
-  manager: conda
-  platform: linux-aarch64
-  dependencies:
-    execnet: '>=1.1'
-    pytest: '>=6.2.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
-  hash:
-    md5: 816073bb54ef59f33f0f26c14f88311b
-    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
-  category: dev
-  optional: true
 - name: readme_renderer
-  version: '37.3'
+  version: '40.0'
   manager: conda
   platform: linux-aarch64
   dependencies:
     bleach: '>=2.1.0'
     cmarkgfm: '>=0.8.0'
     docutils: '>=0.13.1'
     pygments: '>=2.5.1'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 82e8ab317fe8f1d2a944688438dce868
-    sha256: 3f6d5ffe4c07bbddfcc7d108d01a1cbd78d38e9b860de46f16ca617bd4f42cd1
+    md5: 9ba2b509f6fe88364512caa9089ea886
+    sha256: 37a3b585fab825fb737ff0b2c1d2b9446ffb27b0ec42529ef7102558cafe331f
   category: dev
   optional: true
 - name: secretstorage
   version: 3.3.3
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -4139,60 +4195,60 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/secretstorage-3.3.3-py311hfecb2dc_1.tar.bz2
   hash:
     md5: 0884db687814f9c4e60ef52039cf50c5
     sha256: 32c4ff6632485b55fbc3ae7e5b5ea961df867f3969a508feddc2bb9eba9c42d6
   category: main
   optional: false
 - name: virtualenv
-  version: 20.23.0
+  version: 20.24.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     distlib: <1,>=0.3.6
-    filelock: <4,>=3.11
-    platformdirs: <4,>=3.2
+    filelock: <4,>=3.12
+    platformdirs: <4,>=3.5.1
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.0-pyhd8ed1ab_0.conda
   hash:
-    md5: a920e114c4c2ced2280e266da65ab5e6
-    sha256: 13d667887ea08b6d1fe2eb09d2d737f9af7343735d3bfa5ffaa3f67eec8eaff7
+    md5: 1b4a286252e336bef9ef8fa589eefdd1
+    sha256: d8b3a1badec92e81aed61d24fa33268ead568eae02372333d95bc38fce296330
   category: main
   optional: false
 - name: keyring
-  version: 23.13.1
+  version: 24.2.0
   manager: conda
   platform: linux-aarch64
   dependencies:
     importlib_metadata: '>=4.11.4'
     jaraco.classes: ''
     jeepney: '>=0.4.2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     secretstorage: '>=3.2'
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/keyring-23.13.1-py311hec3470c_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/keyring-24.2.0-py311hec3470c_0.conda
   hash:
-    md5: 0a88f265618ad87b8aafe9c4dc678a3a
-    sha256: fa9b8531c2d940c0fd21b2803ad3dee86a5ff8a9706d1302581b4d08064485a8
+    md5: a1797691fb1f85ab019560400c478d7a
+    sha256: a3fd7543a77f221d82a7db357c40299d3c7070b6ee1cf1e3c86355b7f5b7ebc2
   category: main
   optional: false
 - name: pre-commit
-  version: 3.3.2
+  version: 3.3.3
   manager: conda
   platform: linux-aarch64
   dependencies:
     cfgv: '>=2.0.0'
     identify: '>=1.0.0'
     nodeenv: '>=0.11.1'
     python: '>=3.8'
     pyyaml: '>=5.1'
     virtualenv: '>=20.10.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.2-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.3-pyha770c72_0.conda
   hash:
-    md5: dbb0111b18ea5c9983fb8db0aef6000b
-    sha256: a55d8a19bb00c2c5bf8a074c94d5ac1ffed8d63c53c9df4cee76f3764ad7a304
+    md5: dd64a0e440754ed97610b3e6b502b6b1
+    sha256: 3df1434057ce827d88cdd84578732030b3d4b5a0bc6c58bff12b7f8001c1be5b
   category: dev
   optional: true
 - name: urllib3
   version: 1.26.15
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -4236,29 +4292,29 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda
   hash:
     md5: 9f0b2eb5f5dd2cec36d5342a80adfec0
     sha256: 894e2f4c59221b9633c60281a17fefe09ba0bf5d996992cebeb504d0585dd0dd
   category: main
   optional: false
 - name: docker-py
-  version: 6.1.0
+  version: 6.1.3
   manager: conda
   platform: linux-aarch64
   dependencies:
     packaging: '>=14.0'
     paramiko: '>=2.4.3'
     python: '>=3.7'
     pywin32-on-windows: ''
     requests: '>=2.26.0'
     urllib3: '>=1.26.0'
     websocket-client: '>=0.32.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.3-pyhd8ed1ab_0.conda
   hash:
-    md5: 543336c6aa9516cfb29c51d5c162b177
-    sha256: 5e01e15e20ee573c99b530633a0d5c71fd515e4ac6d2f5f5f57baece8b915cc3
+    md5: c95d23d8bae7e21491868cc7772d7c73
+    sha256: 7c3031602e92fd7682302ef98a45bdf7374d48a849cdd3900b7c68a32d162177
   category: dev
   optional: true
 - name: doctr
   version: 1.9.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -4285,32 +4341,32 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: c99ae3abf501990769047b4b40a98f17
     sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
   category: main
   optional: false
 - name: mkdocs-material
-  version: 9.1.15
+  version: 9.1.18
   manager: conda
   platform: linux-aarch64
   dependencies:
     colorama: '>=0.4'
     jinja2: '>=3.0'
     markdown: '>=3.2'
     mkdocs: '>=1.4.2'
     mkdocs-material-extensions: '>=1.1'
     pygments: '>=2.14'
-    pymdown-extensions: '>=9.9'
+    pymdown-extensions: '>=9.9.1'
     python: '>=3.7'
     regex: '>=2022.4.24'
     requests: '>=2.26'
-  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.15-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.18-pyhd8ed1ab_0.conda
   hash:
-    md5: 11383355f8c54b2a89ffd689c0cc5276
-    sha256: 445cacaa27a2c96fdb852b0d0d281e196fba89b6879ac4dd1988fa75270af04a
+    md5: 8fca138f1f46db013daf43d342169612
+    sha256: b23684c0774d7c9a08e265f97c0411d8d1737f27b94e484d37bf161c2ca52f4b
   category: dev
   optional: true
 - name: requests-toolbelt
   version: 1.0.0
   manager: conda
   platform: linux-aarch64
   dependencies:
@@ -4376,22 +4432,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda
   hash:
     md5: b704e4b79ba0d887c4870b7b09d6a4df
     sha256: a06c9c788de81da3a3868ac56781680cc1fc50a0b5a545d4453818975c141b2c
   category: main
   optional: false
 - name: libcxx
-  version: 16.0.5
+  version: 16.0.6
   manager: conda
   platform: osx-64
   dependencies: {}
-  url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.5-hd57cbcb_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
   hash:
-    md5: d34eed0a4fb993f0d934db6394ba23ef
-    sha256: 1661ffd4e62593aed05da9ee1f7b1905711d8374a25b187e61cb7e55823440df
+    md5: 7d6972792161077908b62971802f289a
+    sha256: 9063271847cf05f3a6cc6cae3e7f0ced032ab5f3a3c9d3f943f876f39c5c2549
   category: main
   optional: false
 - name: libexpat
   version: 2.5.0
   manager: conda
   platform: osx-64
   dependencies: {}
@@ -4424,18 +4480,18 @@
   category: dev
   optional: true
 - name: libzlib
   version: 1.2.13
   manager: conda
   platform: osx-64
   dependencies: {}
-  url: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
   hash:
-    md5: 35eb3fce8d51ed3c1fd4122bad48250b
-    sha256: 0d954350222cc12666a1f4852dbc9bcf4904d8e467d29505f2b04ded6518f890
+    md5: 4a3ad23f6e16f99c04e166767193d700
+    sha256: fc58ad7f47ffea10df1f2165369978fba0a1cc32594aad778f5eec725f334867
   category: main
   optional: false
 - name: ncurses
   version: '6.4'
   manager: conda
   platform: osx-64
   dependencies: {}
@@ -4534,34 +4590,34 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2
   hash:
     md5: 8e9480d9c47061db2ed1b4ecce519a7f
     sha256: 331aa1137a264fd9cc905f04f09a161c801fe504b93da08b4e6697bd7c9ae6a6
   category: main
   optional: false
 - name: python
-  version: 3.11.3
+  version: 3.11.4
   manager: conda
   platform: osx-64
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     libexpat: '>=2.5.0,<3.0a0'
     libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    ncurses: '>=6.4,<7.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     readline: '>=8.2,<9.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     xz: '>=5.2.6,<6.0a0'
     pip: ''
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.11.3-h99528f9_0_cpython.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda
   hash:
-    md5: c3291f9411424fc587d53a2ea57fb075
-    sha256: 576781d2c245e0d5cc9f896cd9ab195d2c4e8175f0162fbb616b7a1e6c11087a
+    md5: e40b3075f85db0184d5f61d17c580ef7
+    sha256: d2c00c7b1a616ad309afd864db6a7be33935710a68a7572509526495346655dc
   category: main
   optional: false
 - name: appdirs
   version: 1.4.4
   manager: conda
   platform: osx-64
   dependencies:
@@ -4605,36 +4661,36 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: ebb5f5f7dc4f1a3780ef7ea7738db08c
     sha256: fbc03537a27ef756162c49b1d0608bf7ab12fa5e38ceb8563d6f4859e835ac5c
   category: dev
   optional: true
 - name: charset-normalizer
-  version: 3.1.0
+  version: 3.2.0
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   category: main
   optional: false
 - name: click
-  version: 8.1.3
+  version: 8.1.5
   manager: conda
   platform: osx-64
   dependencies:
     __unix: ''
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.5-unix_pyh707e725_0.conda
   hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+    md5: 4f63f3e01a26e7058eabfa5f984cd6f3
+    sha256: fa46a7053309ff3f4b90b9c32b3c2a7353e3cf1e9807c08e75aed480630848b7
   category: main
   optional: false
 - name: colorama
   version: 0.4.6
   manager: conda
   platform: osx-64
   dependencies:
@@ -4691,47 +4747,47 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda
   hash:
     md5: 0536cbe889e20101b7f8e6d6b1dbcbf4
     sha256: d812133349ab80a0114235088d6cc6c2b93ce24f7507f3295d770a5852415aa3
   category: dev
   optional: true
 - name: exceptiongroup
-  version: 1.1.1
+  version: 1.1.2
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   category: dev
   optional: true
 - name: execnet
-  version: 1.9.0
+  version: 2.0.2
   manager: conda
   platform: osx-64
   dependencies:
-    python: 2.7|>=3.5
-  url: https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/execnet-2.0.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 0e521f7a5e60d508b121d38b04874fb2
-    sha256: 1900bbc1764d01405e55be2e369d1b830fb435eb0f27c57033372c60f34c675c
+    md5: 67de0d8241e1060a479e3c37793e26f9
+    sha256: 88ea68a360198af39368beecf057af6b31f0ae38071b2bdb2aa961b6ae5427c0
   category: dev
   optional: true
 - name: filelock
-  version: 3.12.1
+  version: 3.12.2
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1f262528bc0ca9d410b98c02d09de3ac
-    sha256: dbb815b1f9c893cdf9a17360148509c439ed83e23128eb6d0be2a9459371c0f2
+    md5: 53522ec72e6adae42bd373ef58357230
+    sha256: 1cbae9f05860f2e566e2977f14dfcd5494beb22c028b0a853ade4ec381d9de71
   category: main
   optional: false
 - name: flaky
   version: 3.7.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -4947,23 +5003,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
   hash:
     md5: be1e9f1c65a1ed0f2ae9352fec99db64
     sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
   category: main
   optional: false
 - name: pluggy
-  version: 1.0.0
+  version: 1.2.0
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   category: dev
   optional: true
 - name: psutil
   version: 5.9.5
   manager: conda
   platform: osx-64
   dependencies:
@@ -5110,23 +5166,23 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py311h5547dcb_1.conda
   hash:
     md5: fdae97fc41b9e4aa53d644cca8ba6c54
     sha256: 2f520ea162e5316a8b44b2450517ef0e70ce2fc1934d7c73cd2c703e7d268249
   category: main
   optional: false
 - name: setuptools
-  version: 67.7.2
+  version: 68.0.0
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 3b68bc43ec6baa48f7354a446267eefe
-    sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
+    md5: 5a7739d0f57ee64133c9d32e6507c46d
+    sha256: 083a0913f5b56644051f31ac40b4eeea762a88c00aa12437817191b85a753cec
   category: main
   optional: false
 - name: six
   version: 1.16.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5194,23 +5250,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 92facfec94bc02d6ccf42e7173831a36
     sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
   category: main
   optional: false
 - name: typing_extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   category: main
   optional: false
 - name: webencodings
   version: 0.5.1
   manager: conda
   platform: osx-64
   dependencies:
@@ -5218,23 +5274,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   category: main
   optional: false
 - name: websocket-client
-  version: 1.5.3
+  version: 1.6.1
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.3-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   hash:
-    md5: 9beb712a1de20fea4e339a2d62851564
-    sha256: 5176f7157b3152535e11c360b089d45d7eaf4c6c0e2116952138ab2ae195419f
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   category: dev
   optional: true
 - name: wheel
   version: 0.40.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5255,38 +5311,38 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/wrapt-1.15.0-py311h5547dcb_0.conda
   hash:
     md5: 0f4705844b199f9c5ca4e227e35bdd5d
     sha256: 53292bd1cea711c4d34be2f62ae0cb673e639aced8072d5ff0507d125ea3f3c3
   category: dev
   optional: true
 - name: zipp
-  version: 3.15.0
+  version: 3.16.2
   manager: conda
   platform: osx-64
   dependencies:
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   category: main
   optional: false
 - name: astroid
-  version: 2.15.5
+  version: 2.15.6
   manager: conda
   platform: osx-64
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     wrapt: <2,>=1.14
-  url: https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.5-py311h6eed73b_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.6-py311h6eed73b_0.conda
   hash:
-    md5: 72fc260525c8fe2372466697996ce9c9
-    sha256: f33bfe89813d8a041e49a175fed8773b5ac6e7c2125a166e95d5e279c1e4aede
+    md5: 914770ec2b9e7ac8a57a023b743aadc6
+    sha256: 21a5b195d39ac6bb433bca5c90e60af04ff6bca764ba26219372c73756ae86ef
   category: dev
   optional: true
 - name: bleach
   version: 6.0.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5396,24 +5452,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
   hash:
     md5: b2355343d6315c892543200231d7154a
     sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
   category: main
   optional: false
 - name: importlib-metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
   hash:
-    md5: f91a5d5175fb7ff2a91952ec7da59cb9
-    sha256: 33d49065756a73fbb92277c756fa00a41891408528eb90ae05ff3367a401ae6e
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   category: main
   optional: false
 - name: isort
   version: 5.12.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5422,24 +5478,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/isort-5.12.0-pyhd8ed1ab_1.conda
   hash:
     md5: 07ed3421bad60867234c7a9282ea39d4
     sha256: d34a62e33ac7acc8fd3167ceb0e2aee4e7974b94de263f52d752716429d95bcb
   category: dev
   optional: true
 - name: jaraco.classes
-  version: 3.2.3
+  version: 3.3.0
   manager: conda
   platform: osx-64
   dependencies:
     more-itertools: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
   category: main
   optional: false
 - name: jinja2
   version: 3.1.2
   manager: conda
   platform: osx-64
   dependencies:
@@ -5448,42 +5504,41 @@
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
   category: main
   optional: false
 - name: markdown-it-py
-  version: 2.2.0
+  version: 3.0.0
   manager: conda
   platform: osx-64
   dependencies:
     mdurl: '>=0.1,<1'
-    python: '>=3.7'
-    typing_extensions: '>=3.7.4'
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: b2928a6c6d52d7e3562b4a59c3214e3a
-    sha256: 65ed439862c1851463f03a9bc5109992ce3e3e025e9a2d76d13ca19f576eee9f
+    md5: 93a8e71256479c62074356ef6ebf501b
+    sha256: c041b0eaf7a6af3344d5dd452815cdc148d6284fec25a4fa3f4263b3a021e962
   category: dev
   optional: true
 - name: mypy
-  version: 1.3.0
+  version: 1.4.1
   manager: conda
   platform: osx-64
   dependencies:
     mypy_extensions: '>=0.4.3'
     psutil: '>=4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     tomli: '>=1.1.0'
     typing_extensions: '>=3.10'
-  url: https://conda.anaconda.org/conda-forge/osx-64/mypy-1.3.0-py311h2725bcf_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/mypy-1.4.1-py311h2725bcf_0.conda
   hash:
-    md5: 6fec4a3d2e20813fd64547c45085485f
-    sha256: da19009d6ec196ec4c7791f0ac58bc68f3e11e55cdc8d3d06daf1573419ae0ae
+    md5: a29b75d2d8ddd4a6208ba8e6548e661f
+    sha256: cd4c55fa0ad4ae2cd2ace3f9f4c3b5680c640cef4eb837ab81967a9dc052dba6
   category: dev
   optional: true
 - name: nodeenv
   version: 1.8.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5492,25 +5547,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
   hash:
     md5: 2a75b296096adabbabadd5e9782e5fcc
     sha256: 1320306234552717149f36f825ddc7e27ea295f24829e9db4cc6ceaff0b032bd
   category: dev
   optional: true
 - name: pip
-  version: 23.1.2
+  version: '23.2'
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
     setuptools: ''
     wheel: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7288da0d36821349cf1126e8670292df
-    sha256: 4fe1f47f6eac5b2635a622b6f985640bf835843c1d8d7ccbbae0f7d27cadec92
+    md5: fb90dfe13ce16c0a3374e3d34e3291c5
+    sha256: 31e71fc25dbc411c1595661c8eb2c2491e71895ce6954ea2d0e9a585d39eed57
   category: dev
   optional: true
 - name: pyproject_hooks
   version: 1.0.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5518,14 +5573,32 @@
     tomli: '>=1.1.0'
   url: https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda
   hash:
     md5: 21de50391d584eb7f4441b9de1ad773f
     sha256: 016340837fcfef57b351febcbe855eedf0c1f0ecfc910ed48c7fbd20535f9847
   category: dev
   optional: true
+- name: pytest
+  version: 7.4.0
+  manager: conda
+  platform: osx-64
+  dependencies:
+    colorama: ''
+    exceptiongroup: '>=1.0.0rc8'
+    iniconfig: ''
+    packaging: ''
+    pluggy: '>=0.12,<2.0'
+    python: '>=3.7'
+    tomli: '>=1.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3cfe9b9e958e7238a386933c75d190db
+    sha256: 52b2eb4e8d0380d92d45643d0c9706725e691ce8404dab4c2db4aaf58e48a23c
+  category: dev
+  optional: true
 - name: python-dateutil
   version: 2.8.2
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.6'
     six: '>=1.5'
@@ -5545,38 +5618,38 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 626ed9060ddeb681ddc42bcad89156ab
     sha256: 900319483135730d9836855a807822f0500b1a239520749103e9ef9b7ba9f246
   category: dev
   optional: true
 - name: ruamel.yaml
-  version: 0.17.31
+  version: 0.17.32
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     ruamel.yaml.clib: '>=0.1.2'
     setuptools: ''
-  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.31-py311h2725bcf_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py311h2725bcf_0.conda
   hash:
-    md5: a81b5091605ed21fb00f03a110c14cf8
-    sha256: f9e487873897fa6523c6d7377c492f2eb17b07f96dca637d895d8054277137d1
+    md5: c5c5f7cf4ca556cfdb605e05cfbc8bec
+    sha256: 32598264288373706a9b2b38066b74e23d82359b22e726e2341a3622d8eab73f
   category: main
   optional: false
 - name: typing-extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: osx-64
   dependencies:
-    typing_extensions: 4.6.3
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
+    typing_extensions: 4.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   category: main
   optional: false
 - name: watchdog
   version: 3.0.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5585,14 +5658,27 @@
     pyyaml: '>=3.10'
   url: https://conda.anaconda.org/conda-forge/osx-64/watchdog-3.0.0-py311h6fddac2_0.conda
   hash:
     md5: e7f600fb722f84d31d8df250f6ed11fc
     sha256: 2a021fd2dc13a02c22e81b5187b5c5184fd7c04f69e2e551a1fe89ff5254a1fd
   category: dev
   optional: true
+- name: annotated-types
+  version: 0.5.0
+  manager: conda
+  platform: osx-64
+  dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  category: main
+  optional: false
 - name: bcrypt
   version: 3.2.2
   manager: conda
   platform: osx-64
   dependencies:
     cffi: '>=1.1'
     pip: ''
@@ -5630,26 +5716,26 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/cmarkgfm-0.8.0-py311h5547dcb_2.tar.bz2
   hash:
     md5: 69cd422f24f98fb4f8a9a896798bff06
     sha256: d102d79eb8a370f3c69969e74257befa59c46040b74d715583d1676319f67f90
   category: dev
   optional: true
 - name: cryptography
-  version: 41.0.1
+  version: 41.0.2
   manager: conda
   platform: osx-64
   dependencies:
     cffi: '>=1.12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py311h892b619_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.2-py311h892b619_0.conda
   hash:
-    md5: d1e57a1ae104a8d97fd68c4d61c26323
-    sha256: bc51bff6253a62c4705be526d1ca36bf82a0cd2eeb05a4a4abc9e420d45b26e9
+    md5: f3975c6d2c0406f204760ac434e3b785
+    sha256: 3fa286690f39b0dc3f17f673f8cffa039ec36f8397e6b6e19183a085314e8669
   category: main
   optional: false
 - name: flake8-builtins
   version: 2.1.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5697,37 +5783,37 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   category: dev
   optional: true
 - name: gitpython
-  version: 3.1.31
+  version: 3.1.32
   manager: conda
   platform: osx-64
   dependencies:
     gitdb: '>=4.0.1,<5'
     python: '>=3.7'
     typing_extensions: '>=3.7.4.3'
-  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda
   hash:
-    md5: f6e6b482110246a81c3f03e81c68752d
-    sha256: 77c531def610089bc190508fcf304cf96c085c5fe977ab8f7d7c1641769592ac
+    md5: 5809a12901d57388444c3293c975d0bb
+    sha256: 07008a94189e570fcabe003b99bd50b8263f60c824f36f81a8819bb7cf7eab1b
   category: main
   optional: false
 - name: importlib_metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: osx-64
   dependencies:
-    importlib-metadata: '>=6.6.0,<6.6.1.0a0'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
   hash:
-    md5: 3cbc9615f10a3d471532b83e4250b971
-    sha256: 5de35d3c019d8a36e0a0deeb04a62689837bd68234a0a73a3355b860b442eca4
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   category: main
   optional: false
 - name: markdown
   version: 3.3.7
   manager: conda
   platform: osx-64
   dependencies:
@@ -5736,38 +5822,38 @@
   url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.3.7-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 0a0bed31742342688a8570b3b8a50f36
     sha256: 4af5d3f376295753d787be5013900ebca572bd8f30d59e34fbae512ec414eb5e
   category: dev
   optional: true
 - name: platformdirs
-  version: 3.5.1
+  version: 3.8.1
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.7'
-    typing-extensions: '>=4.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda
+    typing-extensions: '>=4.6.3'
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda
   hash:
-    md5: e2be672aece1f060adf7154f76531a35
-    sha256: d7845c01a9ee5a224cc9242782befed7d12dc6aac1103650ec87917b20f3579e
+    md5: e76070baecfaca6ecdb5fbd5af7c9309
+    sha256: b5012d6fd30f2462b6ca595539cfdae9aaf61b3b7a56e51ab94aef0fd9efcd3d
   category: main
   optional: false
-- name: pydantic
-  version: 1.10.9
+- name: pydantic-core
+  version: 2.3.0
   manager: conda
   platform: osx-64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-    typing-extensions: '>=4.2.0'
-  url: https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.9-py311h2725bcf_0.conda
+    typing-extensions: '>=4.6.0'
+  url: https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.3.0-py311h299eb51_0.conda
   hash:
-    md5: c6e744d388e4de3c75aa3b00b102503c
-    sha256: 9ac15182a35ecb251b265f707f4fb444631b34ae2b40713c739d4410e2a4e817
+    md5: 4d627a3cb4e813bcc47256c9a01bf90f
+    sha256: 82c5d31f662a0509f28d2b2d0cbb1a30dd84300bf8de506683124fa63e49515e
   category: main
   optional: false
 - name: pynacl
   version: 1.5.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5778,31 +5864,68 @@
     six: ''
   url: https://conda.anaconda.org/conda-forge/osx-64/pynacl-1.5.0-py311h5547dcb_2.tar.bz2
   hash:
     md5: 1a11896b683621c56cd646820124585c
     sha256: ba2a29c21fcc12af9598bc5f96c069c172c25b343a4236f112eeaf790ac16c0e
   category: dev
   optional: true
-- name: pytest
-  version: 7.3.1
+- name: pytest-cov
+  version: 4.1.0
   manager: conda
   platform: osx-64
   dependencies:
-    colorama: ''
-    exceptiongroup: ''
-    importlib-metadata: '>=0.12'
-    iniconfig: ''
-    packaging: ''
-    pluggy: '>=0.12,<2.0'
-    python: '>=3.8'
-    tomli: '>=1.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.1-pyhd8ed1ab_0.conda
+    coverage: '>=5.2.1'
+    pytest: '>=4.6'
+    python: '>=3.7'
+    toml: ''
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 06eb685a3a0b146347a58dda979485da
+    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
+  category: dev
+  optional: true
+- name: pytest-flake8
+  version: 1.1.1
+  manager: conda
+  platform: osx-64
+  dependencies:
+    flake8: '>=4.0'
+    pytest: '>=7.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
   hash:
-    md5: 547c7de697ec99b494a28ddde185b5a4
-    sha256: 42f89db577266b9dc195d09189b92f3af3354fb50c98b1f996c580322dffa8b5
+    md5: d717971066d534fd18dfe80a79146f38
+    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
+  category: dev
+  optional: true
+- name: pytest-timeout
+  version: 2.1.0
+  manager: conda
+  platform: osx-64
+  dependencies:
+    pytest: '>=5.0.0'
+    python: '>=3.6'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 2b23b25991cbc6886b95942704fc5c62
+    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
+  category: dev
+  optional: true
+- name: pytest-xdist
+  version: 3.3.1
+  manager: conda
+  platform: osx-64
+  dependencies:
+    execnet: '>=1.1'
+    pytest: '>=6.2.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 816073bb54ef59f33f0f26c14f88311b
+    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
   category: dev
   optional: true
 - name: python-build
   version: 0.10.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -5815,26 +5938,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda
   hash:
     md5: 0ab47ce574f6a8bcb9f2076436e7fedb
     sha256: 4c2cd519c85aa8b8e584723ca5f452aa5941d18374470adebfe73bf30fd27573
   category: dev
   optional: true
 - name: rich
-  version: 13.4.1
+  version: 13.4.2
   manager: conda
   platform: osx-64
   dependencies:
-    markdown-it-py: '>=2.2.0,<3.0.0'
+    markdown-it-py: '>=2.2.0'
     pygments: '>=2.13.0,<3.0.0'
     python: '>=3.7.0'
     typing_extensions: '>=4.0.0,<5.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: c3bcbe0d086f15e5918568d3865e4dbf
-    sha256: 312f2628e06a591096a851bf678833fe670ecb16e9b15517ce8e03d7c9d9e600
+    md5: f993baacc175e83fafd6b846e9c4c8a2
+    sha256: d0f6506b0bf1f5563b6b42cf018002b7007bd49e62ad4a178c2a50bf3a7fe45f
   category: dev
   optional: true
 - name: ukkonen
   version: 1.0.1
   manager: conda
   platform: osx-64
   dependencies:
@@ -5845,29 +5968,29 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py311hd2070f0_3.tar.bz2
   hash:
     md5: cc38bdf32e077ea689d6ca9aa94b8a76
     sha256: c82d22ae794e6f956989640027023a096087bec40ccb19c92b50e850291f6ac4
   category: dev
   optional: true
 - name: black
-  version: 23.3.0
+  version: 23.7.0
   manager: conda
   platform: osx-64
   dependencies:
     click: '>=8.0.0'
     mypy_extensions: '>=0.4.3'
     packaging: '>=22.0'
     pathspec: '>=0.9'
     platformdirs: '>=2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/osx-64/black-23.3.0-py311h6eed73b_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/black-23.7.0-py311h6eed73b_1.conda
   hash:
-    md5: 2783c68e84c0573fece0880488c7c001
-    sha256: 78b007b394be2e0ddd42224970be1b212639a8941fee0e7d724986155e517e24
+    md5: 476e9030b804b5428b52e33e3f7bbecf
+    sha256: 4fdcc09a0630cb949e8e91957fb70d4203ce5bd55d66fb4cf4885bb3bbc1607f
   category: dev
   optional: true
 - name: check-manifest
   version: '0.49'
   manager: conda
   platform: osx-64
   dependencies:
@@ -5878,25 +6001,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/check-manifest-0.49-pyhd8ed1ab_0.conda
   hash:
     md5: 65b3059f2f0807433ee3c2673a886123
     sha256: f8d03ad89aacf5278b74f73f6720588cfa41481c959206147fd58d54f7974487
   category: dev
   optional: true
 - name: flake8-comprehensions
-  version: 3.12.0
+  version: 3.13.0
   manager: conda
   platform: osx-64
   dependencies:
     flake8: '>=3.0,!=3.2.0'
     importlib_metadata: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.12.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.13.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 18c6bc2bb3cd3950029569362cca2e33
-    sha256: c825986cf7a2f617b61373e421d74e9383696d48def52e4619af2bea1b747e8d
+    md5: f1fca1448e90eaa8fc5a3676813b4c0c
+    sha256: 3fd60ba3cfedd29fcceea147141aea74763483e3491e32afdeaa4357cf8eb92e
   category: dev
   optional: true
 - name: identify
   version: 2.5.24
   manager: conda
   platform: osx-64
   dependencies:
@@ -5905,26 +6028,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.24-pyhd8ed1ab_0.conda
   hash:
     md5: a4085ab0562d5081a9333435837b538a
     sha256: 4027103c59220a68b41aed056d2ce89d46e4971033d259293ca07198a8a81fdc
   category: dev
   optional: true
 - name: keyring
-  version: 23.13.1
+  version: 24.2.0
   manager: conda
   platform: osx-64
   dependencies:
     importlib_metadata: '>=4.11.4'
     jaraco.classes: ''
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py311h6eed73b_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/keyring-24.2.0-py311h6eed73b_0.conda
   hash:
-    md5: ae2618c59c8f3481aa7014de862c6d57
-    sha256: e18ee3cda4eecce96526f9c4df5b1f17ee3e0edfd09524583b678310507336ec
+    md5: 8ba03d96e54958cd02110dc032d0bda2
+    sha256: 2ba79400b7ab0812130b517ba65e0a5ef09a25944480904bd4c8c7da01d0aed4
   category: main
   optional: false
 - name: mkdocs
   version: 1.4.3
   manager: conda
   platform: osx-64
   dependencies:
@@ -5972,14 +6095,30 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/paramiko-3.2.0-pyhd8ed1ab_0.conda
   hash:
     md5: f212c7eb95e909df4795297f73690993
     sha256: e425a03e5e2ef2ec5a78711686c59cfceeeeec3a98165fbc7d186bd6a5cb78de
   category: dev
   optional: true
+- name: pydantic
+  version: 2.0.3
+  manager: conda
+  platform: osx-64
+  dependencies:
+    annotated-types: '>=0.4.0'
+    pydantic-core: 2.3.0
+    python: '>=3.11,<3.12.0a0'
+    python_abi: 3.11.*
+    typing-extensions: '>=4.6.1'
+  url: https://conda.anaconda.org/conda-forge/osx-64/pydantic-2.0.3-py311h2725bcf_0.conda
+  hash:
+    md5: 127a35a7eab49a7df20b96431a24ca41
+    sha256: bd7718391b0949037c82eae8324d3f139c51b474c71881677d612b25779adaf4
+  category: main
+  optional: false
 - name: pylint
   version: 2.17.4
   manager: conda
   platform: osx-64
   dependencies:
     astroid: '>=2.15.4,<2.17.0-dev0'
     colorama: '>=0.4.5'
@@ -5994,25 +6133,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pylint-2.17.4-pyhd8ed1ab_0.conda
   hash:
     md5: a9d97fe4617aba393d90ea81576b6b46
     sha256: dec2a299b39212fc311771faec9d5cd854a18f8655d04930b8d69139c9d8a546
   category: dev
   optional: true
 - name: pymdown-extensions
-  version: 10.0.1
+  version: 10.1.0
   manager: conda
   platform: osx-64
   dependencies:
     markdown: '>=3.2'
     python: '>=3.7'
     pyyaml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.0.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.1.0-pyhd8ed1ab_0.conda
   hash:
-    md5: c97339cff97ae0c82dcfd7ccf72cb3d1
-    sha256: fac9ac7e236925056e69bcdec34b219a2fa860bf9434d4391986dad6afd22859
+    md5: ab329864b9f57210f3d2f9c6cd30b921
+    sha256: 892c9409b5d3d8329c8b435d91f9075df271f06bde4ed04ec23fb19831502b02
   category: dev
   optional: true
 - name: pyopenssl
   version: 23.2.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -6020,116 +6159,60 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   category: main
   optional: false
-- name: pytest-cov
-  version: 4.1.0
-  manager: conda
-  platform: osx-64
-  dependencies:
-    coverage: '>=5.2.1'
-    pytest: '>=4.6'
-    python: '>=3.7'
-    toml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
-  hash:
-    md5: 06eb685a3a0b146347a58dda979485da
-    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
-  category: dev
-  optional: true
-- name: pytest-flake8
-  version: 1.1.1
-  manager: conda
-  platform: osx-64
-  dependencies:
-    flake8: '>=4.0'
-    pytest: '>=7.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
-  hash:
-    md5: d717971066d534fd18dfe80a79146f38
-    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
-  category: dev
-  optional: true
-- name: pytest-timeout
-  version: 2.1.0
-  manager: conda
-  platform: osx-64
-  dependencies:
-    pytest: '>=5.0.0'
-    python: '>=3.6'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
-  hash:
-    md5: 2b23b25991cbc6886b95942704fc5c62
-    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
-  category: dev
-  optional: true
-- name: pytest-xdist
-  version: 3.3.1
-  manager: conda
-  platform: osx-64
-  dependencies:
-    execnet: '>=1.1'
-    pytest: '>=6.2.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
-  hash:
-    md5: 816073bb54ef59f33f0f26c14f88311b
-    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
-  category: dev
-  optional: true
 - name: readme_renderer
-  version: '37.3'
+  version: '40.0'
   manager: conda
   platform: osx-64
   dependencies:
     bleach: '>=2.1.0'
     cmarkgfm: '>=0.8.0'
     docutils: '>=0.13.1'
     pygments: '>=2.5.1'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 82e8ab317fe8f1d2a944688438dce868
-    sha256: 3f6d5ffe4c07bbddfcc7d108d01a1cbd78d38e9b860de46f16ca617bd4f42cd1
+    md5: 9ba2b509f6fe88364512caa9089ea886
+    sha256: 37a3b585fab825fb737ff0b2c1d2b9446ffb27b0ec42529ef7102558cafe331f
   category: dev
   optional: true
 - name: virtualenv
-  version: 20.23.0
+  version: 20.24.0
   manager: conda
   platform: osx-64
   dependencies:
     distlib: <1,>=0.3.6
-    filelock: <4,>=3.11
-    platformdirs: <4,>=3.2
+    filelock: <4,>=3.12
+    platformdirs: <4,>=3.5.1
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.0-pyhd8ed1ab_0.conda
   hash:
-    md5: a920e114c4c2ced2280e266da65ab5e6
-    sha256: 13d667887ea08b6d1fe2eb09d2d737f9af7343735d3bfa5ffaa3f67eec8eaff7
+    md5: 1b4a286252e336bef9ef8fa589eefdd1
+    sha256: d8b3a1badec92e81aed61d24fa33268ead568eae02372333d95bc38fce296330
   category: main
   optional: false
 - name: pre-commit
-  version: 3.3.2
+  version: 3.3.3
   manager: conda
   platform: osx-64
   dependencies:
     cfgv: '>=2.0.0'
     identify: '>=1.0.0'
     nodeenv: '>=0.11.1'
     python: '>=3.8'
     pyyaml: '>=5.1'
     virtualenv: '>=20.10.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.2-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.3-pyha770c72_0.conda
   hash:
-    md5: dbb0111b18ea5c9983fb8db0aef6000b
-    sha256: a55d8a19bb00c2c5bf8a074c94d5ac1ffed8d63c53c9df4cee76f3764ad7a304
+    md5: dd64a0e440754ed97610b3e6b502b6b1
+    sha256: 3df1434057ce827d88cdd84578732030b3d4b5a0bc6c58bff12b7f8001c1be5b
   category: dev
   optional: true
 - name: urllib3
   version: 1.26.15
   manager: conda
   platform: osx-64
   dependencies:
@@ -6173,29 +6256,29 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda
   hash:
     md5: 9f0b2eb5f5dd2cec36d5342a80adfec0
     sha256: 894e2f4c59221b9633c60281a17fefe09ba0bf5d996992cebeb504d0585dd0dd
   category: main
   optional: false
 - name: docker-py
-  version: 6.1.0
+  version: 6.1.3
   manager: conda
   platform: osx-64
   dependencies:
     packaging: '>=14.0'
     paramiko: '>=2.4.3'
     python: '>=3.7'
     pywin32-on-windows: ''
     requests: '>=2.26.0'
     urllib3: '>=1.26.0'
     websocket-client: '>=0.32.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.3-pyhd8ed1ab_0.conda
   hash:
-    md5: 543336c6aa9516cfb29c51d5c162b177
-    sha256: 5e01e15e20ee573c99b530633a0d5c71fd515e4ac6d2f5f5f57baece8b915cc3
+    md5: c95d23d8bae7e21491868cc7772d7c73
+    sha256: 7c3031602e92fd7682302ef98a45bdf7374d48a849cdd3900b7c68a32d162177
   category: dev
   optional: true
 - name: doctr
   version: 1.9.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -6222,32 +6305,32 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: c99ae3abf501990769047b4b40a98f17
     sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
   category: main
   optional: false
 - name: mkdocs-material
-  version: 9.1.15
+  version: 9.1.18
   manager: conda
   platform: osx-64
   dependencies:
     colorama: '>=0.4'
     jinja2: '>=3.0'
     markdown: '>=3.2'
     mkdocs: '>=1.4.2'
     mkdocs-material-extensions: '>=1.1'
     pygments: '>=2.14'
-    pymdown-extensions: '>=9.9'
+    pymdown-extensions: '>=9.9.1'
     python: '>=3.7'
     regex: '>=2022.4.24'
     requests: '>=2.26'
-  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.15-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.18-pyhd8ed1ab_0.conda
   hash:
-    md5: 11383355f8c54b2a89ffd689c0cc5276
-    sha256: 445cacaa27a2c96fdb852b0d0d281e196fba89b6879ac4dd1988fa75270af04a
+    md5: 8fca138f1f46db013daf43d342169612
+    sha256: b23684c0774d7c9a08e265f97c0411d8d1737f27b94e484d37bf161c2ca52f4b
   category: dev
   optional: true
 - name: requests-toolbelt
   version: 1.0.0
   manager: conda
   platform: osx-64
   dependencies:
@@ -6313,22 +6396,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2023.5.7-hf0a4a13_0.conda
   hash:
     md5: a8387be82224743cf849fb907790b91a
     sha256: 27214b54d1cb9a92455689e20d0007a0ff9ace99b853867d53a05a04c24bdae5
   category: main
   optional: false
 - name: libcxx
-  version: 16.0.5
+  version: 16.0.6
   manager: conda
   platform: osx-arm64
   dependencies: {}
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.5-h4653b0c_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
   hash:
-    md5: d36fb4372ff02b2d1596366ee1d984bc
-    sha256: 14452e6dab03eb5260101cca926b4b96764f28726e5965067d0ba0101949e9e4
+    md5: 9d7d724faf0413bf1dbc5a85935700c8
+    sha256: 11d3fb51c14832d9e4f6d84080a375dec21ea8a3a381a1910e67ff9cedc20355
   category: main
   optional: false
 - name: libexpat
   version: 2.5.0
   manager: conda
   platform: osx-arm64
   dependencies: {}
@@ -6361,18 +6444,18 @@
   category: dev
   optional: true
 - name: libzlib
   version: 1.2.13
   manager: conda
   platform: osx-arm64
   dependencies: {}
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h03a7124_4.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
   hash:
-    md5: 780852dc54c4c07e64b276a97f89c162
-    sha256: a1bf4a1c107838fea4570a7f1750306d65d84fcf2913d4e0d30b4db785e8f223
+    md5: 1a47f5236db2e06a320ffa0392f81bd8
+    sha256: ab1c8aefa2d54322a63aaeeefe9cf877411851738616c4068e0dccc66b9c758a
   category: main
   optional: false
 - name: ncurses
   version: '6.4'
   manager: conda
   platform: osx-arm64
   dependencies: {}
@@ -6471,34 +6554,34 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.12-he1e0b03_0.tar.bz2
   hash:
     md5: 2cb3d18eac154109107f093860bd545f
     sha256: 9e43ec80045892e28233e4ca4d974e09d5837392127702fb952f3935b5e985a4
   category: main
   optional: false
 - name: python
-  version: 3.11.3
+  version: 3.11.4
   manager: conda
   platform: osx-arm64
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     libexpat: '>=2.5.0,<3.0a0'
     libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    ncurses: '>=6.4,<7.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     readline: '>=8.2,<9.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     xz: '>=5.2.6,<6.0a0'
     pip: ''
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.11.3-h1456518_0_cpython.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.11.4-h47c9636_0_cpython.conda
   hash:
-    md5: 9a215527aee438cb9926e66ea6538caa
-    sha256: 808fff7e53017753eb4fbd6e3faeb192a370cb517309fa3c104a94f505ad6fda
+    md5: b790b3cac8db7bdf2aaced9460bdbce4
+    sha256: 7865a28f7ec5c453cd8d3e7f539e02028ba5aa2aa33ccaa9915ba2654ae03ab2
   category: main
   optional: false
 - name: appdirs
   version: 1.4.4
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -6542,36 +6625,36 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: ebb5f5f7dc4f1a3780ef7ea7738db08c
     sha256: fbc03537a27ef756162c49b1d0608bf7ab12fa5e38ceb8563d6f4859e835ac5c
   category: dev
   optional: true
 - name: charset-normalizer
-  version: 3.1.0
+  version: 3.2.0
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   category: main
   optional: false
 - name: click
-  version: 8.1.3
+  version: 8.1.5
   manager: conda
   platform: osx-arm64
   dependencies:
     __unix: ''
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.5-unix_pyh707e725_0.conda
   hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+    md5: 4f63f3e01a26e7058eabfa5f984cd6f3
+    sha256: fa46a7053309ff3f4b90b9c32b3c2a7353e3cf1e9807c08e75aed480630848b7
   category: main
   optional: false
 - name: colorama
   version: 0.4.6
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -6628,47 +6711,47 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/docutils-0.20.1-py311h267d04e_0.conda
   hash:
     md5: 1d28040de4fff5330e56cbf601ad3508
     sha256: 74e5ebf3520135ae4d34089279ffa90f6f14456710fda0049ff6ad5ec7e4219a
   category: dev
   optional: true
 - name: exceptiongroup
-  version: 1.1.1
+  version: 1.1.2
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   category: dev
   optional: true
 - name: execnet
-  version: 1.9.0
+  version: 2.0.2
   manager: conda
   platform: osx-arm64
   dependencies:
-    python: 2.7|>=3.5
-  url: https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/execnet-2.0.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 0e521f7a5e60d508b121d38b04874fb2
-    sha256: 1900bbc1764d01405e55be2e369d1b830fb435eb0f27c57033372c60f34c675c
+    md5: 67de0d8241e1060a479e3c37793e26f9
+    sha256: 88ea68a360198af39368beecf057af6b31f0ae38071b2bdb2aa961b6ae5427c0
   category: dev
   optional: true
 - name: filelock
-  version: 3.12.1
+  version: 3.12.2
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1f262528bc0ca9d410b98c02d09de3ac
-    sha256: dbb815b1f9c893cdf9a17360148509c439ed83e23128eb6d0be2a9459371c0f2
+    md5: 53522ec72e6adae42bd373ef58357230
+    sha256: 1cbae9f05860f2e566e2977f14dfcd5494beb22c028b0a853ade4ec381d9de71
   category: main
   optional: false
 - name: flaky
   version: 3.7.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -6884,23 +6967,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
   hash:
     md5: be1e9f1c65a1ed0f2ae9352fec99db64
     sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
   category: main
   optional: false
 - name: pluggy
-  version: 1.0.0
+  version: 1.2.0
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   category: dev
   optional: true
 - name: psutil
   version: 5.9.5
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7047,23 +7130,23 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ruamel.yaml.clib-0.2.7-py311he2be06e_1.conda
   hash:
     md5: 693e8b069d8b9dac3900d78ae86d79e4
     sha256: 2f59d7a72c1bf793d3c5548b236e4570b443634fbca369ce5fee397d90fa76f2
   category: main
   optional: false
 - name: setuptools
-  version: 67.7.2
+  version: 68.0.0
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 3b68bc43ec6baa48f7354a446267eefe
-    sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
+    md5: 5a7739d0f57ee64133c9d32e6507c46d
+    sha256: 083a0913f5b56644051f31ac40b4eeea762a88c00aa12437817191b85a753cec
   category: main
   optional: false
 - name: six
   version: 1.16.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7131,23 +7214,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 92facfec94bc02d6ccf42e7173831a36
     sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
   category: main
   optional: false
 - name: typing_extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   category: main
   optional: false
 - name: webencodings
   version: 0.5.1
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7155,23 +7238,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   category: main
   optional: false
 - name: websocket-client
-  version: 1.5.3
+  version: 1.6.1
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.3-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   hash:
-    md5: 9beb712a1de20fea4e339a2d62851564
-    sha256: 5176f7157b3152535e11c360b089d45d7eaf4c6c0e2116952138ab2ae195419f
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   category: dev
   optional: true
 - name: wheel
   version: 0.40.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7192,38 +7275,38 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/wrapt-1.15.0-py311he2be06e_0.conda
   hash:
     md5: a86a42e2238e314d5a504102670d778c
     sha256: 5a220790c596d5198da6bf00b3ef4dbac8dcd0afbdc7ccb2c2c7e9f760a94ae1
   category: dev
   optional: true
 - name: zipp
-  version: 3.15.0
+  version: 3.16.2
   manager: conda
   platform: osx-arm64
   dependencies:
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   category: main
   optional: false
 - name: astroid
-  version: 2.15.5
+  version: 2.15.6
   manager: conda
   platform: osx-arm64
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     wrapt: <2,>=1.14
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/astroid-2.15.5-py311h267d04e_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/astroid-2.15.6-py311h267d04e_0.conda
   hash:
-    md5: 4ce48297fcade75a82df35b0d9cc8c66
-    sha256: 8389704028115abb52b346eb6eb97258c500873e37ec99317a9dbe6013a6877e
+    md5: a8a1724f1de66793d23362462078ab95
+    sha256: 3f0cd39f2f2176eb373c06b9e4ad4aa88470b1d0c510f4fa9faea8112541eaff
   category: dev
   optional: true
 - name: bleach
   version: 6.0.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7333,24 +7416,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
   hash:
     md5: b2355343d6315c892543200231d7154a
     sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
   category: main
   optional: false
 - name: importlib-metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
   hash:
-    md5: f91a5d5175fb7ff2a91952ec7da59cb9
-    sha256: 33d49065756a73fbb92277c756fa00a41891408528eb90ae05ff3367a401ae6e
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   category: main
   optional: false
 - name: isort
   version: 5.12.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7359,24 +7442,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/isort-5.12.0-pyhd8ed1ab_1.conda
   hash:
     md5: 07ed3421bad60867234c7a9282ea39d4
     sha256: d34a62e33ac7acc8fd3167ceb0e2aee4e7974b94de263f52d752716429d95bcb
   category: dev
   optional: true
 - name: jaraco.classes
-  version: 3.2.3
+  version: 3.3.0
   manager: conda
   platform: osx-arm64
   dependencies:
     more-itertools: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
   category: main
   optional: false
 - name: jinja2
   version: 3.1.2
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7385,42 +7468,41 @@
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
   category: main
   optional: false
 - name: markdown-it-py
-  version: 2.2.0
+  version: 3.0.0
   manager: conda
   platform: osx-arm64
   dependencies:
     mdurl: '>=0.1,<1'
-    python: '>=3.7'
-    typing_extensions: '>=3.7.4'
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: b2928a6c6d52d7e3562b4a59c3214e3a
-    sha256: 65ed439862c1851463f03a9bc5109992ce3e3e025e9a2d76d13ca19f576eee9f
+    md5: 93a8e71256479c62074356ef6ebf501b
+    sha256: c041b0eaf7a6af3344d5dd452815cdc148d6284fec25a4fa3f4263b3a021e962
   category: dev
   optional: true
 - name: mypy
-  version: 1.3.0
+  version: 1.4.1
   manager: conda
   platform: osx-arm64
   dependencies:
     mypy_extensions: '>=0.4.3'
     psutil: '>=4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     tomli: '>=1.1.0'
     typing_extensions: '>=3.10'
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/mypy-1.3.0-py311heffc1b2_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/mypy-1.4.1-py311heffc1b2_0.conda
   hash:
-    md5: ab7b5eb1025c4ca0d1a990840764b5c1
-    sha256: 18d481d5c7557b287c5cfd5704526215bd09d024d9edca735c6d6a805288f948
+    md5: 388c8df4d57c047bec3f17bd274843e2
+    sha256: 534eb1914c32392372c236740868bf72f769563315c3df54deef145a2924ebfa
   category: dev
   optional: true
 - name: nodeenv
   version: 1.8.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7429,25 +7511,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
   hash:
     md5: 2a75b296096adabbabadd5e9782e5fcc
     sha256: 1320306234552717149f36f825ddc7e27ea295f24829e9db4cc6ceaff0b032bd
   category: dev
   optional: true
 - name: pip
-  version: 23.1.2
+  version: '23.2'
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
     setuptools: ''
     wheel: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7288da0d36821349cf1126e8670292df
-    sha256: 4fe1f47f6eac5b2635a622b6f985640bf835843c1d8d7ccbbae0f7d27cadec92
+    md5: fb90dfe13ce16c0a3374e3d34e3291c5
+    sha256: 31e71fc25dbc411c1595661c8eb2c2491e71895ce6954ea2d0e9a585d39eed57
   category: dev
   optional: true
 - name: pyproject_hooks
   version: 1.0.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7455,14 +7537,32 @@
     tomli: '>=1.1.0'
   url: https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda
   hash:
     md5: 21de50391d584eb7f4441b9de1ad773f
     sha256: 016340837fcfef57b351febcbe855eedf0c1f0ecfc910ed48c7fbd20535f9847
   category: dev
   optional: true
+- name: pytest
+  version: 7.4.0
+  manager: conda
+  platform: osx-arm64
+  dependencies:
+    colorama: ''
+    exceptiongroup: '>=1.0.0rc8'
+    iniconfig: ''
+    packaging: ''
+    pluggy: '>=0.12,<2.0'
+    python: '>=3.7'
+    tomli: '>=1.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3cfe9b9e958e7238a386933c75d190db
+    sha256: 52b2eb4e8d0380d92d45643d0c9706725e691ce8404dab4c2db4aaf58e48a23c
+  category: dev
+  optional: true
 - name: python-dateutil
   version: 2.8.2
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.6'
     six: '>=1.5'
@@ -7482,38 +7582,38 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 626ed9060ddeb681ddc42bcad89156ab
     sha256: 900319483135730d9836855a807822f0500b1a239520749103e9ef9b7ba9f246
   category: dev
   optional: true
 - name: ruamel.yaml
-  version: 0.17.31
+  version: 0.17.32
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     ruamel.yaml.clib: '>=0.1.2'
     setuptools: ''
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/ruamel.yaml-0.17.31-py311heffc1b2_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ruamel.yaml-0.17.32-py311heffc1b2_0.conda
   hash:
-    md5: 695bb9751794cbc55edd5559c8a0e957
-    sha256: 2347e3eef99c24605efdfe504a6227ca676204b2941835d4e9f0f664b12b5ff3
+    md5: 905e130803eaa5de60e0bcfdcc623a83
+    sha256: 98a7003af9ad9265030e2b358f9dab6a7f163c6c069cf7fa81861f0ca562f366
   category: main
   optional: false
 - name: typing-extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: osx-arm64
   dependencies:
-    typing_extensions: 4.6.3
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
+    typing_extensions: 4.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   category: main
   optional: false
 - name: watchdog
   version: 3.0.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7522,14 +7622,27 @@
     pyyaml: '>=3.10'
   url: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-3.0.0-py311he2be06e_0.conda
   hash:
     md5: 60c2e70552300f9cc702b414600d2a31
     sha256: b527d26615278a95f61a61e72d116e3b0d4b9dbfc3af8eb808e4840def2dcd05
   category: dev
   optional: true
+- name: annotated-types
+  version: 0.5.0
+  manager: conda
+  platform: osx-arm64
+  dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  category: main
+  optional: false
 - name: bcrypt
   version: 3.2.2
   manager: conda
   platform: osx-arm64
   dependencies:
     cffi: '>=1.1'
     pip: ''
@@ -7567,26 +7680,26 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/cmarkgfm-0.8.0-py311he2be06e_2.tar.bz2
   hash:
     md5: 58e73f320125ea0f607cb27f0703e398
     sha256: de8527b0909164dc8cf7772daf673dc20fb3de6dcb51544632448c984bbef3e1
   category: dev
   optional: true
 - name: cryptography
-  version: 41.0.1
+  version: 41.0.2
   manager: conda
   platform: osx-arm64
   dependencies:
     cffi: '>=1.12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/cryptography-41.0.1-py311h5fb2c35_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/cryptography-41.0.2-py311h5fb2c35_0.conda
   hash:
-    md5: 9125db72046748f65e0356b2f80513fa
-    sha256: 8fac59d34c046989a25c8f12774ba1a5674b887473eeff68332e1400ea936202
+    md5: 9decab11e17627524e390b32b242dc84
+    sha256: 3154389a6f57d83a21acedaab7ccebc71275719fc7f6196a4b514673605d8c87
   category: main
   optional: false
 - name: flake8-builtins
   version: 2.1.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7634,37 +7747,37 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   category: dev
   optional: true
 - name: gitpython
-  version: 3.1.31
+  version: 3.1.32
   manager: conda
   platform: osx-arm64
   dependencies:
     gitdb: '>=4.0.1,<5'
     python: '>=3.7'
     typing_extensions: '>=3.7.4.3'
-  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda
   hash:
-    md5: f6e6b482110246a81c3f03e81c68752d
-    sha256: 77c531def610089bc190508fcf304cf96c085c5fe977ab8f7d7c1641769592ac
+    md5: 5809a12901d57388444c3293c975d0bb
+    sha256: 07008a94189e570fcabe003b99bd50b8263f60c824f36f81a8819bb7cf7eab1b
   category: main
   optional: false
 - name: importlib_metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: osx-arm64
   dependencies:
-    importlib-metadata: '>=6.6.0,<6.6.1.0a0'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
   hash:
-    md5: 3cbc9615f10a3d471532b83e4250b971
-    sha256: 5de35d3c019d8a36e0a0deeb04a62689837bd68234a0a73a3355b860b442eca4
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   category: main
   optional: false
 - name: markdown
   version: 3.3.7
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7673,38 +7786,38 @@
   url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.3.7-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 0a0bed31742342688a8570b3b8a50f36
     sha256: 4af5d3f376295753d787be5013900ebca572bd8f30d59e34fbae512ec414eb5e
   category: dev
   optional: true
 - name: platformdirs
-  version: 3.5.1
+  version: 3.8.1
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.7'
-    typing-extensions: '>=4.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda
+    typing-extensions: '>=4.6.3'
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda
   hash:
-    md5: e2be672aece1f060adf7154f76531a35
-    sha256: d7845c01a9ee5a224cc9242782befed7d12dc6aac1103650ec87917b20f3579e
+    md5: e76070baecfaca6ecdb5fbd5af7c9309
+    sha256: b5012d6fd30f2462b6ca595539cfdae9aaf61b3b7a56e51ab94aef0fd9efcd3d
   category: main
   optional: false
-- name: pydantic
-  version: 1.10.9
+- name: pydantic-core
+  version: 2.3.0
   manager: conda
   platform: osx-arm64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-    typing-extensions: '>=4.2.0'
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/pydantic-1.10.9-py311heffc1b2_0.conda
+    typing-extensions: '>=4.6.0'
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pydantic-core-2.3.0-py311h0563b04_0.conda
   hash:
-    md5: 674a19ff03be58f01999a57c3ed16e65
-    sha256: 64f7ac7527fd0b924515574d09c700792fc29341682ec44e8ec53dcf16d30d70
+    md5: 942ffe6ef2e94d96dcbf9c5befe0ac43
+    sha256: 6a8e62532b182d62741fd1b65719e6b5e8e554b137b58aad3019c5d221dd6458
   category: main
   optional: false
 - name: pynacl
   version: 1.5.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7715,31 +7828,68 @@
     six: ''
   url: https://conda.anaconda.org/conda-forge/osx-arm64/pynacl-1.5.0-py311he2be06e_2.tar.bz2
   hash:
     md5: eca1fa347f4e35aa289b802f7cb0a772
     sha256: 1dde9f3fa1ea62ac728b9c25d79cfd6b946ec064de5b2692c84d7a469a39df51
   category: dev
   optional: true
-- name: pytest
-  version: 7.3.1
+- name: pytest-cov
+  version: 4.1.0
   manager: conda
   platform: osx-arm64
   dependencies:
-    colorama: ''
-    exceptiongroup: ''
-    importlib-metadata: '>=0.12'
-    iniconfig: ''
-    packaging: ''
-    pluggy: '>=0.12,<2.0'
-    python: '>=3.8'
-    tomli: '>=1.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.1-pyhd8ed1ab_0.conda
+    coverage: '>=5.2.1'
+    pytest: '>=4.6'
+    python: '>=3.7'
+    toml: ''
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 06eb685a3a0b146347a58dda979485da
+    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
+  category: dev
+  optional: true
+- name: pytest-flake8
+  version: 1.1.1
+  manager: conda
+  platform: osx-arm64
+  dependencies:
+    flake8: '>=4.0'
+    pytest: '>=7.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
+  hash:
+    md5: d717971066d534fd18dfe80a79146f38
+    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
+  category: dev
+  optional: true
+- name: pytest-timeout
+  version: 2.1.0
+  manager: conda
+  platform: osx-arm64
+  dependencies:
+    pytest: '>=5.0.0'
+    python: '>=3.6'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
   hash:
-    md5: 547c7de697ec99b494a28ddde185b5a4
-    sha256: 42f89db577266b9dc195d09189b92f3af3354fb50c98b1f996c580322dffa8b5
+    md5: 2b23b25991cbc6886b95942704fc5c62
+    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
+  category: dev
+  optional: true
+- name: pytest-xdist
+  version: 3.3.1
+  manager: conda
+  platform: osx-arm64
+  dependencies:
+    execnet: '>=1.1'
+    pytest: '>=6.2.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 816073bb54ef59f33f0f26c14f88311b
+    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
   category: dev
   optional: true
 - name: python-build
   version: 0.10.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7752,26 +7902,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda
   hash:
     md5: 0ab47ce574f6a8bcb9f2076436e7fedb
     sha256: 4c2cd519c85aa8b8e584723ca5f452aa5941d18374470adebfe73bf30fd27573
   category: dev
   optional: true
 - name: rich
-  version: 13.4.1
+  version: 13.4.2
   manager: conda
   platform: osx-arm64
   dependencies:
-    markdown-it-py: '>=2.2.0,<3.0.0'
+    markdown-it-py: '>=2.2.0'
     pygments: '>=2.13.0,<3.0.0'
     python: '>=3.7.0'
     typing_extensions: '>=4.0.0,<5.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: c3bcbe0d086f15e5918568d3865e4dbf
-    sha256: 312f2628e06a591096a851bf678833fe670ecb16e9b15517ce8e03d7c9d9e600
+    md5: f993baacc175e83fafd6b846e9c4c8a2
+    sha256: d0f6506b0bf1f5563b6b42cf018002b7007bd49e62ad4a178c2a50bf3a7fe45f
   category: dev
   optional: true
 - name: ukkonen
   version: 1.0.1
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7782,29 +7932,29 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ukkonen-1.0.1-py311hd6ee22a_3.tar.bz2
   hash:
     md5: 1ec575f5b11dab96ae76895d39d26730
     sha256: 967412b3b4b6cf61485eba4b54e6236d77b4cdfe9b2e183b18d2a90d5e4def3b
   category: dev
   optional: true
 - name: black
-  version: 23.3.0
+  version: 23.7.0
   manager: conda
   platform: osx-arm64
   dependencies:
     click: '>=8.0.0'
     mypy_extensions: '>=0.4.3'
     packaging: '>=22.0'
     pathspec: '>=0.9'
     platformdirs: '>=2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/black-23.3.0-py311h267d04e_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/black-23.7.0-py311h267d04e_1.conda
   hash:
-    md5: 6df8788f081abb97d20ffa83de27d029
-    sha256: 6968e8bcc232a32cd34934d14ada2a9a2549db7f8276ba9709eb16595e5545fd
+    md5: 55c4246206ef4b4e910d052ebf15edac
+    sha256: 8854ff7a5546e915bae9c6cf4ec7d341b73eb5f1f9fd94b49c40769289b2440b
   category: dev
   optional: true
 - name: check-manifest
   version: '0.49'
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7815,25 +7965,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/check-manifest-0.49-pyhd8ed1ab_0.conda
   hash:
     md5: 65b3059f2f0807433ee3c2673a886123
     sha256: f8d03ad89aacf5278b74f73f6720588cfa41481c959206147fd58d54f7974487
   category: dev
   optional: true
 - name: flake8-comprehensions
-  version: 3.12.0
+  version: 3.13.0
   manager: conda
   platform: osx-arm64
   dependencies:
     flake8: '>=3.0,!=3.2.0'
     importlib_metadata: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.12.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.13.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 18c6bc2bb3cd3950029569362cca2e33
-    sha256: c825986cf7a2f617b61373e421d74e9383696d48def52e4619af2bea1b747e8d
+    md5: f1fca1448e90eaa8fc5a3676813b4c0c
+    sha256: 3fd60ba3cfedd29fcceea147141aea74763483e3491e32afdeaa4357cf8eb92e
   category: dev
   optional: true
 - name: identify
   version: 2.5.24
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7842,26 +7992,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.24-pyhd8ed1ab_0.conda
   hash:
     md5: a4085ab0562d5081a9333435837b538a
     sha256: 4027103c59220a68b41aed056d2ce89d46e4971033d259293ca07198a8a81fdc
   category: dev
   optional: true
 - name: keyring
-  version: 23.13.1
+  version: 24.2.0
   manager: conda
   platform: osx-arm64
   dependencies:
     importlib_metadata: '>=4.11.4'
     jaraco.classes: ''
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/keyring-23.13.1-py311h267d04e_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/keyring-24.2.0-py311h267d04e_0.conda
   hash:
-    md5: 5e309e7f2ccc2db9808c071e9b8b0ed1
-    sha256: 049354bc5b34428c621fdbe96809e4030346ce57cd548c9b9819a83a066e1fd0
+    md5: 750d8502144296ed68c9f7589735c25d
+    sha256: 46ef6b8097aa21ba38f0d8c0274193d265ce5206b723d10451c092a5c055eba2
   category: main
   optional: false
 - name: mkdocs
   version: 1.4.3
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7909,14 +8059,30 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/paramiko-3.2.0-pyhd8ed1ab_0.conda
   hash:
     md5: f212c7eb95e909df4795297f73690993
     sha256: e425a03e5e2ef2ec5a78711686c59cfceeeeec3a98165fbc7d186bd6a5cb78de
   category: dev
   optional: true
+- name: pydantic
+  version: 2.0.3
+  manager: conda
+  platform: osx-arm64
+  dependencies:
+    annotated-types: '>=0.4.0'
+    pydantic-core: 2.3.0
+    python: '>=3.11,<3.12.0a0'
+    python_abi: 3.11.*
+    typing-extensions: '>=4.6.1'
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pydantic-2.0.3-py311heffc1b2_0.conda
+  hash:
+    md5: 05089df1a05ce41fe726c269f39856cf
+    sha256: 67bcc1d2d932da9da1f784716cd8f60259a159184258b5bcb0cc21a5a94d539e
+  category: main
+  optional: false
 - name: pylint
   version: 2.17.4
   manager: conda
   platform: osx-arm64
   dependencies:
     astroid: '>=2.15.4,<2.17.0-dev0'
     colorama: '>=0.4.5'
@@ -7931,25 +8097,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pylint-2.17.4-pyhd8ed1ab_0.conda
   hash:
     md5: a9d97fe4617aba393d90ea81576b6b46
     sha256: dec2a299b39212fc311771faec9d5cd854a18f8655d04930b8d69139c9d8a546
   category: dev
   optional: true
 - name: pymdown-extensions
-  version: 10.0.1
+  version: 10.1.0
   manager: conda
   platform: osx-arm64
   dependencies:
     markdown: '>=3.2'
     python: '>=3.7'
     pyyaml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.0.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.1.0-pyhd8ed1ab_0.conda
   hash:
-    md5: c97339cff97ae0c82dcfd7ccf72cb3d1
-    sha256: fac9ac7e236925056e69bcdec34b219a2fa860bf9434d4391986dad6afd22859
+    md5: ab329864b9f57210f3d2f9c6cd30b921
+    sha256: 892c9409b5d3d8329c8b435d91f9075df271f06bde4ed04ec23fb19831502b02
   category: dev
   optional: true
 - name: pyopenssl
   version: 23.2.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -7957,116 +8123,60 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   category: main
   optional: false
-- name: pytest-cov
-  version: 4.1.0
-  manager: conda
-  platform: osx-arm64
-  dependencies:
-    coverage: '>=5.2.1'
-    pytest: '>=4.6'
-    python: '>=3.7'
-    toml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
-  hash:
-    md5: 06eb685a3a0b146347a58dda979485da
-    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
-  category: dev
-  optional: true
-- name: pytest-flake8
-  version: 1.1.1
-  manager: conda
-  platform: osx-arm64
-  dependencies:
-    flake8: '>=4.0'
-    pytest: '>=7.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
-  hash:
-    md5: d717971066d534fd18dfe80a79146f38
-    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
-  category: dev
-  optional: true
-- name: pytest-timeout
-  version: 2.1.0
-  manager: conda
-  platform: osx-arm64
-  dependencies:
-    pytest: '>=5.0.0'
-    python: '>=3.6'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
-  hash:
-    md5: 2b23b25991cbc6886b95942704fc5c62
-    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
-  category: dev
-  optional: true
-- name: pytest-xdist
-  version: 3.3.1
-  manager: conda
-  platform: osx-arm64
-  dependencies:
-    execnet: '>=1.1'
-    pytest: '>=6.2.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
-  hash:
-    md5: 816073bb54ef59f33f0f26c14f88311b
-    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
-  category: dev
-  optional: true
 - name: readme_renderer
-  version: '37.3'
+  version: '40.0'
   manager: conda
   platform: osx-arm64
   dependencies:
     bleach: '>=2.1.0'
     cmarkgfm: '>=0.8.0'
     docutils: '>=0.13.1'
     pygments: '>=2.5.1'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 82e8ab317fe8f1d2a944688438dce868
-    sha256: 3f6d5ffe4c07bbddfcc7d108d01a1cbd78d38e9b860de46f16ca617bd4f42cd1
+    md5: 9ba2b509f6fe88364512caa9089ea886
+    sha256: 37a3b585fab825fb737ff0b2c1d2b9446ffb27b0ec42529ef7102558cafe331f
   category: dev
   optional: true
 - name: virtualenv
-  version: 20.23.0
+  version: 20.24.0
   manager: conda
   platform: osx-arm64
   dependencies:
     distlib: <1,>=0.3.6
-    filelock: <4,>=3.11
-    platformdirs: <4,>=3.2
+    filelock: <4,>=3.12
+    platformdirs: <4,>=3.5.1
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.0-pyhd8ed1ab_0.conda
   hash:
-    md5: a920e114c4c2ced2280e266da65ab5e6
-    sha256: 13d667887ea08b6d1fe2eb09d2d737f9af7343735d3bfa5ffaa3f67eec8eaff7
+    md5: 1b4a286252e336bef9ef8fa589eefdd1
+    sha256: d8b3a1badec92e81aed61d24fa33268ead568eae02372333d95bc38fce296330
   category: main
   optional: false
 - name: pre-commit
-  version: 3.3.2
+  version: 3.3.3
   manager: conda
   platform: osx-arm64
   dependencies:
     cfgv: '>=2.0.0'
     identify: '>=1.0.0'
     nodeenv: '>=0.11.1'
     python: '>=3.8'
     pyyaml: '>=5.1'
     virtualenv: '>=20.10.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.2-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.3-pyha770c72_0.conda
   hash:
-    md5: dbb0111b18ea5c9983fb8db0aef6000b
-    sha256: a55d8a19bb00c2c5bf8a074c94d5ac1ffed8d63c53c9df4cee76f3764ad7a304
+    md5: dd64a0e440754ed97610b3e6b502b6b1
+    sha256: 3df1434057ce827d88cdd84578732030b3d4b5a0bc6c58bff12b7f8001c1be5b
   category: dev
   optional: true
 - name: urllib3
   version: 1.26.15
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -8110,29 +8220,29 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda
   hash:
     md5: 9f0b2eb5f5dd2cec36d5342a80adfec0
     sha256: 894e2f4c59221b9633c60281a17fefe09ba0bf5d996992cebeb504d0585dd0dd
   category: main
   optional: false
 - name: docker-py
-  version: 6.1.0
+  version: 6.1.3
   manager: conda
   platform: osx-arm64
   dependencies:
     packaging: '>=14.0'
     paramiko: '>=2.4.3'
     python: '>=3.7'
     pywin32-on-windows: ''
     requests: '>=2.26.0'
     urllib3: '>=1.26.0'
     websocket-client: '>=0.32.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.3-pyhd8ed1ab_0.conda
   hash:
-    md5: 543336c6aa9516cfb29c51d5c162b177
-    sha256: 5e01e15e20ee573c99b530633a0d5c71fd515e4ac6d2f5f5f57baece8b915cc3
+    md5: c95d23d8bae7e21491868cc7772d7c73
+    sha256: 7c3031602e92fd7682302ef98a45bdf7374d48a849cdd3900b7c68a32d162177
   category: dev
   optional: true
 - name: doctr
   version: 1.9.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -8159,32 +8269,32 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: c99ae3abf501990769047b4b40a98f17
     sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
   category: main
   optional: false
 - name: mkdocs-material
-  version: 9.1.15
+  version: 9.1.18
   manager: conda
   platform: osx-arm64
   dependencies:
     colorama: '>=0.4'
     jinja2: '>=3.0'
     markdown: '>=3.2'
     mkdocs: '>=1.4.2'
     mkdocs-material-extensions: '>=1.1'
     pygments: '>=2.14'
-    pymdown-extensions: '>=9.9'
+    pymdown-extensions: '>=9.9.1'
     python: '>=3.7'
     regex: '>=2022.4.24'
     requests: '>=2.26'
-  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.15-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.18-pyhd8ed1ab_0.conda
   hash:
-    md5: 11383355f8c54b2a89ffd689c0cc5276
-    sha256: 445cacaa27a2c96fdb852b0d0d281e196fba89b6879ac4dd1988fa75270af04a
+    md5: 8fca138f1f46db013daf43d342169612
+    sha256: b23684c0774d7c9a08e265f97c0411d8d1737f27b94e484d37bf161c2ca52f4b
   category: dev
   optional: true
 - name: requests-toolbelt
   version: 1.0.0
   manager: conda
   platform: osx-arm64
   dependencies:
@@ -8283,47 +8393,47 @@
   url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
   hash:
     md5: 72608f6cd3e5898229c3ea16deb1ac43
     sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
   category: main
   optional: false
 - name: vc14_runtime
-  version: 14.34.31931
+  version: 14.36.32532
   manager: conda
   platform: win-64
   dependencies:
     ucrt: '>=10.0.20348.0'
-  url: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda
   hash:
-    md5: 22125178654c6a8a393f9743d585704b
-    sha256: 1161f4848e1c0663897a6324fbc4ff13dafd11650b42c9864428da73593dda95
+    md5: 91c1ecaf3996889532fc0456178b1058
+    sha256: e76986c555647347a0185e646ef65625dabed60da255f6b30367df8bd6dc6cd8
   category: main
   optional: false
 - name: vc
   version: '14.3'
   manager: conda
   platform: win-64
   dependencies:
-    vc14_runtime: '>=14.32.31332'
-  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda
+    vc14_runtime: '>=14.36.32532'
+  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda
   hash:
-    md5: ea326b37e3bd6d2616988e09f3a9396c
-    sha256: 29bc108d66150ca75cab937f844f4ac4a836beb6ea3ee167d03c611444bb2a82
+    md5: 67ff6791f235bb606659bf2a5c169191
+    sha256: 86ae94bf680980776aa761c2b0909a0ddbe1f817e7eeb8b16a1730f10f8891b6
   category: main
   optional: false
 - name: vs2015_runtime
-  version: 14.34.31931
+  version: 14.36.32532
   manager: conda
   platform: win-64
   dependencies:
-    vc14_runtime: '>=14.34.31931'
-  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda
+    vc14_runtime: '>=14.36.32532'
+  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda
   hash:
-    md5: 0374eae69b6dbfb27c3dc27167109eb4
-    sha256: 25d852887a501ca8cb6753a4f3dae1549fa49592d51aec1a230b1f0c85fe4297
+    md5: 4618046c39f7c81861e53ded842e738a
+    sha256: 5ecbd731dc7f13762d67be0eadc47eb7f14713005e430d9b5fc680e965ac0f81
   category: main
   optional: false
 - name: bzip2
   version: 1.0.8
   manager: conda
   platform: win-64
   dependencies:
@@ -8365,19 +8475,19 @@
 - name: libzlib
   version: 1.2.13
   manager: conda
   platform: win-64
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  url: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2
+    vc14_runtime: '>=14.29.30139'
+  url: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
   hash:
-    md5: 0cc5c5cc64ee1637f37f8540a175854c
-    sha256: 184da12b4296088a47086f4e69e65eb5f8537a824ee3131d8076775e1d1ea767
+    md5: 5fdb9c6a113b6b6cb5e517fd972d5f41
+    sha256: c161822ee8130b71e08b6d282b9919c1de2c5274b29921a867bca0f7d30cad26
   category: main
   optional: false
 - name: openssl
   version: 3.1.1
   manager: conda
   platform: win-64
   dependencies:
@@ -8427,35 +8537,35 @@
   url: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
   hash:
     md5: adbfb9f45d1004a26763652246a33764
     sha256: 4e2246383003acbad9682c7c63178e2e715ad0eb84f03a8df1fbfba455dfedc5
   category: main
   optional: false
 - name: python
-  version: 3.11.3
+  version: 3.11.4
   manager: conda
   platform: win-64
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     libexpat: '>=2.5.0,<3.0a0'
     libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
     xz: '>=5.2.6,<6.0a0'
     pip: ''
-  url: https://conda.anaconda.org/conda-forge/win-64/python-3.11.3-h2628c8c_0_cpython.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda
   hash:
-    md5: 8f82e0e0ba51bed311f28eb6450393f6
-    sha256: 092b7bc17a0065b82f512d56910c521fd665e8020536014f1a9e3f2a47b448bb
+    md5: 3187a32fba79e835f099ecea054026f4
+    sha256: d43fa70a3549fea27d3993f79ba2584ec6d6fe2aaf6e5890847f974e89a744e0
   category: main
   optional: false
 - name: appdirs
   version: 1.4.4
   manager: conda
   platform: win-64
   dependencies:
@@ -8499,23 +8609,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: ebb5f5f7dc4f1a3780ef7ea7738db08c
     sha256: fbc03537a27ef756162c49b1d0608bf7ab12fa5e38ceb8563d6f4859e835ac5c
   category: dev
   optional: true
 - name: charset-normalizer
-  version: 3.1.0
+  version: 3.2.0
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   category: main
   optional: false
 - name: colorama
   version: 0.4.6
   manager: conda
   platform: win-64
   dependencies:
@@ -8572,47 +8682,47 @@
   url: https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda
   hash:
     md5: 851f4c302cc7f5a617cc03a3c2090634
     sha256: 6baece0c4fcb3c6bbfd097c80eda9de8fe12cdc3170635a3080a4a760625d4bd
   category: dev
   optional: true
 - name: exceptiongroup
-  version: 1.1.1
+  version: 1.1.2
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   category: dev
   optional: true
 - name: execnet
-  version: 1.9.0
+  version: 2.0.2
   manager: conda
   platform: win-64
   dependencies:
-    python: 2.7|>=3.5
-  url: https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/execnet-2.0.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 0e521f7a5e60d508b121d38b04874fb2
-    sha256: 1900bbc1764d01405e55be2e369d1b830fb435eb0f27c57033372c60f34c675c
+    md5: 67de0d8241e1060a479e3c37793e26f9
+    sha256: 88ea68a360198af39368beecf057af6b31f0ae38071b2bdb2aa961b6ae5427c0
   category: dev
   optional: true
 - name: filelock
-  version: 3.12.1
+  version: 3.12.2
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1f262528bc0ca9d410b98c02d09de3ac
-    sha256: dbb815b1f9c893cdf9a17360148509c439ed83e23128eb6d0be2a9459371c0f2
+    md5: 53522ec72e6adae42bd373ef58357230
+    sha256: 1cbae9f05860f2e566e2977f14dfcd5494beb22c028b0a853ade4ec381d9de71
   category: main
   optional: false
 - name: flaky
   version: 3.7.0
   manager: conda
   platform: win-64
   dependencies:
@@ -8836,23 +8946,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
   hash:
     md5: be1e9f1c65a1ed0f2ae9352fec99db64
     sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
   category: main
   optional: false
 - name: pluggy
-  version: 1.0.0
+  version: 1.2.0
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   category: dev
   optional: true
 - name: psutil
   version: 5.9.5
   manager: conda
   platform: win-64
   dependencies:
@@ -8940,24 +9050,24 @@
   url: https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py311h12c1d0e_2.tar.bz2
   hash:
     md5: 20a2d8e73b0be8e27ca4096d4f3a7053
     sha256: cdefd0688f776940bcc74fd981328a5d45e734006538dca6d686f8d21051c753
   category: dev
   optional: true
 - name: pywin32-ctypes
-  version: 0.2.0
+  version: 0.2.2
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.0-py311h1ea47a8_1006.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py311h1ea47a8_0.conda
   hash:
-    md5: 86ee973a16f5449d9ded34b512331dce
-    sha256: 79e45223e67b424f397936b08c500a5a6ef0f36896aad9c9f2f32669e9089e2b
+    md5: 93204e67d63d9ea4ef2b878172222b74
+    sha256: eaf4333628281e829efef8ed1163f326fa673a65d270d7d0c1ca25ccdf81b4e5
   category: main
   optional: false
 - name: pyyaml
   version: '6.0'
   manager: conda
   platform: win-64
   dependencies:
@@ -9014,23 +9124,23 @@
   url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py311ha68e1ae_1.conda
   hash:
     md5: 654fbe603c79490699cd7447e4627aee
     sha256: 407ea37bbf6da39261294624f6eb5a247bf8674a1c73fe8e89878331e233f431
   category: main
   optional: false
 - name: setuptools
-  version: 67.7.2
+  version: 68.0.0
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 3b68bc43ec6baa48f7354a446267eefe
-    sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
+    md5: 5a7739d0f57ee64133c9d32e6507c46d
+    sha256: 083a0913f5b56644051f31ac40b4eeea762a88c00aa12437817191b85a753cec
   category: main
   optional: false
 - name: six
   version: 1.16.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9098,23 +9208,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 92facfec94bc02d6ccf42e7173831a36
     sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
   category: main
   optional: false
 - name: typing_extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   category: main
   optional: false
 - name: webencodings
   version: 0.5.1
   manager: conda
   platform: win-64
   dependencies:
@@ -9122,23 +9232,23 @@
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   category: main
   optional: false
 - name: websocket-client
-  version: 1.5.3
+  version: 1.6.1
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.3-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   hash:
-    md5: 9beb712a1de20fea4e339a2d62851564
-    sha256: 5176f7157b3152535e11c360b089d45d7eaf4c6c0e2116952138ab2ae195419f
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   category: dev
   optional: true
 - name: wheel
   version: 0.40.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9175,38 +9285,38 @@
   url: https://conda.anaconda.org/conda-forge/win-64/wrapt-1.15.0-py311ha68e1ae_0.conda
   hash:
     md5: 35cd340b3649a688d4326c90bc388a3a
     sha256: b551dbff1aab4d38383746b7a2e11315c41029049931fdb262709efa12b42213
   category: dev
   optional: true
 - name: zipp
-  version: 3.15.0
+  version: 3.16.2
   manager: conda
   platform: win-64
   dependencies:
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   category: main
   optional: false
 - name: astroid
-  version: 2.15.5
+  version: 2.15.6
   manager: conda
   platform: win-64
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     wrapt: <2,>=1.14
-  url: https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.5-py311h1ea47a8_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.6-py311h1ea47a8_0.conda
   hash:
-    md5: adc9ceb237b4dab4b68ced77af9bdc62
-    sha256: 32ec284383dfbd2d4b93fb578f4c04e0dabc741a31c92ec7f2e11ec28c378946
+    md5: 7371f19d8ab99ce21b46af7f5a5bcfda
+    sha256: 45a03112ca819b4fff826b0809de32ae6a38f05104e7c67a5a397076789a4b63
   category: dev
   optional: true
 - name: bleach
   version: 6.0.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9235,25 +9345,25 @@
   url: https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda
   hash:
     md5: a8524727eb956b4741e25a64af79edb8
     sha256: 49ce08187365f97c67476d504411de0a17e69b972ab6b80521d01dc80dd657e6
   category: main
   optional: false
 - name: click
-  version: 8.1.3
+  version: 8.1.5
   manager: conda
   platform: win-64
   dependencies:
     __win: ''
     colorama: ''
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.5-win_pyh7428d3b_0.conda
   hash:
-    md5: 6b58680207b526c42dcff68b543803dd
-    sha256: 84e80a33e9a8e5398d3e97209366b57f635462a5b894f8076ec8c95e56672c44
+    md5: e04d94cb02f7938996e31e330f2d0263
+    sha256: 5e3247d3d57dbb58e9a5e44c1d287094022084e8c15b1f4d258ac70e6bce937e
   category: main
   optional: false
 - name: clikit
   version: 0.6.2
   manager: conda
   platform: win-64
   dependencies:
@@ -9322,24 +9432,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
   hash:
     md5: b2355343d6315c892543200231d7154a
     sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
   category: main
   optional: false
 - name: importlib-metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
   hash:
-    md5: f91a5d5175fb7ff2a91952ec7da59cb9
-    sha256: 33d49065756a73fbb92277c756fa00a41891408528eb90ae05ff3367a401ae6e
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   category: main
   optional: false
 - name: isort
   version: 5.12.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9348,24 +9458,24 @@
   url: https://conda.anaconda.org/conda-forge/noarch/isort-5.12.0-pyhd8ed1ab_1.conda
   hash:
     md5: 07ed3421bad60867234c7a9282ea39d4
     sha256: d34a62e33ac7acc8fd3167ceb0e2aee4e7974b94de263f52d752716429d95bcb
   category: dev
   optional: true
 - name: jaraco.classes
-  version: 3.2.3
+  version: 3.3.0
   manager: conda
   platform: win-64
   dependencies:
     more-itertools: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
   category: main
   optional: false
 - name: jinja2
   version: 3.1.2
   manager: conda
   platform: win-64
   dependencies:
@@ -9374,45 +9484,44 @@
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
   category: main
   optional: false
 - name: markdown-it-py
-  version: 2.2.0
+  version: 3.0.0
   manager: conda
   platform: win-64
   dependencies:
     mdurl: '>=0.1,<1'
-    python: '>=3.7'
-    typing_extensions: '>=3.7.4'
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
   hash:
-    md5: b2928a6c6d52d7e3562b4a59c3214e3a
-    sha256: 65ed439862c1851463f03a9bc5109992ce3e3e025e9a2d76d13ca19f576eee9f
+    md5: 93a8e71256479c62074356ef6ebf501b
+    sha256: c041b0eaf7a6af3344d5dd452815cdc148d6284fec25a4fa3f4263b3a021e962
   category: dev
   optional: true
 - name: mypy
-  version: 1.3.0
+  version: 1.4.1
   manager: conda
   platform: win-64
   dependencies:
     mypy_extensions: '>=0.4.3'
     psutil: '>=4.0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     tomli: '>=1.1.0'
     typing_extensions: '>=3.10'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
-  url: https://conda.anaconda.org/conda-forge/win-64/mypy-1.3.0-py311ha68e1ae_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/mypy-1.4.1-py311ha68e1ae_0.conda
   hash:
-    md5: a63b769ed254671c8ecc27d67a220546
-    sha256: aaa1537d4c8905d2e69fa38f65205541d74ff204762fda58e4b943ecb62618aa
+    md5: 6d8c5eed03be56e4ceedee017d5edb83
+    sha256: 821f051883edbee804c3f1be27fa3e0fe652d0e686dca5c98bc3d031f5a919ad
   category: dev
   optional: true
 - name: nodeenv
   version: 1.8.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9421,25 +9530,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
   hash:
     md5: 2a75b296096adabbabadd5e9782e5fcc
     sha256: 1320306234552717149f36f825ddc7e27ea295f24829e9db4cc6ceaff0b032bd
   category: dev
   optional: true
 - name: pip
-  version: 23.1.2
+  version: '23.2'
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
     setuptools: ''
     wheel: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 7288da0d36821349cf1126e8670292df
-    sha256: 4fe1f47f6eac5b2635a622b6f985640bf835843c1d8d7ccbbae0f7d27cadec92
+    md5: fb90dfe13ce16c0a3374e3d34e3291c5
+    sha256: 31e71fc25dbc411c1595661c8eb2c2491e71895ce6954ea2d0e9a585d39eed57
   category: dev
   optional: true
 - name: pyproject_hooks
   version: 1.0.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9461,14 +9570,32 @@
     win_inet_pton: ''
   url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2
   hash:
     md5: 56cd9fe388baac0e90c7149cfac95b60
     sha256: b3a612bc887f3dd0fb7c4199ad8e342bd148cf69a9b74fd9468a18cf2bef07b7
   category: main
   optional: false
+- name: pytest
+  version: 7.4.0
+  manager: conda
+  platform: win-64
+  dependencies:
+    colorama: ''
+    exceptiongroup: '>=1.0.0rc8'
+    iniconfig: ''
+    packaging: ''
+    pluggy: '>=0.12,<2.0'
+    python: '>=3.7'
+    tomli: '>=1.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3cfe9b9e958e7238a386933c75d190db
+    sha256: 52b2eb4e8d0380d92d45643d0c9706725e691ce8404dab4c2db4aaf58e48a23c
+  category: dev
+  optional: true
 - name: python-dateutil
   version: 2.8.2
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.6'
     six: '>=1.5'
@@ -9501,41 +9628,41 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 626ed9060ddeb681ddc42bcad89156ab
     sha256: 900319483135730d9836855a807822f0500b1a239520749103e9ef9b7ba9f246
   category: dev
   optional: true
 - name: ruamel.yaml
-  version: 0.17.31
+  version: 0.17.32
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     ruamel.yaml.clib: '>=0.1.2'
     setuptools: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
-  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.31-py311ha68e1ae_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.32-py311ha68e1ae_0.conda
   hash:
-    md5: 211e024535a77ae712ad05d2ec7ac4fe
-    sha256: f4c7a2a94f5530edfcb6c343e9afb66d213bb7798ddc8893a468eb198feaa36a
+    md5: 1a51f29331338bfde51127db204d7757
+    sha256: b287388ea53da5437ceac8bd9ff9ee161d3a2433275a0f74b332c6b032d9ef50
   category: main
   optional: false
 - name: typing-extensions
-  version: 4.6.3
+  version: 4.7.1
   manager: conda
   platform: win-64
   dependencies:
-    typing_extensions: 4.6.3
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
+    typing_extensions: 4.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   category: main
   optional: false
 - name: watchdog
   version: 3.0.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9544,14 +9671,27 @@
     pyyaml: '>=3.10'
   url: https://conda.anaconda.org/conda-forge/win-64/watchdog-3.0.0-py311h1ea47a8_0.conda
   hash:
     md5: 0b230f93a075fce059f6cd52bcc4aea7
     sha256: 8228e93ccdf87f6ec2daec2862a629b8f21b64157e180b8594f7fe27b9c5f639
   category: dev
   optional: true
+- name: annotated-types
+  version: 0.5.0
+  manager: conda
+  platform: win-64
+  dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  category: main
+  optional: false
 - name: bcrypt
   version: 3.2.2
   manager: conda
   platform: win-64
   dependencies:
     cffi: '>=1.1'
     pip: ''
@@ -9611,29 +9751,29 @@
   url: https://conda.anaconda.org/conda-forge/win-64/cmarkgfm-0.8.0-py311ha68e1ae_2.tar.bz2
   hash:
     md5: 206cb594ef199270b7e0d3d17aa87cbe
     sha256: 34ef87f3d6700f63b15e8d9fd3f7d89e804f0a1d76c76b4042206e5d85dc6a91
   category: dev
   optional: true
 - name: cryptography
-  version: 41.0.1
+  version: 41.0.2
   manager: conda
   platform: win-64
   dependencies:
     cffi: '>=1.12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
-  url: https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.1-py311h28e9c30_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.2-py311h28e9c30_0.conda
   hash:
-    md5: d2b52be40a519bd255397a884bd3fb1c
-    sha256: 30686db21c188b51c6835342341ab464fcb5e19c6188894f23c6aa7833ca307f
+    md5: ea9fc978bfef9ceeb950687f0063c460
+    sha256: bf01795e9d5ddf58a8d18fcf44d72b8f520f813b76617f40c587a479ca910a83
   category: main
   optional: false
 - name: flake8-builtins
   version: 2.1.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9681,37 +9821,37 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   category: dev
   optional: true
 - name: gitpython
-  version: 3.1.31
+  version: 3.1.32
   manager: conda
   platform: win-64
   dependencies:
     gitdb: '>=4.0.1,<5'
     python: '>=3.7'
     typing_extensions: '>=3.7.4.3'
-  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda
   hash:
-    md5: f6e6b482110246a81c3f03e81c68752d
-    sha256: 77c531def610089bc190508fcf304cf96c085c5fe977ab8f7d7c1641769592ac
+    md5: 5809a12901d57388444c3293c975d0bb
+    sha256: 07008a94189e570fcabe003b99bd50b8263f60c824f36f81a8819bb7cf7eab1b
   category: main
   optional: false
 - name: importlib_metadata
-  version: 6.6.0
+  version: 6.8.0
   manager: conda
   platform: win-64
   dependencies:
-    importlib-metadata: '>=6.6.0,<6.6.1.0a0'
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
   hash:
-    md5: 3cbc9615f10a3d471532b83e4250b971
-    sha256: 5de35d3c019d8a36e0a0deeb04a62689837bd68234a0a73a3355b860b442eca4
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   category: main
   optional: false
 - name: markdown
   version: 3.3.7
   manager: conda
   platform: win-64
   dependencies:
@@ -9720,41 +9860,41 @@
   url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.3.7-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: 0a0bed31742342688a8570b3b8a50f36
     sha256: 4af5d3f376295753d787be5013900ebca572bd8f30d59e34fbae512ec414eb5e
   category: dev
   optional: true
 - name: platformdirs
-  version: 3.5.1
+  version: 3.8.1
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.7'
-    typing-extensions: '>=4.5'
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda
+    typing-extensions: '>=4.6.3'
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda
   hash:
-    md5: e2be672aece1f060adf7154f76531a35
-    sha256: d7845c01a9ee5a224cc9242782befed7d12dc6aac1103650ec87917b20f3579e
+    md5: e76070baecfaca6ecdb5fbd5af7c9309
+    sha256: b5012d6fd30f2462b6ca595539cfdae9aaf61b3b7a56e51ab94aef0fd9efcd3d
   category: main
   optional: false
-- name: pydantic
-  version: 1.10.9
+- name: pydantic-core
+  version: 2.3.0
   manager: conda
   platform: win-64
   dependencies:
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-    typing-extensions: '>=4.2.0'
+    typing-extensions: '>=4.6.0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
-  url: https://conda.anaconda.org/conda-forge/win-64/pydantic-1.10.9-py311ha68e1ae_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.3.0-py311hc37eb10_0.conda
   hash:
-    md5: b086521bbe799f96dcc8006869496d1a
-    sha256: b0637e383a407f04e3dadf79f18b7bac80134d0ad307cc11bab5d4652232afc1
+    md5: 9259b7da3dde8b3c247e944cfbe13b87
+    sha256: 12135c4ff6ffd54966d60f7d41cb7fc8a458ce08ff7ee630ca0bfc3e64afc475
   category: main
   optional: false
 - name: pynacl
   version: 1.5.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9767,31 +9907,68 @@
     vs2015_runtime: '>=14.29.30139'
   url: https://conda.anaconda.org/conda-forge/win-64/pynacl-1.5.0-py311hd53affc_2.tar.bz2
   hash:
     md5: 92a424fa00e261904d4b9589e8652ae0
     sha256: 5bf57da0e5fad94240a415bcf8f98d2a765d861559ebc724597ce35cb0b193c7
   category: dev
   optional: true
-- name: pytest
-  version: 7.3.1
+- name: pytest-cov
+  version: 4.1.0
   manager: conda
   platform: win-64
   dependencies:
-    colorama: ''
-    exceptiongroup: ''
-    importlib-metadata: '>=0.12'
-    iniconfig: ''
-    packaging: ''
-    pluggy: '>=0.12,<2.0'
-    python: '>=3.8'
-    tomli: '>=1.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.1-pyhd8ed1ab_0.conda
+    coverage: '>=5.2.1'
+    pytest: '>=4.6'
+    python: '>=3.7'
+    toml: ''
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 06eb685a3a0b146347a58dda979485da
+    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
+  category: dev
+  optional: true
+- name: pytest-flake8
+  version: 1.1.1
+  manager: conda
+  platform: win-64
+  dependencies:
+    flake8: '>=4.0'
+    pytest: '>=7.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
   hash:
-    md5: 547c7de697ec99b494a28ddde185b5a4
-    sha256: 42f89db577266b9dc195d09189b92f3af3354fb50c98b1f996c580322dffa8b5
+    md5: d717971066d534fd18dfe80a79146f38
+    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
+  category: dev
+  optional: true
+- name: pytest-timeout
+  version: 2.1.0
+  manager: conda
+  platform: win-64
+  dependencies:
+    pytest: '>=5.0.0'
+    python: '>=3.6'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 2b23b25991cbc6886b95942704fc5c62
+    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
+  category: dev
+  optional: true
+- name: pytest-xdist
+  version: 3.3.1
+  manager: conda
+  platform: win-64
+  dependencies:
+    execnet: '>=1.1'
+    pytest: '>=6.2.0'
+    python: '>=3.7'
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 816073bb54ef59f33f0f26c14f88311b
+    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
   category: dev
   optional: true
 - name: python-build
   version: 0.10.0
   manager: conda
   platform: win-64
   dependencies:
@@ -9804,26 +9981,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda
   hash:
     md5: 0ab47ce574f6a8bcb9f2076436e7fedb
     sha256: 4c2cd519c85aa8b8e584723ca5f452aa5941d18374470adebfe73bf30fd27573
   category: dev
   optional: true
 - name: rich
-  version: 13.4.1
+  version: 13.4.2
   manager: conda
   platform: win-64
   dependencies:
-    markdown-it-py: '>=2.2.0,<3.0.0'
+    markdown-it-py: '>=2.2.0'
     pygments: '>=2.13.0,<3.0.0'
     python: '>=3.7.0'
     typing_extensions: '>=4.0.0,<5.0.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: c3bcbe0d086f15e5918568d3865e4dbf
-    sha256: 312f2628e06a591096a851bf678833fe670ecb16e9b15517ce8e03d7c9d9e600
+    md5: f993baacc175e83fafd6b846e9c4c8a2
+    sha256: d0f6506b0bf1f5563b6b42cf018002b7007bd49e62ad4a178c2a50bf3a7fe45f
   category: dev
   optional: true
 - name: ukkonen
   version: 1.0.1
   manager: conda
   platform: win-64
   dependencies:
@@ -9836,29 +10013,29 @@
   url: https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py311h005e61a_3.tar.bz2
   hash:
     md5: 345c6b3bee32bb1d87a4e8759ec6cbff
     sha256: 657648ad15dd3062d417040371935983ac5c9a57ec8ff14e9c862a57058a242f
   category: dev
   optional: true
 - name: black
-  version: 23.3.0
+  version: 23.7.0
   manager: conda
   platform: win-64
   dependencies:
     click: '>=8.0.0'
     mypy_extensions: '>=0.4.3'
     packaging: '>=22.0'
     pathspec: '>=0.9'
     platformdirs: '>=2'
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-  url: https://conda.anaconda.org/conda-forge/win-64/black-23.3.0-py311h1ea47a8_1.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/black-23.7.0-py311h1ea47a8_1.conda
   hash:
-    md5: cff72d53d4ea05005adc2f478447a0a1
-    sha256: 12f319748c11697ee3ea154413c7c4895db2dfcc18b44b0bdb2019da1144abdb
+    md5: 335ab55360386db3b594370694d3a22c
+    sha256: b96092341f6e6d5eeb8bf69b0690d17439410a776ed3fbd58999f52d56b16f2c
   category: dev
   optional: true
 - name: check-manifest
   version: '0.49'
   manager: conda
   platform: win-64
   dependencies:
@@ -9869,25 +10046,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/check-manifest-0.49-pyhd8ed1ab_0.conda
   hash:
     md5: 65b3059f2f0807433ee3c2673a886123
     sha256: f8d03ad89aacf5278b74f73f6720588cfa41481c959206147fd58d54f7974487
   category: dev
   optional: true
 - name: flake8-comprehensions
-  version: 3.12.0
+  version: 3.13.0
   manager: conda
   platform: win-64
   dependencies:
     flake8: '>=3.0,!=3.2.0'
     importlib_metadata: ''
     python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.12.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/flake8-comprehensions-3.13.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 18c6bc2bb3cd3950029569362cca2e33
-    sha256: c825986cf7a2f617b61373e421d74e9383696d48def52e4619af2bea1b747e8d
+    md5: f1fca1448e90eaa8fc5a3676813b4c0c
+    sha256: 3fd60ba3cfedd29fcceea147141aea74763483e3491e32afdeaa4357cf8eb92e
   category: dev
   optional: true
 - name: identify
   version: 2.5.24
   manager: conda
   platform: win-64
   dependencies:
@@ -9896,27 +10073,27 @@
   url: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.24-pyhd8ed1ab_0.conda
   hash:
     md5: a4085ab0562d5081a9333435837b538a
     sha256: 4027103c59220a68b41aed056d2ce89d46e4971033d259293ca07198a8a81fdc
   category: dev
   optional: true
 - name: keyring
-  version: 23.13.1
+  version: 24.2.0
   manager: conda
   platform: win-64
   dependencies:
     importlib_metadata: '>=4.11.4'
     jaraco.classes: ''
     python: '>=3.11,<3.12.0a0'
     python_abi: 3.11.*
-    pywin32-ctypes: ''
-  url: https://conda.anaconda.org/conda-forge/win-64/keyring-23.13.1-py311h1ea47a8_0.conda
+    pywin32-ctypes: '>=0.2.0'
+  url: https://conda.anaconda.org/conda-forge/win-64/keyring-24.2.0-py311h1ea47a8_0.conda
   hash:
-    md5: ff14a49b769ea59ee6709a890e17f317
-    sha256: 33886e99ffcf6b957cb819ec97b6056a3444a1b77fb5a2cfcf004ab453684c8f
+    md5: 6a5239529cb5af3437bdd24c1082c2eb
+    sha256: 6f49ddde7f3db90fd7c8e8d70cb282835584ddb3140f74b4404005d5018f014f
   category: main
   optional: false
 - name: mkdocs
   version: 1.4.3
   manager: conda
   platform: win-64
   dependencies:
@@ -9964,14 +10141,33 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/paramiko-3.2.0-pyhd8ed1ab_0.conda
   hash:
     md5: f212c7eb95e909df4795297f73690993
     sha256: e425a03e5e2ef2ec5a78711686c59cfceeeeec3a98165fbc7d186bd6a5cb78de
   category: dev
   optional: true
+- name: pydantic
+  version: 2.0.3
+  manager: conda
+  platform: win-64
+  dependencies:
+    annotated-types: '>=0.4.0'
+    pydantic-core: 2.3.0
+    python: '>=3.11,<3.12.0a0'
+    python_abi: 3.11.*
+    typing-extensions: '>=4.6.1'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
+  url: https://conda.anaconda.org/conda-forge/win-64/pydantic-2.0.3-py311ha68e1ae_0.conda
+  hash:
+    md5: 1869781f1593f5e6a0a756bedb36a78f
+    sha256: a238e666fb9ee6554322d0cb20cae5401761292fd0b3c5c9638410d5eaf2b272
+  category: main
+  optional: false
 - name: pylint
   version: 2.17.4
   manager: conda
   platform: win-64
   dependencies:
     astroid: '>=2.15.4,<2.17.0-dev0'
     colorama: '>=0.4.5'
@@ -9986,25 +10182,25 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pylint-2.17.4-pyhd8ed1ab_0.conda
   hash:
     md5: a9d97fe4617aba393d90ea81576b6b46
     sha256: dec2a299b39212fc311771faec9d5cd854a18f8655d04930b8d69139c9d8a546
   category: dev
   optional: true
 - name: pymdown-extensions
-  version: 10.0.1
+  version: 10.1.0
   manager: conda
   platform: win-64
   dependencies:
     markdown: '>=3.2'
     python: '>=3.7'
     pyyaml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.0.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.1.0-pyhd8ed1ab_0.conda
   hash:
-    md5: c97339cff97ae0c82dcfd7ccf72cb3d1
-    sha256: fac9ac7e236925056e69bcdec34b219a2fa860bf9434d4391986dad6afd22859
+    md5: ab329864b9f57210f3d2f9c6cd30b921
+    sha256: 892c9409b5d3d8329c8b435d91f9075df271f06bde4ed04ec23fb19831502b02
   category: dev
   optional: true
 - name: pyopenssl
   version: 23.2.0
   manager: conda
   platform: win-64
   dependencies:
@@ -10012,116 +10208,60 @@
     python: '>=3.6'
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   category: main
   optional: false
-- name: pytest-cov
-  version: 4.1.0
-  manager: conda
-  platform: win-64
-  dependencies:
-    coverage: '>=5.2.1'
-    pytest: '>=4.6'
-    python: '>=3.7'
-    toml: ''
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda
-  hash:
-    md5: 06eb685a3a0b146347a58dda979485da
-    sha256: f07d3b44cabbed7843de654c4a6990a08475ce3b708bb735c7da9842614586f2
-  category: dev
-  optional: true
-- name: pytest-flake8
-  version: 1.1.1
-  manager: conda
-  platform: win-64
-  dependencies:
-    flake8: '>=4.0'
-    pytest: '>=7.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-flake8-1.1.1-pyhd8ed1ab_1.tar.bz2
-  hash:
-    md5: d717971066d534fd18dfe80a79146f38
-    sha256: 9a24571a3fc2ac7ad09a93f479a2ef94b2fb2fcf6b8d001a0c7bd1041168dec3
-  category: dev
-  optional: true
-- name: pytest-timeout
-  version: 2.1.0
-  manager: conda
-  platform: win-64
-  dependencies:
-    pytest: '>=5.0.0'
-    python: '>=3.6'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-timeout-2.1.0-pyhd8ed1ab_0.tar.bz2
-  hash:
-    md5: 2b23b25991cbc6886b95942704fc5c62
-    sha256: 4bb56fbdd1e3487428a0ec120ce62bb20b3abe8cce459b9c87201f55292cbc35
-  category: dev
-  optional: true
-- name: pytest-xdist
-  version: 3.3.1
-  manager: conda
-  platform: win-64
-  dependencies:
-    execnet: '>=1.1'
-    pytest: '>=6.2.0'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda
-  hash:
-    md5: 816073bb54ef59f33f0f26c14f88311b
-    sha256: 5df2d0f1e42041476cbdf12b808890d668e7f0272b51f0f3fa7aab84732150b6
-  category: dev
-  optional: true
 - name: readme_renderer
-  version: '37.3'
+  version: '40.0'
   manager: conda
   platform: win-64
   dependencies:
     bleach: '>=2.1.0'
     cmarkgfm: '>=0.8.0'
     docutils: '>=0.13.1'
     pygments: '>=2.5.1'
-    python: '>=3.7'
-  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2
+    python: '>=3.8'
+  url: https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 82e8ab317fe8f1d2a944688438dce868
-    sha256: 3f6d5ffe4c07bbddfcc7d108d01a1cbd78d38e9b860de46f16ca617bd4f42cd1
+    md5: 9ba2b509f6fe88364512caa9089ea886
+    sha256: 37a3b585fab825fb737ff0b2c1d2b9446ffb27b0ec42529ef7102558cafe331f
   category: dev
   optional: true
 - name: virtualenv
-  version: 20.23.0
+  version: 20.24.0
   manager: conda
   platform: win-64
   dependencies:
     distlib: <1,>=0.3.6
-    filelock: <4,>=3.11
-    platformdirs: <4,>=3.2
+    filelock: <4,>=3.12
+    platformdirs: <4,>=3.5.1
     python: '>=3.8'
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.0-pyhd8ed1ab_0.conda
   hash:
-    md5: a920e114c4c2ced2280e266da65ab5e6
-    sha256: 13d667887ea08b6d1fe2eb09d2d737f9af7343735d3bfa5ffaa3f67eec8eaff7
+    md5: 1b4a286252e336bef9ef8fa589eefdd1
+    sha256: d8b3a1badec92e81aed61d24fa33268ead568eae02372333d95bc38fce296330
   category: main
   optional: false
 - name: pre-commit
-  version: 3.3.2
+  version: 3.3.3
   manager: conda
   platform: win-64
   dependencies:
     cfgv: '>=2.0.0'
     identify: '>=1.0.0'
     nodeenv: '>=0.11.1'
     python: '>=3.8'
     pyyaml: '>=5.1'
     virtualenv: '>=20.10.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.2-pyha770c72_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.3.3-pyha770c72_0.conda
   hash:
-    md5: dbb0111b18ea5c9983fb8db0aef6000b
-    sha256: a55d8a19bb00c2c5bf8a074c94d5ac1ffed8d63c53c9df4cee76f3764ad7a304
+    md5: dd64a0e440754ed97610b3e6b502b6b1
+    sha256: 3df1434057ce827d88cdd84578732030b3d4b5a0bc6c58bff12b7f8001c1be5b
   category: dev
   optional: true
 - name: urllib3
   version: 1.26.15
   manager: conda
   platform: win-64
   dependencies:
@@ -10165,29 +10305,29 @@
   url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda
   hash:
     md5: 9f0b2eb5f5dd2cec36d5342a80adfec0
     sha256: 894e2f4c59221b9633c60281a17fefe09ba0bf5d996992cebeb504d0585dd0dd
   category: main
   optional: false
 - name: docker-py
-  version: 6.1.0
+  version: 6.1.3
   manager: conda
   platform: win-64
   dependencies:
     packaging: '>=14.0'
     paramiko: '>=2.4.3'
     python: '>=3.7'
     pywin32-on-windows: ''
     requests: '>=2.26.0'
     urllib3: '>=1.26.0'
     websocket-client: '>=0.32.0'
-  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/docker-py-6.1.3-pyhd8ed1ab_0.conda
   hash:
-    md5: 543336c6aa9516cfb29c51d5c162b177
-    sha256: 5e01e15e20ee573c99b530633a0d5c71fd515e4ac6d2f5f5f57baece8b915cc3
+    md5: c95d23d8bae7e21491868cc7772d7c73
+    sha256: 7c3031602e92fd7682302ef98a45bdf7374d48a849cdd3900b7c68a32d162177
   category: dev
   optional: true
 - name: doctr
   version: 1.9.0
   manager: conda
   platform: win-64
   dependencies:
@@ -10214,32 +10354,32 @@
   url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
   hash:
     md5: c99ae3abf501990769047b4b40a98f17
     sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
   category: main
   optional: false
 - name: mkdocs-material
-  version: 9.1.15
+  version: 9.1.18
   manager: conda
   platform: win-64
   dependencies:
     colorama: '>=0.4'
     jinja2: '>=3.0'
     markdown: '>=3.2'
     mkdocs: '>=1.4.2'
     mkdocs-material-extensions: '>=1.1'
     pygments: '>=2.14'
-    pymdown-extensions: '>=9.9'
+    pymdown-extensions: '>=9.9.1'
     python: '>=3.7'
     regex: '>=2022.4.24'
     requests: '>=2.26'
-  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.15-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.1.18-pyhd8ed1ab_0.conda
   hash:
-    md5: 11383355f8c54b2a89ffd689c0cc5276
-    sha256: 445cacaa27a2c96fdb852b0d0d281e196fba89b6879ac4dd1988fa75270af04a
+    md5: 8fca138f1f46db013daf43d342169612
+    sha256: b23684c0774d7c9a08e265f97c0411d8d1737f27b94e484d37bf161c2ca52f4b
   category: dev
   optional: true
 - name: requests-toolbelt
   version: 1.0.0
   manager: conda
   platform: win-64
   dependencies:
```

### Comparing `conda_lock-2.1.1/example/pangeo/conda-lock.yml` & `conda_lock-2.1.2/example/pangeo/conda-lock.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/example/zlib/conda-lock.yml` & `conda_lock-2.1.2/example/zlib/conda-lock.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/LICENSE` & `conda_lock-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/README.md` & `conda_lock-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.1/pyproject.toml` & `conda_lock-2.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,26 +22,27 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 license-files = { paths = ["LICENSE"] }
 dependencies = [
+    # conda-lock dependencies
     "click >=8.0",
     "click-default-group",
     "ensureconda >=1.3",
     "gitpython >=3.1.30",
     "jinja2",
-    "pydantic >=1.8.1",
+    "pydantic >=1.10",
     "pyyaml >= 5.1",
-    "ruamel.yaml",
     'tomli; python_version<"3.11"',
     "typing-extensions",
+    # conda dependencies
+    "ruamel.yaml",
     "toolz >=0.12.0,<1.0.0",
-    "filelock >=3.8.0",
     # The following dependencies were added in the process of vendoring Poetry 1.1.15.
     # poetry:
     "cachecontrol[filecache] >=0.12.9",
     # poetry:
     "cachy >=0.3.0",
     # cleo, poetry:
     "clikit >=0.6.2",
```

### Comparing `conda_lock-2.1.1/PKG-INFO` & `conda_lock-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda_lock
-Version: 2.1.1
+Version: 2.1.2
 Summary: Lockfiles for conda
 Project-URL: Homepage, https://github.com/conda/conda-lock
 Project-URL: Repository, https://github.com/conda/conda-lock
 Project-URL: Documentation, https://conda.github.io/conda-lock/
 Project-URL: Issue Tracker, https://github.com/conda/conda-lock/issues
 Project-URL: Conda-Forge Feedstock, https://github.com/conda-forge/conda-lock-feedstock
 Project-URL: Anaconda.org, https://anaconda.org/conda-forge/conda-lock
@@ -25,23 +25,22 @@
 Requires-Dist: cachecontrol[filecache]>=0.12.9
 Requires-Dist: cachy>=0.3.0
 Requires-Dist: click-default-group
 Requires-Dist: click>=8.0
 Requires-Dist: clikit>=0.6.2
 Requires-Dist: crashtest>=0.3.0
 Requires-Dist: ensureconda>=1.3
-Requires-Dist: filelock>=3.8.0
 Requires-Dist: gitpython>=3.1.30
 Requires-Dist: html5lib>=1.0
 Requires-Dist: importlib-metadata>=1.7.0; python_version <= '3.7'
 Requires-Dist: jinja2
 Requires-Dist: keyring>=21.2.0
 Requires-Dist: packaging>=20.4
 Requires-Dist: pkginfo>=1.4
-Requires-Dist: pydantic>=1.8.1
+Requires-Dist: pydantic>=1.10
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: requests>=2.18
 Requires-Dist: ruamel-yaml
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: tomlkit>=0.7.0
 Requires-Dist: toolz<1.0.0,>=0.12.0
 Requires-Dist: typing-extensions
```

