# Comparing `tmp/tensorboardX-2.6.1.tar.gz` & `tmp/tensorboardX-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorboardX-2.6.1.tar", last modified: Sun Jun 18 16:42:12 2023, max compression
+gzip compressed data, was "tensorboardX-2.6.2.tar", last modified: Sun Jul 30 14:05:06 2023, max compression
```

## Comparing `tensorboardX-2.6.1.tar` & `tensorboardX-2.6.2.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/feature-requests-or-general-questions.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/workflows/build-pip.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/compile.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.509843 tensorboardX-2.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/docs/_static/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.509843 tensorboardX-2.6.1/docs/_static/img/tensorboard/
--rw-r--r--   0 runner    (1001) docker     (123)    48135 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_histogram.png
--rw-r--r--   0 runner    (1001) docker     (123)    64086 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_hparam.png
--rw-r--r--   0 runner    (1001) docker     (123)    47119 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_image.png
--rw-r--r--   0 runner    (1001) docker     (123)    76694 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_images.png
--rw-r--r--   0 runner    (1001) docker     (123)   571509 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_mesh.png
--rw-r--r--   0 runner    (1001) docker     (123)    45941 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalar.png
--rw-r--r--   0 runner    (1001) docker     (123)   146137 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalar_global.png
--rw-r--r--   0 runner    (1001) docker     (123)    99156 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalars.png
--rw-r--r--   0 runner    (1001) docker     (123)   160926 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/hier_tags.png
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/tensorboard.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/tutorial_zh.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/utils.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/run_pytest.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.513843 tensorboardX-2.6.1/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   490837 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/Demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/audio.png
--rw-r--r--   0 runner    (1001) docker     (123)  1373389 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/comet.gif
--rw-r--r--   0 runner    (1001) docker     (123)    65080 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/distribution.png
--rw-r--r--   0 runner    (1001) docker     (123)   181800 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/embedding.png
--rw-r--r--   0 runner    (1001) docker     (123)    71618 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/graph.png
--rw-r--r--   0 runner    (1001) docker     (123)   257734 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/histogram.png
--rw-r--r--   0 runner    (1001) docker     (123)  1077074 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/image.png
--rw-r--r--   0 runner    (1001) docker     (123)   119007 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/scalar.png
--rw-r--r--   0 runner    (1001) docker     (123)    38551 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/text.png
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX/beholder/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/beholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/file_system_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/shared_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/video_writing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/caffe2_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/comet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/crc32c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/event_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/global_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/onnx_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/openvino_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/api.proto
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/attr_value.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/attr_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/event.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/graph.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/layout.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/layout_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/node_def.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/node_def_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_text.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/resource_handle.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/resource_handle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/summary.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/summary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor_shape.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor_shape_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/types.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/versions.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/versions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/record_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/torchvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/visdom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    52414 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/x2num.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.521844 tensorboardX-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/event_file_writer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/tests/expect/
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/caffe_mnist.expect
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/caffe_overfeat.expect
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_caffe2.test_simple_cnnmodel.expect
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_caffe2.test_simple_model.expect
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_pr_curve.test_pr_purve.expect
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_pr_curve.test_pr_purve_raw.expect
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_audio.expect
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_custom_scalars.expect
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_float32_image.expect
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_histogram_auto.expect
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_histogram_doane.expect
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_histogram_fd.expect
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_hparams.expect
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_hparams_bool.expect
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_hparams_string.expect
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_3_channel_batched.expect
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_boxes.expect
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_four_channel.expect
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_four_channel_batched.expect
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_one_channel.expect
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_one_channel_batched.expect
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_without_channel.expect
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_mesh.expect
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_text.expect
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_uint8_image.expect
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_video.expect
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    26454 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/mnist-8.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/record_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_beholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_chainer_np.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_crc32c.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_multiprocess_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_onnx_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_openvino_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_pr_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_pytorch_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_pytorch_np.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_record_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_summary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_visdom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.175265 tensorboardX-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.143265 tensorboardX-2.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.147265 tensorboardX-2.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.github/ISSUE_TEMPLATE/feature-requests-or-general-questions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.147265 tensorboardX-2.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.github/workflows/build-pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-30 14:05:06.175265 tensorboardX-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/compile.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.147265 tensorboardX-2.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.143265 tensorboardX-2.6.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.143265 tensorboardX-2.6.2/docs/_static/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.151265 tensorboardX-2.6.2/docs/_static/img/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    48135 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_histogram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64086 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_hparam.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47119 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76694 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_images.png
+-rw-r--r--   0 runner    (1001) docker     (123)   571509 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_mesh.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45941 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_scalar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146137 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_scalar_global.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99156 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/add_scalars.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160926 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/_static/img/tensorboard/hier_tags.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/tensorboard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/tutorial_zh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/docs/utils.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/run_pytest.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.159265 tensorboardX-2.6.2/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   490837 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/Demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/audio.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1373389 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/comet.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    65080 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/distribution.png
+-rw-r--r--   0 runner    (1001) docker     (123)   181800 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/embedding.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71618 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)   257734 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/histogram.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1077074 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)   119007 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/scalar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38551 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/screenshots/text.png
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-30 14:05:06.175265 tensorboardX-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.159265 tensorboardX-2.6.2/tensorboardX/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 14:05:05.000000 tensorboardX-2.6.2/tensorboardX/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.163265 tensorboardX-2.6.2/tensorboardX/beholder/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/beholder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/beholder/beholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/beholder/file_system_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/beholder/shared_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/beholder/video_writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/caffe2_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/comet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/crc32c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/event_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/global_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/openvino_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.167265 tensorboardX-2.6.2/tensorboardX/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/api.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/attr_value.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/attr_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/event.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/graph.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/layout.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/layout_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/node_def.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/node_def_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_hparams.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_hparams_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_mesh.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_pr_curve.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_pr_curve_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_text.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/plugin_text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/resource_handle.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/resource_handle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/summary.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/summary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/tensor.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/tensor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/tensor_shape.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/tensor_shape_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/types.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/versions.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/proto/versions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/record_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24491 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/torchvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/visdom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52424 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tensorboardX/x2num.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.163265 tensorboardX-2.6.2/tensorboardX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-30 14:05:06.000000 tensorboardX-2.6.2/tensorboardX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-30 14:05:06.000000 tensorboardX-2.6.2/tensorboardX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:05:06.000000 tensorboardX-2.6.2/tensorboardX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:05:06.000000 tensorboardX-2.6.2/tensorboardX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 14:05:06.000000 tensorboardX-2.6.2/tensorboardX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 14:05:06.000000 tensorboardX-2.6.2/tensorboardX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.171265 tensorboardX-2.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/event_file_writer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:05:06.175265 tensorboardX-2.6.2/tests/expect/
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/caffe_mnist.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/caffe_overfeat.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_caffe2.test_simple_cnnmodel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_caffe2.test_simple_model.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_pr_curve.test_pr_purve.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_pr_curve.test_pr_purve_raw.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_audio.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_custom_scalars.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_float32_image.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_histogram_auto.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_histogram_doane.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_histogram_fd.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_hparams.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_hparams_bool.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_hparams_string.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_3_channel_batched.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_boxes.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_four_channel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_four_channel_batched.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_one_channel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_one_channel_batched.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_image_without_channel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_mesh.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_text.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_uint8_image.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect/test_summary.test_video.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/expect_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26454 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/mnist-8.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/record_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_beholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_chainer_np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_crc32c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_multiprocess_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_openvino_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_pr_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_pytorch_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_pytorch_np.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_record_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_summary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_visdom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-30 14:04:59.000000 tensorboardX-2.6.2/tests/test_writer.py
```

### Comparing `tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `tensorboardX-2.6.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/.github/workflows/build-pip.yml` & `tensorboardX-2.6.2/.github/workflows/build-pip.yml`

 * *Files 16% similar despite different names*

```diff
@@ -13,25 +13,28 @@
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python 3.9
       uses: actions/setup-python@v3
       with:
         python-version: 3.9
 
+    - name: Get tags
+      run: git fetch --tags origin
+
     - name: Install pypa/build
       run: >-
         python -m
         pip install
         build wheel
         --user
 
     - name: Build a binary wheel and a source tarball
       run: |
         echo `pwd`
-        echo `git log|head -n 50`
+        echo `git describe --tags`
         python setup.py -q sdist bdist_wheel --universal
 
     - name: Archive production artifacts
       uses: actions/upload-artifact@v3
       with:
         name: dist-pip-whl
         path: |
```

### Comparing `tensorboardX-2.6.1/.github/workflows/publish-pypi.yml` & `tensorboardX-2.6.2/.github/workflows/publish-pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 
     - uses: actions/checkout@v3
     - name: Set up Python 3.9
       uses: actions/setup-python@v3
       with:
         python-version: 3.9
 
+    - name: Get tags and checkout target version
+      run: |
+        git fetch --tags origin
+        git checkout ${{ github.event.inputs.publish_version }}
+
     - name: Install pypa/build
       run: >-
         python -m
         pip install
         build wheel
         --user
```

### Comparing `tensorboardX-2.6.1/.github/workflows/python-app.yml` & `tensorboardX-2.6.2/.github/workflows/python-app.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -61,7 +61,25 @@
         python examples/demo_graph.py
         python examples/demo_embedding.py
         python examples/demo_custom_scalars.py
         python examples/demo_multiple_embedding.py
         python examples/demo_purge.py
         python examples/demo_matplotlib.py
 
+  test-protobuf-versions:
+    needs: build
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        protobuf-version: ["3.20", "4.21", "4.22", "4.23"]
+    steps:
+    - uses: actions/checkout@v2
+    - name: Set up Python 3.11
+      uses: actions/setup-python@v2
+      with:
+        python-version: 3.11
+    - name: Run examples
+      run: |
+        pip install numpy protobuf==${{ matrix.protobuf-version }}
+        python -c "import tensorboardX"
+
+
```

### Comparing `tensorboardX-2.6.1/HISTORY.rst` & `tensorboardX-2.6.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 History
 =======
+2.6.2 (2023-07-30)
+-------------------
+* Removed version limit for protobuf
+
 2.6.1 (2023-06-18)
 -------------------
 * Expose use_strict_trace parameter in add_graph (#694)
 * Upgrade to protobuf 4
 * Fix git based package versioning
 * Fix GCS Connection Error #606 (#686)
```

### Comparing `tensorboardX-2.6.1/LICENSE` & `tensorboardX-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/PKG-INFO` & `tensorboardX-2.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: tensorboardX
-Version: 2.6.1
+Version: 2.6.2
 Summary: TensorBoardX lets you watch Tensors Flow without Tensorflow
 Home-page: https://github.com/lanpa/tensorboardX
 Author: Tzu-Wei Huang
 Author-email: huang.dexter@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 History
 =======
+2.6.2 (2023-07-30)
+-------------------
+* Removed version limit for protobuf
+
 2.6.1 (2023-06-18)
 -------------------
 * Expose use_strict_trace parameter in add_graph (#694)
 * Upgrade to protobuf 4
 * Fix git based package versioning
 * Fix GCS Connection Error #606 (#686)
```

### Comparing `tensorboardX-2.6.1/README.md` & `tensorboardX-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/compile.sh` & `tensorboardX-2.6.2/compile.sh`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/Makefile` & `tensorboardX-2.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_histogram.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_histogram.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_hparam.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_hparam.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_image.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_image.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_images.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_images.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_mesh.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_mesh.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalar.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_scalar.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalar_global.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_scalar_global.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalars.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/add_scalars.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/_static/img/tensorboard/hier_tags.png` & `tensorboardX-2.6.2/docs/_static/img/tensorboard/hier_tags.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/conf.py` & `tensorboardX-2.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/tutorial.rst` & `tensorboardX-2.6.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/docs/tutorial_zh.rst` & `tensorboardX-2.6.2/docs/tutorial_zh.rst`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/Demo.gif` & `tensorboardX-2.6.2/screenshots/Demo.gif`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/audio.png` & `tensorboardX-2.6.2/screenshots/audio.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/comet.gif` & `tensorboardX-2.6.2/screenshots/comet.gif`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/distribution.png` & `tensorboardX-2.6.2/screenshots/distribution.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/embedding.png` & `tensorboardX-2.6.2/screenshots/embedding.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/graph.png` & `tensorboardX-2.6.2/screenshots/graph.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/histogram.png` & `tensorboardX-2.6.2/screenshots/histogram.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/image.png` & `tensorboardX-2.6.2/screenshots/image.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/scalar.png` & `tensorboardX-2.6.2/screenshots/scalar.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/screenshots/text.png` & `tensorboardX-2.6.2/screenshots/text.png`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/setup.py` & `tensorboardX-2.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
     'numpy',
     'packaging',
-    'protobuf>=4.22.3',
+    'protobuf',
 ]
 
 
 setup(
     name='tensorboardX',
     description='TensorBoardX lets you watch Tensors Flow without Tensorflow',
     long_description=history,
@@ -55,14 +55,15 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     cmdclass={
         'develop': PostDevelopCommand,
         'install': PostInstallCommand,
     },
 )
```

### Comparing `tensorboardX-2.6.1/tensorboardX/beholder/__init__.py` & `tensorboardX-2.6.2/tensorboardX/beholder/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/beholder/beholder.py` & `tensorboardX-2.6.2/tensorboardX/beholder/beholder.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 import time
 
 import numpy as np
 # import tensorflow as tf
 
 # from tensorboard.plugins.beholder import im_util
 # from . import im_util
-from .file_system_tools import read_pickle,\
+from .file_system_tools import read_pickle, \
     write_pickle, write_file
-from .shared_config import PLUGIN_NAME, TAG_NAME,\
+from .shared_config import PLUGIN_NAME, TAG_NAME, \
     SUMMARY_FILENAME, DEFAULT_CONFIG, CONFIG_FILENAME, SUMMARY_COLLECTION_KEY_NAME, SECTION_INFO_FILENAME
 from . import video_writing
 # from .visualizer import Visualizer
 
 
 class Beholder(object):
```

### Comparing `tensorboardX-2.6.1/tensorboardX/beholder/file_system_tools.py` & `tensorboardX-2.6.2/tensorboardX/beholder/file_system_tools.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/beholder/shared_config.py` & `tensorboardX-2.6.2/tensorboardX/beholder/shared_config.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/beholder/video_writing.py` & `tensorboardX-2.6.2/tensorboardX/beholder/video_writing.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/caffe2_graph.py` & `tensorboardX-2.6.2/tensorboardX/caffe2_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/comet_utils.py` & `tensorboardX-2.6.2/tensorboardX/comet_utils.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/crc32c.py` & `tensorboardX-2.6.2/tensorboardX/crc32c.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/embedding.py` & `tensorboardX-2.6.2/tensorboardX/embedding.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/event_file_writer.py` & `tensorboardX-2.6.2/tensorboardX/event_file_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/global_writer.py` & `tensorboardX-2.6.2/tensorboardX/global_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/onnx_graph.py` & `tensorboardX-2.6.2/tensorboardX/onnx_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/openvino_graph.py` & `tensorboardX-2.6.2/tensorboardX/openvino_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/api.proto` & `tensorboardX-2.6.2/tensorboardX/proto/api.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/api_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/attr_value.proto` & `tensorboardX-2.6.2/tensorboardX/proto/attr_value.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/attr_value_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/attr_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/event.proto` & `tensorboardX-2.6.2/tensorboardX/proto/event.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/event_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/event_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/graph.proto` & `tensorboardX-2.6.2/tensorboardX/proto/graph.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/graph_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/layout.proto` & `tensorboardX-2.6.2/tensorboardX/proto/layout.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/layout_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/layout_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/node_def.proto` & `tensorboardX-2.6.2/tensorboardX/proto/node_def.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/node_def_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/node_def_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams.proto` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_hparams.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_hparams_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh.proto` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_mesh.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve.proto` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_pr_curve.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_pr_curve_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_text.proto` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_text.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/plugin_text_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/plugin_text_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/resource_handle.proto` & `tensorboardX-2.6.2/tensorboardX/proto/resource_handle.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/resource_handle_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/resource_handle_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/summary.proto` & `tensorboardX-2.6.2/tensorboardX/proto/summary.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/summary_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/tensor.proto` & `tensorboardX-2.6.2/tensorboardX/proto/tensor.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/tensor_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/tensor_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/tensor_shape.proto` & `tensorboardX-2.6.2/tensorboardX/proto/tensor_shape.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/tensor_shape_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/tensor_shape_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/types.proto` & `tensorboardX-2.6.2/tensorboardX/proto/types.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/types_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/types_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/versions.proto` & `tensorboardX-2.6.2/tensorboardX/proto/versions.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/proto/versions_pb2.py` & `tensorboardX-2.6.2/tensorboardX/proto/versions_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/record_writer.py` & `tensorboardX-2.6.2/tensorboardX/record_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/summary.py` & `tensorboardX-2.6.2/tensorboardX/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     draw = ImageDraw.Draw(image)
     (left, right, top, bottom) = (xmin, xmax, ymin, ymax)
     draw.line([(left, top), (left, bottom), (right, bottom),
                (right, top), (left, top)], width=thickness, fill=color)
     if display_str:
         text_bottom = bottom
         # Reverse list and print from bottom to top.
-        text_width, text_height = font.getsize(display_str)
+        l, t, r, b = font.getbbox(display_str)
+        text_width, text_height = r - l, b - t
         margin = np.ceil(0.05 * text_height)
         draw.rectangle(
             [(left, text_bottom - text_height - 2 * margin),
              (left + text_width, text_bottom)], fill=color
         )
         draw.text(
             (left + margin, text_bottom - text_height - margin),
@@ -146,15 +147,15 @@
       A scalar `Tensor` of type `string`. Which contains a `Summary` protobuf.
     Raises:
       ValueError: If tensor has the wrong shape or type.
     """
     name = _clean_tag(name)
     scalar = make_np(scalar)
     assert scalar.squeeze().ndim == 0, 'scalar should be 0D'
-    scalar = float(scalar)
+    scalar = float(scalar.squeeze())
     if display_name == "" and summary_description == "":
         return Summary(value=[Summary.Value(tag=name, simple_value=scalar)])
 
     metadata = SummaryMetadata(display_name=display_name, summary_description=summary_description)
     return Summary(value=[Summary.Value(tag=name, simple_value=scalar, metadata=metadata)])
```

### Comparing `tensorboardX-2.6.1/tensorboardX/torchvis.py` & `tensorboardX-2.6.2/tensorboardX/torchvis.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/utils.py` & `tensorboardX-2.6.2/tensorboardX/utils.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/visdom_writer.py` & `tensorboardX-2.6.2/tensorboardX/visdom_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX/writer.py` & `tensorboardX-2.6.2/tensorboardX/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         """This adds an entry to the self.scalar_dict datastructure with format
         {writer_id : [[timestamp, step, value], ...], ...}.
         """
         from .x2num import make_np
         if tag not in self.scalar_dict.keys():
             self.scalar_dict[tag] = []
         self.scalar_dict[tag].append(
-            [timestamp, global_step, float(make_np(scalar_value))])
+            [timestamp, global_step, float(make_np(scalar_value).squeeze())])
 
     def _check_caffe2_blob(self, item):
         """
         Caffe2 users have the option of passing a string representing the name of
         a blob in the workspace instead of passing the actual Tensor/array containing
         the numeric values. Thus, we need to check if we received a string as input
         instead of an actual Tensor/array, and if so, we need to fetch the Blob
```

### Comparing `tensorboardX-2.6.1/tensorboardX/x2num.py` & `tensorboardX-2.6.2/tensorboardX/x2num.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tensorboardX.egg-info/PKG-INFO` & `tensorboardX-2.6.2/tensorboardX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: tensorboardX
-Version: 2.6.1
+Version: 2.6.2
 Summary: TensorBoardX lets you watch Tensors Flow without Tensorflow
 Home-page: https://github.com/lanpa/tensorboardX
 Author: Tzu-Wei Huang
 Author-email: huang.dexter@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 History
 =======
+2.6.2 (2023-07-30)
+-------------------
+* Removed version limit for protobuf
+
 2.6.1 (2023-06-18)
 -------------------
 * Expose use_strict_trace parameter in add_graph (#694)
 * Upgrade to protobuf 4
 * Fix git based package versioning
 * Fix GCS Connection Error #606 (#686)
```

### Comparing `tensorboardX-2.6.1/tensorboardX.egg-info/SOURCES.txt` & `tensorboardX-2.6.2/tensorboardX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/event_file_writer_test.py` & `tensorboardX-2.6.2/tests/event_file_writer_test.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/caffe_mnist.expect` & `tensorboardX-2.6.2/tests/expect/caffe_mnist.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/caffe_overfeat.expect` & `tensorboardX-2.6.2/tests/expect/caffe_overfeat.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_caffe2.test_simple_cnnmodel.expect` & `tensorboardX-2.6.2/tests/expect/test_caffe2.test_simple_cnnmodel.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_caffe2.test_simple_model.expect` & `tensorboardX-2.6.2/tests/expect/test_caffe2.test_simple_model.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_pr_curve.test_pr_purve_raw.expect` & `tensorboardX-2.6.2/tests/expect/test_pr_curve.test_pr_purve_raw.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_audio.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_audio.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_hparams.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_hparams.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_hparams_bool.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_hparams_bool.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_hparams_string.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_hparams_string.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_boxes.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_image_with_boxes.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_mesh.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_mesh.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect/test_summary.test_video.expect` & `tensorboardX-2.6.2/tests/expect/test_summary.test_video.expect`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/expect_reader.py` & `tensorboardX-2.6.2/tests/expect_reader.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/mnist-8.onnx` & `tensorboardX-2.6.2/tests/mnist-8.onnx`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/record_writer_test.py` & `tensorboardX-2.6.2/tests/record_writer_test.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_beholder.py` & `tensorboardX-2.6.2/tests/test_beholder.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_chainer_np.py` & `tensorboardX-2.6.2/tests/test_chainer_np.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_embedding.py` & `tensorboardX-2.6.2/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_figure.py` & `tensorboardX-2.6.2/tests/test_figure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
+import matplotlib
+matplotlib.use('agg')
+
 import matplotlib.pyplot as plt
 import unittest
 
 from tensorboardX import SummaryWriter
 
 
 class FigureTest(unittest.TestCase):
```

### Comparing `tensorboardX-2.6.1/tests/test_hparams.py` & `tensorboardX-2.6.2/tests/test_hparams.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_multiprocess_write.py` & `tensorboardX-2.6.2/tests/test_multiprocess_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tensorboardX.proto import event_pb2
 import multiprocessing as mp
 import numpy as np
 import pytest
 import unittest
 import time
 
+mp.set_start_method('fork')
 
 class GlobalWriterTest(unittest.TestCase):
     def test_flush(self):
         N_TEST = 5
         w = SummaryWriter(flush_secs=1)
         f = w.file_writer.event_writer._ev_writer._file_name
         for i in range(N_TEST):
@@ -84,8 +85,9 @@
             ev = event_pb2.Event()
             value = ev.FromString(r.record()).summary.value
             collected_values.append(value[0].simple_value)
 
         collected_values = sorted(collected_values)
         for i in range(TEST_LEN):
             for j in range(N_PROC):
-                assert collected_values[i*N_PROC+j] == i 
+                assert collected_values[i*N_PROC+j] == i
+
```

### Comparing `tensorboardX-2.6.1/tests/test_numpy.py` & `tensorboardX-2.6.2/tests/test_numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,17 @@
     def test_scalar(self):
         res = x2num.make_np(1.1)
         assert isinstance(res, np.ndarray) and res.shape == (1,)
         res = x2num.make_np(1 << 64 - 1)  # uint64_max
         assert isinstance(res, np.ndarray) and res.shape == (1,)
         res = x2num.make_np(np.float16(1.00000087))
         assert isinstance(res, np.ndarray) and res.shape == (1,)
-        res = x2num.make_np(np.float128(1.00008 + 9))
-        assert isinstance(res, np.ndarray) and res.shape == (1,)
+        if hasattr(np, 'float128'):
+            res = x2num.make_np(np.float128(1.00008 + 9))
+            assert isinstance(res, np.ndarray) and res.shape == (1,)
         res = x2num.make_np(np.int64(100000000000))
         assert isinstance(res, np.ndarray) and res.shape == (1,)
 
     def test_make_grid(self):
         pass
 
     def test_numpy_vid(self):
```

### Comparing `tensorboardX-2.6.1/tests/test_pr_curve.py` & `tensorboardX-2.6.2/tests/test_pr_curve.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_pytorch_graph.py` & `tensorboardX-2.6.2/tests/test_pytorch_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_pytorch_np.py` & `tensorboardX-2.6.2/tests/test_pytorch_np.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_record_writer.py` & `tensorboardX-2.6.2/tests/test_record_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_summary.py` & `tensorboardX-2.6.2/tests/test_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 from tensorboardX import summary
 from .expect_reader import compare_proto, write_proto
 import numpy as np
 import pytest
 import unittest
+import torch
 # compare_proto = write_proto  # massive update expect
 
 def tensor_N(shape, dtype=float):
     numel = np.prod(shape)
     x = (np.arange(numel, dtype=dtype)).reshape(shape)
     return x
 
@@ -35,14 +36,22 @@
         b = summary.image(tensor=green_float32, tag='')
         self.assertEqual(a, b)
 
     def test_list_input(self):
         with pytest.raises(Exception):
             summary.histogram('dummy', [1, 3, 4, 5, 6], 'tensorflow')
 
+    def test_0d_input(self):
+        x = torch.rand(1)
+        summary.scalar('0d', x[0])
+
+    def test_1d_input(self):
+        x = torch.rand(1)
+        summary.scalar('0d', x)
+
     def test_empty_input(self):
         print('expect error here:')
         with pytest.raises(Exception):
             summary.histogram('dummy', np.ndarray(0), 'tensorflow')
 
     def test_image_with_boxes(self):
         compare_proto(summary.image_boxes('dummy',
```

### Comparing `tensorboardX-2.6.1/tests/test_summary_writer.py` & `tensorboardX-2.6.2/tests/test_summary_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from tensorboardX import SummaryWriter
+import tempfile
 import unittest
 
 
 class SummaryWriterTest(unittest.TestCase):
     def test_summary_writer_ctx(self):
         # after using a SummaryWriter as a ctx it should be closed
         with SummaryWriter(filename_suffix='.test') as writer:
             writer.add_scalar('test', 1)
         assert writer.file_writer is None
 
-    def test_summary_writer_backcomapt(self):
-        with SummaryWriter(log_dir='/tmp/tbxtest') as writer:
-            writer.add_scalar('test', 1)
+    def test_summary_writer_backcompat(self):
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            with SummaryWriter(log_dir=tmp_dir) as writer:
+                writer.add_scalar('test', 1)
 
     def test_summary_writer_close(self):
         # Opening and closing SummaryWriter a lot should not run into
         # OSError: [Errno 24] Too many open files
         for i in range(1000):
             writer = SummaryWriter()
             writer.close()
```

### Comparing `tensorboardX-2.6.1/tests/test_utils.py` & `tensorboardX-2.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_visdom.py` & `tensorboardX-2.6.2/tests/test_visdom.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6.1/tests/test_writer.py` & `tensorboardX-2.6.2/tests/test_writer.py`

 * *Files identical despite different names*

