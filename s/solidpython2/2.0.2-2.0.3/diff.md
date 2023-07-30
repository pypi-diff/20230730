# Comparing `tmp/solidpython2-2.0.2.tar.gz` & `tmp/solidpython2-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidpython2-2.0.2.tar", max compression
+gzip compressed data, was "solidpython2-2.0.3.tar", max compression
```

## Comparing `solidpython2-2.0.2.tar` & `solidpython2-2.0.3.tar`

### file list

```diff
@@ -1,253 +1,254 @@
--rw-r--r--   0        0        0    22930 2023-03-15 13:23:46.110122 solidpython2-2.0.2/README.rst
--rw-r--r--   0        0        0     1116 2023-05-09 10:27:48.203458 solidpython2-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      108 2023-04-24 23:08:31.053339 solidpython2-2.0.2/solid2/__init__.py
--rw-r--r--   0        0        0     1681 2023-04-26 10:51:37.721722 solidpython2-2.0.2/solid2/config.py
--rw-r--r--   0        0        0      381 2023-05-09 10:20:41.792164 solidpython2-2.0.2/solid2/core/__init__.py
--rw-r--r--   0        0        0       53 2023-04-26 17:53:48.422660 solidpython2-2.0.2/solid2/core/builtins/__init__.py
--rw-r--r--   0        0        0     3633 2023-04-21 22:55:04.234686 solidpython2-2.0.2/solid2/core/builtins/convenience.py
--rw-r--r--   0        0        0     1040 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/implicit.primitives
--rw-r--r--   0        0        0      754 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/openscad.mutators
--rw-r--r--   0        0        0     1968 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/openscad.primitives
--rw-r--r--   0        0        0    25400 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/openscad_primitives.py
--rw-r--r--   0        0        0      367 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/primitives.py
--rw-r--r--   0        0        0      938 2022-09-03 20:01:15.234639 solidpython2-2.0.2/solid2/core/extension_manager.py
--rw-r--r--   0        0        0       32 2023-03-19 13:30:20.199884 solidpython2-2.0.2/solid2/core/object_base/__init__.py
--rw-r--r--   0        0        0     3522 2023-03-20 14:58:07.769013 solidpython2-2.0.2/solid2/core/object_base/access_syntax_mixin.py
--rw-r--r--   0        0        0     6866 2023-05-02 10:30:45.741949 solidpython2-2.0.2/solid2/core/object_base/object_base_impl.py
--rw-r--r--   0        0        0     2253 2023-03-20 14:58:07.769013 solidpython2-2.0.2/solid2/core/object_base/operator_mixin.py
--rw-r--r--   0        0        0     3994 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/core/object_factory.py
--rw-r--r--   0        0        0     3428 2023-04-26 10:51:10.097683 solidpython2-2.0.2/solid2/core/parse_scad.py
--rw-r--r--   0        0        0     5489 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/scad_import.py
--rw-r--r--   0        0        0     3051 2023-05-02 10:30:37.857979 solidpython2-2.0.2/solid2/core/scad_render.py
--rw-r--r--   0        0        0     2016 2023-04-24 10:34:26.227909 solidpython2-2.0.2/solid2/core/utils.py
--rwxr-xr-x   0        0        0      559 2023-04-28 10:25:21.909011 solidpython2-2.0.2/solid2/examples/01-basics.py
--rwxr-xr-x   0        0        0      846 2023-04-21 12:24:05.601732 solidpython2-2.0.2/solid2/examples/02-vars-and-operators.py
--rwxr-xr-x   0        0        0      647 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/03-debug-background.py
--rwxr-xr-x   0        0        0     1272 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/04-convenience.py
--rwxr-xr-x   0        0        0      934 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/05-access-style-syntax.py
--rwxr-xr-x   0        0        0     1182 2023-03-15 22:58:40.236989 solidpython2-2.0.2/solid2/examples/06-functions.py
--rwxr-xr-x   0        0        0      425 2023-04-24 18:27:22.516007 solidpython2-2.0.2/solid2/examples/07-libs-bosl2-attachable.py
--rw-r--r--   0        0        0     3329 2023-04-11 09:39:25.912704 solidpython2-2.0.2/solid2/examples/07-libs-bosl2-logo.py
--rwxr-xr-x   0        0        0     1762 2023-04-23 11:52:48.014465 solidpython2-2.0.2/solid2/examples/07-libs-bosl2.py
--rwxr-xr-x   0        0        0      620 2023-04-21 23:01:13.315397 solidpython2-2.0.2/solid2/examples/07-libs.x.py
--rwxr-xr-x   0        0        0     2448 2023-03-20 14:58:07.769013 solidpython2-2.0.2/solid2/examples/08-extensions.py
--rwxr-xr-x   0        0        0     1656 2023-04-24 18:33:54.580435 solidpython2-2.0.2/solid2/examples/09-code-attach-extension.py
--rwxr-xr-x   0        0        0      906 2023-04-21 22:55:04.234686 solidpython2-2.0.2/solid2/examples/10-customizer.py
--rw-r--r--   0        0        0      158 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/11-font/LICENSE_README
--rw-r--r--   0        0        0    47404 2022-08-12 15:59:10.187877 solidpython2-2.0.2/solid2/examples/11-font/RichEatin.otf
--rwxr-xr-x   0        0        0      192 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/examples/11-fonts.x.py
--rwxr-xr-x   0        0        0      335 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/examples/12-animation.py
--rwxr-xr-x   0        0        0     2032 2023-03-19 12:43:05.625475 solidpython2-2.0.2/solid2/examples/13-animated-bouncing-ball.py
--rwxr-xr-x   0        0        0     1381 2023-04-21 23:01:13.315397 solidpython2-2.0.2/solid2/examples/14-implicitCAD.x.py
--rwxr-xr-x   0        0        0     1794 2023-04-21 23:01:13.315397 solidpython2-2.0.2/solid2/examples/15-implicitCAD2.x.py
--rwxr-xr-x   0        0        0     1102 2022-08-12 15:59:10.187877 solidpython2-2.0.2/solid2/examples/16-mazebox-bosl2.py
--rwxr-xr-x   0        0        0     2243 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/examples/17-greedy-scad-interface.py
--rw-r--r--   0        0        0     1196 2022-08-12 15:59:10.187877 solidpython2-2.0.2/solid2/examples/maze7.png
--rw-r--r--   0        0        0        1 2023-04-24 16:33:55.353741 solidpython2-2.0.2/solid2/extensions/__init__.py
--rw-r--r--   0        0        0       51 2023-04-21 22:55:14.018704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.git
--rw-r--r--   0        0        0      522 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      655 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      318 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/check_for_tabs.json
--rw-r--r--   0        0        0      307 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/openscad_docsgen.json
--rw-r--r--   0        0        0     1214 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_docs.yml
--rw-r--r--   0        0        0     1448 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_tutorials.yml
--rw-r--r--   0        0        0     2823 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/main.yml
--rw-r--r--   0        0        0     1253 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.gitignore
--rw-r--r--   0        0        0     1197 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.openscad_docsgen_rc
--rw-r--r--   0        0        0      132 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.openscad_mdimggen_rc
--rw-r--r--   0        0        0     2142 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1323 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/LICENSE
--rw-r--r--   0        0        0     2926 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/README.md
--rw-r--r--   0        0        0    37745 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/WRITING_DOCS.md
--rw-r--r--   0        0        0    18422 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/affine.scad
--rw-r--r--   0        0        0   158011 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/attachments.scad
--rw-r--r--   0        0        0    10326 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/ball_bearings.scad
--rw-r--r--   0        0        0    76076 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/beziers.scad
--rw-r--r--   0        0        0     3557 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bosl1compat.scad
--rw-r--r--   0        0        0    53194 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bottlecaps.scad
--rw-r--r--   0        0        0     1257 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/builtins.scad
--rw-r--r--   0        0        0     8302 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/color.scad
--rw-r--r--   0        0        0    40080 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/comparisons.scad
--rw-r--r--   0        0        0     9779 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/constants.scad
--rw-r--r--   0        0        0    18570 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/coords.scad
--rw-r--r--   0        0        0    28607 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/cubetruss.scad
--rw-r--r--   0        0        0    88642 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/distributors.scad
--rw-r--r--   0        0        0    62214 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/drawing.scad
--rw-r--r--   0        0        0     1389 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/BOSL2logo.scad
--rw-r--r--   0        0        0      559 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/attachments.scad
--rw-r--r--   0        0        0     1344 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/boolean_geometry.scad
--rw-r--r--   0        0        0      505 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/fractal_tree.scad
--rw-r--r--   0        0        0     4168 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/lsystems.scad
--rw-r--r--   0        0        0     2465 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/orientations.scad
--rw-r--r--   0        0        0      704 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/spherical_patch.scad
--rw-r--r--   0        0        0    56985 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/fnliterals.scad
--rw-r--r--   0        0        0    65959 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/gears.scad
--rw-r--r--   0        0        0   125434 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/geometry.scad
--rw-r--r--   0        0        0    31047 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/hinges.scad
--rw-r--r--   0        0        0   117043 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/images/BOSL2logo.png
--rw-r--r--   0        0        0    58197 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/joiners.scad
--rw-r--r--   0        0        0    31481 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linalg.scad
--rw-r--r--   0        0        0     8378 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linear_bearings.scad
--rw-r--r--   0        0        0    47932 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/lists.scad
--rw-r--r--   0        0        0    24740 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks2d.scad
--rw-r--r--   0        0        0    26185 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks3d.scad
--rw-r--r--   0        0        0    54569 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/math.scad
--rw-r--r--   0        0        0    23837 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/metric_screws.scad
--rw-r--r--   0        0        0     9089 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/modular_hose.scad
--rw-r--r--   0        0        0    21204 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/mutators.scad
--rw-r--r--   0        0        0    10102 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/nema_steppers.scad
--rw-r--r--   0        0        0    25544 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/partitions.scad
--rw-r--r--   0        0        0    55148 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/paths.scad
--rw-r--r--   0        0        0    44343 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/polyhedra.scad
--rw-r--r--   0        0        0    62670 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/regions.scad
--rw-r--r--   0        0        0   220660 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/rounding.scad
--rw-r--r--   0        0        0    14301 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screw_drive.scad
--rw-r--r--   0        0        0   179010 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screws.scad
--rwxr-xr-x   0        0        0      115 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/check_for_tabs.sh
--rwxr-xr-x   0        0        0      569 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/find_modular_asserts.sh
--rwxr-xr-x   0        0        0     2784 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/func_coverage.py
--rwxr-xr-x   0        0        0     2345 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/img2scad.py
--rwxr-xr-x   0        0        0      545 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/increment_version.sh
--rwxr-xr-x   0        0        0      511 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/linecount.sh
--rwxr-xr-x   0        0        0      368 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/purge_wiki_history.sh
--rwxr-xr-x   0        0        0      790 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/run_tests.sh
--rw-r--r--   0        0        0    91055 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes2d.scad
--rw-r--r--   0        0        0   181418 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes3d.scad
--rw-r--r--   0        0        0   238386 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/skin.scad
--rw-r--r--   0        0        0     6786 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/sliders.scad
--rw-r--r--   0        0        0     1071 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/std.scad
--rw-r--r--   0        0        0    34155 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/strings.scad
--rw-r--r--   0        0        0     5355 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/structs.scad
--rw-r--r--   0        0        0      186 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/README.txt
--rw-r--r--   0        0        0     1443 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/polyhedra.scad
--rw-r--r--   0        0        0     4998 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_affine.scad
--rw-r--r--   0        0        0      371 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_attachments.scad
--rw-r--r--   0        0        0    16598 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_comparisons.scad
--rw-r--r--   0        0        0    12026 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_coords.scad
--rw-r--r--   0        0        0      393 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_cubetruss.scad
--rw-r--r--   0        0        0      999 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_distributors.scad
--rw-r--r--   0        0        0     5679 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_drawing.scad
--rw-r--r--   0        0        0     9824 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_edges.scad
--rw-r--r--   0        0        0    23237 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_fnliterals.scad
--rw-r--r--   0        0        0    62561 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_geometry.scad
--rw-r--r--   0        0        0    11660 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_linalg.scad
--rw-r--r--   0        0        0      425 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_linear_bearings.scad
--rw-r--r--   0        0        0    13578 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_lists.scad
--rw-r--r--   0        0        0     8961 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_masks2d.scad
--rw-r--r--   0        0        0    26667 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_math.scad
--rw-r--r--   0        0        0     1351 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_mutators.scad
--rw-r--r--   0        0        0    12273 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_paths.scad
--rw-r--r--   0        0        0     7958 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_regions.scad
--rw-r--r--   0        0        0     8862 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_rounding.scad
--rw-r--r--   0        0        0      700 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_screw_drive.scad
--rw-r--r--   0        0        0    64080 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_shapes2d.scad
--rw-r--r--   0        0        0    24086 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_shapes3d.scad
--rw-r--r--   0        0        0      861 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_skin.scad
--rw-r--r--   0        0        0    13469 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_strings.scad
--rw-r--r--   0        0        0     2713 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_structs.scad
--rw-r--r--   0        0        0    16142 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_transforms.scad
--rw-r--r--   0        0        0     1777 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_trigonometry.scad
--rw-r--r--   0        0        0    13375 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_utility.scad
--rw-r--r--   0        0        0    10291 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_vectors.scad
--rw-r--r--   0        0        0     3493 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_version.scad
--rw-r--r--   0        0        0     3259 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_vnf.scad
--rw-r--r--   0        0        0   102085 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/threading.scad
--rw-r--r--   0        0        0    63253 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/transforms.scad
--rw-r--r--   0        0        0    15310 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/trigonometry.scad
--rw-r--r--   0        0        0     4103 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tripod_mounts.scad
--rw-r--r--   0        0        0    48075 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/turtle3d.scad
--rw-r--r--   0        0        0    49578 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Attachments.md
--rw-r--r--   0        0        0     6344 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Distributors.md
--rw-r--r--   0        0        0     3329 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/FractalTree.md
--rw-r--r--   0        0        0     7580 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Mutators.md
--rw-r--r--   0        0        0    14859 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Paths.md
--rw-r--r--   0        0        0    20047 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Shapes2d.md
--rw-r--r--   0        0        0     9378 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Shapes3d.md
--rw-r--r--   0        0        0     6553 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Transforms.md
--rw-r--r--   0        0        0     7054 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/VNF.md
--rw-r--r--   0        0        0    37770 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/utility.scad
--rw-r--r--   0        0        0    25847 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vectors.scad
--rw-r--r--   0        0        0     6572 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/version.scad
--rw-r--r--   0        0        0    85308 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vnf.scad
--rw-r--r--   0        0        0    16411 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/walls.scad
--rw-r--r--   0        0        0     3545 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/wiring.scad
--rw-r--r--   0        0        0      210 2023-04-11 09:14:35.909512 solidpython2-2.0.2/solid2/extensions/bosl2/__init__.py
--rw-r--r--   0        0        0     3318 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/affine.py
--rw-r--r--   0        0        0    13302 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/attachments.py
--rw-r--r--   0        0        0      878 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/ball_bearings.py
--rw-r--r--   0        0        0     7573 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/beziers.py
--rw-r--r--   0        0        0    15500 2023-04-26 17:41:35.972132 solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py
--rw-r--r--   0        0        0     1002 2023-04-11 09:15:15.373553 solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_base.py
--rw-r--r--   0        0        0      611 2023-04-23 17:29:35.094413 solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_patches.py
--rw-r--r--   0        0        0    10956 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/bottlecaps.py
--rw-r--r--   0        0        0     1540 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/color.py
--rw-r--r--   0        0        0     7214 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/comparisons.py
--rw-r--r--   0        0        0     1138 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/constants.py
--rw-r--r--   0        0        0     3010 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/coords.py
--rw-r--r--   0        0        0     3617 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/cubetruss.py
--rw-r--r--   0        0        0    10735 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/distributors.py
--rw-r--r--   0        0        0     8136 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/drawing.py
--rw-r--r--   0        0        0    12654 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/fnliterals.py
--rw-r--r--   0        0        0    12638 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/gears.py
--rw-r--r--   0        0        0    19278 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/geometry.py
--rw-r--r--   0        0        0     5046 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/hinges.py
--rw-r--r--   0        0        0     9519 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/joiners.py
--rw-r--r--   0        0        0     5626 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/linalg.py
--rw-r--r--   0        0        0     1829 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/linear_bearings.py
--rw-r--r--   0        0        0     6946 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/lists.py
--rw-r--r--   0        0        0     4345 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/masks2d.py
--rw-r--r--   0        0        0     8165 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/masks3d.py
--rw-r--r--   0        0        0    12662 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/math.py
--rw-r--r--   0        0        0     3781 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/metric_screws.py
--rw-r--r--   0        0        0     1357 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/modular_hose.py
--rw-r--r--   0        0        0     2333 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/mutators.py
--rw-r--r--   0        0        0     1187 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/nema_steppers.py
--rw-r--r--   0        0        0     6047 2023-04-26 17:41:37.688128 solidpython2-2.0.2/solid2/extensions/bosl2/openscad.py
--rw-r--r--   0        0        0     4055 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/partitions.py
--rw-r--r--   0        0        0     7787 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/paths.py
--rw-r--r--   0        0        0     3387 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/polyhedra.py
--rw-r--r--   0        0        0     7754 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/regions.py
--rw-r--r--   0        0        0    20788 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/rounding.py
--rw-r--r--   0        0        0     3052 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/screw_drive.py
--rw-r--r--   0        0        0    14577 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/screws.py
--rw-r--r--   0        0        0    14150 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/shapes2d.py
--rw-r--r--   0        0        0    26881 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/shapes3d.py
--rw-r--r--   0        0        0    17224 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/skin.py
--rw-r--r--   0        0        0     1595 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/sliders.py
--rw-r--r--   0        0        0      679 2023-04-26 17:41:35.796132 solidpython2-2.0.2/solid2/extensions/bosl2/std.py
--rw-r--r--   0        0        0     7256 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/strings.py
--rw-r--r--   0        0        0     1720 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/structs.py
--rw-r--r--   0        0        0    36860 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/threading.py
--rw-r--r--   0        0        0     8559 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/transforms.py
--rw-r--r--   0        0        0     4784 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/trigonometry.py
--rw-r--r--   0        0        0      609 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/tripod_mounts.py
--rw-r--r--   0        0        0     3058 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/turtle3d.py
--rw-r--r--   0        0        0     7956 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/utility.py
--rw-r--r--   0        0        0     4555 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/vectors.py
--rw-r--r--   0        0        0     1770 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/version.py
--rw-r--r--   0        0        0     9786 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/vnf.py
--rw-r--r--   0        0        0     2163 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/walls.py
--rw-r--r--   0        0        0     1043 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/wiring.py
--rwxr-xr-x   0        0        0     3575 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2_generator.py
--rw-r--r--   0        0        0      264 2023-04-24 23:08:43.905363 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/__init__.py
--rw-r--r--   0        0        0     1647 2023-03-19 12:43:05.633475 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/customizer_widgets.py
--rw-r--r--   0        0        0      871 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_interface.py
--rw-r--r--   0        0        0     1034 2023-04-24 23:08:38.709354 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_variable.py
--rwxr-xr-x   0        0        0     3623 2023-04-24 16:39:42.154697 solidpython2-2.0.2/solid2/extensions/openscad_extension_generator.py
--rwxr-xr-x   0        0        0     3650 2023-04-26 17:33:19.525225 solidpython2-2.0.2/solid2/extensions/scad2solid.py
--rw-r--r--   0        0        0        0 2022-08-12 15:59:10.203877 solidpython2-2.0.2/solid2/libs/__init__.py
--rw-r--r--   0        0        0       56 2023-04-21 22:55:14.022704 solidpython2-2.0.2/solid2/libs/py_scadparser/.git
--rw-r--r--   0        0        0     1855 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/.gitignore
--rw-r--r--   0        0        0     7048 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/LICENSE
--rw-r--r--   0        0        0      722 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/README.md
--rw-r--r--   0        0        0    44947 2023-04-23 20:12:18.566240 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-310.pyc
--rw-r--r--   0        0        0     2673 2023-04-23 20:09:17.734159 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-310.pyc
--rw-r--r--   0        0        0    10330 2023-04-23 20:09:17.730159 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2696 2023-04-23 20:09:17.738159 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-310.pyc
--rw-r--r--   0        0        0    48312 2023-04-23 20:09:17.922159 solidpython2-2.0.2/solid2/libs/py_scadparser/parsetab.py
--rw-r--r--   0        0        0     1229 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/scad_ast.py
--rw-r--r--   0        0        0     8328 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/scad_parser.py
--rw-r--r--   0        0        0     2706 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/scad_tokens.py
--rw-r--r--   0        0        0      280 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/test.scad
--rw-r--r--   0        0        0    24920 1970-01-01 00:00:00.000000 solidpython2-2.0.2/setup.py
--rw-r--r--   0        0        0    24246 1970-01-01 00:00:00.000000 solidpython2-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    21301 2023-07-30 15:30:41.474465 solidpython2-2.0.3/README.rst
+-rw-r--r--   0        0        0     1116 2023-07-30 15:24:53.576556 solidpython2-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-04-24 23:08:31.053339 solidpython2-2.0.3/solid2/__init__.py
+-rw-r--r--   0        0        0     1681 2023-07-30 12:20:04.750192 solidpython2-2.0.3/solid2/config.py
+-rw-r--r--   0        0        0      381 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/core/__init__.py
+-rw-r--r--   0        0        0       87 2023-07-22 23:02:54.670729 solidpython2-2.0.3/solid2/core/builtins/__init__.py
+-rw-r--r--   0        0        0     3701 2023-07-30 11:30:09.782296 solidpython2-2.0.3/solid2/core/builtins/convenience.py
+-rw-r--r--   0        0        0     1040 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/core/builtins/implicit.primitives
+-rw-r--r--   0        0        0      754 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/core/builtins/openscad.mutators
+-rw-r--r--   0        0        0     1968 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/core/builtins/openscad.primitives
+-rw-r--r--   0        0        0     1445 2023-07-22 23:02:54.670729 solidpython2-2.0.3/solid2/core/builtins/openscad_functions.py
+-rw-r--r--   0        0        0    25400 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/core/builtins/openscad_primitives.py
+-rw-r--r--   0        0        0      367 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/core/builtins/primitives.py
+-rw-r--r--   0        0        0      938 2022-09-03 20:01:15.234639 solidpython2-2.0.3/solid2/core/extension_manager.py
+-rw-r--r--   0        0        0       32 2023-03-19 13:30:20.199884 solidpython2-2.0.3/solid2/core/object_base/__init__.py
+-rw-r--r--   0        0        0     3522 2023-03-20 14:58:07.769013 solidpython2-2.0.3/solid2/core/object_base/access_syntax_mixin.py
+-rw-r--r--   0        0        0     6866 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/core/object_base/object_base_impl.py
+-rw-r--r--   0        0        0     2253 2023-03-20 14:58:07.769013 solidpython2-2.0.3/solid2/core/object_base/operator_mixin.py
+-rw-r--r--   0        0        0     3994 2022-08-12 15:59:10.183877 solidpython2-2.0.3/solid2/core/object_factory.py
+-rw-r--r--   0        0        0     3428 2023-04-26 10:51:10.097683 solidpython2-2.0.3/solid2/core/parse_scad.py
+-rw-r--r--   0        0        0     5489 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/core/scad_import.py
+-rw-r--r--   0        0        0     3051 2023-05-02 10:30:37.857979 solidpython2-2.0.3/solid2/core/scad_render.py
+-rw-r--r--   0        0        0     1948 2023-07-22 23:02:54.670729 solidpython2-2.0.3/solid2/core/utils.py
+-rwxr-xr-x   0        0        0      559 2023-04-28 10:25:21.909011 solidpython2-2.0.3/solid2/examples/01-basics.py
+-rwxr-xr-x   0        0        0      808 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/examples/02-vars-and-operators.py
+-rwxr-xr-x   0        0        0      647 2022-08-12 15:59:10.183877 solidpython2-2.0.3/solid2/examples/03-debug-background.py
+-rwxr-xr-x   0        0        0     1275 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/examples/04-convenience.py
+-rwxr-xr-x   0        0        0      912 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/examples/05-access-style-syntax.py
+-rwxr-xr-x   0        0        0     1126 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/examples/06-functions.py
+-rwxr-xr-x   0        0        0      425 2023-04-24 18:27:22.516007 solidpython2-2.0.3/solid2/examples/07-libs-bosl2-attachable.py
+-rw-r--r--   0        0        0     3296 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/examples/07-libs-bosl2-logo.py
+-rwxr-xr-x   0        0        0     1762 2023-04-23 11:52:48.014465 solidpython2-2.0.3/solid2/examples/07-libs-bosl2.py
+-rwxr-xr-x   0        0        0      620 2023-04-21 23:01:13.315397 solidpython2-2.0.3/solid2/examples/07-libs.x.py
+-rwxr-xr-x   0        0        0     2448 2023-03-20 14:58:07.769013 solidpython2-2.0.3/solid2/examples/08-extensions.py
+-rwxr-xr-x   0        0        0     1656 2023-04-24 18:33:54.580435 solidpython2-2.0.3/solid2/examples/09-code-attach-extension.py
+-rwxr-xr-x   0        0        0      906 2023-04-21 22:55:04.234686 solidpython2-2.0.3/solid2/examples/10-customizer.py
+-rw-r--r--   0        0        0      158 2022-08-12 15:59:10.183877 solidpython2-2.0.3/solid2/examples/11-font/LICENSE_README
+-rw-r--r--   0        0        0    47404 2022-08-12 15:59:10.187877 solidpython2-2.0.3/solid2/examples/11-font/RichEatin.otf
+-rwxr-xr-x   0        0        0      192 2023-03-15 13:23:46.114122 solidpython2-2.0.3/solid2/examples/11-fonts.x.py
+-rwxr-xr-x   0        0        0      335 2023-03-15 13:23:46.114122 solidpython2-2.0.3/solid2/examples/12-animation.py
+-rwxr-xr-x   0        0        0     2032 2023-03-19 12:43:05.625475 solidpython2-2.0.3/solid2/examples/13-animated-bouncing-ball.py
+-rwxr-xr-x   0        0        0     1381 2023-04-21 23:01:13.315397 solidpython2-2.0.3/solid2/examples/14-implicitCAD.x.py
+-rwxr-xr-x   0        0        0     1794 2023-04-21 23:01:13.315397 solidpython2-2.0.3/solid2/examples/15-implicitCAD2.x.py
+-rwxr-xr-x   0        0        0     1102 2022-08-12 15:59:10.187877 solidpython2-2.0.3/solid2/examples/16-mazebox-bosl2.py
+-rwxr-xr-x   0        0        0     2243 2023-07-22 23:03:48.790438 solidpython2-2.0.3/solid2/examples/17-greedy-scad-interface.py
+-rw-r--r--   0        0        0     1196 2022-08-12 15:59:10.187877 solidpython2-2.0.3/solid2/examples/maze7.png
+-rw-r--r--   0        0        0        1 2023-04-24 16:33:55.353741 solidpython2-2.0.3/solid2/extensions/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-21 22:55:14.018704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.git
+-rw-r--r--   0        0        0      522 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      655 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      318 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/check_for_tabs.json
+-rw-r--r--   0        0        0      307 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/openscad_docsgen.json
+-rw-r--r--   0        0        0     1214 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_docs.yml
+-rw-r--r--   0        0        0     1448 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_tutorials.yml
+-rw-r--r--   0        0        0     2823 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1253 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.gitignore
+-rw-r--r--   0        0        0     1197 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.openscad_docsgen_rc
+-rw-r--r--   0        0        0      132 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.openscad_mdimggen_rc
+-rw-r--r--   0        0        0     2142 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1323 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/LICENSE
+-rw-r--r--   0        0        0     2926 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/README.md
+-rw-r--r--   0        0        0    37745 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/WRITING_DOCS.md
+-rw-r--r--   0        0        0    18422 2023-04-21 22:55:14.034704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/affine.scad
+-rw-r--r--   0        0        0   158011 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/attachments.scad
+-rw-r--r--   0        0        0    10326 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/ball_bearings.scad
+-rw-r--r--   0        0        0    76076 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/beziers.scad
+-rw-r--r--   0        0        0     3557 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/bosl1compat.scad
+-rw-r--r--   0        0        0    53194 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/bottlecaps.scad
+-rw-r--r--   0        0        0     1257 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/builtins.scad
+-rw-r--r--   0        0        0     8302 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/color.scad
+-rw-r--r--   0        0        0    40080 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/comparisons.scad
+-rw-r--r--   0        0        0     9779 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/constants.scad
+-rw-r--r--   0        0        0    18570 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/coords.scad
+-rw-r--r--   0        0        0    28607 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/cubetruss.scad
+-rw-r--r--   0        0        0    88642 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/distributors.scad
+-rw-r--r--   0        0        0    62214 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/drawing.scad
+-rw-r--r--   0        0        0     1389 2023-04-21 22:55:14.038704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/BOSL2logo.scad
+-rw-r--r--   0        0        0      559 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/attachments.scad
+-rw-r--r--   0        0        0     1344 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/boolean_geometry.scad
+-rw-r--r--   0        0        0      505 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/fractal_tree.scad
+-rw-r--r--   0        0        0     4168 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/lsystems.scad
+-rw-r--r--   0        0        0     2465 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/orientations.scad
+-rw-r--r--   0        0        0      704 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/spherical_patch.scad
+-rw-r--r--   0        0        0    56985 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/fnliterals.scad
+-rw-r--r--   0        0        0    65959 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/gears.scad
+-rw-r--r--   0        0        0   125434 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/geometry.scad
+-rw-r--r--   0        0        0    31047 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/hinges.scad
+-rw-r--r--   0        0        0   117043 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/images/BOSL2logo.png
+-rw-r--r--   0        0        0    58197 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/joiners.scad
+-rw-r--r--   0        0        0    31481 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/linalg.scad
+-rw-r--r--   0        0        0     8378 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/linear_bearings.scad
+-rw-r--r--   0        0        0    47932 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/lists.scad
+-rw-r--r--   0        0        0    24740 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/masks2d.scad
+-rw-r--r--   0        0        0    26185 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/masks3d.scad
+-rw-r--r--   0        0        0    54569 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/math.scad
+-rw-r--r--   0        0        0    23837 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/metric_screws.scad
+-rw-r--r--   0        0        0     9089 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/modular_hose.scad
+-rw-r--r--   0        0        0    21204 2023-04-21 22:55:14.042704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/mutators.scad
+-rw-r--r--   0        0        0    10102 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/nema_steppers.scad
+-rw-r--r--   0        0        0    25544 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/partitions.scad
+-rw-r--r--   0        0        0    55148 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/paths.scad
+-rw-r--r--   0        0        0    44343 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/polyhedra.scad
+-rw-r--r--   0        0        0    62670 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/regions.scad
+-rw-r--r--   0        0        0   220660 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/rounding.scad
+-rw-r--r--   0        0        0    14301 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/screw_drive.scad
+-rw-r--r--   0        0        0   179010 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/screws.scad
+-rwxr-xr-x   0        0        0      115 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/check_for_tabs.sh
+-rwxr-xr-x   0        0        0      569 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/find_modular_asserts.sh
+-rwxr-xr-x   0        0        0     2784 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/func_coverage.py
+-rwxr-xr-x   0        0        0     2345 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/img2scad.py
+-rwxr-xr-x   0        0        0      545 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/increment_version.sh
+-rwxr-xr-x   0        0        0      511 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/linecount.sh
+-rwxr-xr-x   0        0        0      368 2023-04-21 22:55:14.046704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/purge_wiki_history.sh
+-rwxr-xr-x   0        0        0      790 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/run_tests.sh
+-rw-r--r--   0        0        0    91055 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/shapes2d.scad
+-rw-r--r--   0        0        0   181418 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/shapes3d.scad
+-rw-r--r--   0        0        0   238386 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/skin.scad
+-rw-r--r--   0        0        0     6786 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/sliders.scad
+-rw-r--r--   0        0        0     1071 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/std.scad
+-rw-r--r--   0        0        0    34155 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/strings.scad
+-rw-r--r--   0        0        0     5355 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/structs.scad
+-rw-r--r--   0        0        0      186 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/README.txt
+-rw-r--r--   0        0        0     1443 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/polyhedra.scad
+-rw-r--r--   0        0        0     4998 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_affine.scad
+-rw-r--r--   0        0        0      371 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_attachments.scad
+-rw-r--r--   0        0        0    16598 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_comparisons.scad
+-rw-r--r--   0        0        0    12026 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_coords.scad
+-rw-r--r--   0        0        0      393 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_cubetruss.scad
+-rw-r--r--   0        0        0      999 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_distributors.scad
+-rw-r--r--   0        0        0     5679 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_drawing.scad
+-rw-r--r--   0        0        0     9824 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_edges.scad
+-rw-r--r--   0        0        0    23237 2023-04-21 22:55:14.050704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_fnliterals.scad
+-rw-r--r--   0        0        0    62561 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_geometry.scad
+-rw-r--r--   0        0        0    11660 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_linalg.scad
+-rw-r--r--   0        0        0      425 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_linear_bearings.scad
+-rw-r--r--   0        0        0    13578 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_lists.scad
+-rw-r--r--   0        0        0     8961 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_masks2d.scad
+-rw-r--r--   0        0        0    26667 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_math.scad
+-rw-r--r--   0        0        0     1351 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_mutators.scad
+-rw-r--r--   0        0        0    12273 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_paths.scad
+-rw-r--r--   0        0        0     7958 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_regions.scad
+-rw-r--r--   0        0        0     8862 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_rounding.scad
+-rw-r--r--   0        0        0      700 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_screw_drive.scad
+-rw-r--r--   0        0        0    64080 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_shapes2d.scad
+-rw-r--r--   0        0        0    24086 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_shapes3d.scad
+-rw-r--r--   0        0        0      861 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_skin.scad
+-rw-r--r--   0        0        0    13469 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_strings.scad
+-rw-r--r--   0        0        0     2713 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_structs.scad
+-rw-r--r--   0        0        0    16142 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_transforms.scad
+-rw-r--r--   0        0        0     1777 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_trigonometry.scad
+-rw-r--r--   0        0        0    13375 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_utility.scad
+-rw-r--r--   0        0        0    10291 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_vectors.scad
+-rw-r--r--   0        0        0     3493 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_version.scad
+-rw-r--r--   0        0        0     3259 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_vnf.scad
+-rw-r--r--   0        0        0   102085 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/threading.scad
+-rw-r--r--   0        0        0    63253 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/transforms.scad
+-rw-r--r--   0        0        0    15310 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/trigonometry.scad
+-rw-r--r--   0        0        0     4103 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tripod_mounts.scad
+-rw-r--r--   0        0        0    48075 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/turtle3d.scad
+-rw-r--r--   0        0        0    49578 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Attachments.md
+-rw-r--r--   0        0        0     6344 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Distributors.md
+-rw-r--r--   0        0        0     3329 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/FractalTree.md
+-rw-r--r--   0        0        0     7580 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Mutators.md
+-rw-r--r--   0        0        0    14859 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Paths.md
+-rw-r--r--   0        0        0    20047 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Shapes2d.md
+-rw-r--r--   0        0        0     9378 2023-04-21 22:55:14.054704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Shapes3d.md
+-rw-r--r--   0        0        0     6553 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Transforms.md
+-rw-r--r--   0        0        0     7054 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/VNF.md
+-rw-r--r--   0        0        0    37770 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/utility.scad
+-rw-r--r--   0        0        0    25847 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/vectors.scad
+-rw-r--r--   0        0        0     6572 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/version.scad
+-rw-r--r--   0        0        0    85308 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/vnf.scad
+-rw-r--r--   0        0        0    16411 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/walls.scad
+-rw-r--r--   0        0        0     3545 2023-04-21 22:55:14.058704 solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/wiring.scad
+-rw-r--r--   0        0        0      210 2023-04-11 09:14:35.909512 solidpython2-2.0.3/solid2/extensions/bosl2/__init__.py
+-rw-r--r--   0        0        0     3318 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/affine.py
+-rw-r--r--   0        0        0    13302 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/attachments.py
+-rw-r--r--   0        0        0      878 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/ball_bearings.py
+-rw-r--r--   0        0        0     7573 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/beziers.py
+-rw-r--r--   0        0        0    15500 2023-04-26 17:41:35.972132 solidpython2-2.0.3/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py
+-rw-r--r--   0        0        0     1002 2023-04-11 09:15:15.373553 solidpython2-2.0.3/solid2/extensions/bosl2/bosl2_base.py
+-rw-r--r--   0        0        0      611 2023-04-23 17:29:35.094413 solidpython2-2.0.3/solid2/extensions/bosl2/bosl2_patches.py
+-rw-r--r--   0        0        0    10956 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/bottlecaps.py
+-rw-r--r--   0        0        0     1540 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/color.py
+-rw-r--r--   0        0        0     7214 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/comparisons.py
+-rw-r--r--   0        0        0     1138 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/constants.py
+-rw-r--r--   0        0        0     3010 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/coords.py
+-rw-r--r--   0        0        0     3617 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/cubetruss.py
+-rw-r--r--   0        0        0    10735 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/distributors.py
+-rw-r--r--   0        0        0     8136 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/drawing.py
+-rw-r--r--   0        0        0    12654 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/fnliterals.py
+-rw-r--r--   0        0        0    12638 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/gears.py
+-rw-r--r--   0        0        0    19278 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/geometry.py
+-rw-r--r--   0        0        0     5046 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/hinges.py
+-rw-r--r--   0        0        0     9519 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/joiners.py
+-rw-r--r--   0        0        0     5626 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/linalg.py
+-rw-r--r--   0        0        0     1829 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/linear_bearings.py
+-rw-r--r--   0        0        0     6946 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/lists.py
+-rw-r--r--   0        0        0     4345 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/masks2d.py
+-rw-r--r--   0        0        0     8165 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/masks3d.py
+-rw-r--r--   0        0        0    12662 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/math.py
+-rw-r--r--   0        0        0     3781 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/metric_screws.py
+-rw-r--r--   0        0        0     1357 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/modular_hose.py
+-rw-r--r--   0        0        0     2333 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/mutators.py
+-rw-r--r--   0        0        0     1187 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/nema_steppers.py
+-rw-r--r--   0        0        0     6047 2023-04-26 17:41:37.688128 solidpython2-2.0.3/solid2/extensions/bosl2/openscad.py
+-rw-r--r--   0        0        0     4055 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/partitions.py
+-rw-r--r--   0        0        0     7787 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/paths.py
+-rw-r--r--   0        0        0     3387 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/polyhedra.py
+-rw-r--r--   0        0        0     7754 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/regions.py
+-rw-r--r--   0        0        0    20788 2023-05-02 09:54:08.391238 solidpython2-2.0.3/solid2/extensions/bosl2/rounding.py
+-rw-r--r--   0        0        0     3052 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/screw_drive.py
+-rw-r--r--   0        0        0    14577 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/screws.py
+-rw-r--r--   0        0        0    14150 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/shapes2d.py
+-rw-r--r--   0        0        0    26881 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/shapes3d.py
+-rw-r--r--   0        0        0    17224 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/skin.py
+-rw-r--r--   0        0        0     1595 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/sliders.py
+-rw-r--r--   0        0        0      679 2023-04-26 17:41:35.796132 solidpython2-2.0.3/solid2/extensions/bosl2/std.py
+-rw-r--r--   0        0        0     7256 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/strings.py
+-rw-r--r--   0        0        0     1720 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/structs.py
+-rw-r--r--   0        0        0    36860 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/threading.py
+-rw-r--r--   0        0        0     8559 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/transforms.py
+-rw-r--r--   0        0        0     4784 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/trigonometry.py
+-rw-r--r--   0        0        0      609 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/tripod_mounts.py
+-rw-r--r--   0        0        0     3058 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/turtle3d.py
+-rw-r--r--   0        0        0     7956 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/utility.py
+-rw-r--r--   0        0        0     4555 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/vectors.py
+-rw-r--r--   0        0        0     1770 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/version.py
+-rw-r--r--   0        0        0     9786 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/vnf.py
+-rw-r--r--   0        0        0     2163 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/walls.py
+-rw-r--r--   0        0        0     1043 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2/wiring.py
+-rwxr-xr-x   0        0        0     3575 2023-05-02 09:54:08.395238 solidpython2-2.0.3/solid2/extensions/bosl2_generator.py
+-rw-r--r--   0        0        0      264 2023-04-24 23:08:43.905363 solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/__init__.py
+-rw-r--r--   0        0        0     1647 2023-03-19 12:43:05.633475 solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/customizer_widgets.py
+-rw-r--r--   0        0        0      871 2023-03-15 13:23:46.114122 solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/scad_interface.py
+-rw-r--r--   0        0        0     1034 2023-04-24 23:08:38.709354 solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/scad_variable.py
+-rwxr-xr-x   0        0        0     3623 2023-04-24 16:39:42.154697 solidpython2-2.0.3/solid2/extensions/openscad_extension_generator.py
+-rwxr-xr-x   0        0        0     3650 2023-04-26 17:33:19.525225 solidpython2-2.0.3/solid2/extensions/scad2solid.py
+-rw-r--r--   0        0        0        0 2022-08-12 15:59:10.203877 solidpython2-2.0.3/solid2/libs/__init__.py
+-rw-r--r--   0        0        0       56 2023-04-21 22:55:14.022704 solidpython2-2.0.3/solid2/libs/py_scadparser/.git
+-rw-r--r--   0        0        0     1855 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/.gitignore
+-rw-r--r--   0        0        0     7048 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/LICENSE
+-rw-r--r--   0        0        0      722 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/README.md
+-rw-r--r--   0        0        0    44947 2023-04-23 20:12:18.566240 solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-310.pyc
+-rw-r--r--   0        0        0     2673 2023-04-23 20:09:17.734159 solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-310.pyc
+-rw-r--r--   0        0        0    10330 2023-04-23 20:09:17.730159 solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2696 2023-04-23 20:09:17.738159 solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-310.pyc
+-rw-r--r--   0        0        0    48312 2023-04-23 20:09:17.922159 solidpython2-2.0.3/solid2/libs/py_scadparser/parsetab.py
+-rw-r--r--   0        0        0     1229 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/scad_ast.py
+-rw-r--r--   0        0        0     8328 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/scad_parser.py
+-rw-r--r--   0        0        0     2706 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/scad_tokens.py
+-rw-r--r--   0        0        0      280 2023-04-21 22:55:14.070704 solidpython2-2.0.3/solid2/libs/py_scadparser/test.scad
+-rw-r--r--   0        0        0    23208 1970-01-01 00:00:00.000000 solidpython2-2.0.3/setup.py
+-rw-r--r--   0        0        0    22617 1970-01-01 00:00:00.000000 solidpython2-2.0.3/PKG-INFO
```

### Comparing `solidpython2-2.0.2/README.rst` & `solidpython2-2.0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 **If you switch from the regular SolidPython:master branch to this branch, have a
 look at** `Version 2.x.x`_.
 
 SolidPython
 ===========
 
 .. contents::
-   
+
 OpenSCAD for Python
 -------------------
 
 SolidPython is a generalization of Phillip Tiefenbacher's openscad
 module, found on `Thingiverse <http://www.thingiverse.com/thing:1481>`__. It
 generates valid OpenSCAD code from Python code with minimal overhead. Here's a
 simple example:
@@ -41,15 +41,15 @@
 
 That doesn't seem like such a savings, but the following SolidPython code is a
 lot shorter (and I think clearer) than the SCAD code it compiles to:
 
 .. code:: python
 
     from solid2 import *
-    d = cube(5) + right(5)(sphere(5)) - cylinder(r=2, h=6)
+    d = cube(5) + sphere(5).right(5) - cylinder(r=2, h=6)
 
 Generates this OpenSCAD code:
 
 .. code::
 
     difference(){
         union(){
@@ -98,16 +98,16 @@
    `PyPI <https://pypi.python.org/pypi/solidpython2>`__:
 
    .. code:: bash
 
        pip install solidpython2
 
    (You may need to use ``sudo pip install solidpython2``, depending on
-   your environment. This is commonly discouraged though. You'll be happiest 
-   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__ 
+   your environment. This is commonly discouraged though. You'll be happiest
+   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__
    where you can easily control dependencies for a given project)
 
 - Install current master straight from Github:
 
   .. code:: bash
 
       pip install git+https://github.com/jeff-dh/SolidPython
@@ -117,20 +117,20 @@
 
 -  Include SolidPython at the top of your Python file:
 
    .. code:: python
 
        from solid2 import *
 
-   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for 
+   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for
    a discussion of other import styles)
 
 -  OpenSCAD uses curly-brace blocks ({}) to create its tree. SolidPython
-   uses parentheses with comma-delimited lists. 
-   
+   uses parentheses with comma-delimited lists.
+
    **OpenSCAD:**
 
    .. code::
 
        difference(){
            cube(10);
            sphere(15);
@@ -152,89 +152,26 @@
 -  If ``filepath.scad`` is open in the OpenSCAD IDE and Design => 'Automatic
    Reload and Compile' is checked in the OpenSCAD IDE, running
    ``py_scad_obj.save_as_scad()`` from Python will load the object in the
    IDE.
 -  Alternately, you could call OpenSCAD's command line and render
    straight to STL.
 
-Importing OpenSCAD code
+Tutorial - Example Code
 -----------------------
 
-- Use ``solid2.import_scad(path)`` to import OpenSCAD code. Relative paths will check the current location designated in `OpenSCAD library directories <https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Libraries>`__.
-
-**Ex:** 
-
-``scadfile.scad``
-
-.. code::
-
-    module box(w,h,d){
-        cube([w,h,d]);
-    }
-
-``your_file.py``
-
-.. code:: python
-
-    from solid2 import *
-
-    scadfile = import_scad('/path/to/scadfile.scad') 
-    b = scadfile.box(2,4,6)
-    b.save_as_scad('out_file.scad')
-
-- Recursively import OpenSCAD code by calling ``import_scad()`` with a directory argument.
-
-.. code:: python
-
-    from solid2 import *
-
-    # MCAD is OpenSCAD's most common utility library: https://github.com/openscad/MCAD
-    # If it's installed for OpenSCAD (on MacOS, at: ``$HOME/Documents/OpenSCAD/libraries``)
-    mcad = import_scad('MCAD')
-
-    # MCAD contains about 15 separate packages, each included as its own namespace
-    print(dir(mcad)) # => ['bearing', 'bitmap', 'boxes', etc...]
-    mount = mcad.motors.stepper_motor_mount(nema_standard=17)
-    mount.save_as_scad('motor_mount_file.scad')
-
-- OpenSCAD has the ``use()`` and ``include()`` statements for importing SCAD code, and SolidPython has them, too. They pollute the global namespace, though, and you may have better luck with ``import_scad()``,
-
-**Ex:**
-
-``scadfile.scad``
-
-.. code::
-
-    module box(w,h,d){
-        cube([w,h,d]);
-    }
-
-``your_file.py``
-
-.. code:: python
-
-    from solid2 import *
-
-    # use() puts the module `box()` into the global namespace
-    use('/path/to/scadfile.scad') 
-    b = box(2,4,6)
-    scad_render_to_file(b, 'out_file.scad')
-
-
-Example Code
-------------
-
 The best way to learn how SolidPython works is to look at the included
-example code. If you've installed SolidPython, the following line of
-Python will print (the location of) the examples directory:
+example code. They are kind of a minimalistic SolidPython tutorial. If
+you've installed SolidPython, the following line of Python will print
+(the location of) the examples directory:
 
 .. code:: python
 
     import os, solid2; print(os.path.dirname(solid2.__file__) + '/examples')
-        
+
 
 Or browse the example code on Github
 `here <https://github.com/jeff-dh/SolidPython/tree/exp_solid/solid2/examples>`__
 
 Extra syntactic sugar
 =====================
 
@@ -376,15 +313,15 @@
 SolidPython 2.x.x is a refactored version of SolidPython 1.x.x.
 The refactoring process was based on the following proposal:
 https://github.com/SolidCode/SolidPython/issues/169
 
 The goal was to
 
 * extract the "core" from SolidPython
-* make a solid package that only contains the fundamentals (+ a few convenience features) 
+* make a solid package that only contains the fundamentals (+ a few convenience features)
 * make it extendible
 * try to get complex libraries working properly (mcad, bosl, bosl2)
 * **KISS**: ``from solid2 import *`` -> imports only ~1000 lines of source code and has (almost?) all the feautres SolidPython 1.x.x has
 * be a drop in replacement for SolidPython 1.x.x -- as far as possible, see Backwards Compatibility Section
 * get all kinds of nice features working (see Features section)
 
 The result is a refactored and in some parts rewritten version of SolidPython we would like to release as SolidPython 2.x.x. The major improvement is a code base that should be better maintainable and extendible.
@@ -495,17 +432,17 @@
         * all *illegal* python idetifiers are escape with a single prepending underscore
         * special variables ``$fn -> _fn`` (*note*: ``segments`` still works)
         * identifier starting with a digit ``module 12ptStar() -> _12ptStar()`` (*note*: ``__12ptStar`` still works)
         * python keywords ``module import() -> _import()`` (*note*: ``import\_``  still works)
 
 * import paths have changed (a lot)
     * as long as you only import the root package it should be fine, otherwise probably not
-    
+
     .. code:: python
-    
+
             from solid2 import * #fine
             from solid2 import objects #crash
             from solid2 import solidpython #crash
             from solid2 import splines #crash
             from solid2 import utils #crash
 
 * all extensions have been moved:
@@ -553,11 +490,11 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 General Public License for more details.
 
 `Full text of the
 license <http://www.gnu.org/licenses/old-licenses/lgpl-2.1.txt>`__.
 
 Some class docstrings are derived from the `OpenSCAD User Manual
-<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so 
+<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so
 are available under the `Creative Commons Attribution-ShareAlike License
-<https://creativecommons.org/licenses/by-sa/3.0/>`__. 
+<https://creativecommons.org/licenses/by-sa/3.0/>`__.
```

### Comparing `solidpython2-2.0.2/pyproject.toml` & `solidpython2-2.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solidpython2"
-version = "2.0.2"
+version = "2.0.3"
 description = "Python interface to the OpenSCAD declarative geometry language"
 authors = ["jeff"]
 homepage = "https://github.com/jeff-dh/SolidPython"
 repository = "https://github.com/jeff-dh/SolidPython"
 license = "LGPL-2.1"
 readme = "README.rst"
 keywords = [
```

### Comparing `solidpython2-2.0.2/solid2/config.py` & `solidpython2-2.0.3/solid2/config.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/builtins/convenience.py` & `solidpython2-2.0.3/solid2/core/builtins/convenience.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ...config import config
-from ..object_base import ObjectBase
+from ..object_base import ObjectBase, OperatorMixin, AccessSyntaxMixin
 from .primitives import *
 
 # =============
 # = modifiers =
 # =============
-class ModifierBase(ObjectBase):
+class ModifierBase(ObjectBase, OperatorMixin, AccessSyntaxMixin):
     def __init__(self, child=None):
         super().__init__()
         if child:
             self._children += [child]
 
 class debug(ModifierBase):
     def _render(self):
```

### Comparing `solidpython2-2.0.2/solid2/core/builtins/implicit.primitives` & `solidpython2-2.0.3/solid2/core/builtins/implicit.primitives`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/builtins/openscad.mutators` & `solidpython2-2.0.3/solid2/core/builtins/openscad.mutators`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/builtins/openscad.primitives` & `solidpython2-2.0.3/solid2/core/builtins/openscad.primitives`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/builtins/openscad_primitives.py` & `solidpython2-2.0.3/solid2/core/builtins/openscad_primitives.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/extension_manager.py` & `solidpython2-2.0.3/solid2/core/extension_manager.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/object_base/access_syntax_mixin.py` & `solidpython2-2.0.3/solid2/core/object_base/access_syntax_mixin.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/object_base/object_base_impl.py` & `solidpython2-2.0.3/solid2/core/object_base/object_base_impl.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/object_base/operator_mixin.py` & `solidpython2-2.0.3/solid2/core/object_base/operator_mixin.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/object_factory.py` & `solidpython2-2.0.3/solid2/core/object_factory.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/parse_scad.py` & `solidpython2-2.0.3/solid2/core/parse_scad.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/scad_import.py` & `solidpython2-2.0.3/solid2/core/scad_import.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/scad_render.py` & `solidpython2-2.0.3/solid2/core/scad_render.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/core/utils.py` & `solidpython2-2.0.3/solid2/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,14 @@
 
     return None
 
 def py2openscad(o):
     from .object_base import ObjectBase
     if type(o) == bool:
         return str(o).lower()
-    if type(o) == float:
-        return f"{o:.10f}"  # type: ignore
     if type(o) == str:
         return f'\"{o}\"'  # type: ignore
     if isinstance(o, ObjectBase):
         return o._render()[:-2] #[:-1] removing traling ;\n
     if hasattr(o, "__iter__"):
         scadVals = [py2openscad(i) for i in o]
         return f"[{', '.join(scadVals)}]"
```

### Comparing `solidpython2-2.0.2/solid2/examples/01-basics.py` & `solidpython2-2.0.3/solid2/examples/01-basics.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/02-vars-and-operators.py` & `solidpython2-2.0.3/solid2/examples/02-vars-and-operators.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # you can store any "openscad" object in a regular variable. No matter whether
 # it's just a primitive or a complete assembly
 c = cube([10, 20, 30])
 s = sphere(10)
 
 d = c - s
-# Operators: This is from the operators extension.
+# Operators:
 # The following operators are defined:
 #
 #   operator    |   action
 #   ------------|-------------
 #      +, |     | union
 #      -        | difference
 #      *, &     | intersection
```

### Comparing `solidpython2-2.0.2/solid2/examples/03-debug-background.py` & `solidpython2-2.0.3/solid2/examples/03-debug-background.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/04-convenience.py` & `solidpython2-2.0.3/solid2/examples/04-convenience.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! /usr/bin/env python
 
 from solid2 import *
 
-# the convenience extension defines some convenience functions and "overloads"
-# some transformations and primitives to get a more convient access to it.
+# the convenience module defines some convenience functions and "overloads" for
+# some transformations and primitives to get a more convenient access to it.
 # It provides for all OpenSCAD modules which need a "size" parameter to pass in
 # single integers / floats (not wrapped in a list or tuple). In other words: you
 # don't need to wrap sizes in [ and ]:
 #
 #       translate(10, 0, 0)(cube(1, 2, 3))
 #
 # The following transformations and modules are "overloaded":
```

### Comparing `solidpython2-2.0.2/solid2/examples/05-access-style-syntax.py` & `solidpython2-2.0.3/solid2/examples/05-access-style-syntax.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 
 from solid2 import *
 
-# Since I don't like the OpenSCAD syntax I added the "access-style" syntax
-# extension. This allows you to call all OpenSCAD builtin transformations, the
-# convenience functions (up, down, left,...) and the modifiers (debug,
-# background, ...) as if you would call a member function.
+# Since I don't like the OpenSCAD syntax I added "access-style" syntax. This
+# allows to call all OpenSCAD builtin transformations, the convenience
+# functions (up, down, left,...) and the modifiers (debug, background, ...) as
+# if you would call a member function.
 #
 #       cube(10).up(5)
 #
 # is equivalent to
 #
 #       up(5)(cube(10))
 
@@ -17,15 +17,15 @@
         down(5).\
             rotate(45, 45, 45)
 
 s = ~sphere(10).forward(5)
 
 (c-s).save_as_scad()
 
-# generates the exactly the same code as 04-convenience.py:
+# generates exactly the same code as 04-convenience.py:
 #
 #    // Generated by ExpSolidPython
 #
 #    difference() {
 #            rotate(a = [45, 45, 45]) {
 #                    translate(v = [0, 0, -5]) {
 #                            cube(size = [10, 20, 30]);
```

### Comparing `solidpython2-2.0.2/solid2/examples/06-functions.py` & `solidpython2-2.0.3/solid2/examples/06-functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #! /usr/bin/env python
 
 from solid2 import *
 
-# as soon as the objects get more complicated it makes sense to use functions
+# as soon as the objects get more sophisticated it makes sense to use functions
 # to hierarchically assemble them.
 # You can use python functions pretty much the same way as OpenSCAD modules
 # except the children stuff. This is not possible with SolidPython but you
-# should be albe to pass other OpenSCAD objects as parameters if neccessary.
-# I haven't tried it but it should work....
+# can pass other OpenSCAD objects as parameters to a function.
 #
 # This simple example assembles a car similar to the one from the OpenSCAD
 # tutorial:
 
 def wheel():
     return cylinder(r=35, h=15, center=True).rotate(0, 90, 0)
```

### Comparing `solidpython2-2.0.2/solid2/examples/07-libs-bosl2-logo.py` & `solidpython2-2.0.3/solid2/examples/07-libs-bosl2-logo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from solid2.extensions.bosl2 import *
 from solid2.extensions.bosl2 import gears, beziers, screws, cubetruss
 
 # $fa=1;
 # $fs=1;
 
-from solid2.extensions.greedy_scad_interface import set_global_fa, set_global_fs
+from solid2 import set_global_fa, set_global_fs
 set_global_fa(1)
 set_global_fs(1)
 
 def B():
 	# recolor("#f77")
 	# diff("hole")
 	# cuboid([45,45,10], chamfer=10, edges=[RIGHT+BACK,RIGHT+FRONT], anchor=FRONT) {
```

### Comparing `solidpython2-2.0.2/solid2/examples/07-libs-bosl2.py` & `solidpython2-2.0.3/solid2/examples/07-libs-bosl2.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/07-libs.x.py` & `solidpython2-2.0.3/solid2/examples/07-libs.x.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/08-extensions.py` & `solidpython2-2.0.3/solid2/examples/08-extensions.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/09-code-attach-extension.py` & `solidpython2-2.0.3/solid2/examples/09-code-attach-extension.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/10-customizer.py` & `solidpython2-2.0.3/solid2/examples/10-customizer.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/11-font/RichEatin.otf` & `solidpython2-2.0.3/solid2/examples/11-font/RichEatin.otf`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/13-animated-bouncing-ball.py` & `solidpython2-2.0.3/solid2/examples/13-animated-bouncing-ball.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/14-implicitCAD.x.py` & `solidpython2-2.0.3/solid2/examples/14-implicitCAD.x.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/15-implicitCAD2.x.py` & `solidpython2-2.0.3/solid2/examples/15-implicitCAD2.x.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/16-mazebox-bosl2.py` & `solidpython2-2.0.3/solid2/examples/16-mazebox-bosl2.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/17-greedy-scad-interface.py` & `solidpython2-2.0.3/solid2/examples/17-greedy-scad-interface.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/examples/maze7.png` & `solidpython2-2.0.3/solid2/examples/maze7.png`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/bug_report.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/feature_request.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_docs.yml` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_docs.yml`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_tutorials.yml` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_tutorials.yml`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/main.yml` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.gitignore` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.gitignore`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.openscad_docsgen_rc` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/.openscad_docsgen_rc`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/CONTRIBUTING.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/LICENSE` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/LICENSE`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/README.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/README.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/WRITING_DOCS.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/WRITING_DOCS.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/affine.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/affine.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/attachments.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/attachments.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/ball_bearings.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/ball_bearings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/beziers.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/beziers.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bosl1compat.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/bosl1compat.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bottlecaps.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/bottlecaps.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/builtins.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/builtins.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/color.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/color.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/comparisons.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/comparisons.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/constants.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/constants.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/coords.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/coords.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/cubetruss.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/cubetruss.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/distributors.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/distributors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/drawing.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/drawing.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/BOSL2logo.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/BOSL2logo.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/attachments.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/attachments.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/boolean_geometry.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/boolean_geometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/lsystems.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/lsystems.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/orientations.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/orientations.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/spherical_patch.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/examples/spherical_patch.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/fnliterals.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/fnliterals.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/gears.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/gears.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/geometry.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/geometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/hinges.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/hinges.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/images/BOSL2logo.png` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/images/BOSL2logo.png`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/joiners.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/joiners.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linalg.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/linalg.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linear_bearings.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/linear_bearings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/lists.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/lists.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks2d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/masks2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks3d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/masks3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/math.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/math.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/metric_screws.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/metric_screws.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/modular_hose.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/modular_hose.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/mutators.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/mutators.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/nema_steppers.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/nema_steppers.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/partitions.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/partitions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/paths.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/paths.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/polyhedra.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/polyhedra.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/regions.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/regions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/rounding.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/rounding.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screw_drive.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/screw_drive.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screws.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/screws.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/find_modular_asserts.sh` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/find_modular_asserts.sh`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/func_coverage.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/func_coverage.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/img2scad.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/img2scad.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/increment_version.sh` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/increment_version.sh`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/run_tests.sh` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/scripts/run_tests.sh`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes2d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/shapes2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes3d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/shapes3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/skin.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/skin.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/sliders.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/sliders.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/std.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/std.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/strings.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/strings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/structs.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/structs.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/polyhedra.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/polyhedra.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_affine.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_affine.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_comparisons.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_comparisons.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_coords.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_coords.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_distributors.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_distributors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_drawing.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_drawing.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_edges.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_edges.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_fnliterals.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_fnliterals.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_geometry.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_geometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_linalg.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_linalg.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_lists.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_lists.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_masks2d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_masks2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_math.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_math.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_mutators.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_mutators.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_paths.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_paths.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_regions.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_regions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_rounding.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_rounding.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_screw_drive.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_screw_drive.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_shapes2d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_shapes2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_shapes3d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_shapes3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_skin.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_skin.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_strings.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_strings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_structs.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_structs.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_transforms.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_transforms.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_trigonometry.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_trigonometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_utility.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_utility.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_vectors.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_vectors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_version.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_version.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_vnf.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tests/test_vnf.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/threading.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/threading.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/transforms.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/transforms.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/trigonometry.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/trigonometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tripod_mounts.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tripod_mounts.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/turtle3d.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/turtle3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Attachments.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Attachments.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Distributors.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Distributors.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/FractalTree.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/FractalTree.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Mutators.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Mutators.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Paths.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Paths.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Shapes2d.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Shapes2d.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Shapes3d.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Shapes3d.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Transforms.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/Transforms.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/VNF.md` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/tutorials/VNF.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/utility.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/utility.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vectors.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/vectors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/version.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/version.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vnf.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/vnf.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/walls.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/walls.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/wiring.scad` & `solidpython2-2.0.3/solid2/extensions/bosl2/BOSL2/wiring.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/affine.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/affine.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/attachments.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/attachments.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/ball_bearings.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/ball_bearings.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/beziers.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/beziers.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_base.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/bosl2_base.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_patches.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/bosl2_patches.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/bottlecaps.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/bottlecaps.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/color.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/color.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/comparisons.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/comparisons.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/constants.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/constants.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/coords.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/coords.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/cubetruss.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/cubetruss.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/distributors.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/distributors.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/drawing.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/drawing.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/fnliterals.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/fnliterals.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/gears.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/gears.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/geometry.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/geometry.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/hinges.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/hinges.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/joiners.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/joiners.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/linalg.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/linalg.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/linear_bearings.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/linear_bearings.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/lists.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/lists.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/masks2d.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/masks2d.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/masks3d.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/masks3d.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/math.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/math.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/metric_screws.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/metric_screws.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/modular_hose.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/modular_hose.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/mutators.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/mutators.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/nema_steppers.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/nema_steppers.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/openscad.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/openscad.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/partitions.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/partitions.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/paths.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/paths.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/polyhedra.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/polyhedra.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/regions.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/regions.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/rounding.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/rounding.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/screw_drive.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/screw_drive.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/screws.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/screws.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/shapes2d.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/shapes2d.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/shapes3d.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/shapes3d.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/skin.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/skin.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/sliders.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/sliders.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/std.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/std.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/strings.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/strings.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/structs.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/structs.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/threading.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/threading.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/transforms.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/transforms.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/trigonometry.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/trigonometry.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/tripod_mounts.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/tripod_mounts.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/turtle3d.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/turtle3d.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/utility.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/utility.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/vectors.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/vectors.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/version.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/version.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/vnf.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/vnf.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/walls.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/walls.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2/wiring.py` & `solidpython2-2.0.3/solid2/extensions/bosl2/wiring.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/bosl2_generator.py` & `solidpython2-2.0.3/solid2/extensions/bosl2_generator.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/customizer_widgets.py` & `solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/customizer_widgets.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_interface.py` & `solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/scad_interface.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_variable.py` & `solidpython2-2.0.3/solid2/extensions/greedy_scad_interface/scad_variable.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/openscad_extension_generator.py` & `solidpython2-2.0.3/solid2/extensions/openscad_extension_generator.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/extensions/scad2solid.py` & `solidpython2-2.0.3/solid2/extensions/scad2solid.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/.gitignore` & `solidpython2-2.0.3/solid2/libs/py_scadparser/.gitignore`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/LICENSE` & `solidpython2-2.0.3/solid2/libs/py_scadparser/LICENSE`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/README.md` & `solidpython2-2.0.3/solid2/libs/py_scadparser/README.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-310.pyc` & `solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-310.pyc` & `solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-310.pyc` & `solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-310.pyc` & `solidpython2-2.0.3/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/parsetab.py` & `solidpython2-2.0.3/solid2/libs/py_scadparser/parsetab.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/scad_ast.py` & `solidpython2-2.0.3/solid2/libs/py_scadparser/scad_ast.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/scad_parser.py` & `solidpython2-2.0.3/solid2/libs/py_scadparser/scad_parser.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/solid2/libs/py_scadparser/scad_tokens.py` & `solidpython2-2.0.3/solid2/libs/py_scadparser/scad_tokens.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.2/setup.py` & `solidpython2-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
                              'BOSL2/tutorials/*']}
 
 install_requires = \
 ['ply>=3.11,<4.0', 'setuptools>=65.6.3']
 
 setup_kwargs = {
     'name': 'solidpython2',
-    'version': '2.0.2',
+    'version': '2.0.3',
     'description': 'Python interface to the OpenSCAD declarative geometry language',
-    'long_description': '\n.. image:: https://readthedocs.org/projects/solidpython2/badge/?version=latest\n    :target: http://solidpython2.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n**If you switch from the regular SolidPython:master branch to this branch, have a\nlook at** `Version 2.x.x`_.\n\nSolidPython\n===========\n\n.. contents::\n   \nOpenSCAD for Python\n-------------------\n\nSolidPython is a generalization of Phillip Tiefenbacher\'s openscad\nmodule, found on `Thingiverse <http://www.thingiverse.com/thing:1481>`__. It\ngenerates valid OpenSCAD code from Python code with minimal overhead. Here\'s a\nsimple example:\n\nThis Python code:\n\n.. code:: python\n\n    from solid2 import *\n    d = difference()(\n        cube(10),\n        sphere(15)\n    )\n    d.as_scad()\n\nGenerates this OpenSCAD code:\n\n.. code:: python\n\n    difference(){\n        cube(10);\n        sphere(15);\n    }\n\nThat doesn\'t seem like such a savings, but the following SolidPython code is a\nlot shorter (and I think clearer) than the SCAD code it compiles to:\n\n.. code:: python\n\n    from solid2 import *\n    d = cube(5) + right(5)(sphere(5)) - cylinder(r=2, h=6)\n\nGenerates this OpenSCAD code:\n\n.. code::\n\n    difference(){\n        union(){\n            cube(5);\n            translate( [5, 0,0]){\n                sphere(5);\n            }\n        }\n        cylinder(r=2, h=6);\n    }\n\nAdvantages\n----------\n\nIn contrast to OpenSCAD -- which is a constrained domain specific language --\nPython is a full blown modern programming language and as such supports\npretty much all modern programming features. Furthermore a huge number of\nlibraries is available.\n\nSolidPython lets you use all these fancy python features to generate your\nconstructive solid geometry models.\n\nOn the one hand it makes the generation of your models a lot easier, because\nyou don\'t need to learn another domain specific language and you can use all\nthe programming technique you\'re already familiar with. On the other hand it\ngives you a lot more power, because you can use all the comprehensive python\nlibraries to generate your models.\n\nI would almost say this enables you to do what ever you want with ease.\nAs (maybe little uncommon) example, you could write a program that:\n\n  - looks up the mail adress of your actuall president (based on your ip address)\n  - writes a mail to him or her and asks for a portrait\n  - waits for a reply\n  - generates a heightmap from the picture you received and maps it onto a vase\n\nThis should be pretty straight forward with SolidPython but is impossible with\npure OpenSCAD.\n\nFurhtermore SolidPython 2.x.x is designed to be extendible. As such you can extend SolidPython itself using python. Actually parts of SolidPython itself are implemented as extensions (everything but the core one-to-one mapping of OpenScad to Python), these include operators, access style syntax, convenience functions, scad_interface and bosl2 support. Furthermore some of the SolidPython 1.x.x solid.utils features are also implemented as extensions (bill of material & part-hole).\n\nInstalling SolidPython\n----------------------\n\n-  Install latest release via\n   `PyPI <https://pypi.python.org/pypi/solidpython2>`__:\n\n   .. code:: bash\n\n       pip install solidpython2\n\n   (You may need to use ``sudo pip install solidpython2``, depending on\n   your environment. This is commonly discouraged though. You\'ll be happiest \n   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__ \n   where you can easily control dependencies for a given project)\n\n- Install current master straight from Github:\n\n  .. code:: bash\n\n      pip install git+https://github.com/jeff-dh/SolidPython\n\nUsing SolidPython\n-----------------\n\n-  Include SolidPython at the top of your Python file:\n\n   .. code:: python\n\n       from solid2 import *\n\n   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for \n   a discussion of other import styles)\n\n-  OpenSCAD uses curly-brace blocks ({}) to create its tree. SolidPython\n   uses parentheses with comma-delimited lists. \n   \n   **OpenSCAD:**\n\n   .. code::\n\n       difference(){\n           cube(10);\n           sphere(15);\n       }\n\n   **SolidPython:**\n\n   .. code::\n\n       d = difference()(\n           cube(10),  # Note the comma between each element!\n           sphere(15)\n       )\n\n-  Call ``py_scad_obj.as_scad()`` to generate SCAD code. This returns\n   a string of valid OpenSCAD code.\n-  *or*: call ``py_scad_obj.save_as_scad("filepath.scad")`` to store\n   that code in a file.\n-  If ``filepath.scad`` is open in the OpenSCAD IDE and Design => \'Automatic\n   Reload and Compile\' is checked in the OpenSCAD IDE, running\n   ``py_scad_obj.save_as_scad()`` from Python will load the object in the\n   IDE.\n-  Alternately, you could call OpenSCAD\'s command line and render\n   straight to STL.\n\nImporting OpenSCAD code\n-----------------------\n\n- Use ``solid2.import_scad(path)`` to import OpenSCAD code. Relative paths will check the current location designated in `OpenSCAD library directories <https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Libraries>`__.\n\n**Ex:** \n\n``scadfile.scad``\n\n.. code::\n\n    module box(w,h,d){\n        cube([w,h,d]);\n    }\n\n``your_file.py``\n\n.. code:: python\n\n    from solid2 import *\n\n    scadfile = import_scad(\'/path/to/scadfile.scad\') \n    b = scadfile.box(2,4,6)\n    b.save_as_scad(\'out_file.scad\')\n\n- Recursively import OpenSCAD code by calling ``import_scad()`` with a directory argument.\n\n.. code:: python\n\n    from solid2 import *\n\n    # MCAD is OpenSCAD\'s most common utility library: https://github.com/openscad/MCAD\n    # If it\'s installed for OpenSCAD (on MacOS, at: ``$HOME/Documents/OpenSCAD/libraries``)\n    mcad = import_scad(\'MCAD\')\n\n    # MCAD contains about 15 separate packages, each included as its own namespace\n    print(dir(mcad)) # => [\'bearing\', \'bitmap\', \'boxes\', etc...]\n    mount = mcad.motors.stepper_motor_mount(nema_standard=17)\n    mount.save_as_scad(\'motor_mount_file.scad\')\n\n- OpenSCAD has the ``use()`` and ``include()`` statements for importing SCAD code, and SolidPython has them, too. They pollute the global namespace, though, and you may have better luck with ``import_scad()``,\n\n**Ex:**\n\n``scadfile.scad``\n\n.. code::\n\n    module box(w,h,d){\n        cube([w,h,d]);\n    }\n\n``your_file.py``\n\n.. code:: python\n\n    from solid2 import *\n\n    # use() puts the module `box()` into the global namespace\n    use(\'/path/to/scadfile.scad\') \n    b = box(2,4,6)\n    scad_render_to_file(b, \'out_file.scad\')\n\n\nExample Code\n------------\n\nThe best way to learn how SolidPython works is to look at the included\nexample code. If you\'ve installed SolidPython, the following line of\nPython will print (the location of) the examples directory:\n\n.. code:: python\n\n    import os, solid2; print(os.path.dirname(solid2.__file__) + \'/examples\')\n        \n\nOr browse the example code on Github\n`here <https://github.com/jeff-dh/SolidPython/tree/exp_solid/solid2/examples>`__\n\nExtra syntactic sugar\n=====================\n\nBasic operators\n---------------\n\nSolidPython overrides the basic operators + and | (union), - (difference), \\*\nand & (intersection) and ~ (debug). So\n\n.. code:: python\n\n    c = cylinder(r=10, h=5) + cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = union()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nLikewise:\n\n.. code:: python\n\n    c = cylinder(r=10, h=5)\n    c -= cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = difference()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nAccess Style Syntax\n-------------------\n\nSince at least some people (including me) don\'t like the OpenSCAD Syntax, SolidPython 2.x.x introduces the support for the so called "Access-Style-Syntax". This enables you to call some of the SolidPython / OpenSCAD functions as member functions of any OpenSCADObject instead of wrapping it in an instance of it.\n\nIn other words, e.g. code:\n\n.. code:: python\n\n  up(10)(cube(1))\n  #is equal to\n  cube(1).up(10)\n\nThe available member functions are the following:\n\n.. code:: python\n\n  union, difference, intersection, translate, scale, rotate, mirror, resize,\n  color, offset, hull, render, projection, surface, linear_extrude,\n  rotate_extrude, debug, background, root and disable\n\nAlso the convenience functions are available:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back, translateX, translateY, translateZ,\n  rotateX, rotateY, rotateZ, mirrorX, mirrorY, mirrorZ, scaleX, scaleY, scaleZ,\n  resizeX, resizeY, resizeZ\n\nFurthermore you can chain these functions, because they all return the transformed OpenSCADObject, e.g.:\n\n.. code:: python\n\n  cube(1).up(10).back(20).rotate(10, 0, 5).mirror(1, 0, 0).color("green").root()\n\nConvenience functions\n---------------------\n\nSolidPython includes a number of convenience functions. Currently these\ninclude:\n\nDirections for arranging things:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back\n\nTransformations per dimension:\n\n.. code:: python\n\n  translateX, translateY, translateZ, rotateX, rotateY, rotateZ, mirrorX,\n  mirrorY, mirrorZ, resizeX, resizeY, resizeZ, scaleX, scaleY, scaleZ\n\nFurthermore the operations `translate, scale, resize, mirror, rotate, cube and square` are overwritten in a way that they accept single integer or float values as first parameter. (`translate(1, 2, 3)` equals `translate([1, 2, 3])`)\n\n.. code:: python\n\n    cylinder().rotateY(90).up(10)\n\nseems a lot clearer to me than:\n\n.. code:: python\n\n    translate([0,0,10])(\n        rotate([0, 90, 0])(\n          cylinder()\n    ))\n\nFeatures\n========\n\nBOSL2\n-----\n\nSolidPython supports -- at least -- quite a lot of the **bosl2** library. You can use it by importing the ``solid2.extensions.bosl2``. Take a look at `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_ to get an idea how to use it and what\'s possible.\n\nI would suggest to use it as kind of a standard library for SolidPython.\nTake a look at their `Wiki <https://github.com/revarbat/BOSL2/wiki>`_ to get an idea about it\'s features.\n\n\nAnimation, Customizer, custom Fonts, ImplicitCad, Extensions\n------------------------------------------------------------\n\nSolidPython supports the following features\n\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n* SolidPython is extendible `extensions example 1 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/08-extensions.py>`_  `extension example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/09-code-attach-extension.py>`_\n\nJupyter Renderer\n================\n\nSolidPython can be rendered inside a Jupyter Notebook using ViewScad. Unfortunately the pypi version of ``viewscad`` seems to be not compatible with ``solid2``. @jreiberkyle created `this viewscad fork <https://github.com/jreiberkyle/ViewSCAD>`__ and made it work with `solid2` (`#7 <https://github.com/jeff-dh/SolidPython/issues/7>`__)\n\nVersion 2.x.x\n=============\n\nSolidPython 2.x.x is a refactored version of SolidPython 1.x.x.\nThe refactoring process was based on the following proposal:\nhttps://github.com/SolidCode/SolidPython/issues/169\n\nThe goal was to\n\n* extract the "core" from SolidPython\n* make a solid package that only contains the fundamentals (+ a few convenience features) \n* make it extendible\n* try to get complex libraries working properly (mcad, bosl, bosl2)\n* **KISS**: ``from solid2 import *`` -> imports only ~1000 lines of source code and has (almost?) all the feautres SolidPython 1.x.x has\n* be a drop in replacement for SolidPython 1.x.x -- as far as possible, see Backwards Compatibility Section\n* get all kinds of nice features working (see Features section)\n\nThe result is a refactored and in some parts rewritten version of SolidPython we would like to release as SolidPython 2.x.x. The major improvement is a code base that should be better maintainable and extendible.\n\nBesides these benefits SolidPython 2.x.x implemented quite a few nice new features (cf. Features section).\n\nFeatures\n--------\n\nSolidPython 2.x.x has support for the following new features:\n\n* **bosl2** - SolidPython is now able to handle bosl2 pretty well (don\'t know whether everything works, but quite a lot). `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ and `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ and `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n\nFurthermore it has several minor improvements, like these which are based on ideas from *posts* from the SolidPython universe:\n\n* use invert operator (~) as # in OpenSCAD `#167 <https://github.com/SolidCode/SolidPython/pull/167>`_\n* convenience function including to pass sizes as integer parameters (``translate(10, 20, 30)``) `#63 <https://github.com/SolidCode/SolidPython/pull/63#issuecomment-688171416>`_\n* *access-style* syntax: ``cube(1).up(5).rotate(45, 0, 0)`` `#66 <https://github.com/SolidCode/SolidPython/pull/66>`_ This is additional! The OpenSCAD / SolidPython style syntax is still fully supported.\n\nAnother nice little feature especially to play around and debug it is that the ``__repr__`` operator of each "OpenSCADObject" now calls ``scad_render``. With this the python shell becomes pretty good in debuging and playing around with solid code and the library itself:\n\n.. code:: python\n\n  >>> from solid2 import *\n  >>> c = cube(5)\n  >>> c.up(5)\n  translate(v = [0, 0, 5]) {\n          cube(size = 5);\n  };\n  >>> c.up(5).save_as_scad()\n  \'/home/xxx/xxx/xxx/SolidPython/expsolid_out.scad\'\n  >>>\n\nBackwards compatibility\n-----------------------\n\nSolidPython 2.x.x should be a complete and mostly backwards compatible drop in\nreplacement for SolidPython 1.x.x.\nThe backwards compatibility is not 100% as depicted by the version number.\nSomethings (and even interfaces) changed. We tried to stay as backward\ncompatible as possible.  The package should behave 98% the same as SolidPython\nunless you do some "deep access" -- that\'s by 99% chance not backwards\ncompatible (like modifying OpenSCADObjects or import internal modules).\n\nAs long as you stick to:\n\n.. code:: python\n\n  from solid2 import *\n\nyou shoul be fine.\n\n**solid.utils**\n\n``solid.utils`` consisted of convenience functions and "modelling extensions" (kind of a small third party library like `mcad, bosl, bosl2`).\nThe convenience functions are now -- or the missing ones are supposed to be -- part of `solid2.extensions.convenience` and are automatically importet with the main package.\n\nConcerning the "modelling extensions" I would actually like to get rid of them as part of the SolidPython 2.x.x package. The resons are the following:\n\n* these modelling extensions (like `extrude_along_path, splines, screw_threads, part_hole,...`) don\'t align with the (core) purpose of SolidPython as I understand it (I think SolidPython is supposed to be a python "wrapper" / interface for OpenSCAD)\n* these modelling extensions are "yet another implementation" of common modelling task that need to be maintained. I would prefere a SolidPython design where these features are outsourced into a third party library\n* SolidPython 2.x.x has a pretty good **bosl2** support and bosl2 has all (?) the features provided by `solid.utils`:\n\n  * extrude_along_path: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-path_extrude\n  * First-class Negative Space (Holes): https://github.com/revarbat/BOSL2/wiki/attachments.scad#module-diff\n  * Splines / Bezier: https://github.com/revarbat/BOSL2/wiki/beziers.scad\n  * Screw threads: https://github.com/revarbat/BOSL2/wiki/screws.scad https://github.com/revarbat/BOSL2/wiki/metric_screws.scad https://github.com/revarbat/BOSL2/wiki/threading.scad\n  * distributors: https://github.com/revarbat/BOSL2/wiki/distributors.scad\n  * bouding boxes: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-bounding_box\n  * arcs, pie slices, tubes, ...: https://github.com/revarbat/BOSL2/wiki/shapes3d.scad https://github.com/revarbat/BOSL2/wiki/drawing.scad\n  * cut models in "half" / by a plane: https://github.com/revarbat/BOSL2/wiki/mutators.scad#functionmodule-half_of\n  * attachments: https://github.com/revarbat/BOSL2/wiki/attachments.scad\n\nAnd a looooot more.....\n\nI don\'t see why SolidPython should implement and maintain its own set of these features. Furthermore I assume a third party library (like `bosl2`) is probably able to provide more sophisticated implementations than we will ever be able to provide.\n\nPlease take a look at the `bosl2` implementations. I did some very basic tests in ``examples/07-libs-bosl2.py`` and -- at least -- was able to create basic examples for the core `solid.utils` features using bosl2.\n\nI would also be fine with a python third party library that implements these features, but I would like to seperate it from SolidPython itself. The reason is to achieve a SolidPython module which is independent from it (development, bugs, maintainance) with the goal to get an as solid and stable as possible SolidPython (core) package.\n\nBUT, since I assume quite a few people out there are using `solid.utils` up until now and simply getting rid of it might cause some brouhaha, my suggestion for a compromise is the `solid_legay` extension.\n\n**solid2_legacy**\n\nThe `solid2_legacy` extension is basicly everything that used to be `solid.utils`. Furhtermore it tries to "mimic" the SolidPython 1.x.x interface. This is the effort to become as backward compatible as possible. This might for example be useful when trying to get existing SolidPython 1.x.x code running.\n\nThe `solid2_legacy` extension got extracted into a seperate repo (and pip package). You should be able to just import the package if it is installed or somewhere in your import path.\n\nIf you want to use those features import the extension and take a look at it.\n\n.. code:: python\n\n  from solid2_legacy import *\n\nAnyway SolidPython 1.x.x `imports` do not work with SolidPython 2.x.x! (see Interface changes - imoprt paths have changed)\n\nI was able to get the SolidPython 1.x.x examples running just by changing the imports and they all (except for the splines example which seems to have an internal issue) worked "out of the box".\n\n\n**Interface changes**\n\n* OpenSCAD identifier escaping:\n        * all *illegal* python idetifiers are escape with a single prepending underscore\n        * special variables ``$fn -> _fn`` (*note*: ``segments`` still works)\n        * identifier starting with a digit ``module 12ptStar() -> _12ptStar()`` (*note*: ``__12ptStar`` still works)\n        * python keywords ``module import() -> _import()`` (*note*: ``import\\_``  still works)\n\n* import paths have changed (a lot)\n    * as long as you only import the root package it should be fine, otherwise probably not\n    \n    .. code:: python\n    \n            from solid2 import * #fine\n            from solid2 import objects #crash\n            from solid2 import solidpython #crash\n            from solid2 import splines #crash\n            from solid2 import utils #crash\n\n* all extensions have been moved:\n    * solid.utils has been moved to ``solid2_legacy``. If you want to use them import that extension\n    * there are some example implementations of the part / hole feature and\n      bill of materials in ``solid2_legacy``. They seem to work but are\n      not tested extensively. Take a look at ``examples/xx_legacy*``.\n    * please take a look at the bosl2 example. BOSL2 provides many features which\n      might be alternatives.\n\n* OpenSCADObject internally changed a lot\n    If you access it directly\n    (e.g. mycube.set_modifier) this might not work. But if you import\n    ``solid2_legacy`` some dummy methods will be monkey patched onto\n    OpenSCADObject so you might be able to at least run the code, but it\n    might render not correctly.\n\n* maybe some more things I can\'t remember. Some function signatures changed\n  slightly. But as long as as you stick to the regular public interface\n  everything should be fine.\n\n\nContact\n=======\n\nEnjoy!\n\nIf you have any questions or bug reports please report them to the SolidPython\n`GitHub page <https://github.com/jeff-dh/SolidPython>`__!\n\n\n\nCheers!\n\nLicense\n=======\n\nThis library is free software; you can redistribute it and/or modify it\nunder the terms of the GNU Lesser General Public License as published by\nthe Free Software Foundation; either version 2.1 of the License, or (at\nyour option) any later version.\n\nThis library is distributed in the hope that it will be useful, but\nWITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\nGeneral Public License for more details.\n\n`Full text of the\nlicense <http://www.gnu.org/licenses/old-licenses/lgpl-2.1.txt>`__.\n\nSome class docstrings are derived from the `OpenSCAD User Manual\n<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so \nare available under the `Creative Commons Attribution-ShareAlike License\n<https://creativecommons.org/licenses/by-sa/3.0/>`__. \n\n',
+    'long_description': '\n.. image:: https://readthedocs.org/projects/solidpython2/badge/?version=latest\n    :target: http://solidpython2.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n**If you switch from the regular SolidPython:master branch to this branch, have a\nlook at** `Version 2.x.x`_.\n\nSolidPython\n===========\n\n.. contents::\n\nOpenSCAD for Python\n-------------------\n\nSolidPython is a generalization of Phillip Tiefenbacher\'s openscad\nmodule, found on `Thingiverse <http://www.thingiverse.com/thing:1481>`__. It\ngenerates valid OpenSCAD code from Python code with minimal overhead. Here\'s a\nsimple example:\n\nThis Python code:\n\n.. code:: python\n\n    from solid2 import *\n    d = difference()(\n        cube(10),\n        sphere(15)\n    )\n    d.as_scad()\n\nGenerates this OpenSCAD code:\n\n.. code:: python\n\n    difference(){\n        cube(10);\n        sphere(15);\n    }\n\nThat doesn\'t seem like such a savings, but the following SolidPython code is a\nlot shorter (and I think clearer) than the SCAD code it compiles to:\n\n.. code:: python\n\n    from solid2 import *\n    d = cube(5) + sphere(5).right(5) - cylinder(r=2, h=6)\n\nGenerates this OpenSCAD code:\n\n.. code::\n\n    difference(){\n        union(){\n            cube(5);\n            translate( [5, 0,0]){\n                sphere(5);\n            }\n        }\n        cylinder(r=2, h=6);\n    }\n\nAdvantages\n----------\n\nIn contrast to OpenSCAD -- which is a constrained domain specific language --\nPython is a full blown modern programming language and as such supports\npretty much all modern programming features. Furthermore a huge number of\nlibraries is available.\n\nSolidPython lets you use all these fancy python features to generate your\nconstructive solid geometry models.\n\nOn the one hand it makes the generation of your models a lot easier, because\nyou don\'t need to learn another domain specific language and you can use all\nthe programming technique you\'re already familiar with. On the other hand it\ngives you a lot more power, because you can use all the comprehensive python\nlibraries to generate your models.\n\nI would almost say this enables you to do what ever you want with ease.\nAs (maybe little uncommon) example, you could write a program that:\n\n  - looks up the mail adress of your actuall president (based on your ip address)\n  - writes a mail to him or her and asks for a portrait\n  - waits for a reply\n  - generates a heightmap from the picture you received and maps it onto a vase\n\nThis should be pretty straight forward with SolidPython but is impossible with\npure OpenSCAD.\n\nFurhtermore SolidPython 2.x.x is designed to be extendible. As such you can extend SolidPython itself using python. Actually parts of SolidPython itself are implemented as extensions (everything but the core one-to-one mapping of OpenScad to Python), these include operators, access style syntax, convenience functions, scad_interface and bosl2 support. Furthermore some of the SolidPython 1.x.x solid.utils features are also implemented as extensions (bill of material & part-hole).\n\nInstalling SolidPython\n----------------------\n\n-  Install latest release via\n   `PyPI <https://pypi.python.org/pypi/solidpython2>`__:\n\n   .. code:: bash\n\n       pip install solidpython2\n\n   (You may need to use ``sudo pip install solidpython2``, depending on\n   your environment. This is commonly discouraged though. You\'ll be happiest\n   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__\n   where you can easily control dependencies for a given project)\n\n- Install current master straight from Github:\n\n  .. code:: bash\n\n      pip install git+https://github.com/jeff-dh/SolidPython\n\nUsing SolidPython\n-----------------\n\n-  Include SolidPython at the top of your Python file:\n\n   .. code:: python\n\n       from solid2 import *\n\n   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for\n   a discussion of other import styles)\n\n-  OpenSCAD uses curly-brace blocks ({}) to create its tree. SolidPython\n   uses parentheses with comma-delimited lists.\n\n   **OpenSCAD:**\n\n   .. code::\n\n       difference(){\n           cube(10);\n           sphere(15);\n       }\n\n   **SolidPython:**\n\n   .. code::\n\n       d = difference()(\n           cube(10),  # Note the comma between each element!\n           sphere(15)\n       )\n\n-  Call ``py_scad_obj.as_scad()`` to generate SCAD code. This returns\n   a string of valid OpenSCAD code.\n-  *or*: call ``py_scad_obj.save_as_scad("filepath.scad")`` to store\n   that code in a file.\n-  If ``filepath.scad`` is open in the OpenSCAD IDE and Design => \'Automatic\n   Reload and Compile\' is checked in the OpenSCAD IDE, running\n   ``py_scad_obj.save_as_scad()`` from Python will load the object in the\n   IDE.\n-  Alternately, you could call OpenSCAD\'s command line and render\n   straight to STL.\n\nTutorial - Example Code\n-----------------------\n\nThe best way to learn how SolidPython works is to look at the included\nexample code. They are kind of a minimalistic SolidPython tutorial. If\nyou\'ve installed SolidPython, the following line of Python will print\n(the location of) the examples directory:\n\n.. code:: python\n\n    import os, solid2; print(os.path.dirname(solid2.__file__) + \'/examples\')\n\n\nOr browse the example code on Github\n`here <https://github.com/jeff-dh/SolidPython/tree/exp_solid/solid2/examples>`__\n\nExtra syntactic sugar\n=====================\n\nBasic operators\n---------------\n\nSolidPython overrides the basic operators + and | (union), - (difference), \\*\nand & (intersection) and ~ (debug). So\n\n.. code:: python\n\n    c = cylinder(r=10, h=5) + cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = union()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nLikewise:\n\n.. code:: python\n\n    c = cylinder(r=10, h=5)\n    c -= cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = difference()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nAccess Style Syntax\n-------------------\n\nSince at least some people (including me) don\'t like the OpenSCAD Syntax, SolidPython 2.x.x introduces the support for the so called "Access-Style-Syntax". This enables you to call some of the SolidPython / OpenSCAD functions as member functions of any OpenSCADObject instead of wrapping it in an instance of it.\n\nIn other words, e.g. code:\n\n.. code:: python\n\n  up(10)(cube(1))\n  #is equal to\n  cube(1).up(10)\n\nThe available member functions are the following:\n\n.. code:: python\n\n  union, difference, intersection, translate, scale, rotate, mirror, resize,\n  color, offset, hull, render, projection, surface, linear_extrude,\n  rotate_extrude, debug, background, root and disable\n\nAlso the convenience functions are available:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back, translateX, translateY, translateZ,\n  rotateX, rotateY, rotateZ, mirrorX, mirrorY, mirrorZ, scaleX, scaleY, scaleZ,\n  resizeX, resizeY, resizeZ\n\nFurthermore you can chain these functions, because they all return the transformed OpenSCADObject, e.g.:\n\n.. code:: python\n\n  cube(1).up(10).back(20).rotate(10, 0, 5).mirror(1, 0, 0).color("green").root()\n\nConvenience functions\n---------------------\n\nSolidPython includes a number of convenience functions. Currently these\ninclude:\n\nDirections for arranging things:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back\n\nTransformations per dimension:\n\n.. code:: python\n\n  translateX, translateY, translateZ, rotateX, rotateY, rotateZ, mirrorX,\n  mirrorY, mirrorZ, resizeX, resizeY, resizeZ, scaleX, scaleY, scaleZ\n\nFurthermore the operations `translate, scale, resize, mirror, rotate, cube and square` are overwritten in a way that they accept single integer or float values as first parameter. (`translate(1, 2, 3)` equals `translate([1, 2, 3])`)\n\n.. code:: python\n\n    cylinder().rotateY(90).up(10)\n\nseems a lot clearer to me than:\n\n.. code:: python\n\n    translate([0,0,10])(\n        rotate([0, 90, 0])(\n          cylinder()\n    ))\n\nFeatures\n========\n\nBOSL2\n-----\n\nSolidPython supports -- at least -- quite a lot of the **bosl2** library. You can use it by importing the ``solid2.extensions.bosl2``. Take a look at `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_ to get an idea how to use it and what\'s possible.\n\nI would suggest to use it as kind of a standard library for SolidPython.\nTake a look at their `Wiki <https://github.com/revarbat/BOSL2/wiki>`_ to get an idea about it\'s features.\n\n\nAnimation, Customizer, custom Fonts, ImplicitCad, Extensions\n------------------------------------------------------------\n\nSolidPython supports the following features\n\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n* SolidPython is extendible `extensions example 1 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/08-extensions.py>`_  `extension example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/09-code-attach-extension.py>`_\n\nJupyter Renderer\n================\n\nSolidPython can be rendered inside a Jupyter Notebook using ViewScad. Unfortunately the pypi version of ``viewscad`` seems to be not compatible with ``solid2``. @jreiberkyle created `this viewscad fork <https://github.com/jreiberkyle/ViewSCAD>`__ and made it work with `solid2` (`#7 <https://github.com/jeff-dh/SolidPython/issues/7>`__)\n\nVersion 2.x.x\n=============\n\nSolidPython 2.x.x is a refactored version of SolidPython 1.x.x.\nThe refactoring process was based on the following proposal:\nhttps://github.com/SolidCode/SolidPython/issues/169\n\nThe goal was to\n\n* extract the "core" from SolidPython\n* make a solid package that only contains the fundamentals (+ a few convenience features)\n* make it extendible\n* try to get complex libraries working properly (mcad, bosl, bosl2)\n* **KISS**: ``from solid2 import *`` -> imports only ~1000 lines of source code and has (almost?) all the feautres SolidPython 1.x.x has\n* be a drop in replacement for SolidPython 1.x.x -- as far as possible, see Backwards Compatibility Section\n* get all kinds of nice features working (see Features section)\n\nThe result is a refactored and in some parts rewritten version of SolidPython we would like to release as SolidPython 2.x.x. The major improvement is a code base that should be better maintainable and extendible.\n\nBesides these benefits SolidPython 2.x.x implemented quite a few nice new features (cf. Features section).\n\nFeatures\n--------\n\nSolidPython 2.x.x has support for the following new features:\n\n* **bosl2** - SolidPython is now able to handle bosl2 pretty well (don\'t know whether everything works, but quite a lot). `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ and `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ and `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n\nFurthermore it has several minor improvements, like these which are based on ideas from *posts* from the SolidPython universe:\n\n* use invert operator (~) as # in OpenSCAD `#167 <https://github.com/SolidCode/SolidPython/pull/167>`_\n* convenience function including to pass sizes as integer parameters (``translate(10, 20, 30)``) `#63 <https://github.com/SolidCode/SolidPython/pull/63#issuecomment-688171416>`_\n* *access-style* syntax: ``cube(1).up(5).rotate(45, 0, 0)`` `#66 <https://github.com/SolidCode/SolidPython/pull/66>`_ This is additional! The OpenSCAD / SolidPython style syntax is still fully supported.\n\nAnother nice little feature especially to play around and debug it is that the ``__repr__`` operator of each "OpenSCADObject" now calls ``scad_render``. With this the python shell becomes pretty good in debuging and playing around with solid code and the library itself:\n\n.. code:: python\n\n  >>> from solid2 import *\n  >>> c = cube(5)\n  >>> c.up(5)\n  translate(v = [0, 0, 5]) {\n          cube(size = 5);\n  };\n  >>> c.up(5).save_as_scad()\n  \'/home/xxx/xxx/xxx/SolidPython/expsolid_out.scad\'\n  >>>\n\nBackwards compatibility\n-----------------------\n\nSolidPython 2.x.x should be a complete and mostly backwards compatible drop in\nreplacement for SolidPython 1.x.x.\nThe backwards compatibility is not 100% as depicted by the version number.\nSomethings (and even interfaces) changed. We tried to stay as backward\ncompatible as possible.  The package should behave 98% the same as SolidPython\nunless you do some "deep access" -- that\'s by 99% chance not backwards\ncompatible (like modifying OpenSCADObjects or import internal modules).\n\nAs long as you stick to:\n\n.. code:: python\n\n  from solid2 import *\n\nyou shoul be fine.\n\n**solid.utils**\n\n``solid.utils`` consisted of convenience functions and "modelling extensions" (kind of a small third party library like `mcad, bosl, bosl2`).\nThe convenience functions are now -- or the missing ones are supposed to be -- part of `solid2.extensions.convenience` and are automatically importet with the main package.\n\nConcerning the "modelling extensions" I would actually like to get rid of them as part of the SolidPython 2.x.x package. The resons are the following:\n\n* these modelling extensions (like `extrude_along_path, splines, screw_threads, part_hole,...`) don\'t align with the (core) purpose of SolidPython as I understand it (I think SolidPython is supposed to be a python "wrapper" / interface for OpenSCAD)\n* these modelling extensions are "yet another implementation" of common modelling task that need to be maintained. I would prefere a SolidPython design where these features are outsourced into a third party library\n* SolidPython 2.x.x has a pretty good **bosl2** support and bosl2 has all (?) the features provided by `solid.utils`:\n\n  * extrude_along_path: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-path_extrude\n  * First-class Negative Space (Holes): https://github.com/revarbat/BOSL2/wiki/attachments.scad#module-diff\n  * Splines / Bezier: https://github.com/revarbat/BOSL2/wiki/beziers.scad\n  * Screw threads: https://github.com/revarbat/BOSL2/wiki/screws.scad https://github.com/revarbat/BOSL2/wiki/metric_screws.scad https://github.com/revarbat/BOSL2/wiki/threading.scad\n  * distributors: https://github.com/revarbat/BOSL2/wiki/distributors.scad\n  * bouding boxes: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-bounding_box\n  * arcs, pie slices, tubes, ...: https://github.com/revarbat/BOSL2/wiki/shapes3d.scad https://github.com/revarbat/BOSL2/wiki/drawing.scad\n  * cut models in "half" / by a plane: https://github.com/revarbat/BOSL2/wiki/mutators.scad#functionmodule-half_of\n  * attachments: https://github.com/revarbat/BOSL2/wiki/attachments.scad\n\nAnd a looooot more.....\n\nI don\'t see why SolidPython should implement and maintain its own set of these features. Furthermore I assume a third party library (like `bosl2`) is probably able to provide more sophisticated implementations than we will ever be able to provide.\n\nPlease take a look at the `bosl2` implementations. I did some very basic tests in ``examples/07-libs-bosl2.py`` and -- at least -- was able to create basic examples for the core `solid.utils` features using bosl2.\n\nI would also be fine with a python third party library that implements these features, but I would like to seperate it from SolidPython itself. The reason is to achieve a SolidPython module which is independent from it (development, bugs, maintainance) with the goal to get an as solid and stable as possible SolidPython (core) package.\n\nBUT, since I assume quite a few people out there are using `solid.utils` up until now and simply getting rid of it might cause some brouhaha, my suggestion for a compromise is the `solid_legay` extension.\n\n**solid2_legacy**\n\nThe `solid2_legacy` extension is basicly everything that used to be `solid.utils`. Furhtermore it tries to "mimic" the SolidPython 1.x.x interface. This is the effort to become as backward compatible as possible. This might for example be useful when trying to get existing SolidPython 1.x.x code running.\n\nThe `solid2_legacy` extension got extracted into a seperate repo (and pip package). You should be able to just import the package if it is installed or somewhere in your import path.\n\nIf you want to use those features import the extension and take a look at it.\n\n.. code:: python\n\n  from solid2_legacy import *\n\nAnyway SolidPython 1.x.x `imports` do not work with SolidPython 2.x.x! (see Interface changes - imoprt paths have changed)\n\nI was able to get the SolidPython 1.x.x examples running just by changing the imports and they all (except for the splines example which seems to have an internal issue) worked "out of the box".\n\n\n**Interface changes**\n\n* OpenSCAD identifier escaping:\n        * all *illegal* python idetifiers are escape with a single prepending underscore\n        * special variables ``$fn -> _fn`` (*note*: ``segments`` still works)\n        * identifier starting with a digit ``module 12ptStar() -> _12ptStar()`` (*note*: ``__12ptStar`` still works)\n        * python keywords ``module import() -> _import()`` (*note*: ``import\\_``  still works)\n\n* import paths have changed (a lot)\n    * as long as you only import the root package it should be fine, otherwise probably not\n\n    .. code:: python\n\n            from solid2 import * #fine\n            from solid2 import objects #crash\n            from solid2 import solidpython #crash\n            from solid2 import splines #crash\n            from solid2 import utils #crash\n\n* all extensions have been moved:\n    * solid.utils has been moved to ``solid2_legacy``. If you want to use them import that extension\n    * there are some example implementations of the part / hole feature and\n      bill of materials in ``solid2_legacy``. They seem to work but are\n      not tested extensively. Take a look at ``examples/xx_legacy*``.\n    * please take a look at the bosl2 example. BOSL2 provides many features which\n      might be alternatives.\n\n* OpenSCADObject internally changed a lot\n    If you access it directly\n    (e.g. mycube.set_modifier) this might not work. But if you import\n    ``solid2_legacy`` some dummy methods will be monkey patched onto\n    OpenSCADObject so you might be able to at least run the code, but it\n    might render not correctly.\n\n* maybe some more things I can\'t remember. Some function signatures changed\n  slightly. But as long as as you stick to the regular public interface\n  everything should be fine.\n\n\nContact\n=======\n\nEnjoy!\n\nIf you have any questions or bug reports please report them to the SolidPython\n`GitHub page <https://github.com/jeff-dh/SolidPython>`__!\n\n\n\nCheers!\n\nLicense\n=======\n\nThis library is free software; you can redistribute it and/or modify it\nunder the terms of the GNU Lesser General Public License as published by\nthe Free Software Foundation; either version 2.1 of the License, or (at\nyour option) any later version.\n\nThis library is distributed in the hope that it will be useful, but\nWITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\nGeneral Public License for more details.\n\n`Full text of the\nlicense <http://www.gnu.org/licenses/old-licenses/lgpl-2.1.txt>`__.\n\nSome class docstrings are derived from the `OpenSCAD User Manual\n<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so\nare available under the `Creative Commons Attribution-ShareAlike License\n<https://creativecommons.org/licenses/by-sa/3.0/>`__.\n\n',
     'author': 'jeff',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeff-dh/SolidPython',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `solidpython2-2.0.2/PKG-INFO` & `solidpython2-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidpython2
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python interface to the OpenSCAD declarative geometry language
 Home-page: https://github.com/jeff-dh/SolidPython
 License: LGPL-2.1
 Keywords: 3D,CAD,CSG,constructive solid geometry,geometry,modeling,OpenSCAD
 Author: jeff
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
@@ -36,15 +36,15 @@
 **If you switch from the regular SolidPython:master branch to this branch, have a
 look at** `Version 2.x.x`_.
 
 SolidPython
 ===========
 
 .. contents::
-   
+
 OpenSCAD for Python
 -------------------
 
 SolidPython is a generalization of Phillip Tiefenbacher's openscad
 module, found on `Thingiverse <http://www.thingiverse.com/thing:1481>`__. It
 generates valid OpenSCAD code from Python code with minimal overhead. Here's a
 simple example:
@@ -71,15 +71,15 @@
 
 That doesn't seem like such a savings, but the following SolidPython code is a
 lot shorter (and I think clearer) than the SCAD code it compiles to:
 
 .. code:: python
 
     from solid2 import *
-    d = cube(5) + right(5)(sphere(5)) - cylinder(r=2, h=6)
+    d = cube(5) + sphere(5).right(5) - cylinder(r=2, h=6)
 
 Generates this OpenSCAD code:
 
 .. code::
 
     difference(){
         union(){
@@ -128,16 +128,16 @@
    `PyPI <https://pypi.python.org/pypi/solidpython2>`__:
 
    .. code:: bash
 
        pip install solidpython2
 
    (You may need to use ``sudo pip install solidpython2``, depending on
-   your environment. This is commonly discouraged though. You'll be happiest 
-   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__ 
+   your environment. This is commonly discouraged though. You'll be happiest
+   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__
    where you can easily control dependencies for a given project)
 
 - Install current master straight from Github:
 
   .. code:: bash
 
       pip install git+https://github.com/jeff-dh/SolidPython
@@ -147,20 +147,20 @@
 
 -  Include SolidPython at the top of your Python file:
 
    .. code:: python
 
        from solid2 import *
 
-   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for 
+   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for
    a discussion of other import styles)
 
 -  OpenSCAD uses curly-brace blocks ({}) to create its tree. SolidPython
-   uses parentheses with comma-delimited lists. 
-   
+   uses parentheses with comma-delimited lists.
+
    **OpenSCAD:**
 
    .. code::
 
        difference(){
            cube(10);
            sphere(15);
@@ -182,89 +182,26 @@
 -  If ``filepath.scad`` is open in the OpenSCAD IDE and Design => 'Automatic
    Reload and Compile' is checked in the OpenSCAD IDE, running
    ``py_scad_obj.save_as_scad()`` from Python will load the object in the
    IDE.
 -  Alternately, you could call OpenSCAD's command line and render
    straight to STL.
 
-Importing OpenSCAD code
+Tutorial - Example Code
 -----------------------
 
-- Use ``solid2.import_scad(path)`` to import OpenSCAD code. Relative paths will check the current location designated in `OpenSCAD library directories <https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Libraries>`__.
-
-**Ex:** 
-
-``scadfile.scad``
-
-.. code::
-
-    module box(w,h,d){
-        cube([w,h,d]);
-    }
-
-``your_file.py``
-
-.. code:: python
-
-    from solid2 import *
-
-    scadfile = import_scad('/path/to/scadfile.scad') 
-    b = scadfile.box(2,4,6)
-    b.save_as_scad('out_file.scad')
-
-- Recursively import OpenSCAD code by calling ``import_scad()`` with a directory argument.
-
-.. code:: python
-
-    from solid2 import *
-
-    # MCAD is OpenSCAD's most common utility library: https://github.com/openscad/MCAD
-    # If it's installed for OpenSCAD (on MacOS, at: ``$HOME/Documents/OpenSCAD/libraries``)
-    mcad = import_scad('MCAD')
-
-    # MCAD contains about 15 separate packages, each included as its own namespace
-    print(dir(mcad)) # => ['bearing', 'bitmap', 'boxes', etc...]
-    mount = mcad.motors.stepper_motor_mount(nema_standard=17)
-    mount.save_as_scad('motor_mount_file.scad')
-
-- OpenSCAD has the ``use()`` and ``include()`` statements for importing SCAD code, and SolidPython has them, too. They pollute the global namespace, though, and you may have better luck with ``import_scad()``,
-
-**Ex:**
-
-``scadfile.scad``
-
-.. code::
-
-    module box(w,h,d){
-        cube([w,h,d]);
-    }
-
-``your_file.py``
-
-.. code:: python
-
-    from solid2 import *
-
-    # use() puts the module `box()` into the global namespace
-    use('/path/to/scadfile.scad') 
-    b = box(2,4,6)
-    scad_render_to_file(b, 'out_file.scad')
-
-
-Example Code
-------------
-
 The best way to learn how SolidPython works is to look at the included
-example code. If you've installed SolidPython, the following line of
-Python will print (the location of) the examples directory:
+example code. They are kind of a minimalistic SolidPython tutorial. If
+you've installed SolidPython, the following line of Python will print
+(the location of) the examples directory:
 
 .. code:: python
 
     import os, solid2; print(os.path.dirname(solid2.__file__) + '/examples')
-        
+
 
 Or browse the example code on Github
 `here <https://github.com/jeff-dh/SolidPython/tree/exp_solid/solid2/examples>`__
 
 Extra syntactic sugar
 =====================
 
@@ -406,15 +343,15 @@
 SolidPython 2.x.x is a refactored version of SolidPython 1.x.x.
 The refactoring process was based on the following proposal:
 https://github.com/SolidCode/SolidPython/issues/169
 
 The goal was to
 
 * extract the "core" from SolidPython
-* make a solid package that only contains the fundamentals (+ a few convenience features) 
+* make a solid package that only contains the fundamentals (+ a few convenience features)
 * make it extendible
 * try to get complex libraries working properly (mcad, bosl, bosl2)
 * **KISS**: ``from solid2 import *`` -> imports only ~1000 lines of source code and has (almost?) all the feautres SolidPython 1.x.x has
 * be a drop in replacement for SolidPython 1.x.x -- as far as possible, see Backwards Compatibility Section
 * get all kinds of nice features working (see Features section)
 
 The result is a refactored and in some parts rewritten version of SolidPython we would like to release as SolidPython 2.x.x. The major improvement is a code base that should be better maintainable and extendible.
@@ -525,17 +462,17 @@
         * all *illegal* python idetifiers are escape with a single prepending underscore
         * special variables ``$fn -> _fn`` (*note*: ``segments`` still works)
         * identifier starting with a digit ``module 12ptStar() -> _12ptStar()`` (*note*: ``__12ptStar`` still works)
         * python keywords ``module import() -> _import()`` (*note*: ``import\_``  still works)
 
 * import paths have changed (a lot)
     * as long as you only import the root package it should be fine, otherwise probably not
-    
+
     .. code:: python
-    
+
             from solid2 import * #fine
             from solid2 import objects #crash
             from solid2 import solidpython #crash
             from solid2 import splines #crash
             from solid2 import utils #crash
 
 * all extensions have been moved:
@@ -583,12 +520,12 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 General Public License for more details.
 
 `Full text of the
 license <http://www.gnu.org/licenses/old-licenses/lgpl-2.1.txt>`__.
 
 Some class docstrings are derived from the `OpenSCAD User Manual
-<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so 
+<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so
 are available under the `Creative Commons Attribution-ShareAlike License
-<https://creativecommons.org/licenses/by-sa/3.0/>`__. 
+<https://creativecommons.org/licenses/by-sa/3.0/>`__.
```

