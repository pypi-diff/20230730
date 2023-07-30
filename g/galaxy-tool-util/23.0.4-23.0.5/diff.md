# Comparing `tmp/galaxy-tool-util-23.0.4.tar.gz` & `tmp/galaxy-tool-util-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tool_util/dist/.tmp-8pvv9hvx/galaxy-tool-util-23.0.4.tar", last modified: Fri Jun 30 22:04:32 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tool_util/dist/.tmp-m651pd_c/galaxy-tool-util-23.0.5.tar", last modified: Sun Jul 30 10:50:49 2023, max compression
```

## Comparing `galaxy-tool-util-23.0.4.tar` & `galaxy-tool-util-23.0.5.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-tool-util-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/biotools/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/biotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/biotools/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/biotools/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/client/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/cwltool_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)    45995 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/runtime_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25744 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/data/
--rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/data/_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/data/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/data/bundles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/data/bundles/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19572 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/brew_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/brew_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/conda_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/conda_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/mulled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/docker_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/dockerfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/installable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/get_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/invfile.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15814 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/galaxy_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/homebrew.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/lmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/resolver_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/singularity_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/deps/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/edam_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/cwl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    23859 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/stdio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/linters/xml_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/loader_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/locations/dockstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/locations/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/locations/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53080 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/biotools_mappings.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/ontology_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/output_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/cwl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    25328 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/output_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/output_collection_def.py
--rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/output_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/stdio.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    49096 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/parser/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/provided_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65911 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/filters/examples.py.sample
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/integrated_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/lineages/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/lineages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/lineages/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/lineages/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/unittest_utils/interactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/unittest_utils/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)    71060 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/interactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/script.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/test_config.sample.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/verify/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/galaxy.jxb
--rw-r--r--   0 runner    (1001) docker     (123)   319413 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/galaxy.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-30 22:04:32.000000 galaxy-tool-util-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 22:00:50.000000 galaxy-tool-util-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-tool-util-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/biotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/biotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/biotools/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/biotools/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/client/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/cwltool_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45995 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/runtime_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25744 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/data/_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/data/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/data/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/data/bundles/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19572 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/brew_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/brew_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/conda_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/conda_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/mulled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/dockerfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/installable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/get_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/invfile.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15814 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/galaxy_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/homebrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/lmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/resolver_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/singularity_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/deps/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/edam_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23859 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/linters/xml_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/loader_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/locations/dockstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/locations/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/locations/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53080 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/biotools_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/ontology_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/output_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25328 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/output_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/output_collection_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/output_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49096 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/parser/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/provided_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65911 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/filters/examples.py.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/integrated_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/lineages/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/lineages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/lineages/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/lineages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/unittest_utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/unittest_utils/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71018 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/test_config.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/verify/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/galaxy.jxb
+-rw-r--r--   0 runner    (1001) docker     (123)   319413 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/galaxy.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-30 10:50:49.000000 galaxy-tool-util-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-30 10:47:08.000000 galaxy-tool-util-23.0.5/test-requirements.txt
```

### Comparing `galaxy-tool-util-23.0.4/HISTORY.rst` & `galaxy-tool-util-23.0.5/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Allow duplicate labels in linter if outputs contain filters  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15933 <https://github.com/galaxyproject/galaxy/pull/15933>`_
+* Fix parsing tool metadata from bio.tools by `@kysrpex <https://github.com/kysrpex>`_ in `#16449 <https://github.com/galaxyproject/galaxy/pull/16449>`_
+* Linter: fix regex for profile version by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16480 <https://github.com/galaxyproject/galaxy/pull/16480>`_
+* Adjust test_data_download method in GalaxyInteractorApi so an admin user is not required by `@simonbray <https://github.com/simonbray>`_ in `#16482 <https://github.com/galaxyproject/galaxy/pull/16482>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
@@ -33,37 +47,40 @@
 
 
 =========
 Bug fixes
 =========
 
 * 
+* 
 * Don't fail CWL tool parsing when Cheetah not installed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16219 <https://github.com/galaxyproject/galaxy/pull/16219>`_
 * Allow skipping ``expect_num_outputs`` when ``expect_failure`` is set in tool test by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16237 <https://github.com/galaxyproject/galaxy/pull/16237>`_
 
 -------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 =========
 Bug fixes
 =========
 
 * 
 * 
+* 
 * Fix assertion linting to not fail on byte suffixes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15873 <https://github.com/galaxyproject/galaxy/pull/15873>`_
 * Fix ``get_test_from_anaconda()`` and ``base_image_for_targets()`` functions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16125 <https://github.com/galaxyproject/galaxy/pull/16125>`_
 * Fix test search for mulled container hashes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16170 <https://github.com/galaxyproject/galaxy/pull/16170>`_
 
 ============
 Enhancements
 ============
 
 * 
+* 
 * Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
 
 -------------------
 22.1.5 (2022-11-14)
 -------------------
 
 * Set test status to success on expected failure
```

### Comparing `galaxy-tool-util-23.0.4/LICENSE` & `galaxy-tool-util-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/PKG-INFO` & `galaxy-tool-util-23.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tool-util
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy tool and tool dependency utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,28 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Allow duplicate labels in linter if outputs contain filters  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15933 <https://github.com/galaxyproject/galaxy/pull/15933>`_
+* Fix parsing tool metadata from bio.tools by `@kysrpex <https://github.com/kysrpex>`_ in `#16449 <https://github.com/galaxyproject/galaxy/pull/16449>`_
+* Linter: fix regex for profile version by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16480 <https://github.com/galaxyproject/galaxy/pull/16480>`_
+* Adjust test_data_download method in GalaxyInteractorApi so an admin user is not required by `@simonbray <https://github.com/simonbray>`_ in `#16482 <https://github.com/galaxyproject/galaxy/pull/16482>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
@@ -78,37 +92,40 @@
 
 
 =========
 Bug fixes
 =========
 
 * 
+* 
 * Don't fail CWL tool parsing when Cheetah not installed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16219 <https://github.com/galaxyproject/galaxy/pull/16219>`_
 * Allow skipping ``expect_num_outputs`` when ``expect_failure`` is set in tool test by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16237 <https://github.com/galaxyproject/galaxy/pull/16237>`_
 
 -------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 =========
 Bug fixes
 =========
 
 * 
 * 
+* 
 * Fix assertion linting to not fail on byte suffixes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15873 <https://github.com/galaxyproject/galaxy/pull/15873>`_
 * Fix ``get_test_from_anaconda()`` and ``base_image_for_targets()`` functions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16125 <https://github.com/galaxyproject/galaxy/pull/16125>`_
 * Fix test search for mulled container hashes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16170 <https://github.com/galaxyproject/galaxy/pull/16170>`_
 
 ============
 Enhancements
 ============
 
 * 
+* 
 * Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
 
 -------------------
 22.1.5 (2022-11-14)
 -------------------
 
 * Set test status to success on expected failure
```

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/biotools/interface.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/biotools/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     topic: List[dict]
     function: List[dict]
 
     @staticmethod
     def from_json(from_json: Dict[str, Any]) -> "BiotoolsEntry":
         entry = BiotoolsEntry()
         entry.biotoolsID = from_json["biotoolsID"]
-        entry.topic = from_json["topic"]
-        entry.function = from_json["function"]
+        entry.topic = from_json.get("topic", [])
+        entry.function = from_json.get("function", [])
         return entry
 
     @property
     def edam_info(self) -> ParsedBiotoolsEntry:
         parsed = ParsedBiotoolsEntry()
         parsed.biotoolsID = self.biotoolsID
         parsed.edam_topics = list(set(simplify_edam_dicts(self.topic)))
```

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/biotools/source.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/biotools/source.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/client/staging.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/client/staging.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/cwltool_deps.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/cwltool_deps.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/parser.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/representation.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/representation.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/runnable.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/runnable.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/runtime_actions.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/runtime_actions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/schema.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/cwl/util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/cwl/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/data/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/data/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/data/_schema.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/data/_schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/data/bundles/models.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/data/bundles/models.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/brew_exts.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/brew_exts.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/brew_util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/brew_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/conda_compat.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/conda_compat.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/conda_util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/conda_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_classes.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_classes.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/explicit.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/explicit.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_resolvers/mulled.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_resolvers/mulled.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/container_volumes.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/container_volumes.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/containers.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/containers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/dependencies.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/docker_util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/docker_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/dockerfiles.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/dockerfiles.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/installable.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/installable.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/get_tests.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/get_tests.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/invfile.lua` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/invfile.lua`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build_channel.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build_channel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build_files.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_build_tool.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_build_tool.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_hash.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_hash.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_list.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_list.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_search.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_search.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/mulled/util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/mulled/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/requirements.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/requirements.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/conda.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/conda.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/galaxy_packages.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/galaxy_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/homebrew.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/homebrew.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/lmod.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/lmod.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/modules.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/modules.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/resolver_mixins.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/resolver_mixins.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/tool_shed_packages.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/singularity_util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/singularity_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/deps/views.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/deps/views.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/edam_util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/edam_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/fetcher.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/fetcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/lint.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/lint.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/citations.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/citations.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/command.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/command.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/cwl.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/cwl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/general.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ERROR_NAME_MSG = "Tool name is missing or empty."
 VALID_NAME_MSG = "Tool defines a name [%s]."
 
 ERROR_ID_MSG = "Tool does not define an id attribute."
 VALID_ID_MSG = "Tool defines an id [%s]."
 
-PROFILE_PATTERN = re.compile(r"^[1,2]\d\.[0,1]\d$")
+PROFILE_PATTERN = re.compile(r"^[12]\d\.\d{1,2}$")
 PROFILE_INFO_DEFAULT_MSG = "Tool targets 16.01 Galaxy profile."
 PROFILE_INFO_SPECIFIED_MSG = "Tool specifies profile version [%s]."
 PROFILE_INVALID_MSG = "Tool specifies an invalid profile version [%s]."
 
 WARN_WHITESPACE_MSG = "%s contains whitespace, this may cause errors: [%s]."
 WARN_WHITESPACE_PRESUFFIX = "%s is pre/suffixed by whitespace, this may cause errors: [%s]."
 WARN_ID_WHITESPACE_MSG = "Tool ID contains whitespace - this is discouraged: [%s]."
```

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/help.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/inputs.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/inputs.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/outputs.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,22 @@
         if name is not None:
             if name in names:
                 lint_ctx.error(f"Tool output [{name}] has duplicated name", node=output)
             names.add(name)
 
         label = output.attrib.get("label", "${tool.name} on ${on_string}")
         if label in labels:
-            lint_ctx.error(f"Tool output [{name}] uses duplicated label '{label}'", node=output)
+            filter_node = output.find(".//filter")
+            if filter_node is not None:
+                lint_ctx.warn(
+                    f"Tool output [{name}] uses duplicated label '{label}', double check if filters imply disjoint cases",
+                    node=output,
+                )
+            else:
+                lint_ctx.warn(f"Tool output [{name}] uses duplicated label '{label}'", node=output)
         labels.add(label)
 
         format_set = False
         if __check_format(output, lint_ctx):
             format_set = True
         if output.tag == "data":
             if "auto_format" in output.attrib and output.attrib["auto_format"]:
```

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/stdio.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/tests.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/tests.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/linters/xml_order.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/linters/xml_order.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/loader_directory.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/loader_directory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/locations/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/locations/dockstore.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/locations/dockstore.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/biotools_mappings.tsv` & `galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/biotools_mappings.tsv`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/ontologies/ontology_data.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/ontologies/ontology_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/output_checker.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/output_checker.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/cwl.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/cwl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/factory.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/interface.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/output_actions.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/output_actions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/output_collection_def.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/output_collection_def.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/output_objects.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/output_objects.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/stdio.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/xml.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/xml.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/parser/yaml.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/provided_metadata.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/provided_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/base.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/base.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/filters/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/filters/examples.py.sample` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/filters/examples.py.sample`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/integrated_panel.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/integrated_panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/lineages/factory.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/lineages/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/lineages/interface.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/lineages/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/panel.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/parser.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/tags.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/definitions.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/definitions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/edam.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/edam.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/interface.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/sources.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/sources.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/views/static.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/views/static.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/toolbox/watcher.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/toolbox/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/unittest_utils/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/unittest_utils/interactor.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/unittest_utils/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/__init__.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/_util.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/archive.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/archive.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/hdf5.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/hdf5.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/size.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/size.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/tabular.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/tabular.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/text.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/text.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/asserts/xml.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/asserts/xml.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/interactor.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/interactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,17 +449,15 @@
 
     def test_data_download(self, tool_id, filename, mode="file", is_output=True, tool_version=None):
         result = None
         local_path = None
 
         if self.supports_test_data_download:
             version_fragment = f"&tool_version={tool_version}" if tool_version else ""
-            response = self._get(
-                f"tools/{tool_id}/test_data_download?filename={filename}{version_fragment}", admin=True
-            )
+            response = self._get(f"tools/{tool_id}/test_data_download?filename={filename}{version_fragment}")
             if response.status_code == 200:
                 if mode == "file":
                     result = response.content
                 elif mode == "directory":
                     prefix = os.path.basename(filename)
                     path = tempfile.mkdtemp(prefix=prefix)
                     fileobj = io.BytesIO(response.content)
```

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/script.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/test_config.sample.yml` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/test_config.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/test_data.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/verify/wait.py` & `galaxy-tool-util-23.0.5/galaxy/tool_util/verify/wait.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/LICENSE` & `galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/README.md` & `galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/README.md`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/galaxy.jxb` & `galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/galaxy.jxb`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy/tool_util/xsd/galaxy.xsd` & `galaxy-tool-util-23.0.5/galaxy/tool_util/xsd/galaxy.xsd`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/PKG-INFO` & `galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tool-util
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy tool and tool dependency utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,28 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Allow duplicate labels in linter if outputs contain filters  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15933 <https://github.com/galaxyproject/galaxy/pull/15933>`_
+* Fix parsing tool metadata from bio.tools by `@kysrpex <https://github.com/kysrpex>`_ in `#16449 <https://github.com/galaxyproject/galaxy/pull/16449>`_
+* Linter: fix regex for profile version by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16480 <https://github.com/galaxyproject/galaxy/pull/16480>`_
+* Adjust test_data_download method in GalaxyInteractorApi so an admin user is not required by `@simonbray <https://github.com/simonbray>`_ in `#16482 <https://github.com/galaxyproject/galaxy/pull/16482>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
@@ -78,37 +92,40 @@
 
 
 =========
 Bug fixes
 =========
 
 * 
+* 
 * Don't fail CWL tool parsing when Cheetah not installed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16219 <https://github.com/galaxyproject/galaxy/pull/16219>`_
 * Allow skipping ``expect_num_outputs`` when ``expect_failure`` is set in tool test by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16237 <https://github.com/galaxyproject/galaxy/pull/16237>`_
 
 -------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 =========
 Bug fixes
 =========
 
 * 
 * 
+* 
 * Fix assertion linting to not fail on byte suffixes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15873 <https://github.com/galaxyproject/galaxy/pull/15873>`_
 * Fix ``get_test_from_anaconda()`` and ``base_image_for_targets()`` functions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16125 <https://github.com/galaxyproject/galaxy/pull/16125>`_
 * Fix test search for mulled container hashes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16170 <https://github.com/galaxyproject/galaxy/pull/16170>`_
 
 ============
 Enhancements
 ============
 
 * 
+* 
 * Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
 
 -------------------
 22.1.5 (2022-11-14)
 -------------------
 
 * Set test status to success on expected failure
```

### Comparing `galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/SOURCES.txt` & `galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/galaxy_tool_util.egg-info/entry_points.txt` & `galaxy-tool-util-23.0.5/galaxy_tool_util.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.0.4/setup.cfg` & `galaxy-tool-util-23.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tool-util
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util>=22.1
 	conda-package-streaming
 	lxml
```

