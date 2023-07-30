# Comparing `tmp/asposeslidescloud-23.6.0.tar.gz` & `tmp/asposeslidescloud-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asposeslidescloud-23.6.0.tar", last modified: Sun Jul  2 00:10:40 2023, max compression
+gzip compressed data, was "dist/asposeslidescloud-23.7.0.tar", last modified: Wed Jul 26 17:54:22 2023, max compression
```

## Comparing `asposeslidescloud-23.6.0.tar` & `asposeslidescloud-23.7.0.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-07-02 00:10:20.000000 asposeslidescloud-23.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8718 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8330 2023-07-02 00:10:22.000000 asposeslidescloud-23.6.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud/
--rw-rw-r--   0 root         (0) root         (0)    18249 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28146 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/
--rw-rw-r--   0 root         (0) root         (0)      246 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1945 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/api_base.py
--rw-rw-r--   0 root         (0) root         (0)  1445375 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/slides_api.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/error_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/
--rw-rw-r--   0 root         (0) root         (0)    18032 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5035 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/accent_element.py
--rw-rw-r--   0 root         (0) root         (0)    13005 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/access_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4992 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_shape.py
--rw-rw-r--   0 root         (0) root         (0)     6965 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4369 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_ceiling_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_floor_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_inverse_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4416 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4287 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/api_info.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/arc_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    10971 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/array_element.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/arrow_head_properties.py
--rw-rw-r--   0 root         (0) root         (0)    18977 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/audio_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7140 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/axes.py
--rw-rw-r--   0 root         (0) root         (0)    48257 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/axis.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/axis_type.py
--rw-rw-r--   0 root         (0) root         (0)     5740 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bar_element.py
--rw-rw-r--   0 root         (0) root         (0)     4307 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/base64_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4314 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4498 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/block_element.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/blur_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5204 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/blur_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12264 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/border_box_element.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/box_element.py
--rw-rw-r--   0 root         (0) root         (0)     6280 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_series.py
--rw-rw-r--   0 root         (0) root         (0)    10161 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/camera.py
--rw-rw-r--   0 root         (0) root         (0)    19140 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_category.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_lines_format.py
--rw-rw-r--   0 root         (0) root         (0)    22466 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_series_group.py
--rw-rw-r--   0 root         (0) root         (0)     4726 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_title.py
--rw-rw-r--   0 root         (0) root         (0)     8429 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall_type.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/close_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/color_change_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4393 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/color_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12365 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/color_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5159 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/common_slide_view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     9725 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/connector.py
--rw-rw-r--   0 root         (0) root         (0)     7666 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     4031 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/custom_dash_pattern.py
--rw-rw-r--   0 root         (0) root         (0)     8034 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/data_point.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/data_source.py
--rw-rw-r--   0 root         (0) root         (0)    10164 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/delimiter_element.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/disc_usage.py
--rw-rw-r--   0 root         (0) root         (0)     8706 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5707 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document_property.py
--rw-rw-r--   0 root         (0) root         (0)     5081 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/duotone_effect.py
--rw-rw-r--   0 root         (0) root         (0)    25610 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/effect.py
--rw-rw-r--   0 root         (0) root         (0)     9702 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/effect_format.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/entity_exists.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/error.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3772 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5423 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/file_version.py
--rw-rw-r--   0 root         (0) root         (0)     4038 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/file_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/files_list.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/files_upload_result.py
--rw-rw-r--   0 root         (0) root         (0)     4654 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fill_format.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5930 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4827 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_data.py
--rw-rw-r--   0 root         (0) root         (0)     6124 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_fallback_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_set.py
--rw-rw-r--   0 root         (0) root         (0)     5834 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_subst_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fonts_data.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/format_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fraction_element.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/function_element.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_path.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_paths.py
--rw-rw-r--   0 root         (0) root         (0)     9958 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_shape.py
--rw-rw-r--   0 root         (0) root         (0)     7037 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gif_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4577 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/glow_effect.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill_stop.py
--rw-rw-r--   0 root         (0) root         (0)     5294 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/graphical_object.py
--rw-rw-r--   0 root         (0) root         (0)     3582 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gray_scale_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6003 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/group_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8843 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/grouping_character_element.py
--rw-rw-r--   0 root         (0) root         (0)     8424 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/hsl_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5966 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/html5_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    20135 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/html_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14645 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/hyperlink.py
--rw-rw-r--   0 root         (0) root         (0)     3323 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/i_shape_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5762 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    11286 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options_base.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_transform_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/images.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/inner_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5833 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/input.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/input_file.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/interactive_sequence.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slides.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/left_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    11324 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/legend.py
--rw-rw-r--   0 root         (0) root         (0)     9070 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/light_rig.py
--rw-rw-r--   0 root         (0) root         (0)     5686 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/limit_element.py
--rw-rw-r--   0 root         (0) root         (0)    17895 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/line_format.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/line_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     3520 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/literals.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/luminance_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6114 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4461 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/master_slides.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/math_element.py
--rw-rw-r--   0 root         (0) root         (0)     6014 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/math_paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    13599 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/matrix_element.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/merge.py
--rw-rw-r--   0 root         (0) root         (0)     4739 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/merging_source.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/move_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    11633 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/nary_operator_element.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/no_fill.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/normal_view_restored_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5084 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    10510 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/object_exist.py
--rw-rw-r--   0 root         (0) root         (0)    14248 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/ole_object_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7722 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)    15178 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_series.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/ordered_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/outer_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4607 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/output_file.py
--rw-rw-r--   0 root         (0) root         (0)    31046 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    30740 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph_format.py
--rw-rw-r--   0 root         (0) root         (0)     4553 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/paragraphs.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/path_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4960 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/path_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pattern_fill.py
--rw-rw-r--   0 root         (0) root         (0)    28850 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pdf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    12411 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/picture_fill.py
--rw-rw-r--   0 root         (0) root         (0)     6348 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/picture_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4719 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     9383 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/placeholder.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/placeholders.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/plot_area.py
--rw-rw-r--   0 root         (0) root         (0)    39730 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/portion.py
--rw-rw-r--   0 root         (0) root         (0)    38640 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/portion_format.py
--rw-rw-r--   0 root         (0) root         (0)     4322 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/portions.py
--rw-rw-r--   0 root         (0) root         (0)     5838 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pptx_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/presentation_to_merge.py
--rw-rw-r--   0 root         (0) root         (0)     5515 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/presentations_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/preset_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/protection_properties.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5744 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/radical_element.py
--rw-rw-r--   0 root         (0) root         (0)    16340 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/reflection_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/remove_shape.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/remove_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/reorder_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6804 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/replace_text.py
--rw-rw-r--   0 root         (0) root         (0)     4334 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/request_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/reset_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/resource_base.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/resource_uri.py
--rw-rw-r--   0 root         (0) root         (0)     3560 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/response_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     6993 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/right_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     6404 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/save.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/save_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8656 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/save_slide.py
--rw-rw-r--   0 root         (0) root         (0)     7370 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     6662 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_series.py
--rw-rw-r--   0 root         (0) root         (0)     6007 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/section.py
--rw-rw-r--   0 root         (0) root         (0)     6868 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/section_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/sections.py
--rw-rw-r--   0 root         (0) root         (0)    19377 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/series.py
--rw-rw-r--   0 root         (0) root         (0)     8031 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/series_marker.py
--rw-rw-r--   0 root         (0) root         (0)     7749 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape.py
--rw-rw-r--   0 root         (0) root         (0)    17369 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_base.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_bevel.py
--rw-rw-r--   0 root         (0) root         (0)     3457 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7557 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_thumbnail_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_type.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3647 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shapes_alignment_type.py
--rw-rw-r--   0 root         (0) root         (0)    12213 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)     5597 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_animation.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_background.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment_base.py
--rw-rw-r--   0 root         (0) root         (0)     4363 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comments.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_modern_comment.py
--rw-rw-r--   0 root         (0) root         (0)    10980 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)    12171 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_show_properties.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slides.py
--rw-rw-r--   0 root         (0) root         (0)    15341 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_node.py
--rw-rw-r--   0 root         (0) root         (0)     5385 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_shape.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/soft_edge_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/solid_fill.py
--rw-rw-r--   0 root         (0) root         (0)     3448 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/special_slide_type.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/split_document_result.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/storage_exist.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/storage_file.py
--rw-rw-r--   0 root         (0) root         (0)     5049 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/subscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     7774 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7607 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_section.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    18450 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/svg_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    26590 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/swf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15954 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table.py
--rw-rw-r--   0 root         (0) root         (0)    22416 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell.py
--rw-rw-r--   0 root         (0) root         (0)     7735 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_merge_options.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_split_type.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_column.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_row.py
--rw-rw-r--   0 root         (0) root         (0)     4757 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/task.py
--rw-rw-r--   0 root         (0) root         (0)     5843 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     4173 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_element.py
--rw-rw-r--   0 root         (0) root         (0)    24377 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_frame_format.py
--rw-rw-r--   0 root         (0) root         (0)     4652 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_item.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_items.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/theme.py
--rw-rw-r--   0 root         (0) root         (0)    12219 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/three_d_format.py
--rw-rw-r--   0 root         (0) root         (0)    17671 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/tiff_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/tint_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/update_background.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/update_shape.py
--rw-rw-r--   0 root         (0) root         (0)     5880 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/vba_module.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/vba_project.py
--rw-rw-r--   0 root         (0) root         (0)     4613 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/vba_reference.py
--rw-rw-r--   0 root         (0) root         (0)    10340 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/video_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14060 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/video_frame.py
--rw-rw-r--   0 root         (0) root         (0)    16257 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/workbook.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/xaml_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7214 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/xps_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     9382 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/xy_series.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)    10460 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_object.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/oauth_response.py
--rw-rw-r--   0 root         (0) root         (0)    15494 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8718 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11369 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2023-07-02 00:10:27.000000 asposeslidescloud-23.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-26 17:54:01.000000 asposeslidescloud-23.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9040 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8652 2023-07-26 17:54:04.000000 asposeslidescloud-23.7.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud/
+-rw-rw-r--   0 root         (0) root         (0)    18249 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    28146 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud/apis/
+-rw-rw-r--   0 root         (0) root         (0)      246 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/apis/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1945 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/apis/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)  1457015 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/apis/slides_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/error_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/
+-rw-rw-r--   0 root         (0) root         (0)    18032 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5035 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/accent_element.py
+-rw-rw-r--   0 root         (0) root         (0)    13005 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/access_permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     5373 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/add_layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/add_master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4992 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/add_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/add_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4369 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_ceiling_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_floor_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_inverse_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_modulate_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4416 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4287 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4601 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/api_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/arc_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    10971 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/array_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7767 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/arrow_head_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    18977 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/audio_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7140 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/axes.py
+-rw-rw-r--   0 root         (0) root         (0)    48257 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/axis.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/axis_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5740 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/bar_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4307 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/base64_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4314 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4498 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/block_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/blur_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/blur_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12264 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/border_box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6280 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/bubble_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/bubble_series.py
+-rw-rw-r--   0 root         (0) root         (0)    10161 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/camera.py
+-rw-rw-r--   0 root         (0) root         (0)    19140 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart_category.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart_lines_format.py
+-rw-rw-r--   0 root         (0) root         (0)    22466 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart_series_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4726 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart_title.py
+-rw-rw-r--   0 root         (0) root         (0)     8429 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart_wall.py
+-rw-rw-r--   0 root         (0) root         (0)     3417 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/chart_wall_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/close_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/color_change_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4393 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/color_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12365 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/color_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5159 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/common_slide_view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     9725 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/connector.py
+-rw-rw-r--   0 root         (0) root         (0)     7666 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4031 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/custom_dash_pattern.py
+-rw-rw-r--   0 root         (0) root         (0)     8034 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/data_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/delimiter_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/disc_usage.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/document.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/document_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5707 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/document_property.py
+-rw-rw-r--   0 root         (0) root         (0)     5081 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/document_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/duotone_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    29539 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9702 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/effect_format.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/entity_exists.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/error.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3772 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5423 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/file_version.py
+-rw-rw-r--   0 root         (0) root         (0)     4038 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/file_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/files_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/files_upload_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4654 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/fill_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/fill_overlay_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5930 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/fill_overlay_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4827 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/font_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6124 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/font_fallback_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/font_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/font_set.py
+-rw-rw-r--   0 root         (0) root         (0)     5834 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/font_subst_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/fonts_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/format_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/fraction_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/function_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/geometry_path.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/geometry_paths.py
+-rw-rw-r--   0 root         (0) root         (0)     9958 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/geometry_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     7037 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/gif_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4577 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/glow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/gradient_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     4713 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/gradient_fill_stop.py
+-rw-rw-r--   0 root         (0) root         (0)     5294 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/graphical_object.py
+-rw-rw-r--   0 root         (0) root         (0)     3582 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/gray_scale_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6003 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/group_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8843 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/grouping_character_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8424 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/hsl_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5966 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/html5_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    20135 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/html_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14645 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/hyperlink.py
+-rw-rw-r--   0 root         (0) root         (0)     3323 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/i_shape_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5762 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/image_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    11286 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/image_export_options_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/image_transform_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/images.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/inner_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5833 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/input.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/interactive_sequence.py
+-rw-rw-r--   0 root         (0) root         (0)     8009 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/layout_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/left_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    11324 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/legend.py
+-rw-rw-r--   0 root         (0) root         (0)     9070 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/light_rig.py
+-rw-rw-r--   0 root         (0) root         (0)     5686 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/limit_element.py
+-rw-rw-r--   0 root         (0) root         (0)    17895 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/line_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/line_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     3520 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/literals.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/luminance_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4461 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/master_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/math_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6014 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/math_paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    13599 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/matrix_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/merge.py
+-rw-rw-r--   0 root         (0) root         (0)     4739 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/merging_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/move_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    11633 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/nary_operator_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/no_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/normal_view_restored_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5084 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/notes_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/notes_slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    10510 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/notes_slide_header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/object_exist.py
+-rw-rw-r--   0 root         (0) root         (0)    14248 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/ole_object_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7722 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/one_value_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)    15178 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/one_value_series.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/ordered_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/outer_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4607 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/output_file.py
+-rw-rw-r--   0 root         (0) root         (0)    31046 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    30740 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/paragraph_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/paragraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/path_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4960 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/path_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4665 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/pattern_fill.py
+-rw-rw-r--   0 root         (0) root         (0)    28850 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/pdf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    12411 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/picture_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     6348 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/picture_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4719 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/pipeline.py
+-rw-rw-r--   0 root         (0) root         (0)     9383 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/placeholder.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/placeholders.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/plot_area.py
+-rw-rw-r--   0 root         (0) root         (0)    39730 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/portion.py
+-rw-rw-r--   0 root         (0) root         (0)    38640 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/portion_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4322 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/portions.py
+-rw-rw-r--   0 root         (0) root         (0)     5838 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/pptx_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/presentation_to_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     5515 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/presentations_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7553 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/preset_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/protection_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5744 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/radical_element.py
+-rw-rw-r--   0 root         (0) root         (0)    16340 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/reflection_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/remove_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/remove_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/reorder_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6804 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/replace_text.py
+-rw-rw-r--   0 root         (0) root         (0)     4334 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/request_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4204 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/reset_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/resource_base.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/resource_uri.py
+-rw-rw-r--   0 root         (0) root         (0)     3560 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/response_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6993 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/right_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6404 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/save.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/save_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8656 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/save_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     7370 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/scatter_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     6662 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/scatter_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6007 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/section.py
+-rw-rw-r--   0 root         (0) root         (0)     6868 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/section_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/sections.py
+-rw-rw-r--   0 root         (0) root         (0)    19377 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/series.py
+-rw-rw-r--   0 root         (0) root         (0)     8031 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/series_marker.py
+-rw-rw-r--   0 root         (0) root         (0)     7749 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape.py
+-rw-rw-r--   0 root         (0) root         (0)    17369 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape_base.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape_bevel.py
+-rw-rw-r--   0 root         (0) root         (0)     3457 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape_image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape_thumbnail_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shape_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/shapes_alignment_type.py
+-rw-rw-r--   0 root         (0) root         (0)    12213 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5597 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_animation.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_background.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_comment.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_comment_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4363 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_comments.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_modern_comment.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)    12171 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slide_show_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     4413 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/slides.py
+-rw-rw-r--   0 root         (0) root         (0)    15341 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/smart_art.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/smart_art_node.py
+-rw-rw-r--   0 root         (0) root         (0)     5385 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/smart_art_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/soft_edge_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/solid_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     3448 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/special_slide_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/split_document_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/storage_exist.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/storage_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5049 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/subscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7774 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/summary_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7607 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/summary_zoom_section.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    18450 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/svg_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    26590 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/swf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15954 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/table.py
+-rw-rw-r--   0 root         (0) root         (0)    22416 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/table_cell.py
+-rw-rw-r--   0 root         (0) root         (0)     7735 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/table_cell_merge_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/table_cell_split_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/table_column.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/table_row.py
+-rw-rw-r--   0 root         (0) root         (0)     4757 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/task.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/text_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/text_element.py
+-rw-rw-r--   0 root         (0) root         (0)    24377 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/text_frame_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4652 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/text_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/text_items.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/theme.py
+-rw-rw-r--   0 root         (0) root         (0)    12219 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/three_d_format.py
+-rw-rw-r--   0 root         (0) root         (0)    17671 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/tiff_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/tint_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/update_background.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/update_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     5880 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/vba_module.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/vba_project.py
+-rw-rw-r--   0 root         (0) root         (0)     4613 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/vba_reference.py
+-rw-rw-r--   0 root         (0) root         (0)    10340 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/video_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15752 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/video_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    16257 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/workbook.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/xaml_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7214 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/xps_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     9382 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/xy_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    10460 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/models/zoom_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/oauth_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15494 2023-07-26 17:53:58.000000 asposeslidescloud-23.7.0/asposeslidescloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9040 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11369 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/asposeslidescloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 17:54:22.000000 asposeslidescloud-23.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2023-07-26 17:54:10.000000 asposeslidescloud-23.7.0/setup.py
```

### Comparing `asposeslidescloud-23.6.0/LICENSE` & `asposeslidescloud-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/PKG-INFO` & `asposeslidescloud-23.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 23.6.0
+Version: 23.7.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,20 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.7
+
+* New methods **ReplaceTextFormatting** and **ReplaceTextFormatting** allow to replace text with formatting.
+* Added **AfterAnimationType**, **Rewind** and **AfterAnimationColor** methods to **Effect** class.
+* Added **TrimFromStart** and **TrimFromEnd** methods to **VideoFrame** class.
+
 ## Enhancements in Version 23.6
 
 * Added methods ho handle VBA methods: **GetVbaProject**, **GetVbaModule**, **CreateVbaModule**, **UpdateVbaModule** and **DeleteVbaModule**. Added model classes related to VBA: **VbaProject**,  **VbaModule** and  **VbaReference**.
 
 ## Enhancements in Version 23.4
 
 * Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
```

### Comparing `asposeslidescloud-23.6.0/README` & `asposeslidescloud-23.7.0/asposeslidescloud.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: asposeslidescloud
+Version: 23.7.0
+Summary: Aspose.Slides Cloud SDK for Python
+Home-page: 
+Author: Victor Putrov
+Author-email: vistor.putrov@aspose.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -23,14 +36,20 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.7
+
+* New methods **ReplaceTextFormatting** and **ReplaceTextFormatting** allow to replace text with formatting.
+* Added **AfterAnimationType**, **Rewind** and **AfterAnimationColor** methods to **Effect** class.
+* Added **TrimFromStart** and **TrimFromEnd** methods to **VideoFrame** class.
+
 ## Enhancements in Version 23.6
 
 * Added methods ho handle VBA methods: **GetVbaProject**, **GetVbaModule**, **CreateVbaModule**, **UpdateVbaModule** and **DeleteVbaModule**. Added model classes related to VBA: **VbaProject**,  **VbaModule** and  **VbaReference**.
 
 ## Enhancements in Version 23.4
 
 * Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/__init__.py` & `asposeslidescloud-23.7.0/asposeslidescloud/__init__.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/api_client.py` & `asposeslidescloud-23.7.0/asposeslidescloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, configuration=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk v23.6.0'}
+        self.default_headers = {'x-aspose-client': 'python sdk v23.7.0'}
         if configuration.timeout:
             self.default_headers['x-aspose-timeout'] = configuration.timeout
         self.default_headers.update(configuration.custom_headers)
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/apis/api_base.py` & `asposeslidescloud-23.7.0/asposeslidescloud/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/apis/slides_api.py` & `asposeslidescloud-23.7.0/asposeslidescloud/apis/slides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -24927,14 +24927,267 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def replace_text_formatting(self, name, old_value, new_value, portion_format = None, with_masters = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Finds and replaces text in presentation with given format.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, old_value, new_value, portion_format, with_masters, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param old_value Text value to be replaced.
+        :param new_value Text value to replace with.
+        :param portion_format Portion format.
+        :param with_masters Text replacement includes master slides.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Document
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.replace_text_formatting_with_http_info(name, old_value, new_value, portion_format, with_masters, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.replace_text_formatting_with_http_info(name, old_value, new_value, portion_format, with_masters, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def replace_text_formatting_with_http_info(self, name, old_value, new_value, portion_format = None, with_masters = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Finds and replaces text in presentation with given format.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.replace_text_formatting_with_http_info(name, old_value, new_value, portion_format, with_masters, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param old_value Text value to be replaced.
+        :param new_value Text value to replace with.
+        :param portion_format Portion format.
+        :param with_masters Text replacement includes master slides.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Document
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method replace_text_formatting" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `replace_text_formatting`")  # noqa: E501
+        # verify the required parameter 'old_value' is set
+        if not old_value:
+            raise ValueError("Missing the required parameter `old_value` when calling `replace_text_formatting`")  # noqa: E501
+        # verify the required parameter 'new_value' is set
+        if not new_value:
+            raise ValueError("Missing the required parameter `new_value` when calling `replace_text_formatting`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+
+        query_params = []
+        if old_value:
+            query_params.append(('oldValue', old_value))  # noqa: E501
+        if new_value:
+            query_params.append(('newValue', new_value))  # noqa: E501
+        if with_masters:
+            query_params.append(('withMasters', with_masters))  # noqa: E501
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if portion_format:
+            body_params = portion_format
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/replaceTextFormatting', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Document',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def replace_text_formatting_online(self, document, old_value, new_value, portion_format = None, with_masters = None, password = None, **kwargs):  # noqa: E501
+        """Finds and replaces text in presentation with given format.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(document, old_value, new_value, portion_format, with_masters, password, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param document Document data.
+        :param old_value Text value to be replaced.
+        :param new_value Text value to replace with.
+        :param portion_format Portion format.
+        :param with_masters Text replacement includes master slides.
+        :param password Document password.
+        :return: file
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.replace_text_formatting_online_with_http_info(document, old_value, new_value, portion_format, with_masters, password, **kwargs)  # noqa: E501
+        else:
+            (data) = self.replace_text_formatting_online_with_http_info(document, old_value, new_value, portion_format, with_masters, password, **kwargs)  # noqa: E501
+            return data
+
+    def replace_text_formatting_online_with_http_info(self, document, old_value, new_value, portion_format = None, with_masters = None, password = None, **kwargs):  # noqa: E501
+        """Finds and replaces text in presentation with given format.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.replace_text_formatting_online_with_http_info(document, old_value, new_value, portion_format, with_masters, password, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param document Document data.
+        :param old_value Text value to be replaced.
+        :param new_value Text value to replace with.
+        :param portion_format Portion format.
+        :param with_masters Text replacement includes master slides.
+        :param password Document password.
+        :return: file
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method replace_text_formatting_online" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'document' is set
+        if not document:
+            raise ValueError("Missing the required parameter `document` when calling `replace_text_formatting_online`")  # noqa: E501
+        # verify the required parameter 'old_value' is set
+        if not old_value:
+            raise ValueError("Missing the required parameter `old_value` when calling `replace_text_formatting_online`")  # noqa: E501
+        # verify the required parameter 'new_value' is set
+        if not new_value:
+            raise ValueError("Missing the required parameter `new_value` when calling `replace_text_formatting_online`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if old_value:
+            query_params.append(('oldValue', old_value))  # noqa: E501
+        if new_value:
+            query_params.append(('newValue', new_value))  # noqa: E501
+        if with_masters:
+            query_params.append(('withMasters', with_masters))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+        if document:
+            param_files['document'] = document  # noqa: E501
+
+        body_params = None
+        if portion_format:
+            body_params = portion_format
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['multipart/form-data'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['multipart/form-data'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/replaceTextFormatting', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='file',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def save_portion_as_math_ml(self, name, slide_index, shape_index, paragraph_index, portion_index, out_path, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Convert Mathematical Text to MathML Format and saves result to the storage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, slide_index, shape_index, paragraph_index, portion_index, out_path, password, folder, storage, is_async=True)
         >>> result = thread.get()
@@ -32389,15 +32642,15 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_vba_module(self, name, module_index, module_dto = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+    def update_vba_module(self, name, module_index, module_dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update VBA module.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, module_index, module_dto, password, folder, storage, is_async=True)
         >>> result = thread.get()
 
@@ -32415,15 +32668,15 @@
         kwargs['_return_http_data_only'] = True
         if kwargs.get('is_async'):
             return self.update_vba_module_with_http_info(name, module_index, module_dto, password, folder, storage, **kwargs)  # noqa: E501
         else:
             (data) = self.update_vba_module_with_http_info(name, module_index, module_dto, password, folder, storage, **kwargs)  # noqa: E501
             return data
 
-    def update_vba_module_with_http_info(self, name, module_index, module_dto = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+    def update_vba_module_with_http_info(self, name, module_index, module_dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update VBA module.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.update_vba_module_with_http_info(name, module_index, module_dto, password, folder, storage, is_async=True)
         >>> result = thread.get()
 
@@ -32456,14 +32709,17 @@
         del params['kwargs']
         # verify the required parameter 'name' is set
         if not name:
             raise ValueError("Missing the required parameter `name` when calling `update_vba_module`")  # noqa: E501
         # verify the required parameter 'module_index' is set
         if not module_index:
             raise ValueError("Missing the required parameter `module_index` when calling `update_vba_module`")  # noqa: E501
+        # verify the required parameter 'module_dto' is set
+        if not module_dto:
+            raise ValueError("Missing the required parameter `module_dto` when calling `update_vba_module`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         path_params['name'] = name  # noqa: E501
         path_params['moduleIndex'] = module_index  # noqa: E501
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/configuration.py` & `asposeslidescloud-23.7.0/asposeslidescloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,9 +192,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 23.6.0".\
+               "SDK Package Version: 23.7.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/error_message.py` & `asposeslidescloud-23.7.0/asposeslidescloud/error_message.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/__init__.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/accent_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/accent_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/access_permissions.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/access_permissions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/add_layout_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/add_layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/add_master_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/add_master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/add_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/add_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/add_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/add_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_bi_level_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_ceiling_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_ceiling_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_floor_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_floor_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_inverse_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_inverse_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_modulate_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_replace_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/alpha_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/api_info.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/api_info.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/arc_to_path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/arc_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/array_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/array_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/arrow_head_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/arrow_head_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/audio_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/audio_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/axes.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/axes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/axis.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/axis_type.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/axis_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/bar_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/bar_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/base64_input_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/base64_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/bi_level_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/block_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/block_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/blur_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/blur_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/blur_image_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/blur_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/border_box_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/border_box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/box_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_chart_data_point.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/bubble_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_series.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/bubble_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/camera.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/camera.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_category.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart_category.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_lines_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart_lines_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_series_group.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart_series_group.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_title.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart_title.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart_wall.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall_type.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/chart_wall_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/close_path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/close_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/color_change_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/color_change_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/color_replace_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/color_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/color_scheme.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/color_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/common_slide_view_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/common_slide_view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/connector.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/connector.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/custom_dash_pattern.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/custom_dash_pattern.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/data_point.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/data_source.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/data_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/delimiter_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/delimiter_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/disc_usage.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/document.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/document_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/document_property.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/document_replace_result.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/document_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/duotone_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/duotone_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/effect.py`

 * *Files 21% similar despite different names*

```diff
@@ -55,15 +55,18 @@
         'repeat_count': 'float',
         'repeat_duration': 'float',
         'restart': 'str',
         'speed': 'float',
         'trigger_delay_time': 'float',
         'repeat_until_end_slide': 'bool',
         'repeat_until_next_click': 'bool',
-        'stop_previous_sound': 'bool'
+        'stop_previous_sound': 'bool',
+        'rewind': 'bool',
+        'after_animation_type': 'str',
+        'after_animation_color': 'str'
     }
 
     attribute_map = {
         'type': 'type',
         'subtype': 'subtype',
         'preset_class_type': 'presetClassType',
         'shape_index': 'shapeIndex',
@@ -76,21 +79,24 @@
         'repeat_count': 'repeatCount',
         'repeat_duration': 'repeatDuration',
         'restart': 'restart',
         'speed': 'speed',
         'trigger_delay_time': 'triggerDelayTime',
         'repeat_until_end_slide': 'repeatUntilEndSlide',
         'repeat_until_next_click': 'repeatUntilNextClick',
-        'stop_previous_sound': 'stopPreviousSound'
+        'stop_previous_sound': 'stopPreviousSound',
+        'rewind': 'rewind',
+        'after_animation_type': 'afterAnimationType',
+        'after_animation_color': 'afterAnimationColor'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, type=None, subtype=None, preset_class_type=None, shape_index=None, paragraph_index=None, trigger_type=None, accelerate=None, auto_reverse=None, decelerate=None, duration=None, repeat_count=None, repeat_duration=None, restart=None, speed=None, trigger_delay_time=None, repeat_until_end_slide=None, repeat_until_next_click=None, stop_previous_sound=None):  # noqa: E501
+    def __init__(self, type=None, subtype=None, preset_class_type=None, shape_index=None, paragraph_index=None, trigger_type=None, accelerate=None, auto_reverse=None, decelerate=None, duration=None, repeat_count=None, repeat_duration=None, restart=None, speed=None, trigger_delay_time=None, repeat_until_end_slide=None, repeat_until_next_click=None, stop_previous_sound=None, rewind=None, after_animation_type=None, after_animation_color=None):  # noqa: E501
         """Effect - a model defined in Swagger"""  # noqa: E501
 
         self._type = None
         self._subtype = None
         self._preset_class_type = None
         self._shape_index = None
         self._paragraph_index = None
@@ -103,14 +109,17 @@
         self._repeat_duration = None
         self._restart = None
         self._speed = None
         self._trigger_delay_time = None
         self._repeat_until_end_slide = None
         self._repeat_until_next_click = None
         self._stop_previous_sound = None
+        self._rewind = None
+        self._after_animation_type = None
+        self._after_animation_color = None
 
         if type is not None:
             self.type = type
         if subtype is not None:
             self.subtype = subtype
         if preset_class_type is not None:
             self.preset_class_type = preset_class_type
@@ -139,14 +148,20 @@
             self.trigger_delay_time = trigger_delay_time
         if repeat_until_end_slide is not None:
             self.repeat_until_end_slide = repeat_until_end_slide
         if repeat_until_next_click is not None:
             self.repeat_until_next_click = repeat_until_next_click
         if stop_previous_sound is not None:
             self.stop_previous_sound = stop_previous_sound
+        if rewind is not None:
+            self.rewind = rewind
+        if after_animation_type is not None:
+            self.after_animation_type = after_animation_type
+        if after_animation_color is not None:
+            self.after_animation_color = after_animation_color
 
     @property
     def type(self):
         """Gets the type of this Effect.  # noqa: E501
 
         Effect type.  # noqa: E501
 
@@ -616,14 +631,96 @@
         This attribute specifies if the animation effect stops the previous sound.  # noqa: E501
 
         :param stop_previous_sound: The stop_previous_sound of this Effect.  # noqa: E501
         :type: bool
         """
         self._stop_previous_sound = stop_previous_sound
 
+    @property
+    def rewind(self):
+        """Gets the rewind of this Effect.  # noqa: E501
+
+        This attribute specifies if the effect will rewind when done playing.  # noqa: E501
+
+        :return: The rewind of this Effect.  # noqa: E501
+        :rtype: bool
+        """
+        return self._rewind
+
+    @rewind.setter
+    def rewind(self, rewind):
+        """Sets the rewind of this Effect.
+
+        This attribute specifies if the effect will rewind when done playing.  # noqa: E501
+
+        :param rewind: The rewind of this Effect.  # noqa: E501
+        :type: bool
+        """
+        self._rewind = rewind
+
+    @property
+    def after_animation_type(self):
+        """Gets the after_animation_type of this Effect.  # noqa: E501
+
+        Defined an after animation color for effect.  # noqa: E501
+
+        :return: The after_animation_type of this Effect.  # noqa: E501
+        :rtype: str
+        """
+        return self._after_animation_type
+
+    @after_animation_type.setter
+    def after_animation_type(self, after_animation_type):
+        """Sets the after_animation_type of this Effect.
+
+        Defined an after animation color for effect.  # noqa: E501
+
+        :param after_animation_type: The after_animation_type of this Effect.  # noqa: E501
+        :type: str
+        """
+        if after_animation_type is not None:
+            allowed_values = ["DoNotDim", "Color", "HideAfterAnimation", "HideOnNextMouseClick"]  # noqa: E501
+            if after_animation_type.isdigit():
+                int_after_animation_type = int(after_animation_type)
+                if int_after_animation_type < 0 or int_after_animation_type >= len(allowed_values):
+                    raise ValueError(
+                        "Invalid value for `after_animation_type` ({0}), must be one of {1}"  # noqa: E501
+                        .format(after_animation_type, allowed_values)
+                    )
+                self._after_animation_type = allowed_values[int_after_animation_type]
+                return
+            if after_animation_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `after_animation_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(after_animation_type, allowed_values)
+                )
+        self._after_animation_type = after_animation_type
+
+    @property
+    def after_animation_color(self):
+        """Gets the after_animation_color of this Effect.  # noqa: E501
+
+        Defined an after animation color for effect. Applied when the AfterAnimationType property is set to Color.  # noqa: E501
+
+        :return: The after_animation_color of this Effect.  # noqa: E501
+        :rtype: str
+        """
+        return self._after_animation_color
+
+    @after_animation_color.setter
+    def after_animation_color(self, after_animation_color):
+        """Sets the after_animation_color of this Effect.
+
+        Defined an after animation color for effect. Applied when the AfterAnimationType property is set to Color.  # noqa: E501
+
+        :param after_animation_color: The after_animation_color of this Effect.  # noqa: E501
+        :type: str
+        """
+        self._after_animation_color = after_animation_color
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/effect_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/effect_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/entity_exists.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/entity_exists.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/error.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/error_details.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/export_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/file_version.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/file_versions.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/files_list.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/files_upload_result.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/fill_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/fill_overlay_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_image_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/fill_overlay_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/font_data.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/font_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/font_fallback_rule.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/font_fallback_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/font_scheme.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/font_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/font_set.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/font_set.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/font_subst_rule.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/font_subst_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/fonts_data.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/fonts_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/format_scheme.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/format_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/fraction_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/fraction_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/function_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/function_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_path.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/geometry_path.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_paths.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/geometry_paths.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/geometry_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/gif_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/gif_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/glow_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/glow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill_stop.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/graphical_object.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/graphical_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/gray_scale_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/gray_scale_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/group_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/group_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/grouping_character_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/grouping_character_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/header_footer.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/hsl_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/hsl_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/html5_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/html5_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/html_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/html_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/hyperlink.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/i_shape_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/i_shape_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/image.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/image_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options_base.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/image_export_options_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/image_transform_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/image_transform_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/images.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/inner_shadow_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/inner_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/input.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/input.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/input_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/interactive_sequence.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/interactive_sequence.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slides.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/layout_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/left_sub_superscript_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/left_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/legend.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/light_rig.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/light_rig.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/limit_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/limit_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/line_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/line_to_path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/line_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/literals.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/literals.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/luminance_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/luminance_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/master_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/master_slides.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/master_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/math_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/math_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/math_paragraph.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/math_paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/matrix_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/matrix_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/merge.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/merging_source.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/merging_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/move_to_path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/move_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/nary_operator_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/nary_operator_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/no_fill.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/no_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/normal_view_restored_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/normal_view_restored_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/notes_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_export_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/notes_slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_header_footer.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/notes_slide_header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/object_exist.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/ole_object_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/ole_object_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_chart_data_point.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/one_value_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_series.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/one_value_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/ordered_merge_request.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/ordered_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/outer_shadow_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/outer_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/output_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/paragraphs.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/paragraphs.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/path_input_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/path_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/path_output_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/path_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/pattern_fill.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/pdf_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/pdf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/picture_fill.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/picture_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/picture_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/picture_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/pipeline.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/placeholder.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/placeholder.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/placeholders.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/placeholders.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/plot_area.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/portion.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/portion.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/portion_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/portion_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/portions.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/portions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/pptx_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/pptx_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/presentation_to_merge.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/presentation_to_merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/presentations_merge_request.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/presentations_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/preset_shadow_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/preset_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/protection_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/protection_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/radical_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/radical_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/reflection_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/reflection_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/remove_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/remove_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/remove_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/remove_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/reorder_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/reorder_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/replace_text.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/replace_text.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/request_input_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/request_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/reset_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/reset_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/resource_base.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/resource_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/resource_uri.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/response_output_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/response_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/right_sub_superscript_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/right_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/save.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/save.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/save_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/save_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/save_slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/save_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_chart_data_point.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/scatter_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_series.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/scatter_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/section.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/section_zoom_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/section_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/sections.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/sections.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/series.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/series_marker.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/series_marker.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_base.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_bevel.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape_bevel.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_export_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_image_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape_image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_thumbnail_bounds.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape_thumbnail_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_type.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shapes.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/shapes_alignment_type.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/shapes_alignment_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_animation.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_animation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_background.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment_base.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_comment_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comments.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_comments.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_export_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_modern_comment.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_modern_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_replace_result.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_show_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slide_show_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/slides.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/smart_art.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_node.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/smart_art_node.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/smart_art_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/soft_edge_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/soft_edge_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/solid_fill.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/special_slide_type.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/special_slide_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/split_document_result.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/storage_exist.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/storage_file.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/subscript_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/subscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/summary_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_section.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/summary_zoom_section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/superscript_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/svg_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/svg_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/swf_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/swf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/table.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/table.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_merge_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/table_cell_merge_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_split_type.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/table_cell_split_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/table_column.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/table_column.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/table_row.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/task.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/task.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/text_bounds.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/text_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/text_element.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/text_frame_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/text_frame_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/text_item.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/text_items.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/theme.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/theme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/three_d_format.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/three_d_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/tiff_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/tiff_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/tint_effect.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/tint_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/update_background.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/update_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/update_shape.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/update_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/vba_module.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/vba_module.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/vba_project.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/vba_project.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/vba_reference.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/vba_reference.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/video_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/video_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/video_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/video_frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,15 +65,17 @@
         'full_screen_mode': 'bool',
         'hide_at_showing': 'bool',
         'play_loop_mode': 'bool',
         'play_mode': 'str',
         'rewind_video': 'bool',
         'volume': 'str',
         'base64_data': 'str',
-        'picture_fill_format': 'PictureFill'
+        'picture_fill_format': 'PictureFill',
+        'trim_from_start': 'float',
+        'trim_from_end': 'float'
     }
 
     attribute_map = {
         'self_uri': 'selfUri',
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
@@ -95,33 +97,37 @@
         'full_screen_mode': 'fullScreenMode',
         'hide_at_showing': 'hideAtShowing',
         'play_loop_mode': 'playLoopMode',
         'play_mode': 'playMode',
         'rewind_video': 'rewindVideo',
         'volume': 'volume',
         'base64_data': 'base64Data',
-        'picture_fill_format': 'pictureFillFormat'
+        'picture_fill_format': 'pictureFillFormat',
+        'trim_from_start': 'trimFromStart',
+        'trim_from_end': 'trimFromEnd'
     }
 
     type_determiners = {
         'type': 'VideoFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='VideoFrame', shape_type=None, full_screen_mode=None, hide_at_showing=None, play_loop_mode=None, play_mode=None, rewind_video=None, volume=None, base64_data=None, picture_fill_format=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='VideoFrame', shape_type=None, full_screen_mode=None, hide_at_showing=None, play_loop_mode=None, play_mode=None, rewind_video=None, volume=None, base64_data=None, picture_fill_format=None, trim_from_start=None, trim_from_end=None):  # noqa: E501
         """VideoFrame - a model defined in Swagger"""  # noqa: E501
         super(VideoFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
 
         self._full_screen_mode = None
         self._hide_at_showing = None
         self._play_loop_mode = None
         self._play_mode = None
         self._rewind_video = None
         self._volume = None
         self._base64_data = None
         self._picture_fill_format = None
+        self._trim_from_start = None
+        self._trim_from_end = None
         self.type = 'VideoFrame'
 
         if full_screen_mode is not None:
             self.full_screen_mode = full_screen_mode
         if hide_at_showing is not None:
             self.hide_at_showing = hide_at_showing
         if play_loop_mode is not None:
@@ -132,14 +138,18 @@
             self.rewind_video = rewind_video
         if volume is not None:
             self.volume = volume
         if base64_data is not None:
             self.base64_data = base64_data
         if picture_fill_format is not None:
             self.picture_fill_format = picture_fill_format
+        if trim_from_start is not None:
+            self.trim_from_start = trim_from_start
+        if trim_from_end is not None:
+            self.trim_from_end = trim_from_end
 
     @property
     def full_screen_mode(self):
         """Gets the full_screen_mode of this VideoFrame.  # noqa: E501
 
         Determines whether a video is shown in full screen mode.  # noqa: E501
 
@@ -341,14 +351,58 @@
         Picture fill format.  # noqa: E501
 
         :param picture_fill_format: The picture_fill_format of this VideoFrame.  # noqa: E501
         :type: PictureFill
         """
         self._picture_fill_format = picture_fill_format
 
+    @property
+    def trim_from_start(self):
+        """Gets the trim_from_start of this VideoFrame.  # noqa: E501
+
+        Trim start [ms]  # noqa: E501
+
+        :return: The trim_from_start of this VideoFrame.  # noqa: E501
+        :rtype: float
+        """
+        return self._trim_from_start
+
+    @trim_from_start.setter
+    def trim_from_start(self, trim_from_start):
+        """Sets the trim_from_start of this VideoFrame.
+
+        Trim start [ms]  # noqa: E501
+
+        :param trim_from_start: The trim_from_start of this VideoFrame.  # noqa: E501
+        :type: float
+        """
+        self._trim_from_start = trim_from_start
+
+    @property
+    def trim_from_end(self):
+        """Gets the trim_from_end of this VideoFrame.  # noqa: E501
+
+        Trim end [ms]  # noqa: E501
+
+        :return: The trim_from_end of this VideoFrame.  # noqa: E501
+        :rtype: float
+        """
+        return self._trim_from_end
+
+    @trim_from_end.setter
+    def trim_from_end(self, trim_from_end):
+        """Sets the trim_from_end of this VideoFrame.
+
+        Trim end [ms]  # noqa: E501
+
+        :param trim_from_end: The trim_from_end of this VideoFrame.  # noqa: E501
+        :type: float
+        """
+        self._trim_from_end = trim_from_end
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/view_properties.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/workbook.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/xaml_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/xaml_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/xps_export_options.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/xps_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/xy_series.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/xy_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_frame.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_object.py` & `asposeslidescloud-23.7.0/asposeslidescloud/models/zoom_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/oauth_response.py` & `asposeslidescloud-23.7.0/asposeslidescloud/oauth_response.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud/rest.py` & `asposeslidescloud-23.7.0/asposeslidescloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud.egg-info/PKG-INFO` & `asposeslidescloud-23.7.0/README`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: asposeslidescloud
-Version: 23.6.0
-Summary: Aspose.Slides Cloud SDK for Python
-Home-page: 
-Author: Victor Putrov
-Author-email: vistor.putrov@aspose.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -36,14 +23,20 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.7
+
+* New methods **ReplaceTextFormatting** and **ReplaceTextFormatting** allow to replace text with formatting.
+* Added **AfterAnimationType**, **Rewind** and **AfterAnimationColor** methods to **Effect** class.
+* Added **TrimFromStart** and **TrimFromEnd** methods to **VideoFrame** class.
+
 ## Enhancements in Version 23.6
 
 * Added methods ho handle VBA methods: **GetVbaProject**, **GetVbaModule**, **CreateVbaModule**, **UpdateVbaModule** and **DeleteVbaModule**. Added model classes related to VBA: **VbaProject**,  **VbaModule** and  **VbaReference**.
 
 ## Enhancements in Version 23.4
 
 * Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
```

### Comparing `asposeslidescloud-23.6.0/asposeslidescloud.egg-info/SOURCES.txt` & `asposeslidescloud-23.7.0/asposeslidescloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.6.0/setup.py` & `asposeslidescloud-23.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asposeslidescloud",
-    version="23.6.0",
+    version="23.7.0",
     author="Victor Putrov",
     author_email="vistor.putrov@aspose.com",
     description="Aspose.Slides Cloud SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

