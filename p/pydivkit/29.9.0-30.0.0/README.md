# Comparing `tmp/pydivkit-29.9.0.tar.gz` & `tmp/pydivkit-30.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-29.9.0.tar", max compression
+gzip compressed data, was "pydivkit-30.0.0.tar", max compression
```

## Comparing `pydivkit-29.9.0.tar` & `pydivkit-30.0.0.tar`

### file list

```diff
@@ -1,154 +1,158 @@
--rw-r--r--   0        0        0     9446 2024-03-11 13:51:44.836531 pydivkit-29.9.0/README.md
--rw-r--r--   0        0        0      700 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/__init__.py
--rw-r--r--   0        0        0      164 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      445 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/compat.py
--rw-r--r--   0        0        0    28631 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/entities.py
--rw-r--r--   0        0        0     3039 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      728 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    16462 2024-03-11 13:52:24.445063 pydivkit-29.9.0/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      611 2024-03-11 13:52:24.249505 pydivkit-29.9.0/pydivkit/div/array_value.py
--rw-r--r--   0        0        0      857 2024-03-11 13:52:24.249608 pydivkit-29.9.0/pydivkit/div/array_variable.py
--rw-r--r--   0        0        0      613 2024-03-11 13:52:24.249614 pydivkit-29.9.0/pydivkit/div/boolean_value.py
--rw-r--r--   0        0        0      861 2024-03-11 13:52:24.249701 pydivkit-29.9.0/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      627 2024-03-11 13:52:24.249480 pydivkit-29.9.0/pydivkit/div/color_value.py
--rw-r--r--   0        0        0      875 2024-03-11 13:52:24.249639 pydivkit-29.9.0/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      603 2024-03-11 13:52:24.249522 pydivkit-29.9.0/pydivkit/div/content_text.py
--rw-r--r--   0        0        0      621 2024-03-11 13:52:24.249686 pydivkit-29.9.0/pydivkit/div/content_url.py
--rw-r--r--   0        0        0      609 2024-03-11 13:52:24.255942 pydivkit-29.9.0/pydivkit/div/dict_value.py
--rw-r--r--   0        0        0      856 2024-03-11 13:52:24.256851 pydivkit-29.9.0/pydivkit/div/dict_variable.py
--rw-r--r--   0        0        0      863 2024-03-11 13:52:24.255542 pydivkit-29.9.0/pydivkit/div/div.py
--rw-r--r--   0        0        0     1209 2024-03-11 13:52:24.256182 pydivkit-29.9.0/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     3234 2024-03-11 13:52:24.261068 pydivkit-29.9.0/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     4162 2024-03-11 13:52:24.264237 pydivkit-29.9.0/pydivkit/div/div_action.py
--rw-r--r--   0        0        0     1057 2024-03-11 13:52:24.257484 pydivkit-29.9.0/pydivkit/div/div_action_array_insert_value.py
--rw-r--r--   0        0        0      863 2024-03-11 13:52:24.256452 pydivkit-29.9.0/pydivkit/div/div_action_array_remove_value.py
--rw-r--r--   0        0        0      837 2024-03-11 13:52:24.261876 pydivkit-29.9.0/pydivkit/div/div_action_copy_to_clipboard.py
--rw-r--r--   0        0        0      346 2024-03-11 13:52:24.260172 pydivkit-29.9.0/pydivkit/div/div_action_copy_to_clipboard_content.py
--rw-r--r--   0        0        0      732 2024-03-11 13:52:24.262290 pydivkit-29.9.0/pydivkit/div/div_action_focus_element.py
--rw-r--r--   0        0        0      885 2024-03-11 13:52:24.263241 pydivkit-29.9.0/pydivkit/div/div_action_set_variable.py
--rw-r--r--   0        0        0      687 2024-03-11 13:52:24.261478 pydivkit-29.9.0/pydivkit/div/div_action_typed.py
--rw-r--r--   0        0        0      321 2024-03-11 13:52:24.262761 pydivkit-29.9.0/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      309 2024-03-11 13:52:24.265280 pydivkit-29.9.0/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     3016 2024-03-11 13:52:24.271683 pydivkit-29.9.0/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      371 2024-03-11 13:52:24.266235 pydivkit-29.9.0/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      879 2024-03-11 13:52:24.268551 pydivkit-29.9.0/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      557 2024-03-11 13:52:24.265792 pydivkit-29.9.0/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      671 2024-03-11 13:52:24.267263 pydivkit-29.9.0/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      599 2024-03-11 13:52:24.267030 pydivkit-29.9.0/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9678 2024-03-11 13:52:24.279948 pydivkit-29.9.0/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      369 2024-03-11 13:52:24.270048 pydivkit-29.9.0/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0      764 2024-03-11 13:52:24.272387 pydivkit-29.9.0/pydivkit/div/div_blur.py
--rw-r--r--   0        0        0     1734 2024-03-11 13:52:24.272606 pydivkit-29.9.0/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1403 2024-03-11 13:52:24.275608 pydivkit-29.9.0/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      809 2024-03-11 13:52:24.274496 pydivkit-29.9.0/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      420 2024-03-11 13:52:24.272220 pydivkit-29.9.0/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0     1176 2024-03-11 13:52:24.277227 pydivkit-29.9.0/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0     2552 2024-03-11 13:52:24.278176 pydivkit-29.9.0/pydivkit/div/div_collection_item_builder.py
--rw-r--r--   0        0        0    18193 2024-03-11 13:52:24.308836 pydivkit-29.9.0/pydivkit/div/div_container.py
--rw-r--r--   0        0        0      432 2024-03-11 13:52:24.278029 pydivkit-29.9.0/pydivkit/div/div_content_alignment_horizontal.py
--rw-r--r--   0        0        0      420 2024-03-11 13:52:24.278552 pydivkit-29.9.0/pydivkit/div/div_content_alignment_vertical.py
--rw-r--r--   0        0        0     1861 2024-03-11 13:52:24.282521 pydivkit-29.9.0/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      351 2024-03-11 13:52:24.279674 pydivkit-29.9.0/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     1246 2024-03-11 13:52:24.283896 pydivkit-29.9.0/pydivkit/div/div_currency_input_mask.py
--rw-r--r--   0        0        0    10575 2024-03-11 13:52:24.302763 pydivkit-29.9.0/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2826 2024-03-11 13:52:24.285976 pydivkit-29.9.0/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      872 2024-03-11 13:52:24.286182 pydivkit-29.9.0/pydivkit/div/div_default_indicator_item_placement.py
--rw-r--r--   0        0        0      802 2024-03-11 13:52:24.285295 pydivkit-29.9.0/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     3528 2024-03-11 13:52:24.290975 pydivkit-29.9.0/pydivkit/div/div_disappear_action.py
--rw-r--r--   0        0        0     1184 2024-03-11 13:52:24.288759 pydivkit-29.9.0/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      302 2024-03-11 13:52:24.288935 pydivkit-29.9.0/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     2081 2024-03-11 13:52:24.293491 pydivkit-29.9.0/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      804 2024-03-11 13:52:24.291620 pydivkit-29.9.0/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1675 2024-03-11 13:52:24.296687 pydivkit-29.9.0/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      340 2024-03-11 13:52:24.293893 pydivkit-29.9.0/pydivkit/div/div_filter.py
--rw-r--r--   0        0        0      564 2024-03-11 13:52:24.295831 pydivkit-29.9.0/pydivkit/div/div_filter_rtl_mirror.py
--rw-r--r--   0        0        0      686 2024-03-11 13:52:24.299715 pydivkit-29.9.0/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0     3267 2024-03-11 13:52:24.305275 pydivkit-29.9.0/pydivkit/div/div_fixed_length_input_mask.py
--rw-r--r--   0        0        0     1090 2024-03-11 13:52:24.303838 pydivkit-29.9.0/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     2850 2024-03-11 13:52:24.304255 pydivkit-29.9.0/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      300 2024-03-11 13:52:24.301469 pydivkit-29.9.0/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    15161 2024-03-11 13:52:24.327998 pydivkit-29.9.0/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    14187 2024-03-11 13:52:24.330015 pydivkit-29.9.0/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    12660 2024-03-11 13:52:24.329355 pydivkit-29.9.0/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    15911 2024-03-11 13:52:24.337108 pydivkit-29.9.0/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     2530 2024-03-11 13:52:24.314267 pydivkit-29.9.0/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      300 2024-03-11 13:52:24.310451 pydivkit-29.9.0/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    13843 2024-03-11 13:52:24.336847 pydivkit-29.9.0/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      490 2024-03-11 13:52:24.313107 pydivkit-29.9.0/pydivkit/div/div_indicator_item_placement.py
--rw-r--r--   0        0        0      516 2024-03-11 13:52:24.316155 pydivkit-29.9.0/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    16238 2024-03-11 13:52:24.349718 pydivkit-29.9.0/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      478 2024-03-11 13:52:24.318154 pydivkit-29.9.0/pydivkit/div/div_input_mask.py
--rw-r--r--   0        0        0      648 2024-03-11 13:52:24.320834 pydivkit-29.9.0/pydivkit/div/div_input_mask_base.py
--rw-r--r--   0        0        0      424 2024-03-11 13:52:24.323139 pydivkit-29.9.0/pydivkit/div/div_input_validator.py
--rw-r--r--   0        0        0     1277 2024-03-11 13:52:24.328285 pydivkit-29.9.0/pydivkit/div/div_input_validator_base.py
--rw-r--r--   0        0        0     1719 2024-03-11 13:52:24.332768 pydivkit-29.9.0/pydivkit/div/div_input_validator_expression.py
--rw-r--r--   0        0        0     1628 2024-03-11 13:52:24.336382 pydivkit-29.9.0/pydivkit/div/div_input_validator_regex.py
--rw-r--r--   0        0        0      255 2024-03-11 13:52:24.334144 pydivkit-29.9.0/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0     1046 2024-03-11 13:52:24.338070 pydivkit-29.9.0/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      974 2024-03-11 13:52:24.337616 pydivkit-29.9.0/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      858 2024-03-11 13:52:24.339147 pydivkit-29.9.0/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1297 2024-03-11 13:52:24.341486 pydivkit-29.9.0/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      795 2024-03-11 13:52:24.342771 pydivkit-29.9.0/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0    13227 2024-03-11 13:52:24.364321 pydivkit-29.9.0/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      369 2024-03-11 13:52:24.340734 pydivkit-29.9.0/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1928 2024-03-11 13:52:24.346710 pydivkit-29.9.0/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      694 2024-03-11 13:52:24.344315 pydivkit-29.9.0/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      820 2024-03-11 13:52:24.345607 pydivkit-29.9.0/pydivkit/div/div_phone_input_mask.py
--rw-r--r--   0        0        0      357 2024-03-11 13:52:24.345163 pydivkit-29.9.0/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1136 2024-03-11 13:52:24.348597 pydivkit-29.9.0/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      800 2024-03-11 13:52:24.348963 pydivkit-29.9.0/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      768 2024-03-11 13:52:24.348878 pydivkit-29.9.0/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1933 2024-03-11 13:52:24.353543 pydivkit-29.9.0/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      473 2024-03-11 13:52:24.349467 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1156 2024-03-11 13:52:24.353853 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      412 2024-03-11 13:52:24.352085 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      800 2024-03-11 13:52:24.355691 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0     1052 2024-03-11 13:52:24.357231 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1721 2024-03-11 13:52:24.358941 pydivkit-29.9.0/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2300 2024-03-11 13:52:24.360897 pydivkit-29.9.0/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    13666 2024-03-11 13:52:24.383982 pydivkit-29.9.0/pydivkit/div/div_select.py
--rw-r--r--   0        0        0    12833 2024-03-11 13:52:24.381717 pydivkit-29.9.0/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0     1198 2024-03-11 13:52:24.360313 pydivkit-29.9.0/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      380 2024-03-11 13:52:24.360084 pydivkit-29.9.0/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0     1144 2024-03-11 13:52:24.365297 pydivkit-29.9.0/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0     2723 2024-03-11 13:52:24.366636 pydivkit-29.9.0/pydivkit/div/div_sight_action.py
--rw-r--r--   0        0        0      424 2024-03-11 13:52:24.365181 pydivkit-29.9.0/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      256 2024-03-11 13:52:24.365974 pydivkit-29.9.0/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2360 2024-03-11 13:52:24.371447 pydivkit-29.9.0/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    16427 2024-03-11 13:52:24.399701 pydivkit-29.9.0/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      700 2024-03-11 13:52:24.371633 pydivkit-29.9.0/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    13669 2024-03-11 13:52:24.393749 pydivkit-29.9.0/pydivkit/div/div_state.py
--rw-r--r--   0        0        0     1101 2024-03-11 13:52:24.372628 pydivkit-29.9.0/pydivkit/div/div_stretch_indicator_item_placement.py
--rw-r--r--   0        0        0     1000 2024-03-11 13:52:24.374176 pydivkit-29.9.0/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    20352 2024-03-11 13:52:24.414134 pydivkit-29.9.0/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    25985 2024-03-11 13:52:24.463688 pydivkit-29.9.0/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      373 2024-03-11 13:52:24.376478 pydivkit-29.9.0/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0      319 2024-03-11 13:52:24.379306 pydivkit-29.9.0/pydivkit/div/div_text_range_background.py
--rw-r--r--   0        0        0      975 2024-03-11 13:52:24.382345 pydivkit-29.9.0/pydivkit/div/div_text_range_border.py
--rw-r--r--   0        0        0     2706 2024-03-11 13:52:24.387093 pydivkit-29.9.0/pydivkit/div/div_timer.py
--rw-r--r--   0        0        0     2922 2024-03-11 13:52:24.392564 pydivkit-29.9.0/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1171 2024-03-11 13:52:24.389188 pydivkit-29.9.0/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1234 2024-03-11 13:52:24.389715 pydivkit-29.9.0/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      338 2024-03-11 13:52:24.393615 pydivkit-29.9.0/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      333 2024-03-11 13:52:24.394677 pydivkit-29.9.0/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1581 2024-03-11 13:52:24.398851 pydivkit-29.9.0/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      593 2024-03-11 13:52:24.396878 pydivkit-29.9.0/pydivkit/div/div_typed_value.py
--rw-r--r--   0        0        0      663 2024-03-11 13:52:24.397628 pydivkit-29.9.0/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0    14446 2024-03-11 13:52:24.423923 pydivkit-29.9.0/pydivkit/div/div_video.py
--rw-r--r--   0        0        0      276 2024-03-11 13:52:24.398912 pydivkit-29.9.0/pydivkit/div/div_video_scale.py
--rw-r--r--   0        0        0     2331 2024-03-11 13:52:24.408006 pydivkit-29.9.0/pydivkit/div/div_video_source.py
--rw-r--r--   0        0        0      286 2024-03-11 13:52:24.403528 pydivkit-29.9.0/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     3514 2024-03-11 13:52:24.407117 pydivkit-29.9.0/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0     2298 2024-03-11 13:52:24.408418 pydivkit-29.9.0/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      611 2024-03-11 13:52:24.405665 pydivkit-29.9.0/pydivkit/div/integer_value.py
--rw-r--r--   0        0        0      843 2024-03-11 13:52:24.410583 pydivkit-29.9.0/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      611 2024-03-11 13:52:24.411093 pydivkit-29.9.0/pydivkit/div/number_value.py
--rw-r--r--   0        0        0      849 2024-03-11 13:52:24.414604 pydivkit-29.9.0/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      607 2024-03-11 13:52:24.414132 pydivkit-29.9.0/pydivkit/div/string_value.py
--rw-r--r--   0        0        0      837 2024-03-11 13:52:24.415706 pydivkit-29.9.0/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      617 2024-03-11 13:52:24.416283 pydivkit-29.9.0/pydivkit/div/url_value.py
--rw-r--r--   0        0        0      859 2024-03-11 13:52:24.417295 pydivkit-29.9.0/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/py.typed
--rw-r--r--   0        0        0     1697 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pyproject.toml
--rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-29.9.0/PKG-INFO
+-rw-r--r--   0        0        0     9446 2024-05-13 16:24:22.967038 pydivkit-30.0.0/README.md
+-rw-r--r--   0        0        0      700 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    16973 2024-05-13 16:24:54.047636 pydivkit-30.0.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      611 2024-05-13 16:24:53.881331 pydivkit-30.0.0/pydivkit/div/array_value.py
+-rw-r--r--   0        0        0      857 2024-05-13 16:24:53.881465 pydivkit-30.0.0/pydivkit/div/array_variable.py
+-rw-r--r--   0        0        0      613 2024-05-13 16:24:53.881319 pydivkit-30.0.0/pydivkit/div/boolean_value.py
+-rw-r--r--   0        0        0      861 2024-05-13 16:24:53.881477 pydivkit-30.0.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      627 2024-05-13 16:24:53.881300 pydivkit-30.0.0/pydivkit/div/color_value.py
+-rw-r--r--   0        0        0      875 2024-05-13 16:24:53.881639 pydivkit-30.0.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      603 2024-05-13 16:24:53.881312 pydivkit-30.0.0/pydivkit/div/content_text.py
+-rw-r--r--   0        0        0      621 2024-05-13 16:24:53.881312 pydivkit-30.0.0/pydivkit/div/content_url.py
+-rw-r--r--   0        0        0      609 2024-05-13 16:24:53.886818 pydivkit-30.0.0/pydivkit/div/dict_value.py
+-rw-r--r--   0        0        0      856 2024-05-13 16:24:53.887754 pydivkit-30.0.0/pydivkit/div/dict_variable.py
+-rw-r--r--   0        0        0      863 2024-05-13 16:24:53.886231 pydivkit-30.0.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2024-05-13 16:24:53.886891 pydivkit-30.0.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3234 2024-05-13 16:24:53.891681 pydivkit-30.0.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     4138 2024-05-13 16:24:53.894733 pydivkit-30.0.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0     1057 2024-05-13 16:24:53.887839 pydivkit-30.0.0/pydivkit/div/div_action_array_insert_value.py
+-rw-r--r--   0        0        0      863 2024-05-13 16:24:53.887304 pydivkit-30.0.0/pydivkit/div/div_action_array_remove_value.py
+-rw-r--r--   0        0        0      529 2024-05-13 16:24:53.891272 pydivkit-30.0.0/pydivkit/div/div_action_clear_focus.py
+-rw-r--r--   0        0        0      837 2024-05-13 16:24:53.892146 pydivkit-30.0.0/pydivkit/div/div_action_copy_to_clipboard.py
+-rw-r--r--   0        0        0      346 2024-05-13 16:24:53.890730 pydivkit-30.0.0/pydivkit/div/div_action_copy_to_clipboard_content.py
+-rw-r--r--   0        0        0      732 2024-05-13 16:24:53.892529 pydivkit-30.0.0/pydivkit/div/div_action_focus_element.py
+-rw-r--r--   0        0        0      885 2024-05-13 16:24:53.893221 pydivkit-30.0.0/pydivkit/div/div_action_set_variable.py
+-rw-r--r--   0        0        0      759 2024-05-13 16:24:53.891876 pydivkit-30.0.0/pydivkit/div/div_action_typed.py
+-rw-r--r--   0        0        0      321 2024-05-13 16:24:53.895406 pydivkit-30.0.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2024-05-13 16:24:53.895404 pydivkit-30.0.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3016 2024-05-13 16:24:53.900808 pydivkit-30.0.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2024-05-13 16:24:53.896124 pydivkit-30.0.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2024-05-13 16:24:53.897554 pydivkit-30.0.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2024-05-13 16:24:53.895921 pydivkit-30.0.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2024-05-13 16:24:53.896864 pydivkit-30.0.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2024-05-13 16:24:53.898001 pydivkit-30.0.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9648 2024-05-13 16:24:53.909434 pydivkit-30.0.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2024-05-13 16:24:53.899209 pydivkit-30.0.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2024-05-13 16:24:53.900830 pydivkit-30.0.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1734 2024-05-13 16:24:53.901510 pydivkit-30.0.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2024-05-13 16:24:53.903422 pydivkit-30.0.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2024-05-13 16:24:53.902717 pydivkit-30.0.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2024-05-13 16:24:53.901528 pydivkit-30.0.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2024-05-13 16:24:53.904960 pydivkit-30.0.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0     2552 2024-05-13 16:24:53.906384 pydivkit-30.0.0/pydivkit/div/div_collection_item_builder.py
+-rw-r--r--   0        0        0    18163 2024-05-13 16:24:53.933548 pydivkit-30.0.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0      432 2024-05-13 16:24:53.905937 pydivkit-30.0.0/pydivkit/div/div_content_alignment_horizontal.py
+-rw-r--r--   0        0        0      420 2024-05-13 16:24:53.906214 pydivkit-30.0.0/pydivkit/div/div_content_alignment_vertical.py
+-rw-r--r--   0        0        0     1861 2024-05-13 16:24:53.909923 pydivkit-30.0.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2024-05-13 16:24:53.906166 pydivkit-30.0.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1246 2024-05-13 16:24:53.910420 pydivkit-30.0.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10545 2024-05-13 16:24:53.927625 pydivkit-30.0.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2826 2024-05-13 16:24:53.912814 pydivkit-30.0.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2024-05-13 16:24:53.911642 pydivkit-30.0.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2024-05-13 16:24:53.911980 pydivkit-30.0.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     3504 2024-05-13 16:24:53.917469 pydivkit-30.0.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1177 2024-05-13 16:24:53.914358 pydivkit-30.0.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2024-05-13 16:24:53.914367 pydivkit-30.0.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     2081 2024-05-13 16:24:53.918976 pydivkit-30.0.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      804 2024-05-13 16:24:53.918362 pydivkit-30.0.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2024-05-13 16:24:53.921715 pydivkit-30.0.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      340 2024-05-13 16:24:53.917849 pydivkit-30.0.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      564 2024-05-13 16:24:53.919656 pydivkit-30.0.0/pydivkit/div/div_filter_rtl_mirror.py
+-rw-r--r--   0        0        0      686 2024-05-13 16:24:53.923103 pydivkit-30.0.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3267 2024-05-13 16:24:53.928340 pydivkit-30.0.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1070 2024-05-13 16:24:53.925105 pydivkit-30.0.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     2850 2024-05-13 16:24:53.926866 pydivkit-30.0.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      300 2024-05-13 16:24:53.924358 pydivkit-30.0.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    15538 2024-05-13 16:24:53.951008 pydivkit-30.0.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14157 2024-05-13 16:24:53.951488 pydivkit-30.0.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12630 2024-05-13 16:24:53.949692 pydivkit-30.0.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    15881 2024-05-13 16:24:53.956250 pydivkit-30.0.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2530 2024-05-13 16:24:53.936198 pydivkit-30.0.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2024-05-13 16:24:53.931864 pydivkit-30.0.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13813 2024-05-13 16:24:53.955852 pydivkit-30.0.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2024-05-13 16:24:53.934668 pydivkit-30.0.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2024-05-13 16:24:53.937846 pydivkit-30.0.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    16451 2024-05-13 16:24:53.968387 pydivkit-30.0.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      478 2024-05-13 16:24:53.939157 pydivkit-30.0.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      648 2024-05-13 16:24:53.941474 pydivkit-30.0.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2024-05-13 16:24:53.942568 pydivkit-30.0.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1277 2024-05-13 16:24:53.946586 pydivkit-30.0.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1710 2024-05-13 16:24:53.949928 pydivkit-30.0.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1628 2024-05-13 16:24:53.954168 pydivkit-30.0.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2024-05-13 16:24:53.953154 pydivkit-30.0.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2024-05-13 16:24:53.955139 pydivkit-30.0.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2024-05-13 16:24:53.955940 pydivkit-30.0.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2024-05-13 16:24:53.956067 pydivkit-30.0.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2024-05-13 16:24:53.958396 pydivkit-30.0.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2024-05-13 16:24:53.958594 pydivkit-30.0.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0      443 2024-05-13 16:24:53.957785 pydivkit-30.0.0/pydivkit/div/div_page_transformation.py
+-rw-r--r--   0        0        0     3983 2024-05-13 16:24:53.964301 pydivkit-30.0.0/pydivkit/div/div_page_transformation_overlap.py
+-rw-r--r--   0        0        0     3379 2024-05-13 16:24:53.963409 pydivkit-30.0.0/pydivkit/div/div_page_transformation_slide.py
+-rw-r--r--   0        0        0    13945 2024-05-13 16:24:53.980565 pydivkit-30.0.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2024-05-13 16:24:53.959051 pydivkit-30.0.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1928 2024-05-13 16:24:53.965109 pydivkit-30.0.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2024-05-13 16:24:53.963158 pydivkit-30.0.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      820 2024-05-13 16:24:53.963210 pydivkit-30.0.0/pydivkit/div/div_phone_input_mask.py
+-rw-r--r--   0        0        0      357 2024-05-13 16:24:53.962362 pydivkit-30.0.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1116 2024-05-13 16:24:53.968305 pydivkit-30.0.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2024-05-13 16:24:53.967848 pydivkit-30.0.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2024-05-13 16:24:53.966671 pydivkit-30.0.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2024-05-13 16:24:53.969635 pydivkit-30.0.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2024-05-13 16:24:53.966991 pydivkit-30.0.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1136 2024-05-13 16:24:53.970438 pydivkit-30.0.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2024-05-13 16:24:53.970429 pydivkit-30.0.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2024-05-13 16:24:53.972397 pydivkit-30.0.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2024-05-13 16:24:53.972794 pydivkit-30.0.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2024-05-13 16:24:53.974675 pydivkit-30.0.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2024-05-13 16:24:53.975978 pydivkit-30.0.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13636 2024-05-13 16:24:53.996580 pydivkit-30.0.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    12803 2024-05-13 16:24:53.994754 pydivkit-30.0.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2024-05-13 16:24:53.975533 pydivkit-30.0.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2024-05-13 16:24:53.975026 pydivkit-30.0.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2024-05-13 16:24:53.978550 pydivkit-30.0.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0     2699 2024-05-13 16:24:53.980697 pydivkit-30.0.0/pydivkit/div/div_sight_action.py
+-rw-r--r--   0        0        0      424 2024-05-13 16:24:53.978247 pydivkit-30.0.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2024-05-13 16:24:53.979178 pydivkit-30.0.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2024-05-13 16:24:53.984013 pydivkit-30.0.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    16397 2024-05-13 16:24:54.010988 pydivkit-30.0.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2024-05-13 16:24:53.983489 pydivkit-30.0.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13634 2024-05-13 16:24:54.004673 pydivkit-30.0.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2024-05-13 16:24:53.985631 pydivkit-30.0.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2024-05-13 16:24:53.986749 pydivkit-30.0.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    20334 2024-05-13 16:24:54.023084 pydivkit-30.0.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25955 2024-05-13 16:24:54.064063 pydivkit-30.0.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2024-05-13 16:24:53.988227 pydivkit-30.0.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2024-05-13 16:24:53.990461 pydivkit-30.0.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2024-05-13 16:24:53.992481 pydivkit-30.0.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2706 2024-05-13 16:24:53.996669 pydivkit-30.0.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2922 2024-05-13 16:24:54.001842 pydivkit-30.0.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2024-05-13 16:24:53.999027 pydivkit-30.0.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2024-05-13 16:24:54.000775 pydivkit-30.0.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2024-05-13 16:24:54.001841 pydivkit-30.0.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2024-05-13 16:24:54.003879 pydivkit-30.0.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2024-05-13 16:24:54.008426 pydivkit-30.0.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      593 2024-05-13 16:24:54.005151 pydivkit-30.0.0/pydivkit/div/div_typed_value.py
+-rw-r--r--   0        0        0      663 2024-05-13 16:24:54.005538 pydivkit-30.0.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    14416 2024-05-13 16:24:54.031912 pydivkit-30.0.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0      276 2024-05-13 16:24:54.008439 pydivkit-30.0.0/pydivkit/div/div_video_scale.py
+-rw-r--r--   0        0        0     2331 2024-05-13 16:24:54.014105 pydivkit-30.0.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2024-05-13 16:24:54.009838 pydivkit-30.0.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     3490 2024-05-13 16:24:54.015632 pydivkit-30.0.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2024-05-13 16:24:54.016123 pydivkit-30.0.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      611 2024-05-13 16:24:54.014172 pydivkit-30.0.0/pydivkit/div/integer_value.py
+-rw-r--r--   0        0        0      843 2024-05-13 16:24:54.016316 pydivkit-30.0.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      611 2024-05-13 16:24:54.018515 pydivkit-30.0.0/pydivkit/div/number_value.py
+-rw-r--r--   0        0        0      849 2024-05-13 16:24:54.019160 pydivkit-30.0.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      607 2024-05-13 16:24:54.020389 pydivkit-30.0.0/pydivkit/div/string_value.py
+-rw-r--r--   0        0        0      837 2024-05-13 16:24:54.021276 pydivkit-30.0.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      617 2024-05-13 16:24:54.022506 pydivkit-30.0.0/pydivkit/div/url_value.py
+-rw-r--r--   0        0        0      859 2024-05-13 16:24:54.023716 pydivkit-30.0.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2024-05-13 16:24:22.967038 pydivkit-30.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-30.0.0/PKG-INFO
```

### Comparing `pydivkit-29.9.0/README.md` & `pydivkit-30.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/__init__.py` & `pydivkit-30.0.0/pydivkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/core/entities.py` & `pydivkit-30.0.0/pydivkit/core/entities.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/core/fields.py` & `pydivkit-30.0.0/pydivkit/core/fields.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/core/types/union.py` & `pydivkit-30.0.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/__init__.py` & `pydivkit-30.0.0/pydivkit/div/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .div_absolute_edge_insets import DivAbsoluteEdgeInsets
 from .div_accessibility import (
     DivAccessibility, DivAccessibilityMode, DivAccessibilityType,
 )
 from .div_action import DivAction, DivActionMenuItem, DivActionTarget
 from .div_action_array_insert_value import DivActionArrayInsertValue
 from .div_action_array_remove_value import DivActionArrayRemoveValue
+from .div_action_clear_focus import DivActionClearFocus
 from .div_action_copy_to_clipboard import DivActionCopyToClipboard
 from .div_action_copy_to_clipboard_content import (
     DivActionCopyToClipboardContent,
 )
 from .div_action_focus_element import DivActionFocusElement
 from .div_action_set_variable import DivActionSetVariable
 from .div_action_typed import DivActionTyped
@@ -96,14 +97,17 @@
 from .div_input_validator_regex import DivInputValidatorRegex
 from .div_line_style import DivLineStyle
 from .div_linear_gradient import DivLinearGradient
 from .div_match_parent_size import DivMatchParentSize
 from .div_neighbour_page_size import DivNeighbourPageSize
 from .div_nine_patch_background import DivNinePatchBackground
 from .div_page_size import DivPageSize
+from .div_page_transformation import DivPageTransformation
+from .div_page_transformation_overlap import DivPageTransformationOverlap
+from .div_page_transformation_slide import DivPageTransformationSlide
 from .div_pager import DivPager, DivPagerOrientation
 from .div_pager_layout_mode import DivPagerLayoutMode
 from .div_patch import DivPatch, DivPatchChange, DivPatchMode
 from .div_percentage_size import DivPercentageSize
 from .div_phone_input_mask import DivPhoneInputMask
 from .div_pivot import DivPivot
 from .div_pivot_fixed import DivPivotFixed
@@ -185,14 +189,15 @@
 DictVariable.update_forward_refs()
 DivAbsoluteEdgeInsets.update_forward_refs()
 DivAccessibility.update_forward_refs()
 DivAction.update_forward_refs()
 DivActionMenuItem.update_forward_refs()
 DivActionArrayInsertValue.update_forward_refs()
 DivActionArrayRemoveValue.update_forward_refs()
+DivActionClearFocus.update_forward_refs()
 DivActionCopyToClipboard.update_forward_refs()
 DivActionFocusElement.update_forward_refs()
 DivActionSetVariable.update_forward_refs()
 DivAnimation.update_forward_refs()
 DivAppearanceSetTransition.update_forward_refs()
 DivAspect.update_forward_refs()
 DivBase.update_forward_refs()
@@ -238,14 +243,16 @@
 DivInputValidatorExpression.update_forward_refs()
 DivInputValidatorRegex.update_forward_refs()
 DivLinearGradient.update_forward_refs()
 DivMatchParentSize.update_forward_refs()
 DivNeighbourPageSize.update_forward_refs()
 DivNinePatchBackground.update_forward_refs()
 DivPageSize.update_forward_refs()
+DivPageTransformationOverlap.update_forward_refs()
+DivPageTransformationSlide.update_forward_refs()
 DivPager.update_forward_refs()
 DivPatch.update_forward_refs()
 DivPatchChange.update_forward_refs()
 DivPercentageSize.update_forward_refs()
 DivPhoneInputMask.update_forward_refs()
 DivPivotFixed.update_forward_refs()
 DivPivotPercentage.update_forward_refs()
@@ -296,8 +303,8 @@
 NumberValue.update_forward_refs()
 NumberVariable.update_forward_refs()
 StringValue.update_forward_refs()
 StringVariable.update_forward_refs()
 UrlValue.update_forward_refs()
 UrlVariable.update_forward_refs()
 
-__all__ = ("ArrayValue", "ArrayVariable", "BooleanValue", "BooleanVariable", "ColorValue", "ColorVariable", "ContentText", "ContentUrl", "DelimiterStyleOrientation", "DictValue", "DictVariable", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionArrayInsertValue", "DivActionArrayRemoveValue", "DivActionCopyToClipboard", "DivActionCopyToClipboardContent", "DivActionFocusElement", "DivActionMenuItem", "DivActionSetVariable", "DivActionTarget", "DivActionTyped", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivCollectionItemBuilder", "DivCollectionItemBuilderPrototype", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivContentAlignmentHorizontal", "DivContentAlignmentVertical", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFilterRtlMirror", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGalleryScrollbar", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPhoneInputMask", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSightAction", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderRange", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivTypedValue", "DivVariable", "DivVideo", "DivVideoScale", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerValue", "IntegerVariable", "NumberValue", "NumberVariable", "StringValue", "StringVariable", "TabTitleStyleAnimationType", "UrlValue", "UrlVariable")
+__all__ = ("ArrayValue", "ArrayVariable", "BooleanValue", "BooleanVariable", "ColorValue", "ColorVariable", "ContentText", "ContentUrl", "DelimiterStyleOrientation", "DictValue", "DictVariable", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionArrayInsertValue", "DivActionArrayRemoveValue", "DivActionClearFocus", "DivActionCopyToClipboard", "DivActionCopyToClipboardContent", "DivActionFocusElement", "DivActionMenuItem", "DivActionSetVariable", "DivActionTarget", "DivActionTyped", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivCollectionItemBuilder", "DivCollectionItemBuilderPrototype", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivContentAlignmentHorizontal", "DivContentAlignmentVertical", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFilterRtlMirror", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGalleryScrollbar", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPageTransformation", "DivPageTransformationOverlap", "DivPageTransformationSlide", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPhoneInputMask", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSightAction", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderRange", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivTypedValue", "DivVariable", "DivVideo", "DivVideoScale", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerValue", "IntegerVariable", "NumberValue", "NumberVariable", "StringValue", "StringVariable", "TabTitleStyleAnimationType", "UrlValue", "UrlVariable")
```

### Comparing `pydivkit-29.9.0/pydivkit/div/array_value.py` & `pydivkit-30.0.0/pydivkit/div/array_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/array_variable.py` & `pydivkit-30.0.0/pydivkit/div/array_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/boolean_value.py` & `pydivkit-30.0.0/pydivkit/div/boolean_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/boolean_variable.py` & `pydivkit-30.0.0/pydivkit/div/boolean_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/color_value.py` & `pydivkit-30.0.0/pydivkit/div/color_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/color_variable.py` & `pydivkit-30.0.0/pydivkit/div/color_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/content_text.py` & `pydivkit-30.0.0/pydivkit/div/content_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/content_url.py` & `pydivkit-30.0.0/pydivkit/div/content_url.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/dict_value.py` & `pydivkit-30.0.0/pydivkit/div/dict_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/dict_variable.py` & `pydivkit-30.0.0/pydivkit/div/dict_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div.py` & `pydivkit-30.0.0/pydivkit/div/div.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-30.0.0/pydivkit/div/div_absolute_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_accessibility.py` & `pydivkit-30.0.0/pydivkit/div/div_accessibility.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action.py` & `pydivkit-30.0.0/pydivkit/div/div_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
             typed=typed,
             url=url,
             **kwargs,
         )
 
     download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
         description=(
-            "Callbacks that are called after "
-            "[dataloading](../../interaction.dita#loading-data)."
+            "Callbacks that are called after [data "
+            "loading](../../interaction#loading-data)."
         ),
     )
     is_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "The parameter disables the action. Disabled actions stop "
             "listening to theirassociated event (clicks, changes in "
             "visibility, and so on)."
@@ -77,16 +77,15 @@
     )
     typed: typing.Optional[div_action_typed.DivActionTyped] = Field(
     )
     url: typing.Optional[typing.Union[Expr, str]] = Field(
         format="uri", 
         description=(
             "URL. Possible values: `url` or `div-action://`. To learn "
-            "more, see [Interactionwith "
-            "elements](../../interaction.dita)."
+            "more, see [Interactionwith elements](../../interaction)."
         ),
     )
 
 
 class DivActionTarget(str, enum.Enum):
     SELF = "_self"
     BLANK = "_blank"
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action_array_insert_value.py` & `pydivkit-30.0.0/pydivkit/div/div_action_array_insert_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action_array_remove_value.py` & `pydivkit-30.0.0/pydivkit/div/div_action_array_remove_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action_copy_to_clipboard.py` & `pydivkit-30.0.0/pydivkit/div/div_action_copy_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action_focus_element.py` & `pydivkit-30.0.0/pydivkit/div/div_action_focus_element.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action_set_variable.py` & `pydivkit-30.0.0/pydivkit/div/div_action_set_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_action_typed.py` & `pydivkit-30.0.0/pydivkit/div/div_action_typed.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 import typing
 from typing import Union
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_action_array_insert_value, div_action_array_remove_value,
-    div_action_copy_to_clipboard, div_action_focus_element,
-    div_action_set_variable,
+    div_action_clear_focus, div_action_copy_to_clipboard,
+    div_action_focus_element, div_action_set_variable,
 )
 
 
 DivActionTyped = Union[
     div_action_array_insert_value.DivActionArrayInsertValue,
     div_action_array_remove_value.DivActionArrayRemoveValue,
     div_action_set_variable.DivActionSetVariable,
     div_action_focus_element.DivActionFocusElement,
+    div_action_clear_focus.DivActionClearFocus,
     div_action_copy_to_clipboard.DivActionCopyToClipboard,
 ]
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_animation.py` & `pydivkit-30.0.0/pydivkit/div/div_animation.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_appearance_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_appearance_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_aspect.py` & `pydivkit-30.0.0/pydivkit/div/div_aspect.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_background.py` & `pydivkit-30.0.0/pydivkit/div/div_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_base.py` & `pydivkit-30.0.0/pydivkit/div/div_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,27 +114,26 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -177,16 +176,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_blur.py` & `pydivkit-30.0.0/pydivkit/div/div_blur.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_border.py` & `pydivkit-30.0.0/pydivkit/div/div_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_change_set_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_change_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_circle_shape.py` & `pydivkit-30.0.0/pydivkit/div/div_circle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_collection_item_builder.py` & `pydivkit-30.0.0/pydivkit/div/div_collection_item_builder.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_container.py` & `pydivkit-30.0.0/pydivkit/div/div_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,27 +202,26 @@
     doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description="Action when double-clicking on an element.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -313,16 +312,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_corners_radius.py` & `pydivkit-30.0.0/pydivkit/div/div_corners_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_currency_input_mask.py` & `pydivkit-30.0.0/pydivkit/div/div_currency_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_custom.py` & `pydivkit-30.0.0/pydivkit/div/div_custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,27 +131,26 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -197,16 +196,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_data.py` & `pydivkit-30.0.0/pydivkit/div/div_data.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_default_indicator_item_placement.py` & `pydivkit-30.0.0/pydivkit/div/div_default_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_dimension.py` & `pydivkit-30.0.0/pydivkit/div/div_dimension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_disappear_action.py` & `pydivkit-30.0.0/pydivkit/div/div_disappear_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         description=(
             "Time in milliseconds during which an element must be "
             "outside the visible area totrigger `disappear-action`."
         ),
     )
     download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
         description=(
-            "Callbacks that are called after "
-            "[dataloading](../../interaction.dita#loading-data)."
+            "Callbacks that are called after [data "
+            "loading](../../interaction#loading-data)."
         ),
     )
     is_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "The parameter disables the action. Disabled actions stop "
             "listening to theirassociated event (clicks, changes in "
             "visibility, and so on)."
@@ -79,16 +79,15 @@
     )
     typed: typing.Optional[div_action_typed.DivActionTyped] = Field(
     )
     url: typing.Optional[typing.Union[Expr, str]] = Field(
         format="uri", 
         description=(
             "URL. Possible values: `url` or `div-action://`. To learn "
-            "more, see [Interactionwith "
-            "elements](../../interaction.dita)."
+            "more, see [Interactionwith elements](../../interaction)."
         ),
     )
     visibility_percentage: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Percentage of the visible part of an element that triggers "
             "`disappear-action`."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_download_callbacks.py` & `pydivkit-30.0.0/pydivkit/div/div_download_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_action
 
 
-# Callbacks that are called after [data
-# loading](../../interaction.dita#loading-data).
+# Callbacks that are called after [data loading](../../interaction#loading-data).
 class DivDownloadCallbacks(BaseDiv):
 
     def __init__(
         self, *,
         on_fail_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         on_success_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         **kwargs: typing.Any,
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_edge_insets.py` & `pydivkit-30.0.0/pydivkit/div/div_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_extension.py` & `pydivkit-30.0.0/pydivkit/div/div_extension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_fade_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_fade_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_filter_rtl_mirror.py` & `pydivkit-30.0.0/pydivkit/div/div_filter_rtl_mirror.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_fixed_count.py` & `pydivkit-30.0.0/pydivkit/div/div_fixed_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_fixed_length_input_mask.py` & `pydivkit-30.0.0/pydivkit/div/div_fixed_length_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_fixed_size.py` & `pydivkit-30.0.0/pydivkit/div/div_pivot_fixed.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,38 +7,37 @@
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_size_unit
 
 
-# Fixed size of an element.
-class DivFixedSize(BaseDiv):
+# Fixed coordinates of the rotation axis.
+class DivPivotFixed(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "fixed",
+        type: str = "pivot-fixed",
         unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         value: typing.Optional[typing.Union[Expr, int]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             unit=unit,
             value=value,
             **kwargs,
         )
 
-    type: str = Field(default="fixed")
+    type: str = Field(default="pivot-fixed")
     unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
-            "Unit of measurement. To learn more about units of size "
-            "measurement, see [Layoutinside the "
-            "card](../../layout.dita)."
+            "Measurement unit. To learn more about units of size "
+            "measurement, see [Layoutinside the card](../../layout)."
         ),
     )
-    value: typing.Union[Expr, int] = Field(
-        description="Element size.",
+    value: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Coordinate value.",
     )
 
 
-DivFixedSize.update_forward_refs()
+DivPivotFixed.update_forward_refs()
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_focus.py` & `pydivkit-30.0.0/pydivkit/div/div_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_gallery.py` & `pydivkit-30.0.0/pydivkit/div/div_gallery.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_disappear_action, div_edge_insets,
-    div_extension, div_focus, div_size, div_tooltip, div_transform,
-    div_transition_trigger, div_visibility, div_visibility_action,
+    div_border, div_change_transition, div_collection_item_builder,
+    div_disappear_action, div_edge_insets, div_extension, div_focus, div_size,
+    div_tooltip, div_transform, div_transition_trigger, div_visibility,
+    div_visibility_action,
 )
 
 
 # Gallery. It contains a horizontal or vertical set of cards that can be scrolled.
 class DivGallery(BaseDiv):
 
     def __init__(
@@ -35,14 +36,15 @@
         cross_spacing: typing.Optional[typing.Union[Expr, int]] = None,
         default_item: typing.Optional[typing.Union[Expr, int]] = None,
         disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
         extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
         id: typing.Optional[typing.Union[Expr, str]] = None,
+        item_builder: typing.Optional[div_collection_item_builder.DivCollectionItemBuilder] = None,
         item_spacing: typing.Optional[typing.Union[Expr, int]] = None,
         items: typing.Optional[typing.Sequence[div.Div]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         orientation: typing.Optional[typing.Union[Expr, DivGalleryOrientation]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         restrict_parent_scroll: typing.Optional[typing.Union[Expr, bool]] = None,
         row_span: typing.Optional[typing.Union[Expr, int]] = None,
@@ -75,14 +77,15 @@
             cross_spacing=cross_spacing,
             default_item=default_item,
             disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
+            item_builder=item_builder,
             item_spacing=item_spacing,
             items=items,
             margins=margins,
             orientation=orientation,
             paddings=paddings,
             restrict_parent_scroll=restrict_parent_scroll,
             row_span=row_span,
@@ -166,49 +169,54 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
+    item_builder: typing.Optional[div_collection_item_builder.DivCollectionItemBuilder] = Field(
+        description=(
+            "Sets collection elements dynamically using `data` and "
+            "`prototypes`."
+        ),
+    )
     item_spacing: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Spacing between elements.",
     )
     items: typing.Optional[typing.Sequence[div.Div]] = Field(
         description=(
             "Gallery elements. Scrolling to elements can be "
             "implementedusing:`div-action://set_current_item?id=&item=` "
             "— scrolling to the element withan ordinal number `item` "
             "inside an element, with the "
             "specified`id`;`div-action://set_next_item?id=[&overflow={cl"
-            "amp|ring}]` — scrolling to thenext element inside an "
+            "amp\|ring}]` — scrolling to thenext element inside an "
             "element, with the "
             "specified`id`;`div-action://set_previous_item?id=[&overflow"
-            "={clamp|ring}]` — scrolling tothe previous element inside "
+            "={clamp\|ring}]` — scrolling tothe previous element inside "
             "an element, with the specified `id`.</p><p>Theoptional "
             "`overflow` parameter is used to set navigation when the "
             "first or lastelement is reached:`clamp` — transition will "
             "stop at the border element;`ring` —go to the beginning or "
             "end, depending on the current element.</p><p>By "
             "default,`clamp`."
         ),
@@ -276,16 +284,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_gif_image.py` & `pydivkit-30.0.0/pydivkit/div/div_gif_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,31 +175,30 @@
     doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description="Action when double-clicking on an element.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     gif_url: typing.Union[Expr, str] = Field(
         format="uri", 
         description="Direct URL to a GIF image.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -269,16 +268,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_grid.py` & `pydivkit-30.0.0/pydivkit/div/div_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,27 +164,26 @@
     doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description="Action when double-clicking on an element.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -236,16 +235,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_image.py` & `pydivkit-30.0.0/pydivkit/div/div_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,30 +189,29 @@
     doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description="Action when double-clicking on an element.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     filters: typing.Optional[typing.Sequence[div_filter.DivFilter]] = Field(
         description="Image filters.",
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     high_priority_preview_show: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "It sets the priority of displaying the preview — the "
             "preview is decoded in themain stream and displayed as the "
             "first frame. Use the parameter carefully — itwill worsen "
@@ -302,16 +301,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_image_background.py` & `pydivkit-30.0.0/pydivkit/div/div_image_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_indicator.py` & `pydivkit-30.0.0/pydivkit/div/div_indicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,27 +157,26 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -256,16 +255,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_infinity_count.py` & `pydivkit-30.0.0/pydivkit/div/div_infinity_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_input.py` & `pydivkit-30.0.0/pydivkit/div/div_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         height: typing.Optional[div_size.DivSize] = None,
         highlight_color: typing.Optional[typing.Union[Expr, str]] = None,
         hint_color: typing.Optional[typing.Union[Expr, str]] = None,
         hint_text: typing.Optional[typing.Union[Expr, str]] = None,
         id: typing.Optional[typing.Union[Expr, str]] = None,
+        is_enabled: typing.Optional[typing.Union[Expr, bool]] = None,
         keyboard_type: typing.Optional[typing.Union[Expr, DivInputKeyboardType]] = None,
         letter_spacing: typing.Optional[typing.Union[Expr, float]] = None,
         line_height: typing.Optional[typing.Union[Expr, int]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         mask: typing.Optional[div_input_mask.DivInputMask] = None,
         max_visible_lines: typing.Optional[typing.Union[Expr, int]] = None,
         native_interface: typing.Optional[DivInputNativeInterface] = None,
@@ -88,14 +89,15 @@
             font_size_unit=font_size_unit,
             font_weight=font_weight,
             height=height,
             highlight_color=highlight_color,
             hint_color=hint_color,
             hint_text=hint_text,
             id=id,
+            is_enabled=is_enabled,
             keyboard_type=keyboard_type,
             letter_spacing=letter_spacing,
             line_height=line_height,
             margins=margins,
             mask=mask,
             max_visible_lines=max_visible_lines,
             native_interface=native_interface,
@@ -157,15 +159,15 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     font_family: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
@@ -188,16 +190,15 @@
         description="Style.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     highlight_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description=(
             "Text highlight color. If the value isn\'t set, the color "
             "set in the client will beused instead."
@@ -212,14 +213,17 @@
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
+    is_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description="Indicates if the text editing is enabled.",
+    )
     keyboard_type: typing.Optional[typing.Union[Expr, DivInputKeyboardType]] = Field(
         description="Keyboard type.",
     )
     letter_spacing: typing.Optional[typing.Union[Expr, float]] = Field(
         description="Spacing between characters.",
     )
     line_height: typing.Optional[typing.Union[Expr, int]] = Field(
@@ -293,16 +297,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_input_mask_base.py` & `pydivkit-30.0.0/pydivkit/div/div_input_mask_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_input_validator_base.py` & `pydivkit-30.0.0/pydivkit/div/div_input_validator_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_input_validator_expression.py` & `pydivkit-30.0.0/pydivkit/div/div_input_validator_expression.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 
-# [Calculated expression](../../expressions.dita) validator.
+# [Calculated expression](../../expressions) validator.
 class DivInputValidatorExpression(BaseDiv):
 
     def __init__(
         self, *,
         type: str = "expression",
         allow_empty: typing.Optional[typing.Union[Expr, bool]] = None,
         condition: typing.Optional[typing.Union[Expr, bool]] = None,
@@ -32,16 +32,16 @@
 
     type: str = Field(default="expression")
     allow_empty: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Determines whether the empty field value is valid.",
     )
     condition: typing.Union[Expr, bool] = Field(
         description=(
-            "[Calculated expression](../../expressions.dita) used as a "
-            "value validitycondition."
+            "[Calculated expression](../../expressions) used as a value "
+            "validity condition."
         ),
     )
     label_id: typing.Union[Expr, str] = Field(
         description=(
             "ID of the text element containing the error message. The "
             "message will also beused for providing access."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_input_validator_regex.py` & `pydivkit-30.0.0/pydivkit/div/div_input_validator_regex.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_linear_gradient.py` & `pydivkit-30.0.0/pydivkit/div/div_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_match_parent_size.py` & `pydivkit-30.0.0/pydivkit/div/div_match_parent_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-30.0.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_nine_patch_background.py` & `pydivkit-30.0.0/pydivkit/div/div_nine_patch_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_page_size.py` & `pydivkit-30.0.0/pydivkit/div/div_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_pager.py` & `pydivkit-30.0.0/pydivkit/div/div_pager.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_disappear_action, div_edge_insets,
-    div_extension, div_fixed_size, div_focus, div_pager_layout_mode, div_size,
+    div_border, div_change_transition, div_collection_item_builder,
+    div_disappear_action, div_edge_insets, div_extension, div_fixed_size,
+    div_focus, div_page_transformation, div_pager_layout_mode, div_size,
     div_tooltip, div_transform, div_transition_trigger, div_visibility,
     div_visibility_action,
 )
 
 
 # Pager. It contains a horizontal set of cards that can be scrolled page by page.
 # It shows the main page and the beginning of the next one.
@@ -35,20 +36,22 @@
         default_item: typing.Optional[typing.Union[Expr, int]] = None,
         disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
         extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
         id: typing.Optional[typing.Union[Expr, str]] = None,
         infinite_scroll: typing.Optional[typing.Union[Expr, bool]] = None,
+        item_builder: typing.Optional[div_collection_item_builder.DivCollectionItemBuilder] = None,
         item_spacing: typing.Optional[div_fixed_size.DivFixedSize] = None,
         items: typing.Optional[typing.Sequence[div.Div]] = None,
         layout_mode: typing.Optional[div_pager_layout_mode.DivPagerLayoutMode] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         orientation: typing.Optional[typing.Union[Expr, DivPagerOrientation]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
+        page_transformation: typing.Optional[div_page_transformation.DivPageTransformation] = None,
         restrict_parent_scroll: typing.Optional[typing.Union[Expr, bool]] = None,
         row_span: typing.Optional[typing.Union[Expr, int]] = None,
         selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
@@ -72,20 +75,22 @@
             default_item=default_item,
             disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
             infinite_scroll=infinite_scroll,
+            item_builder=item_builder,
             item_spacing=item_spacing,
             items=items,
             layout_mode=layout_mode,
             margins=margins,
             orientation=orientation,
             paddings=paddings,
+            page_transformation=page_transformation,
             restrict_parent_scroll=restrict_parent_scroll,
             row_span=row_span,
             selected_actions=selected_actions,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
@@ -140,60 +145,65 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
     infinite_scroll: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "Enables infinite scrolling of cards. Scrolling is looped: "
             "after the last card isdisplayed, it starts over again."
         ),
     )
+    item_builder: typing.Optional[div_collection_item_builder.DivCollectionItemBuilder] = Field(
+        description=(
+            "Sets collection elements dynamically using `data` and "
+            "`prototypes`."
+        ),
+    )
     item_spacing: typing.Optional[div_fixed_size.DivFixedSize] = Field(
         description="Spacing between elements.",
     )
     items: typing.Optional[typing.Sequence[div.Div]] = Field(
         description=(
             "Pager elements. Page-by-page transition options can be "
             "implementedusing:`div-action://set_current_item?id=&item=` "
             "— set the current page with anordinal number `item` inside "
             "an element, with the "
             "specified`id`;`div-action://set_next_item?id=[&overflow={cl"
-            "amp|ring}]` — go to the nextpage inside an element, with "
+            "amp\|ring}]` — go to the nextpage inside an element, with "
             "the "
             "specified`id`;`div-action://set_previous_item?id=[&overflow"
-            "={clamp|ring}]` — go to theprevious page inside an element, "
-            "with the specified `id`.</p><p>The optional`overflow` "
-            "parameter is used to set navigation when the first or last "
-            "element isreached:`clamp` — transition will stop at the "
-            "border element;`ring` — go to thebeginning or end, "
-            "depending on the current element.</p><p>By default, "
+            "={clamp\|ring}]` — go to theprevious page inside an "
+            "element, with the specified `id`.</p><p>The "
+            "optional`overflow` parameter is used to set navigation when "
+            "the first or last element isreached:`clamp` — transition "
+            "will stop at the border element;`ring` — go to thebeginning "
+            "or end, depending on the current element.</p><p>By default, "
             "`clamp`."
         ),
     )
     layout_mode: div_pager_layout_mode.DivPagerLayoutMode = Field(
         description=(
             "Type of calculation of the main page width:`fixed` — from "
             "the fixed width of thenext page "
@@ -206,14 +216,17 @@
     )
     orientation: typing.Optional[typing.Union[Expr, DivPagerOrientation]] = Field(
         description="Pager orientation.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
+    page_transformation: typing.Optional[div_page_transformation.DivPageTransformation] = Field(
+        description="Page transformation during movement.",
+    )
     restrict_parent_scroll: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "If the parameter is enabled, the pager won\'t transmit the "
             "scroll gesture to theparent element."
         ),
     )
     row_span: typing.Optional[typing.Union[Expr, int]] = Field(
@@ -248,16 +261,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_patch.py` & `pydivkit-30.0.0/pydivkit/div/div_patch.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_percentage_size.py` & `pydivkit-30.0.0/pydivkit/div/div_percentage_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_phone_input_mask.py` & `pydivkit-30.0.0/pydivkit/div/div_phone_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_pivot_fixed.py` & `pydivkit-30.0.0/pydivkit/div/div_fixed_size.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,38 +7,37 @@
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_size_unit
 
 
-# Fixed coordinates of the rotation axis.
-class DivPivotFixed(BaseDiv):
+# Fixed size of an element.
+class DivFixedSize(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "pivot-fixed",
+        type: str = "fixed",
         unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         value: typing.Optional[typing.Union[Expr, int]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             unit=unit,
             value=value,
             **kwargs,
         )
 
-    type: str = Field(default="pivot-fixed")
+    type: str = Field(default="fixed")
     unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
-            "Measurement unit. To learn more about units of size "
-            "measurement, see [Layoutinside the "
-            "card](../../layout.dita)."
+            "Unit of measurement. To learn more about units of size "
+            "measurement, see [Layoutinside the card](../../layout)."
         ),
     )
-    value: typing.Optional[typing.Union[Expr, int]] = Field(
-        description="Coordinate value.",
+    value: typing.Union[Expr, int] = Field(
+        description="Element size.",
     )
 
 
-DivPivotFixed.update_forward_refs()
+DivFixedSize.update_forward_refs()
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_pivot_percentage.py` & `pydivkit-30.0.0/pydivkit/div/div_pivot_percentage.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_point.py` & `pydivkit-30.0.0/pydivkit/div/div_point.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_radial_gradient.py` & `pydivkit-30.0.0/pydivkit/div/div_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-30.0.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
             **kwargs,
         )
 
     type: str = Field(default="fixed")
     unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
             "Unit of measurement. To learn more about units of size "
-            "measurement, see [Layoutinside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layoutinside the card](../../layout)."
         ),
     )
     value: typing.Union[Expr, int] = Field(
         description="Coordinate value.",
     )
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-30.0.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_radius.py` & `pydivkit-30.0.0/pydivkit/div/div_radial_gradient_relative_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_rounded_rectangle_shape.py` & `pydivkit-30.0.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_scale_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_scale_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_select.py` & `pydivkit-30.0.0/pydivkit/div/div_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     font_family: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
@@ -172,16 +172,15 @@
         description="Style.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     hint_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Hint color.",
     )
     hint_text: typing.Optional[typing.Union[Expr, str]] = Field(
@@ -247,16 +246,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_separator.py` & `pydivkit-30.0.0/pydivkit/div/div_separator.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,27 +152,26 @@
     doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description="Action when double-clicking on an element.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -221,16 +220,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_shadow.py` & `pydivkit-30.0.0/pydivkit/div/div_shadow.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_shape_drawable.py` & `pydivkit-30.0.0/pydivkit/div/div_shape_drawable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_sight_action.py` & `pydivkit-30.0.0/pydivkit/div/div_sight_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
             typed=typed,
             url=url,
             **kwargs,
         )
 
     download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
         description=(
-            "Callbacks that are called after "
-            "[dataloading](../../interaction.dita#loading-data)."
+            "Callbacks that are called after [data "
+            "loading](../../interaction#loading-data)."
         ),
     )
     is_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "The parameter disables the action. Disabled actions stop "
             "listening to theirassociated event (clicks, changes in "
             "visibility, and so on)."
@@ -68,14 +68,13 @@
     )
     typed: typing.Optional[div_action_typed.DivActionTyped] = Field(
     )
     url: typing.Optional[typing.Union[Expr, str]] = Field(
         format="uri", 
         description=(
             "URL. Possible values: `url` or `div-action://`. To learn "
-            "more, see [Interactionwith "
-            "elements](../../interaction.dita)."
+            "more, see [Interactionwith elements](../../interaction)."
         ),
     )
 
 
 DivSightAction.update_forward_refs()
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_slide_transition.py` & `pydivkit-30.0.0/pydivkit/div/div_slide_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_slider.py` & `pydivkit-30.0.0/pydivkit/div/div_slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,27 +147,26 @@
     disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         description="Actions when an element disappears from the screen.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -257,16 +256,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_solid_background.py` & `pydivkit-30.0.0/pydivkit/div/div_solid_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_state.py` & `pydivkit-30.0.0/pydivkit/div/div_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,27 +142,26 @@
             "unique at onehierarchy level. @deprecated"
         ),
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -194,15 +193,15 @@
         ),
     )
     states: typing.Sequence[DivStateState] = Field(
         min_items=1, 
         description=(
             "States. Each element can have a few states with a different "
             "layout. Transitionbetween states is performed using "
-            "[special scheme](../../interaction.dita) of "
+            "[special scheme](../../interaction) of "
             "the[action](div-action.md) element."
         ),
     )
     tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
@@ -228,16 +227,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_stretch_indicator_item_placement.py` & `pydivkit-30.0.0/pydivkit/div/div_stretch_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_stroke.py` & `pydivkit-30.0.0/pydivkit/div/div_stroke.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_tabs.py` & `pydivkit-30.0.0/pydivkit/div/div_tabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     div_edge_insets, div_extension, div_focus, div_font_weight, div_size,
     div_size_unit, div_tooltip, div_transform, div_transition_trigger,
     div_visibility, div_visibility_action,
 )
 
 
 # Tabs. Height of the first tab is determined by its contents, and height of the
-# remaining [depends on the platform](../../location.dita#tabs).
+# remaining [depends on the platform](../../location#tabs).
 class DivTabs(BaseDiv):
 
     def __init__(
         self, *,
         type: str = "tabs",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
         alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
@@ -146,30 +146,29 @@
             "browser, the value isalways `true`."
         ),
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     has_separator: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="A separating line between tabs and contents.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -178,17 +177,18 @@
         min_items=1, 
         description=(
             "Tabs. Transition between tabs can be "
             "implementedusing:`div-action://set_current_item?id=&item=` "
             "— set the current tab with anordinal number `item` inside "
             "an element, with the "
             "specified`id`;`div-action://set_next_item?id=[&overflow={cl"
-            "amp|ring}]` — go to the nexttab inside an element, with the "
+            "amp\|ring}]` — go to the nexttab inside an element, with "
+            "the "
             "specified`id`;`div-action://set_previous_item?id=[&overflow"
-            "={clamp|ring}]` — go to theprevious tab inside an element, "
+            "={clamp\|ring}]` — go to theprevious tab inside an element, "
             "with the specified `id`.</p><p>The optional`overflow` "
             "parameter is used to set navigation when the first or last "
             "element isreached:`clamp` — transition will stop at the "
             "border element;`ring` — go to thebeginning or end, "
             "depending on the current element.</p><p>By default, "
             "`clamp`."
         ),
@@ -259,16 +259,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_text.py` & `pydivkit-30.0.0/pydivkit/div/div_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             "exceeds the limit on thenumber of lines."
         ),
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     focused_text_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
@@ -233,16 +233,15 @@
         description="Style.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -343,16 +342,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_text_range_border.py` & `pydivkit-30.0.0/pydivkit/div/div_text_range_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_timer.py` & `pydivkit-30.0.0/pydivkit/div/div_timer.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_tooltip.py` & `pydivkit-30.0.0/pydivkit/div/div_tooltip.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_transform.py` & `pydivkit-30.0.0/pydivkit/div/div_transform.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_transition_base.py` & `pydivkit-30.0.0/pydivkit/div/div_transition_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_trigger.py` & `pydivkit-30.0.0/pydivkit/div/div_trigger.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_typed_value.py` & `pydivkit-30.0.0/pydivkit/div/div_typed_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_variable.py` & `pydivkit-30.0.0/pydivkit/div/div_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_video.py` & `pydivkit-30.0.0/pydivkit/div/div_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     end_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description="Actions performed after the video ends.",
     )
     extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
-            "[DivExtension](../../extensions.dita)."
+            "[DivExtension](../../extensions)."
         ),
     )
     fatal_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         description=(
             "Actions performed when playback can\'t be continued due to "
             "a player error."
         ),
@@ -190,16 +190,15 @@
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
-            "measurement, see [Layout inside the "
-            "card](../../layout.dita)."
+            "measurement, see [Layout inside the card](../../layout)."
         ),
     )
     id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
@@ -275,16 +274,16 @@
         ),
     )
     transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Appearance animation. It is played when an element with a "
             "new ID appears. Tolearn more about the concept of "
             "transitions, see "
-            "[Animatedtransitions](../../interaction.dita#animation/tran"
-            "sition-animation)."
+            "[Animatedtransitions](../../interaction#animation/transitio"
+            "n-animation)."
         ),
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_video_source.py` & `pydivkit-30.0.0/pydivkit/div/div_video_source.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/div_visibility_action.py` & `pydivkit-30.0.0/pydivkit/div/div_visibility_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,16 +40,16 @@
             visibility_duration=visibility_duration,
             visibility_percentage=visibility_percentage,
             **kwargs,
         )
 
     download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
         description=(
-            "Callbacks that are called after "
-            "[dataloading](../../interaction.dita#loading-data)."
+            "Callbacks that are called after [data "
+            "loading](../../interaction#loading-data)."
         ),
     )
     is_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "The parameter disables the action. Disabled actions stop "
             "listening to theirassociated event (clicks, changes in "
             "visibility, and so on)."
@@ -73,16 +73,15 @@
     )
     typed: typing.Optional[div_action_typed.DivActionTyped] = Field(
     )
     url: typing.Optional[typing.Union[Expr, str]] = Field(
         format="uri", 
         description=(
             "URL. Possible values: `url` or `div-action://`. To learn "
-            "more, see [Interactionwith "
-            "elements](../../interaction.dita)."
+            "more, see [Interactionwith elements](../../interaction)."
         ),
     )
     visibility_duration: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Time in milliseconds during which an element must be "
             "visible to trigger`visibility-action`."
         ),
```

### Comparing `pydivkit-29.9.0/pydivkit/div/div_wrap_content_size.py` & `pydivkit-30.0.0/pydivkit/div/div_wrap_content_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/integer_value.py` & `pydivkit-30.0.0/pydivkit/div/integer_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/integer_variable.py` & `pydivkit-30.0.0/pydivkit/div/integer_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/number_value.py` & `pydivkit-30.0.0/pydivkit/div/number_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/number_variable.py` & `pydivkit-30.0.0/pydivkit/div/number_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/string_value.py` & `pydivkit-30.0.0/pydivkit/div/string_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/string_variable.py` & `pydivkit-30.0.0/pydivkit/div/string_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/url_value.py` & `pydivkit-30.0.0/pydivkit/div/url_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pydivkit/div/url_variable.py` & `pydivkit-30.0.0/pydivkit/div/url_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.9.0/pyproject.toml` & `pydivkit-30.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydivkit"
-version = "29.9.0"
+version = "30.0.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
     "Pavel Mosein <p-mosein@yandex-team.ru>",
```

### Comparing `pydivkit-29.9.0/PKG-INFO` & `pydivkit-30.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivkit
-Version: 29.9.0
+Version: 30.0.0
 Summary: DivKit python library
 Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
 Keywords: divkit,sdk
 Author: Vladislav Bakaev
 Author-email: bakaev-vlad@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

