# Comparing `tmp/pydivkit-26.2.1.tar.gz` & `tmp/pydivkit-27.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-26.2.1.tar", max compression
+gzip compressed data, was "pydivkit-27.0.0.tar", max compression
```

## Comparing `pydivkit-26.2.1.tar` & `pydivkit-27.0.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     9446 2023-07-27 10:33:48.528889 pydivkit-26.2.1/README.md
--rw-r--r--   0        0        0      700 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/__init__.py
--rw-r--r--   0        0        0      164 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      445 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/core/compat.py
--rw-r--r--   0        0        0    28631 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/core/entities.py
--rw-r--r--   0        0        0     3039 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      728 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    13901 2023-07-27 10:34:51.636915 pydivkit-26.2.1/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      884 2023-07-27 10:34:51.465911 pydivkit-26.2.1/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      898 2023-07-27 10:34:51.465740 pydivkit-26.2.1/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      879 2023-07-27 10:34:51.465693 pydivkit-26.2.1/pydivkit/div/dict_variable.py
--rw-r--r--   0        0        0      863 2023-07-27 10:34:51.458253 pydivkit-26.2.1/pydivkit/div/div.py
--rw-r--r--   0        0        0     1209 2023-07-27 10:34:51.457037 pydivkit-26.2.1/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     3285 2023-07-27 10:34:51.466955 pydivkit-26.2.1/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     3671 2023-07-27 10:34:51.468478 pydivkit-26.2.1/pydivkit/div/div_action.py
--rw-r--r--   0        0        0      321 2023-07-27 10:34:51.465368 pydivkit-26.2.1/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      309 2023-07-27 10:34:51.470953 pydivkit-26.2.1/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     3038 2023-07-27 10:34:51.476969 pydivkit-26.2.1/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      371 2023-07-27 10:34:51.471032 pydivkit-26.2.1/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      879 2023-07-27 10:34:51.472873 pydivkit-26.2.1/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      557 2023-07-27 10:34:51.470149 pydivkit-26.2.1/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      671 2023-07-27 10:34:51.471050 pydivkit-26.2.1/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      599 2023-07-27 10:34:51.471658 pydivkit-26.2.1/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9833 2023-07-27 10:34:51.485118 pydivkit-26.2.1/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      369 2023-07-27 10:34:51.475645 pydivkit-26.2.1/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0      764 2023-07-27 10:34:51.477730 pydivkit-26.2.1/pydivkit/div/div_blur.py
--rw-r--r--   0        0        0     1697 2023-07-27 10:34:51.477056 pydivkit-26.2.1/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1403 2023-07-27 10:34:51.479483 pydivkit-26.2.1/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      809 2023-07-27 10:34:51.478892 pydivkit-26.2.1/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      420 2023-07-27 10:34:51.476212 pydivkit-26.2.1/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0     1176 2023-07-27 10:34:51.483526 pydivkit-26.2.1/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0    17693 2023-07-27 10:34:51.513114 pydivkit-26.2.1/pydivkit/div/div_container.py
--rw-r--r--   0        0        0      432 2023-07-27 10:34:51.481628 pydivkit-26.2.1/pydivkit/div/div_content_alignment_horizontal.py
--rw-r--r--   0        0        0      420 2023-07-27 10:34:51.483030 pydivkit-26.2.1/pydivkit/div/div_content_alignment_vertical.py
--rw-r--r--   0        0        0     1861 2023-07-27 10:34:51.487498 pydivkit-26.2.1/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      351 2023-07-27 10:34:51.482632 pydivkit-26.2.1/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     1292 2023-07-27 10:34:51.486781 pydivkit-26.2.1/pydivkit/div/div_currency_input_mask.py
--rw-r--r--   0        0        0    10752 2023-07-27 10:34:51.506667 pydivkit-26.2.1/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2915 2023-07-27 10:34:51.491294 pydivkit-26.2.1/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      872 2023-07-27 10:34:51.489653 pydivkit-26.2.1/pydivkit/div/div_default_indicator_item_placement.py
--rw-r--r--   0        0        0      802 2023-07-27 10:34:51.488606 pydivkit-26.2.1/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     2970 2023-07-27 10:34:51.494983 pydivkit-26.2.1/pydivkit/div/div_disappear_action.py
--rw-r--r--   0        0        0     1228 2023-07-27 10:34:51.492845 pydivkit-26.2.1/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      302 2023-07-27 10:34:51.493180 pydivkit-26.2.1/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     2081 2023-07-27 10:34:51.497224 pydivkit-26.2.1/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      827 2023-07-27 10:34:51.496168 pydivkit-26.2.1/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1675 2023-07-27 10:34:51.502418 pydivkit-26.2.1/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      271 2023-07-27 10:34:51.498099 pydivkit-26.2.1/pydivkit/div/div_filter.py
--rw-r--r--   0        0        0      686 2023-07-27 10:34:51.501284 pydivkit-26.2.1/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0     3313 2023-07-27 10:34:51.508319 pydivkit-26.2.1/pydivkit/div/div_fixed_length_input_mask.py
--rw-r--r--   0        0        0     1090 2023-07-27 10:34:51.505153 pydivkit-26.2.1/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     3026 2023-07-27 10:34:51.507567 pydivkit-26.2.1/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      300 2023-07-27 10:34:51.504041 pydivkit-26.2.1/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    14582 2023-07-27 10:34:51.531776 pydivkit-26.2.1/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    14431 2023-07-27 10:34:51.533782 pydivkit-26.2.1/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    12886 2023-07-27 10:34:51.532134 pydivkit-26.2.1/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    16177 2023-07-27 10:34:51.539643 pydivkit-26.2.1/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     2552 2023-07-27 10:34:51.516886 pydivkit-26.2.1/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      300 2023-07-27 10:34:51.512898 pydivkit-26.2.1/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    13998 2023-07-27 10:34:51.539611 pydivkit-26.2.1/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      490 2023-07-27 10:34:51.516403 pydivkit-26.2.1/pydivkit/div/div_indicator_item_placement.py
--rw-r--r--   0        0        0      516 2023-07-27 10:34:51.518303 pydivkit-26.2.1/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    16458 2023-07-27 10:34:51.552504 pydivkit-26.2.1/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      403 2023-07-27 10:34:51.520782 pydivkit-26.2.1/pydivkit/div/div_input_mask.py
--rw-r--r--   0        0        0      671 2023-07-27 10:34:51.522712 pydivkit-26.2.1/pydivkit/div/div_input_mask_base.py
--rw-r--r--   0        0        0      424 2023-07-27 10:34:51.525462 pydivkit-26.2.1/pydivkit/div/div_input_validator.py
--rw-r--r--   0        0        0     1323 2023-07-27 10:34:51.529042 pydivkit-26.2.1/pydivkit/div/div_input_validator_base.py
--rw-r--r--   0        0        0     1765 2023-07-27 10:34:51.535028 pydivkit-26.2.1/pydivkit/div/div_input_validator_expression.py
--rw-r--r--   0        0        0     1697 2023-07-27 10:34:51.538506 pydivkit-26.2.1/pydivkit/div/div_input_validator_regex.py
--rw-r--r--   0        0        0      255 2023-07-27 10:34:51.536969 pydivkit-26.2.1/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0     1046 2023-07-27 10:34:51.538983 pydivkit-26.2.1/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      974 2023-07-27 10:34:51.540600 pydivkit-26.2.1/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      858 2023-07-27 10:34:51.541530 pydivkit-26.2.1/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1297 2023-07-27 10:34:51.544083 pydivkit-26.2.1/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      795 2023-07-27 10:34:51.544544 pydivkit-26.2.1/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0    13014 2023-07-27 10:34:51.565802 pydivkit-26.2.1/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      369 2023-07-27 10:34:51.543352 pydivkit-26.2.1/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1950 2023-07-27 10:34:51.549087 pydivkit-26.2.1/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      694 2023-07-27 10:34:51.546876 pydivkit-26.2.1/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      357 2023-07-27 10:34:51.545062 pydivkit-26.2.1/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1136 2023-07-27 10:34:51.551366 pydivkit-26.2.1/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      800 2023-07-27 10:34:51.551138 pydivkit-26.2.1/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      768 2023-07-27 10:34:51.549184 pydivkit-26.2.1/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1933 2023-07-27 10:34:51.553291 pydivkit-26.2.1/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      473 2023-07-27 10:34:51.550623 pydivkit-26.2.1/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1156 2023-07-27 10:34:51.555635 pydivkit-26.2.1/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      412 2023-07-27 10:34:51.553722 pydivkit-26.2.1/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      800 2023-07-27 10:34:51.556870 pydivkit-26.2.1/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0     1052 2023-07-27 10:34:51.558049 pydivkit-26.2.1/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1721 2023-07-27 10:34:51.559757 pydivkit-26.2.1/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2300 2023-07-27 10:34:51.561872 pydivkit-26.2.1/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    13890 2023-07-27 10:34:51.585325 pydivkit-26.2.1/pydivkit/div/div_select.py
--rw-r--r--   0        0        0    13054 2023-07-27 10:34:51.583449 pydivkit-26.2.1/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0     1198 2023-07-27 10:34:51.561023 pydivkit-26.2.1/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      380 2023-07-27 10:34:51.560035 pydivkit-26.2.1/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0     1144 2023-07-27 10:34:51.565643 pydivkit-26.2.1/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0     2165 2023-07-27 10:34:51.566481 pydivkit-26.2.1/pydivkit/div/div_sight_action.py
--rw-r--r--   0        0        0      424 2023-07-27 10:34:51.565074 pydivkit-26.2.1/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      256 2023-07-27 10:34:51.567040 pydivkit-26.2.1/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2360 2023-07-27 10:34:51.573198 pydivkit-26.2.1/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    15030 2023-07-27 10:34:51.596982 pydivkit-26.2.1/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      700 2023-07-27 10:34:51.572690 pydivkit-26.2.1/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    13360 2023-07-27 10:34:51.594912 pydivkit-26.2.1/pydivkit/div/div_state.py
--rw-r--r--   0        0        0     1101 2023-07-27 10:34:51.575137 pydivkit-26.2.1/pydivkit/div/div_stretch_indicator_item_placement.py
--rw-r--r--   0        0        0     1000 2023-07-27 10:34:51.574505 pydivkit-26.2.1/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    20553 2023-07-27 10:34:51.616267 pydivkit-26.2.1/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    25644 2023-07-27 10:34:51.629865 pydivkit-26.2.1/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      373 2023-07-27 10:34:51.578987 pydivkit-26.2.1/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0      319 2023-07-27 10:34:51.579812 pydivkit-26.2.1/pydivkit/div/div_text_range_background.py
--rw-r--r--   0        0        0      975 2023-07-27 10:34:51.585590 pydivkit-26.2.1/pydivkit/div/div_text_range_border.py
--rw-r--r--   0        0        0     2796 2023-07-27 10:34:51.587645 pydivkit-26.2.1/pydivkit/div/div_timer.py
--rw-r--r--   0        0        0     2923 2023-07-27 10:34:51.594876 pydivkit-26.2.1/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1171 2023-07-27 10:34:51.590744 pydivkit-26.2.1/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1234 2023-07-27 10:34:51.592699 pydivkit-26.2.1/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      338 2023-07-27 10:34:51.595074 pydivkit-26.2.1/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      333 2023-07-27 10:34:51.598576 pydivkit-26.2.1/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1581 2023-07-27 10:34:51.603146 pydivkit-26.2.1/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      613 2023-07-27 10:34:51.599851 pydivkit-26.2.1/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0    13675 2023-07-27 10:34:51.625023 pydivkit-26.2.1/pydivkit/div/div_video.py
--rw-r--r--   0        0        0     2331 2023-07-27 10:34:51.605487 pydivkit-26.2.1/pydivkit/div/div_video_source.py
--rw-r--r--   0        0        0      286 2023-07-27 10:34:51.602151 pydivkit-26.2.1/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     2956 2023-07-27 10:34:51.606947 pydivkit-26.2.1/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0     2298 2023-07-27 10:34:51.610964 pydivkit-26.2.1/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      866 2023-07-27 10:34:51.609872 pydivkit-26.2.1/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      872 2023-07-27 10:34:51.611012 pydivkit-26.2.1/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      860 2023-07-27 10:34:51.612826 pydivkit-26.2.1/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      882 2023-07-27 10:34:51.616100 pydivkit-26.2.1/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pydivkit/py.typed
--rw-r--r--   0        0        0     1697 2023-07-27 10:33:48.528889 pydivkit-26.2.1/pyproject.toml
--rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-26.2.1/PKG-INFO
+-rw-r--r--   0        0        0     9446 2023-07-31 10:18:01.080779 pydivkit-27.0.0/README.md
+-rw-r--r--   0        0        0      700 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    13901 2023-07-31 10:18:51.976436 pydivkit-27.0.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      884 2023-07-31 10:18:51.650277 pydivkit-27.0.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      898 2023-07-31 10:18:51.658286 pydivkit-27.0.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      879 2023-07-31 10:18:51.654522 pydivkit-27.0.0/pydivkit/div/dict_variable.py
+-rw-r--r--   0        0        0      863 2023-07-31 10:18:51.636527 pydivkit-27.0.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2023-07-31 10:18:51.636678 pydivkit-27.0.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3285 2023-07-31 10:18:51.653478 pydivkit-27.0.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     3671 2023-07-31 10:18:51.660842 pydivkit-27.0.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0      321 2023-07-31 10:18:51.649458 pydivkit-27.0.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2023-07-31 10:18:51.661425 pydivkit-27.0.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3038 2023-07-31 10:18:51.674965 pydivkit-27.0.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2023-07-31 10:18:51.662918 pydivkit-27.0.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2023-07-31 10:18:51.667712 pydivkit-27.0.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2023-07-31 10:18:51.664341 pydivkit-27.0.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2023-07-31 10:18:51.664922 pydivkit-27.0.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2023-07-31 10:18:51.669748 pydivkit-27.0.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9833 2023-07-31 10:18:51.702063 pydivkit-27.0.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2023-07-31 10:18:51.673717 pydivkit-27.0.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2023-07-31 10:18:51.675331 pydivkit-27.0.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1697 2023-07-31 10:18:51.676777 pydivkit-27.0.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2023-07-31 10:18:51.682474 pydivkit-27.0.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2023-07-31 10:18:51.681224 pydivkit-27.0.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2023-07-31 10:18:51.676866 pydivkit-27.0.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2023-07-31 10:18:51.689174 pydivkit-27.0.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0    17693 2023-07-31 10:18:51.747620 pydivkit-27.0.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0      432 2023-07-31 10:18:51.683717 pydivkit-27.0.0/pydivkit/div/div_content_alignment_horizontal.py
+-rw-r--r--   0        0        0      420 2023-07-31 10:18:51.689075 pydivkit-27.0.0/pydivkit/div/div_content_alignment_vertical.py
+-rw-r--r--   0        0        0     1861 2023-07-31 10:18:51.696971 pydivkit-27.0.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2023-07-31 10:18:51.688926 pydivkit-27.0.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1292 2023-07-31 10:18:51.699320 pydivkit-27.0.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10752 2023-07-31 10:18:51.736783 pydivkit-27.0.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2915 2023-07-31 10:18:51.705631 pydivkit-27.0.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2023-07-31 10:18:51.702836 pydivkit-27.0.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2023-07-31 10:18:51.701024 pydivkit-27.0.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     2970 2023-07-31 10:18:51.712932 pydivkit-27.0.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1228 2023-07-31 10:18:51.710255 pydivkit-27.0.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2023-07-31 10:18:51.709149 pydivkit-27.0.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     2081 2023-07-31 10:18:51.718123 pydivkit-27.0.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      827 2023-07-31 10:18:51.720025 pydivkit-27.0.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2023-07-31 10:18:51.729579 pydivkit-27.0.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      271 2023-07-31 10:18:51.722111 pydivkit-27.0.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      686 2023-07-31 10:18:51.727277 pydivkit-27.0.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3313 2023-07-31 10:18:51.738677 pydivkit-27.0.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1090 2023-07-31 10:18:51.736771 pydivkit-27.0.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     3026 2023-07-31 10:18:51.744010 pydivkit-27.0.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      300 2023-07-31 10:18:51.738343 pydivkit-27.0.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    14582 2023-07-31 10:18:51.782427 pydivkit-27.0.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14431 2023-07-31 10:18:51.791785 pydivkit-27.0.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12886 2023-07-31 10:18:51.785970 pydivkit-27.0.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    16177 2023-07-31 10:18:51.797085 pydivkit-27.0.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2552 2023-07-31 10:18:51.757666 pydivkit-27.0.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2023-07-31 10:18:51.746946 pydivkit-27.0.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13998 2023-07-31 10:18:51.798225 pydivkit-27.0.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2023-07-31 10:18:51.755029 pydivkit-27.0.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2023-07-31 10:18:51.757300 pydivkit-27.0.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    16458 2023-07-31 10:18:51.815399 pydivkit-27.0.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      403 2023-07-31 10:18:51.762746 pydivkit-27.0.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      671 2023-07-31 10:18:51.765419 pydivkit-27.0.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2023-07-31 10:18:51.770653 pydivkit-27.0.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1323 2023-07-31 10:18:51.776891 pydivkit-27.0.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1765 2023-07-31 10:18:51.785975 pydivkit-27.0.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1697 2023-07-31 10:18:51.795180 pydivkit-27.0.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2023-07-31 10:18:51.791463 pydivkit-27.0.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2023-07-31 10:18:51.799988 pydivkit-27.0.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2023-07-31 10:18:51.798097 pydivkit-27.0.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2023-07-31 10:18:51.802744 pydivkit-27.0.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2023-07-31 10:18:51.803946 pydivkit-27.0.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2023-07-31 10:18:51.805407 pydivkit-27.0.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0    13014 2023-07-31 10:18:51.850133 pydivkit-27.0.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2023-07-31 10:18:51.804332 pydivkit-27.0.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1950 2023-07-31 10:18:51.817163 pydivkit-27.0.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2023-07-31 10:18:51.810604 pydivkit-27.0.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      357 2023-07-31 10:18:51.809299 pydivkit-27.0.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1136 2023-07-31 10:18:51.817174 pydivkit-27.0.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2023-07-31 10:18:51.816123 pydivkit-27.0.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2023-07-31 10:18:51.814014 pydivkit-27.0.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2023-07-31 10:18:51.823838 pydivkit-27.0.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2023-07-31 10:18:51.816502 pydivkit-27.0.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1156 2023-07-31 10:18:51.828211 pydivkit-27.0.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2023-07-31 10:18:51.821874 pydivkit-27.0.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2023-07-31 10:18:51.827839 pydivkit-27.0.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2023-07-31 10:18:51.829299 pydivkit-27.0.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2023-07-31 10:18:51.832438 pydivkit-27.0.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2023-07-31 10:18:51.836368 pydivkit-27.0.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13890 2023-07-31 10:18:51.900940 pydivkit-27.0.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    13054 2023-07-31 10:18:51.873093 pydivkit-27.0.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2023-07-31 10:18:51.838661 pydivkit-27.0.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2023-07-31 10:18:51.835025 pydivkit-27.0.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2023-07-31 10:18:51.843144 pydivkit-27.0.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0     2165 2023-07-31 10:18:51.845805 pydivkit-27.0.0/pydivkit/div/div_sight_action.py
+-rw-r--r--   0        0        0      424 2023-07-31 10:18:51.843528 pydivkit-27.0.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2023-07-31 10:18:51.844786 pydivkit-27.0.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2023-07-31 10:18:51.856670 pydivkit-27.0.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    15030 2023-07-31 10:18:51.900069 pydivkit-27.0.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2023-07-31 10:18:51.855111 pydivkit-27.0.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13360 2023-07-31 10:18:51.889816 pydivkit-27.0.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2023-07-31 10:18:51.858821 pydivkit-27.0.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2023-07-31 10:18:51.859369 pydivkit-27.0.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    20553 2023-07-31 10:18:51.986502 pydivkit-27.0.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25644 2023-07-31 10:18:51.958335 pydivkit-27.0.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2023-07-31 10:18:51.867029 pydivkit-27.0.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2023-07-31 10:18:51.869625 pydivkit-27.0.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2023-07-31 10:18:51.877796 pydivkit-27.0.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2796 2023-07-31 10:18:51.883636 pydivkit-27.0.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2923 2023-07-31 10:18:51.891096 pydivkit-27.0.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2023-07-31 10:18:51.889023 pydivkit-27.0.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2023-07-31 10:18:51.896152 pydivkit-27.0.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2023-07-31 10:18:51.898227 pydivkit-27.0.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2023-07-31 10:18:51.898955 pydivkit-27.0.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2023-07-31 10:18:51.903529 pydivkit-27.0.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      613 2023-07-31 10:18:51.906155 pydivkit-27.0.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    13675 2023-07-31 10:18:51.951274 pydivkit-27.0.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0     2331 2023-07-31 10:18:51.915788 pydivkit-27.0.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2023-07-31 10:18:51.908345 pydivkit-27.0.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     2956 2023-07-31 10:18:51.912578 pydivkit-27.0.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2023-07-31 10:18:51.922691 pydivkit-27.0.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      866 2023-07-31 10:18:51.919507 pydivkit-27.0.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      872 2023-07-31 10:18:51.920534 pydivkit-27.0.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      860 2023-07-31 10:18:51.929376 pydivkit-27.0.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      882 2023-07-31 10:18:51.932892 pydivkit-27.0.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2023-07-31 10:18:01.080779 pydivkit-27.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-27.0.0/PKG-INFO
```

### Comparing `pydivkit-26.2.1/README.md` & `pydivkit-27.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/__init__.py` & `pydivkit-27.0.0/pydivkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/core/entities.py` & `pydivkit-27.0.0/pydivkit/core/entities.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/core/fields.py` & `pydivkit-27.0.0/pydivkit/core/fields.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/core/types/union.py` & `pydivkit-27.0.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/__init__.py` & `pydivkit-27.0.0/pydivkit/div/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/boolean_variable.py` & `pydivkit-27.0.0/pydivkit/div/boolean_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/color_variable.py` & `pydivkit-27.0.0/pydivkit/div/color_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/dict_variable.py` & `pydivkit-27.0.0/pydivkit/div/dict_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div.py` & `pydivkit-27.0.0/pydivkit/div/div.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-27.0.0/pydivkit/div/div_absolute_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_accessibility.py` & `pydivkit-27.0.0/pydivkit/div/div_accessibility.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_action.py` & `pydivkit-27.0.0/pydivkit/div/div_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_animation.py` & `pydivkit-27.0.0/pydivkit/div/div_animation.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_appearance_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_appearance_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_aspect.py` & `pydivkit-27.0.0/pydivkit/div/div_aspect.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_background.py` & `pydivkit-27.0.0/pydivkit/div/div_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_base.py` & `pydivkit-27.0.0/pydivkit/div/div_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_blur.py` & `pydivkit-27.0.0/pydivkit/div/div_blur.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_border.py` & `pydivkit-27.0.0/pydivkit/div/div_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_change_set_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_change_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_circle_shape.py` & `pydivkit-27.0.0/pydivkit/div/div_circle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_container.py` & `pydivkit-27.0.0/pydivkit/div/div_container.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_corners_radius.py` & `pydivkit-27.0.0/pydivkit/div/div_corners_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_currency_input_mask.py` & `pydivkit-27.0.0/pydivkit/div/div_currency_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_custom.py` & `pydivkit-27.0.0/pydivkit/div/div_custom.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_data.py` & `pydivkit-27.0.0/pydivkit/div/div_data.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_default_indicator_item_placement.py` & `pydivkit-27.0.0/pydivkit/div/div_default_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_dimension.py` & `pydivkit-27.0.0/pydivkit/div/div_dimension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_disappear_action.py` & `pydivkit-27.0.0/pydivkit/div/div_disappear_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_download_callbacks.py` & `pydivkit-27.0.0/pydivkit/div/div_download_callbacks.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_edge_insets.py` & `pydivkit-27.0.0/pydivkit/div/div_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_extension.py` & `pydivkit-27.0.0/pydivkit/div/div_extension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_fade_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_fade_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_fixed_count.py` & `pydivkit-27.0.0/pydivkit/div/div_fixed_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_fixed_length_input_mask.py` & `pydivkit-27.0.0/pydivkit/div/div_fixed_length_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_fixed_size.py` & `pydivkit-27.0.0/pydivkit/div/div_fixed_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_focus.py` & `pydivkit-27.0.0/pydivkit/div/div_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_gallery.py` & `pydivkit-27.0.0/pydivkit/div/div_gallery.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_gif_image.py` & `pydivkit-27.0.0/pydivkit/div/div_gif_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_grid.py` & `pydivkit-27.0.0/pydivkit/div/div_grid.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_image.py` & `pydivkit-27.0.0/pydivkit/div/div_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_image_background.py` & `pydivkit-27.0.0/pydivkit/div/div_image_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_indicator.py` & `pydivkit-27.0.0/pydivkit/div/div_indicator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_infinity_count.py` & `pydivkit-27.0.0/pydivkit/div/div_infinity_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_input.py` & `pydivkit-27.0.0/pydivkit/div/div_input.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_input_mask_base.py` & `pydivkit-27.0.0/pydivkit/div/div_input_mask_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_input_validator_base.py` & `pydivkit-27.0.0/pydivkit/div/div_input_validator_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_input_validator_expression.py` & `pydivkit-27.0.0/pydivkit/div/div_input_validator_expression.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_input_validator_regex.py` & `pydivkit-27.0.0/pydivkit/div/div_input_validator_regex.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_linear_gradient.py` & `pydivkit-27.0.0/pydivkit/div/div_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_match_parent_size.py` & `pydivkit-27.0.0/pydivkit/div/div_match_parent_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-27.0.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_nine_patch_background.py` & `pydivkit-27.0.0/pydivkit/div/div_nine_patch_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_page_size.py` & `pydivkit-27.0.0/pydivkit/div/div_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_pager.py` & `pydivkit-27.0.0/pydivkit/div/div_pager.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_patch.py` & `pydivkit-27.0.0/pydivkit/div/div_patch.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_percentage_size.py` & `pydivkit-27.0.0/pydivkit/div/div_percentage_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_pivot_fixed.py` & `pydivkit-27.0.0/pydivkit/div/div_pivot_fixed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_pivot_percentage.py` & `pydivkit-27.0.0/pydivkit/div/div_pivot_percentage.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_point.py` & `pydivkit-27.0.0/pydivkit/div/div_point.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_radial_gradient.py` & `pydivkit-27.0.0/pydivkit/div/div_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-27.0.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-27.0.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_radial_gradient_relative_radius.py` & `pydivkit-27.0.0/pydivkit/div/div_radial_gradient_relative_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_rounded_rectangle_shape.py` & `pydivkit-27.0.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_scale_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_scale_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_select.py` & `pydivkit-27.0.0/pydivkit/div/div_select.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_separator.py` & `pydivkit-27.0.0/pydivkit/div/div_separator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_shadow.py` & `pydivkit-27.0.0/pydivkit/div/div_shadow.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_shape_drawable.py` & `pydivkit-27.0.0/pydivkit/div/div_shape_drawable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_sight_action.py` & `pydivkit-27.0.0/pydivkit/div/div_sight_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_slide_transition.py` & `pydivkit-27.0.0/pydivkit/div/div_slide_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_slider.py` & `pydivkit-27.0.0/pydivkit/div/div_slider.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_solid_background.py` & `pydivkit-27.0.0/pydivkit/div/div_solid_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_state.py` & `pydivkit-27.0.0/pydivkit/div/div_state.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_stretch_indicator_item_placement.py` & `pydivkit-27.0.0/pydivkit/div/div_stretch_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_stroke.py` & `pydivkit-27.0.0/pydivkit/div/div_stroke.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_tabs.py` & `pydivkit-27.0.0/pydivkit/div/div_tabs.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_text.py` & `pydivkit-27.0.0/pydivkit/div/div_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_text_range_border.py` & `pydivkit-27.0.0/pydivkit/div/div_text_range_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_timer.py` & `pydivkit-27.0.0/pydivkit/div/div_timer.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_tooltip.py` & `pydivkit-27.0.0/pydivkit/div/div_tooltip.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_transform.py` & `pydivkit-27.0.0/pydivkit/div/div_transform.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_transition_base.py` & `pydivkit-27.0.0/pydivkit/div/div_transition_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_trigger.py` & `pydivkit-27.0.0/pydivkit/div/div_trigger.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_variable.py` & `pydivkit-27.0.0/pydivkit/div/div_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_video.py` & `pydivkit-27.0.0/pydivkit/div/div_video.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_video_source.py` & `pydivkit-27.0.0/pydivkit/div/div_video_source.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_visibility_action.py` & `pydivkit-27.0.0/pydivkit/div/div_visibility_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/div_wrap_content_size.py` & `pydivkit-27.0.0/pydivkit/div/div_wrap_content_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/integer_variable.py` & `pydivkit-27.0.0/pydivkit/div/integer_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/number_variable.py` & `pydivkit-27.0.0/pydivkit/div/number_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/string_variable.py` & `pydivkit-27.0.0/pydivkit/div/string_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pydivkit/div/url_variable.py` & `pydivkit-27.0.0/pydivkit/div/url_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-26.2.1/pyproject.toml` & `pydivkit-27.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydivkit"
-version = "26.2.1"
+version = "27.0.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
     "Pavel Mosein <p-mosein@yandex-team.ru>",
```

### Comparing `pydivkit-26.2.1/PKG-INFO` & `pydivkit-27.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivkit
-Version: 26.2.1
+Version: 27.0.0
 Summary: DivKit python library
 Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
 Keywords: divkit,sdk
 Author: Vladislav Bakaev
 Author-email: bakaev-vlad@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

