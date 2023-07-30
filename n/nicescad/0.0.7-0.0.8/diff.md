# Comparing `tmp/nicescad-0.0.7.tar.gz` & `tmp/nicescad-0.0.8.tar.gz`

## Comparing `nicescad-0.0.7.tar` & `nicescad-0.0.8.tar`

### file list

```diff
@@ -1,87 +1,91 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.7/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.7/.pydevproject
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.7/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/__init__.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/axes_helper.py
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/blockscad_converter.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/file_selector.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/local_filepicker.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/nicescad_cmd.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/openscad.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/process.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/profiler.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/solidservice.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/version.py
--rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/webserver.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad/web/static/css/pygments.css
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/nicescad_logo.scad
--rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/A10BedLevelKnob.xml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/cube.xml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/cylinder.xml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/blockscad/sphere.xml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/cube.scad
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/cylinder.scad
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/sphere.scad
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/intersection.scad
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/openjscad_logo.scad
--rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/openjscad_logo.stl
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/animation.scad
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/difference.scad
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/offset.scad
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/search.scad
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/translation.scad
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG.scad
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children.scad
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/intersection.scad
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo.scad
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/projection.scad
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface.scad
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/translate.scad
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/union.scad
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/text.scad
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/functions.scad
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/recursion.scad
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/fence.scad
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/install
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/openscad_example_scraper.py
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.7/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/basetest.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_blockscad_converter.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_file_selector.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_openscad.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_solidservice.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.7/tests/test_subprocess.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.7/LICENSE
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nicescad-0.0.7/README.md
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 nicescad-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 nicescad-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.8/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.8/.pydevproject
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.8/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 nicescad-0.0.8/docker/Dockerfile.nicescad
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 nicescad-0.0.8/docker/Dockerfile.p2scad
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 nicescad-0.0.8/docker/docker-compose.yml
+-rwxr-xr-x   0        0        0     3128 2020-02-02 00:00:00.000000 nicescad-0.0.8/docker/start_nicescad
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/__init__.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/axes_helper.py
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/blockscad_converter.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/file_selector.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/local_filepicker.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/nicescad_cmd.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/openscad.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/process.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/profiler.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/solidservice.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/version.py
+-rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/webserver.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad/web/static/css/pygments.css
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/nicescad_logo.scad
+-rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/blockscad/A10BedLevelKnob.xml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/blockscad/cube.xml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/blockscad/cylinder.xml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/blockscad/sphere.xml
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/blockscad_converted/cube.scad
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/blockscad_converted/cylinder.scad
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/blockscad_converted/sphere.scad
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/intersection.scad
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/openjscad_logo.scad
+-rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/openjscad_logo.stl
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/animation.scad
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/difference.scad
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/offset.scad
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/search.scad
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/translation.scad
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/CSG.scad
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/children.scad
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/intersection.scad
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/logo.scad
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/projection.scad
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/surface.scad
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/translate.scad
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/union.scad
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Extrusion/text.scad
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Functions/functions.scad
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Functions/recursion.scad
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/fence.scad
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.8/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.8/scripts/install
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.8/scripts/openscad_example_scraper.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.8/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/basetest.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/test_blockscad_converter.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/test_file_selector.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/test_openscad.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/test_solidservice.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.8/tests/test_subprocess.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nicescad-0.0.8/README.md
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nicescad-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 nicescad-0.0.8/PKG-INFO
```

### Comparing `nicescad-0.0.7/.github/workflows/build.yml` & `nicescad-0.0.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/.github/workflows/upload-to-pypi.yml` & `nicescad-0.0.8/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/axes_helper.py` & `nicescad-0.0.8/nicescad/axes_helper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/blockscad_converter.py` & `nicescad-0.0.8/nicescad/blockscad_converter.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/file_selector.py` & `nicescad-0.0.8/nicescad/file_selector.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/local_filepicker.py` & `nicescad-0.0.8/nicescad/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/nicescad_cmd.py` & `nicescad-0.0.8/nicescad/nicescad_cmd.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/openscad.py` & `nicescad-0.0.8/nicescad/openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/process.py` & `nicescad-0.0.8/nicescad/process.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/profiler.py` & `nicescad-0.0.8/nicescad/profiler.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/solidservice.py` & `nicescad-0.0.8/nicescad/solidservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
         return {"openscad_code": openscad_code}
 
 def main():
     parser = argparse.ArgumentParser(description="Convert Python code to OpenSCAD code.")
     parser.add_argument("--python_code", help="Python code to convert to OpenSCAD code.")
     parser.add_argument("--file", help="File containing Python code to convert to OpenSCAD code.")
     parser.add_argument("--serve", action="store_true", help="Start the FastAPI server.")
+    parser.add_argument("--host", default="0.0.0.0", help="Host address to bind the server to.")
+    parser.add_argument("--port", default=8000, type=int, help="Port number to bind the server to.")
+ 
     args = parser.parse_args()
 
     if args.serve:
         server = FastAPIServer()
         uvicorn.run(server.app, host="0.0.0.0", port=8000)
     else:
         if args.file:
```

### Comparing `nicescad-0.0.7/nicescad/version.py` & `nicescad-0.0.8/nicescad/version.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/webserver.py` & `nicescad-0.0.8/nicescad/webserver.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad/web/static/css/pygments.css` & `nicescad-0.0.8/nicescad/web/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/nicescad_logo.scad` & `nicescad-0.0.8/nicescad_examples/nicescad_logo.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/blockscad/A10BedLevelKnob.xml` & `nicescad-0.0.8/nicescad_examples/blockscad/A10BedLevelKnob.xml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/blockscad/cube.xml` & `nicescad-0.0.8/nicescad_examples/blockscad/cube.xml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/blockscad/cylinder.xml` & `nicescad-0.0.8/nicescad_examples/blockscad/cylinder.xml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad` & `nicescad-0.0.8/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/intersection.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/openjscad_logo.stl` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/openjscad_logo.stl`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/animation.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/animation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/difference.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/difference.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/offset.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/offset.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/search.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/search.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Advanced/translation.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Advanced/translation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/CSG.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/CSG.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/children.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/intersection.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/logo.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/projection.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/projection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/surface.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/translate.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/translate.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Basics/union.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Basics/union.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Extrusion/text.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Extrusion/text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/functions.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Functions/functions.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Functions/recursion.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Functions/recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/fence.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/fence.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad` & `nicescad-0.0.8/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/scripts/doc` & `nicescad-0.0.8/scripts/doc`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/scripts/openscad_example_scraper.py` & `nicescad-0.0.8/scripts/openscad_example_scraper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/tests/basetest.py` & `nicescad-0.0.8/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/tests/test_blockscad_converter.py` & `nicescad-0.0.8/tests/test_blockscad_converter.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/tests/test_file_selector.py` & `nicescad-0.0.8/tests/test_file_selector.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/tests/test_openscad.py` & `nicescad-0.0.8/tests/test_openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/tests/test_solidservice.py` & `nicescad-0.0.8/tests/test_solidservice.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/tests/test_subprocess.py` & `nicescad-0.0.8/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/.gitignore` & `nicescad-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/LICENSE` & `nicescad-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/README.md` & `nicescad-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.7/pyproject.toml` & `nicescad-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 	# https://pypi.org/project/pywin32/
 	'pywin32; platform_system=="Windows"',
 	# https://pypi.org/project/requests/
 	"requests",
 	# https://pypi.org/project/Pygments/
 	"pygments",
 	# nicegui
+    # fastapi
+	# uvicorn
     "nicegui>=1.3.5",
     # openai
-    "openai"
+    "openai",
+	# pydantic
+	"pydantic>=1.8.2"
 ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `nicescad-0.0.7/PKG-INFO` & `nicescad-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicescad
-Version: 0.0.7
+Version: 0.0.8
 Project-URL: Home, https://github.com/WolfgangFahl/nicescad
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicescad
 Project-URL: Source, https://github.com/WolfgangFahl/nicescad
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: nicegui>=1.3.5
 Requires-Dist: openai
+Requires-Dist: pydantic>=1.8.2
 Requires-Dist: pygments
 Requires-Dist: pywin32; platform_system == 'Windows'
 Requires-Dist: requests
 Requires-Dist: solidpython2>=2.0.2
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
```

