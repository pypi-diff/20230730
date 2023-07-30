# Comparing `tmp/irispie-0.1.0.tar.gz` & `tmp/irispie-0.1.1.tar.gz`

## Comparing `irispie-0.1.0.tar` & `irispie-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,71 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/app.json
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/appearance.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/workspace.json
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/snippets/iris.css
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.0/.obsidian/snippets/no-embed-titles.css
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/.obsidian/app.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/.obsidian/appearance.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/.obsidian/workspace.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/architecture/Untitled.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/architecture/steady.canvas
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.0/docs/series/example.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/__init__.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/exceptions.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/incidence.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/quantities.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/requirements
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/session
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/tags
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/test.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/__init__.py
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/databanks.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/dataslabs.py
--rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/dates.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/exports.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/filters.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/imports.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/imports2.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/plotly.py
--rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/series.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/dataman/views.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/equators/abc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/equators/steady.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/jacobians/abc.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/mixins/userdata.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/__init__.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/facade.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/flags.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/gettables.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/invariants.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/simulatables.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/sources.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/steadiables.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/model_source_parser.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.0/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.0/tests/.gitkeep
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 irispie-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.0/LICENCE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 irispie-0.1.0/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 irispie-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 irispie-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 irispie-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/series/example.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/__init__.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/incidence.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/quantities.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/requirements
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/session
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/tags
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/test.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/__init__.py
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/databanks.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/dataslabs.py
+-rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/dates.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/exports.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/filters.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/imports.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/imports2.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/plotly.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/series.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/views.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/abc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/jacobians/abc.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/mixins/userdata.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/facade.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/flags.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/gettables.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/simulatables.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/sources.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/steadiables.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/model_source_parser.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.1/tests/.gitkeep
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.1/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.1/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 irispie-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 irispie-0.1.1/PKG-INFO
```

### Comparing `irispie-0.1.0/docs/algorithms/detach-unit-roots.md` & `irispie-0.1.1/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/docs/milestones/March-2023.md` & `irispie-0.1.1/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/docs/milestones/iris-gray.png` & `irispie-0.1.1/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/docs/series/example.py` & `irispie-0.1.1/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/equations.py` & `irispie-0.1.1/src/irispie/equations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/exceptions.py` & `irispie-0.1.1/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/incidence.py` & `irispie-0.1.1/src/irispie/incidence.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/quantities.py` & `irispie-0.1.1/src/irispie/quantities.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/requirements` & `irispie-0.1.1/src/irispie/requirements`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/session` & `irispie-0.1.1/src/irispie/session`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/tags` & `irispie-0.1.1/src/irispie/tags`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/wrongdoings.py` & `irispie-0.1.1/src/irispie/wrongdoings.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/aldi/adaptations.py` & `irispie-0.1.1/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/aldi/differentiators.py` & `irispie-0.1.1/src/irispie/aldi/differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/aldi/express.py~` & `irispie-0.1.1/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/aldi/finite_differentiators.py` & `irispie-0.1.1/src/irispie/aldi/finite_differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/aldi/invariators.py` & `irispie-0.1.1/src/irispie/aldi/invariators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/aldi/maps.py` & `irispie-0.1.1/src/irispie/aldi/maps.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/databanks.py` & `irispie-0.1.1/src/irispie/dataman/databanks.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/dataslabs.py` & `irispie-0.1.1/src/irispie/dataman/dataslabs.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/dates.py` & `irispie-0.1.1/src/irispie/dataman/dates.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/exports.py` & `irispie-0.1.1/src/irispie/dataman/exports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/filters.py` & `irispie-0.1.1/src/irispie/dataman/filters.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/imports.py` & `irispie-0.1.1/src/irispie/dataman/imports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/imports2.py` & `irispie-0.1.1/src/irispie/dataman/imports2.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/plotly.py` & `irispie-0.1.1/src/irispie/dataman/plotly.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/series.py` & `irispie-0.1.1/src/irispie/dataman/series.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/dataman/views.py` & `irispie-0.1.1/src/irispie/dataman/views.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/equators/abc.py` & `irispie-0.1.1/src/irispie/equators/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/equators/plain.py` & `irispie-0.1.1/src/irispie/equators/plain.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/equators/steady.py` & `irispie-0.1.1/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/evaluators/printers.py` & `irispie-0.1.1/src/irispie/evaluators/printers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/evaluators/steady.py` & `irispie-0.1.1/src/irispie/evaluators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/fords/descriptors.py` & `irispie-0.1.1/src/irispie/fords/descriptors.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/fords/simulators.py` & `irispie-0.1.1/src/irispie/fords/simulators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/fords/solutions.py` & `irispie-0.1.1/src/irispie/fords/solutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/fords/steadiers.py` & `irispie-0.1.1/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/fords/systems.py` & `irispie-0.1.1/src/irispie/fords/systems.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/jacobians/abc.py` & `irispie-0.1.1/src/irispie/jacobians/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/jacobians/steady.py` & `irispie-0.1.1/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/facade.py` & `irispie-0.1.1/src/irispie/models/facade.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/flags.py` & `irispie-0.1.1/src/irispie/models/flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/gettables.py` & `irispie-0.1.1/src/irispie/models/gettables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/invariants.py` & `irispie-0.1.1/src/irispie/models/invariants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/simulatables.py` & `irispie-0.1.1/src/irispie/models/simulatables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/sources.py` & `irispie-0.1.1/src/irispie/models/sources.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/steadiables.py` & `irispie-0.1.1/src/irispie/models/steadiables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/models/variants.py` & `irispie-0.1.1/src/irispie/models/variants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/parsers/common.py` & `irispie-0.1.1/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/parsers/model_source_parser.py` & `irispie-0.1.1/src/irispie/parsers/model_source_parser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/parsers/preparser.py` & `irispie-0.1.1/src/irispie/parsers/preparser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/parsers/pseudofunctions.py` & `irispie-0.1.1/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/src/irispie/parsers/substitutions.py` & `irispie-0.1.1/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/LICENCE` & `irispie-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.1.0/pyproject.toml` & `irispie-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.1.0"
+    version = "0.1.1"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
-    description = "Macroeocnomic modeling package"
+    description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```

### Comparing `irispie-0.1.0/PKG-INFO` & `irispie-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.1.0
-Summary: Macroeocnomic modeling package
+Version: 0.1.1
+Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Iris Pie
 
-A macroeconomic modeling package for Python
+Macroeconomic modeling package for Python
+
```

