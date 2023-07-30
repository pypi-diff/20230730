# Comparing `tmp/nicescad-0.0.6.tar.gz` & `tmp/nicescad-0.0.7.tar.gz`

## Comparing `nicescad-0.0.6.tar` & `nicescad-0.0.7.tar`

### file list

```diff
@@ -1,78 +1,87 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.6/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.6/.pydevproject
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.6/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/__init__.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/axes_helper.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/blockscad_converter.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/file_selector.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/local_filepicker.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/nicescad_cmd.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/openscad.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/process.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/profiler.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/version.py
--rw-r--r--   0        0        0    16566 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/webserver.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/web/static/css/pygments.css
--rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/blockscad/A10BedLevelKnob.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/intersection.scad
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/openjscad_logo.scad
--rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/openjscad_logo.stl
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/animation.scad
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/difference.scad
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/offset.scad
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/search.scad
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/translation.scad
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG.scad
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children.scad
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/intersection.scad
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo.scad
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/projection.scad
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface.scad
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/translate.scad
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/union.scad
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/text.scad
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/functions.scad
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/recursion.scad
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/fence.scad
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/install
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/openscad_example_scraper.py
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/basetest.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_blockscad_converter.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_file_selector.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_openscad.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_subprocess.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.6/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.6/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.7/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.7/.pydevproject
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.7/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/__init__.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/axes_helper.py
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/blockscad_converter.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/file_selector.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/local_filepicker.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/nicescad_cmd.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/openscad.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/process.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/profiler.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/solidservice.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/version.py
+-rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/webserver.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/web/static/css/pygments.css
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/nicescad_logo.scad
+-rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/A10BedLevelKnob.xml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/cube.xml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/cylinder.xml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/sphere.xml
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/cube.scad
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/cylinder.scad
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/sphere.scad
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/intersection.scad
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/openjscad_logo.scad
+-rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/openjscad_logo.stl
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/animation.scad
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/difference.scad
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/offset.scad
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/search.scad
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/translation.scad
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG.scad
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children.scad
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/intersection.scad
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo.scad
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/projection.scad
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface.scad
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/translate.scad
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/union.scad
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/text.scad
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/functions.scad
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/recursion.scad
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/fence.scad
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/install
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/openscad_example_scraper.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/basetest.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_blockscad_converter.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_file_selector.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_openscad.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_solidservice.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_subprocess.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nicescad-0.0.7/README.md
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 nicescad-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 nicescad-0.0.7/PKG-INFO
```

### Comparing `nicescad-0.0.6/.github/workflows/build.yml` & `nicescad-0.0.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/.github/workflows/upload-to-pypi.yml` & `nicescad-0.0.7/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/axes_helper.py` & `nicescad-0.0.7/nicescad/axes_helper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/file_selector.py` & `nicescad-0.0.7/nicescad/file_selector.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/local_filepicker.py` & `nicescad-0.0.7/nicescad/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/nicescad_cmd.py` & `nicescad-0.0.7/nicescad/nicescad_cmd.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/openscad.py` & `nicescad-0.0.7/nicescad/openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/process.py` & `nicescad-0.0.7/nicescad/process.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/profiler.py` & `nicescad-0.0.7/nicescad/profiler.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/version.py` & `nicescad-0.0.7/nicescad/version.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad/webserver.py` & `nicescad-0.0.7/nicescad/webserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
      cube(30,center=true);
      sphere(20);
   }
 }
 example();"""        
         self.input="example.scad"
         self.stl_name="result.stl"
+        self.stl_color="#57B6A9"
         self.stl_object=None
         self.is_local=False
         app.add_static_files('/stl', self.oscad.tmp_dir)
         self.log_view=None
         self.do_trace=True
         self.html_view=None
         self.axes_view=None
@@ -87,28 +88,29 @@
         Args:
             click_args (object): The click event arguments.
         """
         try:
             self.progress_view.visible = True
             ui.notify("rendering ...")
             with self.scene:
-                self.scene.clear()
                 self.stl_link.visible=False
                 self.color_picker_button.disable()
             openscad_str = self.code_area.value
             stl_path=stl_path = os.path.join(self.oscad.tmp_dir, self.stl_name) 
             render_result= await self.oscad.openscad_str_to_file(openscad_str,stl_path)
             # show render result in log
             self.log_view.push(render_result.stderr)
             if render_result.returncode==0:
                 ui.notify("stl created ... loading into scene")
                 self.stl_link.visible=True
                 self.color_picker_button.enable()
                 with self.scene:
-                    self.stl_object=self.scene.stl(f"/stl/{self.stl_name}").move(x=0.0).scale(0.1)    
+                    self.stl_object=self.scene.stl(f"/stl/{self.stl_name}").move(x=0.0).scale(0.1) 
+                    self.stl_object.name=self.stl_name   
+                    self.stl_object.material(self.stl_color)
         except BaseException as ex:
             self.handle_exception(ex,self.do_trace)  
         self.progress_view.visible=False  
             
     def do_read_input(self, input_str: str):
         """Reads the given input.
 
@@ -320,14 +322,15 @@
     
         Note:
             If 'stl_object' is None, the function will only change the color of 'color_picker_button'.
             Otherwise, it changes the color of both 'color_picker_button' and 'stl_object'.
         """
         self.color_picker_button.style(f'background-color:{e.color}!important')
         if self.stl_object:
+            self.stl_color=e.color
             self.stl_object.material(f'{e.color}')
         pass
     
     async def toggle_axes(self):
         """
         toggle the axes of my scene
         """
@@ -341,17 +344,21 @@
     async def toggle_grid(self,_ea):
         """
         toogle the grid of my scene
         """
         try:
             grid=self.scene._props["grid"]
             grid_str="off" if grid else "on"
+            grid_js="false" if grid else "true"
             # try toggling grid
             ui.notify(f"setting grid to {grid_str}")
             grid=not grid
+            # workaround according to https://github.com/zauberzeug/nicegui/discussions/1246
+            js_cmd=f'scene_c{self.scene.id}.children.find(c => c.type === "GridHelper").visible = {grid_js}'
+            await ui.run_javascript(js_cmd, respond=False)
             self.scene._props["grid"]=grid
             self.scene.update()
             # try toggling icon
             self.toggle_icon(self.grid_button)
         except BaseException as ex:
             self.handleExeption(ex)
         pass
@@ -361,15 +368,15 @@
         self.setup_pygments()
         self.setup_menu()
         with ui.column():
             with ui.splitter() as splitter:
                 with splitter.before:
                     self.grid_button=self.tool_button("toggle grid",handler=self.toggle_grid,icon='grid_off',toggle_icon='grid_on')
                     self.axes_button=self.tool_button("toggle axes",icon="polyline",toggle_icon="square",handler=self.toggle_axes)
-                    self.color_picker_button=ui.button(icon='colorize')     
+                    self.color_picker_button=ui.button(icon='colorize',color=self.stl_color)     
                     with self.color_picker_button: 
                         self.color_picker = ui.color_picker(on_pick=self.pick_color)
                     self.color_picker_button.disable()
                     
                     with ui.scene(width=1024, height=768).classes("w-full") as scene:
                         self.scene = scene
                         scene.spot_light(distance=100, intensity=0.2).move(-10, 0, 10)
```

### Comparing `nicescad-0.0.6/nicescad/web/static/css/pygments.css` & `nicescad-0.0.7/nicescad/web/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/intersection.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/openjscad_logo.stl` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/openjscad_logo.stl`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/animation.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/animation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/difference.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/difference.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/offset.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/offset.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/search.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/search.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/translation.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/translation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/intersection.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/projection.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/projection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/translate.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/translate.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/union.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/union.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/text.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/functions.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/functions.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/recursion.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/fence.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/fence.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad` & `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/scripts/doc` & `nicescad-0.0.7/scripts/doc`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/scripts/openscad_example_scraper.py` & `nicescad-0.0.7/scripts/openscad_example_scraper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/tests/basetest.py` & `nicescad-0.0.7/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/tests/test_file_selector.py` & `nicescad-0.0.7/tests/test_file_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def test_get_dir_tree(self):
         """
         test getting the directory tree structure for
         the examples directory
         """
         file_selector=FileSelector(WebServer.examples_path(),".scad")
         debug=self.debug
-        debug=True
+        #debug=True
         if debug:
             print(json.dumps(file_selector.tree_structure, indent=2))
         self.assertTrue("id" in file_selector.tree_structure)
         sample_id="1.1.1.1"
         node=file_selector.find_node_by_id(file_selector.tree_structure,sample_id)
         if debug:
             print(json.dumps(node,indent=2))
```

### Comparing `nicescad-0.0.6/tests/test_openscad.py` & `nicescad-0.0.7/tests/test_openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/tests/test_subprocess.py` & `nicescad-0.0.7/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/.gitignore` & `nicescad-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/LICENSE` & `nicescad-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.6/README.md` & `nicescad-0.0.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -18,8 +18,18 @@
 ## Examples
 * [Basics/logo](https://raw.githubusercontent.com/openscad/openscad/master/examples/Basics/logo.scad)
 * [Intersection](https://raw.githubusercontent.com/WolfgangFahl/nicescad/main/examples/intersection.scad)
 
 ## Links
 * https://openscad.org/
 * https://nicegui.io
+### Alternative online editors
 * https://ochafik.com/openscad2/
+* http://www.implicitcad.org/editor
+* https://www.blockscad3d.com/editor/
+* https://openjscad.azurewebsites.net/
+* https://openjscad.xyz/
+### Jupyter notebook integration
+* https://github.com/nickc92/ViewSCAD
+### Python integration
+* https://github.com/jeff-dh/SolidPython
+
```

### Comparing `nicescad-0.0.6/pyproject.toml` & `nicescad-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 	# https://pypi.org/project/pywin32/
 	'pywin32; platform_system=="Windows"',
 	# https://pypi.org/project/requests/
 	"requests",
 	# https://pypi.org/project/Pygments/
 	"pygments",
 	# nicegui
-    'nicegui>=1.3.5',
+    "nicegui>=1.3.5",
+    # openai
+    "openai"
 ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
@@ -60,7 +62,8 @@
 
 [tool.hatch.build.targets.wheel.sources]
 "nicescad" = "nicescad"
 "nicescad_examples" = "nicescad_examples"
 
 [project.scripts]
 nicescad = "nicescad.nicescad_cmd:main"
+p2scad = "nicescad.solidservice:main"
```

### Comparing `nicescad-0.0.6/PKG-INFO` & `nicescad-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicescad
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: Home, https://github.com/WolfgangFahl/nicescad
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicescad
 Project-URL: Source, https://github.com/WolfgangFahl/nicescad
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: nicegui>=1.3.5
+Requires-Dist: openai
 Requires-Dist: pygments
 Requires-Dist: pywin32; platform_system == 'Windows'
 Requires-Dist: requests
 Requires-Dist: solidpython2>=2.0.2
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
@@ -51,8 +52,18 @@
 ## Examples
 * [Basics/logo](https://raw.githubusercontent.com/openscad/openscad/master/examples/Basics/logo.scad)
 * [Intersection](https://raw.githubusercontent.com/WolfgangFahl/nicescad/main/examples/intersection.scad)
 
 ## Links
 * https://openscad.org/
 * https://nicegui.io
+### Alternative online editors
 * https://ochafik.com/openscad2/
+* http://www.implicitcad.org/editor
+* https://www.blockscad3d.com/editor/
+* https://openjscad.azurewebsites.net/
+* https://openjscad.xyz/
+### Jupyter notebook integration
+* https://github.com/nickc92/ViewSCAD
+### Python integration
+* https://github.com/jeff-dh/SolidPython
+
```

