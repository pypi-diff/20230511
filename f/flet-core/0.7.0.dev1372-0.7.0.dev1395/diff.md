# Comparing `tmp/flet_core-0.7.0.dev1372.tar.gz` & `tmp/flet_core-0.7.0.dev1395.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_core-0.7.0.dev1372.tar", max compression
+gzip compressed data, was "flet_core-0.7.0.dev1395.tar", max compression
```

## Comparing `flet_core-0.7.0.dev1372.tar` & `flet_core-0.7.0.dev1395.tar`

### file list

```diff
@@ -1,131 +1,132 @@
--rw-r--r--   0        0        0      189 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/README.md
--rw-r--r--   0        0        0      723 2023-05-03 03:54:18.850201 flet_core-0.7.0.dev1372/pyproject.toml
--rw-r--r--   0        0        0     6335 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/__init__.py
--rw-r--r--   0        0        0     6774 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/alignment.py
--rw-r--r--   0        0        0     7226 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     2806 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/animation.py
--rw-r--r--   0        0        0     5403 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7301 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/audio.py
--rw-r--r--   0        0        0     5446 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     2826 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2202 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/buttons.py
--rw-r--r--   0        0        0     3044 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/callable_control.py
--rw-r--r--   0        0        0      514 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0     2903 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4629 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1639 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1361 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      837 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1862 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1907 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3486 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1772 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2361 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1963 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     5639 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/card.py
--rw-r--r--   0        0        0     9855 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2061 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6837 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1949 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2924 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11228 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     8258 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5496 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5888 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3824 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0     7122 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/checkbox.py
--rw-r--r--   0        0        0     6739 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3085 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/client_storage.py
--rw-r--r--   0        0        0     1002 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/clipboard.py
--rw-r--r--   0        0        0    10627 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/colors.py
--rw-r--r--   0        0        0     7305 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/column.py
--rw-r--r--   0        0        0     1132 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/connection.py
--rw-r--r--   0        0        0     6848 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    13883 2023-05-03 03:53:46.125657 flet_core-0.7.0.dev1372/src/flet_core/container.py
--rw-r--r--   0        0        0    14162 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/control_event.py
--rw-r--r--   0        0        0    20740 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/datatable.py
--rw-r--r--   0        0        0     2263 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/divider.py
--rw-r--r--   0        0        0     6270 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6063 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/draggable.py
--rw-r--r--   0        0        0     9121 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/dropdown.py
--rw-r--r--   0        0        0     8565 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     2170 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/event.py
--rw-r--r--   0        0        0     1839 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9777 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2638 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     2772 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     2542 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/flet_app.py
--rw-r--r--   0        0        0     7055 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    13925 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    27988 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1531 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/gradients.py
--rw-r--r--   0        0        0     6301 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2134 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3375 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/icon.py
--rw-r--r--   0        0        0     8199 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362652 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/icons.py
--rw-r--r--   0        0        0     6530 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/inline_span.py
--rw-r--r--   0        0        0     8304 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     6206 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/list_view.py
--rw-r--r--   0        0        0     8644 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      223 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/locks.py
--rw-r--r--   0        0        0      583 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/margin.py
--rw-r--r--   0        0        0     6073 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5125 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     8322 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0    11986 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     7250 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/padding.py
--rw-r--r--   0        0        0    52427 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/page.py
--rw-r--r--   0        0        0     2674 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/painting.py
--rw-r--r--   0        0        0     4355 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0     6756 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     4237 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     4435 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4088 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/protocol.py
--rw-r--r--   0        0        0     3419 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/querystring.py
--rw-r--r--   0        0        0     5731 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/radio.py
--rw-r--r--   0        0        0     2389 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/radio_group.py
--rw-r--r--   0        0        0      291 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/ref.py
--rw-r--r--   0        0        0     6354 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     7289 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/row.py
--rw-r--r--   0        0        0     1637 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/semantics.py
--rw-r--r--   0        0        0      576 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5318 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2919 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0     7326 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/slider.py
--rw-r--r--   0        0        0     3971 2023-05-03 03:53:46.129657 flet_core-0.7.0.dev1372/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     4833 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/stack.py
--rw-r--r--   0        0        0     8092 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/switch.py
--rw-r--r--   0        0        0     6776 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10512 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/text.py
--rw-r--r--   0        0        0     7223 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/text_button.py
--rw-r--r--   0        0        0     3092 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1260 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/text_style.py
--rw-r--r--   0        0        0    15388 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/textfield.py
--rw-r--r--   0        0        0     1482 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/theme.py
--rw-r--r--   0        0        0     8362 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/transform.py
--rw-r--r--   0        0        0     2753 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     5186 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/types.py
--rw-r--r--   0        0        0      684 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/user_control.py
--rw-r--r--   0        0        0      409 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/utils.py
--rw-r--r--   0        0        0     2337 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0     6225 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/view.py
--rw-r--r--   0        0        0     4049 2023-05-03 03:53:46.133657 flet_core-0.7.0.dev1372/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.7.0.dev1372/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/README.md
+-rw-r--r--   0        0        0      723 2023-05-11 20:21:34.998906 flet_core-0.7.0.dev1395/pyproject.toml
+-rw-r--r--   0        0        0     6457 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/__init__.py
+-rw-r--r--   0        0        0     6774 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     7226 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     2806 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/animation.py
+-rw-r--r--   0        0        0     5403 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7301 2023-05-11 20:21:00.207028 flet_core-0.7.0.dev1395/src/flet_core/audio.py
+-rw-r--r--   0        0        0     5446 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     2826 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2202 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/buttons.py
+-rw-r--r--   0        0        0     3044 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/callable_control.py
+-rw-r--r--   0        0        0      514 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0     2903 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4629 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1639 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1361 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      837 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1862 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1907 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3486 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1772 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2361 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1963 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     5695 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/card.py
+-rw-r--r--   0        0        0     9855 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2061 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6837 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1949 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2924 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11228 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     8258 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5496 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5888 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3824 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0     7156 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0     6795 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3085 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0     1002 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/clipboard.py
+-rw-r--r--   0        0        0    10708 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/colors.py
+-rw-r--r--   0        0        0     6924 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/column.py
+-rw-r--r--   0        0        0     1132 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/connection.py
+-rw-r--r--   0        0        0     7099 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    14684 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/container.py
+-rw-r--r--   0        0        0    13995 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/control_event.py
+-rw-r--r--   0        0        0    20707 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/datatable.py
+-rw-r--r--   0        0        0     2263 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/divider.py
+-rw-r--r--   0        0        0     6270 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6063 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/draggable.py
+-rw-r--r--   0        0        0     9177 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0     8621 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     1978 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/event.py
+-rw-r--r--   0        0        0     1839 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9777 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2694 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     2828 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     2542 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0     7111 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    13981 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    28044 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1531 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     6804 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2134 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3430 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/icon.py
+-rw-r--r--   0        0        0     8255 2023-05-11 20:21:00.211028 flet_core-0.7.0.dev1395/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362652 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/icons.py
+-rw-r--r--   0        0        0     6585 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0     8360 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     6401 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/list_view.py
+-rw-r--r--   0        0        0     8644 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      223 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/locks.py
+-rw-r--r--   0        0        0      583 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/margin.py
+-rw-r--r--   0        0        0     6129 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5180 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     8322 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0    11986 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     7306 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/padding.py
+-rw-r--r--   0        0        0    53719 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/page.py
+-rw-r--r--   0        0        0     2674 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4410 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0     6811 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     4293 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     4491 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4088 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/protocol.py
+-rw-r--r--   0        0        0     3419 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     5765 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2389 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0      291 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6344 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     6908 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/row.py
+-rw-r--r--   0        0        0     4486 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/scrollable_control.py
+-rw-r--r--   0        0        0     1637 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/semantics.py
+-rw-r--r--   0        0        0      576 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5318 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2919 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0     7382 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/slider.py
+-rw-r--r--   0        0        0     3971 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     4889 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8104 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/switch.py
+-rw-r--r--   0        0        0    10820 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10568 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/text.py
+-rw-r--r--   0        0        0     7279 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3092 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1260 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    15444 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/textfield.py
+-rw-r--r--   0        0        0     6172 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8362 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2753 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     5186 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/types.py
+-rw-r--r--   0        0        0      684 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/user_control.py
+-rw-r--r--   0        0        0      409 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/utils.py
+-rw-r--r--   0        0        0     2337 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0     5852 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/view.py
+-rw-r--r--   0        0        0     4049 2023-05-11 20:21:00.215028 flet_core-0.7.0.dev1395/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.7.0.dev1395/PKG-INFO
```

### Comparing `flet_core-0.7.0.dev1372/pyproject.toml` & `flet_core-0.7.0.dev1395/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-core"
-version = "0.7.0.dev1372"
+version = "0.7.0.dev1395"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/__init__.py` & `flet_core-0.7.0.dev1395/src/flet_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 from flet_core.progress_ring import ProgressRing
 from flet_core.querystring import QueryString
 from flet_core.radio import Radio
 from flet_core.radio_group import RadioGroup
 from flet_core.ref import Ref
 from flet_core.responsive_row import ResponsiveRow
 from flet_core.row import Row
+from flet_core.scrollable_control import OnScrollEvent
 from flet_core.semantics import Semantics
 from flet_core.shader_mask import ShaderMask
 from flet_core.shadow import BoxShadow, ShadowBlurStyle
 from flet_core.shake_detector import ShakeDetector
 from flet_core.slider import Slider
 from flet_core.snack_bar import SnackBar
 from flet_core.stack import Stack
@@ -164,16 +165,20 @@
 from flet_core.template_route import TemplateRoute
 from flet_core.text import Text, TextOverflow, TextThemeStyle
 from flet_core.text_button import TextButton
 from flet_core.text_span import TextSpan
 from flet_core.text_style import TextDecoration, TextDecorationStyle, TextStyle
 from flet_core.textfield import KeyboardType, TextCapitalization, TextField
 from flet_core.theme import (
+    ColorScheme,
     PageTransitionsTheme,
     PageTransitionTheme,
+    ScrollbarTheme,
+    TabsTheme,
+    TextTheme,
     Theme,
     ThemeVisualDensity,
 )
 from flet_core.tooltip import Tooltip
 from flet_core.transform import Offset, Rotate, Scale
 from flet_core.transparent_pointer import TransparentPointer
 from flet_core.types import (
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/alert_dialog.py` & `flet_core-0.7.0.dev1395/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/animated_switcher.py` & `flet_core-0.7.0.dev1395/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/animation.py` & `flet_core-0.7.0.dev1395/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/app_bar.py` & `flet_core-0.7.0.dev1395/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/audio.py` & `flet_core-0.7.0.dev1395/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/banner.py` & `flet_core-0.7.0.dev1395/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/border.py` & `flet_core-0.7.0.dev1395/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/border_radius.py` & `flet_core-0.7.0.dev1395/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/bottom_sheet.py` & `flet_core-0.7.0.dev1395/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/buttons.py` & `flet_core-0.7.0.dev1395/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/callable_control.py` & `flet_core-0.7.0.dev1395/src/flet_core/callable_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/__init__.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/arc.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/canvas.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/circle.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/color.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/fill.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/line.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/oval.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/path.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/points.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/rect.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/shadow.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/canvas/text.py` & `flet_core-0.7.0.dev1395/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/card.py` & `flet_core-0.7.0.dev1395/src/flet_core/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,25 @@
         tooltip: Optional[str] = None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
         # Specific
         #
+        key: Optional[str] = None,
         margin: MarginValue = None,
         elevation: OptionalNumber = None,
         color: Optional[str] = None,
         shadow_color: Optional[str] = None,
         surface_tint_color: Optional[str] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart_group.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart_rod.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/chart_axis.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/chart_axis_label.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/chart_point_shape.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/line_chart.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/line_chart_data.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/line_chart_data_point.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/pie_chart.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/charts/pie_chart_section.py` & `flet_core-0.7.0.dev1395/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/checkbox.py` & `flet_core-0.7.0.dev1395/src/flet_core/checkbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     Online docs: https://flet.dev/docs/controls/checkbox
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -94,14 +95,15 @@
         on_change=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -135,15 +137,15 @@
         self.on_blur = on_blur
 
     def _get_control_name(self):
         return "checkbox"
 
     def _before_build_command(self):
         super()._before_build_command()
-        self._set_attr_json("fillColor", self._wrap_attr_dict(self.__fill_color))
+        self._set_attr_json("fillColor", self.__fill_color)
 
     # value
     @property
     def value(self) -> Optional[bool]:
         return self._get_attr(
             "value", data_type="bool?", def_value=False if not self.tristate else None
         )
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/circle_avatar.py` & `flet_core-0.7.0.dev1395/src/flet_core/circle_avatar.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
     Online docs: https://flet.dev/docs/controls/circleavatar
     """
 
     def __init__(
         self,
         icon: Optional[str] = None,
+        key: Optional[str] = None,
         ref: Optional[Ref] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
@@ -107,14 +108,15 @@
         color: Optional[str] = None,
         bgcolor: Optional[str] = None,
         content: Optional[Control] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/client_storage.py` & `flet_core-0.7.0.dev1395/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/clipboard.py` & `flet_core-0.7.0.dev1395/src/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/colors.py` & `flet_core-0.7.0.dev1395/src/flet_core/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,24 +52,28 @@
 TERTIARY_CONTAINER = "tertiarycontainer"
 ON_TERTIARY_CONTAINER = "ontertiarycontainer"
 ERROR = "error"
 ON_ERROR = "onerror"
 ERROR_CONTAINER = "errorcontainer"
 ON_ERROR_CONTAINER = "onerrorcontainer"
 OUTLINE = "outline"
+OUTLINE_VARIANT = "outlinevariant"
 BACKGROUND = "background"
 ON_BACKGROUND = "onbackground"
 SURFACE = "surface"
 ON_SURFACE = "onsurface"
+SURFACE_TINT = "surfacetint"
 SURFACE_VARIANT = "surfacevariant"
 ON_SURFACE_VARIANT = "onsurfacevariant"
 INVERSE_SURFACE = "inversesurface"
 ON_INVERSE_SURFACE = "oninversesurface"
 INVERSE_PRIMARY = "inverseprimary"
 SHADOW = "shadow"
+SCRIM = "scrim"
+
 WHITE10 = "white10"
 WHITE12 = "white12"
 WHITE24 = "white24"
 WHITE30 = "white30"
 WHITE38 = "white38"
 WHITE54 = "white54"
 WHITE60 = "white60"
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/column.py` & `flet_core-0.7.0.dev1395/src/flet_core/row.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, List, Optional, Union
 
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
+from flet_core.scrollable_control import ScrollableControl
 from flet_core.types import (
     AnimationValue,
     CrossAxisAlignment,
     CrossAxisAlignmentString,
     MainAxisAlignment,
     MainAxisAlignmentString,
     OffsetValue,
@@ -14,54 +15,58 @@
     RotateValue,
     ScaleValue,
     ScrollMode,
     ScrollModeString,
 )
 
 
-class Column(ConstrainedControl):
+class Row(ConstrainedControl, ScrollableControl):
     """
-    Container allows to decorate a control with background color and border and position it with padding, margin and alignment.
+    A control that displays its children in a horizontal array.
+
+    To cause a child control to expand and fill the available horizontal space, set its `expand` property.
 
     Example:
 
     ```
     import flet as ft
 
+
     def main(page: ft.Page):
-        page.title = "Column example"
+        page.title = "Row example"
 
         page.add(
-            ft.Column(
-                expand=True,
+            ft.Row(
                 controls=[
                     ft.Container(
                         expand=1,
                         content=ft.Text("Container 1"),
                         bgcolor=ft.colors.GREEN_100,
                     ),
                     ft.Container(
                         expand=2, content=ft.Text("Container 2"), bgcolor=ft.colors.RED_100
                     ),
                 ],
             ),
         ),
 
+
     ft.app(target=main)
     ```
 
     -----
 
-    Online docs: https://flet.dev/docs/controls/column
+    Online docs: https://flet.dev/docs/controls/row
     """
 
     def __init__(
         self,
         controls: Optional[List[Control]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -78,28 +83,34 @@
         animate_scale: AnimationValue = None,
         animate_offset: AnimationValue = None,
         on_animation_end=None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
-        # Column specific
+        # ScrollableControl specific
+        #
+        scroll: Optional[ScrollMode] = None,
+        auto_scroll: Optional[bool] = None,
+        on_scroll_interval: OptionalNumber = None,
+        on_scroll: Any = None,
+        #
+        # Row specific
         #
         alignment: MainAxisAlignment = MainAxisAlignment.NONE,
-        horizontal_alignment: CrossAxisAlignment = CrossAxisAlignment.NONE,
+        vertical_alignment: CrossAxisAlignment = CrossAxisAlignment.NONE,
         spacing: OptionalNumber = None,
         tight: Optional[bool] = None,
         wrap: Optional[bool] = None,
         run_spacing: OptionalNumber = None,
-        scroll: Optional[ScrollMode] = None,
-        auto_scroll: Optional[bool] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -117,26 +128,32 @@
             animate_offset=animate_offset,
             on_animation_end=on_animation_end,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
+        ScrollableControl.__init__(
+            self,
+            scroll=scroll,
+            auto_scroll=auto_scroll,
+            on_scroll_interval=on_scroll_interval,
+            on_scroll=on_scroll,
+        )
+
         self.controls = controls
-        self.horizontal_alignment = horizontal_alignment
         self.alignment = alignment
+        self.vertical_alignment = vertical_alignment
         self.spacing = spacing
         self.tight = tight
         self.wrap = wrap
         self.run_spacing = run_spacing
-        self.scroll = scroll
-        self.auto_scroll = auto_scroll
 
     def _get_control_name(self):
-        return "column"
+        return "row"
 
     def _get_children(self):
         return self.__controls
 
     def clean(self):
         super().clean()
         self.__controls.clear()
@@ -150,15 +167,15 @@
     def tight(self) -> Optional[bool]:
         return self._get_attr("tight", data_type="bool", def_value=False)
 
     @tight.setter
     def tight(self, value: Optional[bool]):
         self._set_attr("tight", value)
 
-    # alignment
+    # horizontal_alignment
     @property
     def alignment(self) -> MainAxisAlignment:
         return self.__alignment
 
     @alignment.setter
     def alignment(self, value: MainAxisAlignment):
         self.__alignment = value
@@ -166,29 +183,29 @@
             self._set_attr("alignment", value.value)
         else:
             self.__set_alignment(value)
 
     def __set_alignment(self, value: MainAxisAlignmentString):
         self._set_attr("alignment", value)
 
-    # horizontal_alignment
+    # vertical_alignment
     @property
-    def horizontal_alignment(self) -> CrossAxisAlignment:
-        return self.__horizontal_alignment
+    def vertical_alignment(self) -> CrossAxisAlignment:
+        return self.__vertical_alignment
 
-    @horizontal_alignment.setter
-    def horizontal_alignment(self, value: CrossAxisAlignment):
-        self.__horizontal_alignment = value
+    @vertical_alignment.setter
+    def vertical_alignment(self, value: CrossAxisAlignment):
+        self.__vertical_alignment = value
         if isinstance(value, CrossAxisAlignment):
-            self._set_attr("horizontalAlignment", value.value)
+            self._set_attr("verticalAlignment", value.value)
         else:
-            self.__set_horizontal_alignment(value)
+            self.__set_vertical_alignment(value)
 
-    def __set_horizontal_alignment(self, value: CrossAxisAlignmentString):
-        self._set_attr("horizontalAlignment", value)
+    def __set_vertical_alignment(self, value: CrossAxisAlignmentString):
+        self._set_attr("verticalAlignment", value)
 
     # spacing
     @property
     def spacing(self) -> OptionalNumber:
         return self._get_attr("spacing")
 
     @spacing.setter
@@ -209,43 +226,14 @@
     def run_spacing(self) -> OptionalNumber:
         return self._get_attr("runSpacing")
 
     @run_spacing.setter
     def run_spacing(self, value: OptionalNumber):
         self._set_attr("runSpacing", value)
 
-    # scroll
-    @property
-    def scroll(self) -> Optional[ScrollMode]:
-        return self.__scroll
-
-    @scroll.setter
-    def scroll(self, value: Optional[ScrollMode]):
-        self.__scroll = value
-        if isinstance(value, ScrollMode):
-            self._set_attr("scroll", value.value)
-        else:
-            self.__set_scroll(value)
-
-    def __set_scroll(self, value: Optional[ScrollModeString]):
-        if value is True:
-            value = "auto"
-        elif value is False:
-            value = None
-        self._set_attr("scroll", value)
-
-    # auto_scroll
-    @property
-    def auto_scroll(self) -> Optional[bool]:
-        return self._get_attr("autoScroll")
-
-    @auto_scroll.setter
-    def auto_scroll(self, value: Optional[bool]):
-        self._set_attr("autoScroll", value)
-
     # controls
     @property
     def controls(self):
         return self.__controls
 
     @controls.setter
     def controls(self, value: Optional[List[Control]]):
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/connection.py` & `flet_core-0.7.0.dev1395/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/constrained_control.py` & `flet_core-0.7.0.dev1395/src/flet_core/constrained_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         tooltip: Optional[str] = None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
         # ConstrainedControl specific
         #
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         rotate: RotateValue = None,
@@ -51,14 +52,15 @@
             opacity=opacity,
             tooltip=tooltip,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
+        self.key = key
         self.width = width
         self.height = height
         self.left = left
         self.top = top
         self.right = right
         self.bottom = bottom
         self.scale = scale
@@ -81,14 +83,23 @@
         self._set_attr_json("animateOpacity", self.__animate_opacity)
         self._set_attr_json("animateSize", self.__animate_size)
         self._set_attr_json("animatePosition", self.__animate_position)
         self._set_attr_json("animateRotation", self.__animate_rotation)
         self._set_attr_json("animateScale", self.__animate_scale)
         self._set_attr_json("animateOffset", self.__animate_offset)
 
+    # key
+    @property
+    def key(self) -> Optional[str]:
+        return self._get_attr("key")
+
+    @key.setter
+    def key(self, value: Optional[str]):
+        self._set_attr("key", value)
+
     # width
     @property
     def width(self) -> OptionalNumber:
         """
         Control width.
         """
         return self._get_attr("width")
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/container.py` & `flet_core-0.7.0.dev1395/src/flet_core/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.control_event import ControlEvent
 from flet_core.event_handler import EventHandler
 from flet_core.gradients import Gradient
 from flet_core.ref import Ref
 from flet_core.shadow import BoxShadow
+from flet_core.theme import Theme
 from flet_core.types import (
     AnimationValue,
     BlendMode,
     BlendModeString,
     BorderRadiusValue,
     BoxShape,
     ClipBehavior,
@@ -25,14 +26,15 @@
     ImageRepeatString,
     MarginValue,
     OffsetValue,
     PaddingValue,
     ResponsiveNumber,
     RotateValue,
     ScaleValue,
+    ThemeMode,
 )
 
 try:
     from typing import Literal
 except Exception:
     from typing_extensions import Literal
 
@@ -64,14 +66,15 @@
     Online docs: https://flet.dev/docs/controls/container
     """
 
     def __init__(
         self,
         content: Optional[Control] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -114,21 +117,24 @@
         animate: AnimationValue = None,
         blur: Union[
             None, float, int, Tuple[Union[float, int], Union[float, int]], Blur
         ] = None,
         shadow: Union[None, BoxShadow, List[BoxShadow]] = None,
         url: Optional[str] = None,
         url_target: Optional[str] = None,
+        theme: Optional[Theme] = None,
+        theme_mode: Optional[ThemeMode] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -176,14 +182,16 @@
         self.clip_behavior = clip_behavior
         self.ink = ink
         self.animate = animate
         self.blur = blur
         self.shadow = shadow
         self.url = url
         self.url_target = url_target
+        self.theme = theme
+        self.theme_mode = theme_mode
         self.on_click = on_click
         self.on_long_press = on_long_press
         self.on_hover = on_hover
 
     def _get_control_name(self):
         return "container"
 
@@ -194,14 +202,15 @@
         self._set_attr_json("margin", self.__margin)
         self._set_attr_json("padding", self.__padding)
         self._set_attr_json("alignment", self.__alignment)
         self._set_attr_json("gradient", self.__gradient)
         self._set_attr_json("animate", self.__animate)
         self._set_attr_json("blur", self.__blur)
         self._set_attr_json("shadow", self.__shadow if self.__shadow else None)
+        self._set_attr_json("theme", self.__theme)
 
     def _get_children(self):
         children = []
         if self.__content is not None:
             self.__content._set_attr_internal("n", "content")
             children.append(self.__content)
         return children
@@ -439,14 +448,33 @@
     def url_target(self):
         return self._get_attr("urlTarget")
 
     @url_target.setter
     def url_target(self, value):
         self._set_attr("urlTarget", value)
 
+    # theme
+    @property
+    def theme(self) -> Optional[Theme]:
+        return self.__theme
+
+    @theme.setter
+    def theme(self, value: Optional[Theme]):
+        self.__theme = value
+
+    # theme_mode
+    @property
+    def theme_mode(self) -> Optional[ThemeMode]:
+        return self.__theme_mode
+
+    @theme_mode.setter
+    def theme_mode(self, value: Optional[ThemeMode]):
+        self.__theme_mode = value
+        self._set_attr("themeMode", value.value if value is not None else None)
+
     # on_click
     @property
     def on_click(self):
         return self.__on_click
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/control.py` & `flet_core-0.7.0.dev1395/src/flet_core/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     def _is_isolated(self):
         return False
 
     def _build(self):
         pass
 
     def _before_build_command(self):
-        self._set_attr_json("col", self._wrap_attr_dict(self.__col))
+        self._set_attr_json("col", self.__col)
 
     def did_mount(self):
         pass
 
     async def did_mount_async(self):
         pass
 
@@ -141,19 +141,14 @@
     def _convert_attr_json(self, value):
         return (
             json.dumps(value, cls=EmbedJsonEncoder, separators=(",", ":"))
             if value is not None
             else None
         )
 
-    def _wrap_attr_dict(self, value):
-        if value is None or isinstance(value, Dict):
-            return value
-        return {"": value}
-
     def __str__(self):
         attrs = {}
         for k, v in self.__attrs.items():
             attrs[k] = v[0]
         return f"{self._get_control_name()} {attrs}"
 
     # event_handlers
@@ -394,15 +389,14 @@
 
             removed_controls.append(control)
 
         return removed_controls
 
     # private methods
     def _build_add_commands(self, indent=0, index=None, added_controls=None):
-
         self._build()
 
         # remove control from index
         if self.__uid and index is not None and self.__uid in index:
             del index[self.__uid]
 
         commands = []
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/datatable.py` & `flet_core-0.7.0.dev1395/src/flet_core/datatable.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         self.on_select_changed = on_select_changed
 
     def _get_control_name(self):
         return "r"
 
     def _before_build_command(self):
         super()._before_build_command()
-        self._set_attr_json("color", self._wrap_attr_dict(self.__color))
+        self._set_attr_json("color", self.__color)
 
     def _get_children(self):
         return self.__cells
 
     # cells
     @property
     def cells(self):
@@ -297,14 +297,15 @@
 
 class DataTable(ConstrainedControl):
     def __init__(
         self,
         columns: Optional[List[DataColumn]] = None,
         rows: Optional[List[DataRow]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -349,14 +350,15 @@
         sort_ascending: Optional[bool] = None,
         sort_column_index: Optional[int] = None,
         on_select_all=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -409,18 +411,16 @@
     def _before_build_command(self):
         super()._before_build_command()
         self._set_attr_json("border", self.__border)
         self._set_attr_json("gradient", self.__gradient)
         self._set_attr_json("borderRadius", self.__border_radius)
         self._set_attr_json("horizontalLines", self.__horizontal_lines)
         self._set_attr_json("verticalLines", self.__vertical_lines)
-        self._set_attr_json("dataRowColor", self._wrap_attr_dict(self.__data_row_color))
-        self._set_attr_json(
-            "headingRowColor", self._wrap_attr_dict(self.__heading_row_color)
-        )
+        self._set_attr_json("dataRowColor", self.__data_row_color)
+        self._set_attr_json("headingRowColor", self.__heading_row_color)
         self._set_attr_json("dataTextStyle", self.__data_text_style)
         self._set_attr_json("headingTextStyle", self.__heading_text_style)
 
     def _get_children(self):
         children = []
         children.extend(self.__columns)
         children.extend(self.__rows)
@@ -638,15 +638,14 @@
 class Item(Control):
     def __init__(self, obj):
         Control.__init__(self)
         assert obj, "obj cannot be empty"
         self.obj = obj
 
     def _set_attr(self, name, value, dirty=True):
-
         if value is None:
             return
 
         orig_val = self._get_attr(name)
         if orig_val is not None:
             if isinstance(orig_val, bool):
                 value = str(value).lower() == "true"
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/divider.py` & `flet_core-0.7.0.dev1395/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/drag_target.py` & `flet_core-0.7.0.dev1395/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/draggable.py` & `flet_core-0.7.0.dev1395/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/dropdown.py` & `flet_core-0.7.0.dev1395/src/flet_core/dropdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     Online docs: https://flet.dev/docs/controls/dropdown
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         rotate: RotateValue = None,
         scale: ScaleValue = None,
@@ -120,14 +121,15 @@
         on_change=None,
         on_focus=None,
         on_blur=None,
     ):
         FormFieldControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             expand=expand,
             col=col,
             opacity=opacity,
             rotate=rotate,
             scale=scale,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/elevated_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/elevated_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Online docs: https://flet.dev/docs/controls/elevatedbutton
     """
 
     def __init__(
         self,
         text: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -83,14 +84,15 @@
         on_hover=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/event_handler.py` & `flet_core-0.7.0.dev1395/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/file_picker.py` & `flet_core-0.7.0.dev1395/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/filled_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/filled_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     Online docs: https://flet.dev/docs/controls/filledbutton
     """
 
     def __init__(
         self,
         text: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         tooltip: Optional[str] = None,
         visible: Optional[bool] = None,
@@ -58,14 +59,15 @@
         on_click=None,
         on_long_press=None,
         on_hover=None,
     ):
         ElevatedButton.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             expand=expand,
             col=col,
             opacity=opacity,
             tooltip=tooltip,
             visible=visible,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/filled_tonal_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/filled_tonal_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     Online docs: https://flet.dev/docs/controls/filledtonalbutton
     """
 
     def __init__(
         self,
         text: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         tooltip: Optional[str] = None,
         visible: Optional[bool] = None,
@@ -58,14 +59,15 @@
         on_click=None,
         on_long_press=None,
         on_hover=None,
     ):
         ElevatedButton.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             expand=expand,
             col=col,
             opacity=opacity,
             tooltip=tooltip,
             visible=visible,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/flet_app.py` & `flet_core-0.7.0.dev1395/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/floating_action_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/floating_action_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     Online docs: https://flet.dev/docs/controls/floatingactionbutton
     """
 
     def __init__(
         self,
         text: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -102,14 +103,15 @@
         url: Optional[str] = None,
         url_target: Optional[str] = None,
         on_click=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/form_field_control.py` & `flet_core-0.7.0.dev1395/src/flet_core/form_field_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     UNDERLINE = "underline"
 
 
 class FormFieldControl(ConstrainedControl):
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -94,14 +95,15 @@
         suffix_icon: Optional[str] = None,
         suffix_text: Optional[str] = None,
         suffix_style: Optional[TextStyle] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/gesture_detector.py` & `flet_core-0.7.0.dev1395/src/flet_core/gesture_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     Online docs: https://flet.dev/docs/controls/gesturedetector
     """
 
     def __init__(
         self,
         content: Optional[Control] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -169,14 +170,15 @@
         on_enter=None,
         on_exit=None,
         on_scroll=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/gradients.py` & `flet_core-0.7.0.dev1395/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/grid_view.py` & `flet_core-0.7.0.dev1395/src/flet_core/grid_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Any, List, Optional, Union
 
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
+from flet_core.scrollable_control import ScrollableControl
 from flet_core.types import (
     AnimationValue,
     OffsetValue,
     PaddingValue,
     ResponsiveNumber,
     RotateValue,
     ScaleValue,
 )
 
 
-class GridView(ConstrainedControl):
+class GridView(ConstrainedControl, ScrollableControl):
     """
     A scrollable, 2D array of controls.
 
     GridView is very effective for large lists (thousands of items). Prefer it over wrapping `Column` or `Row` for smooth scrolling.
 
     Example:
     ```
@@ -60,14 +61,15 @@
     Online docs: https://flet.dev/docs/controls/gridview
     """
 
     def __init__(
         self,
         controls: Optional[List[Control]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -84,27 +86,34 @@
         animate_scale: AnimationValue = None,
         animate_offset: AnimationValue = None,
         on_animation_end=None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
+        # ScrollableControl specific
+        #
+        auto_scroll: Optional[bool] = None,
+        on_scroll_interval: OptionalNumber = None,
+        on_scroll: Any = None,
+        #
         # Specific
         #
         horizontal: Optional[bool] = None,
         runs_count: Optional[int] = None,
         max_extent: Optional[int] = None,
         spacing: OptionalNumber = None,
         run_spacing: OptionalNumber = None,
         child_aspect_ratio: OptionalNumber = None,
         padding: PaddingValue = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -122,14 +131,21 @@
             animate_offset=animate_offset,
             on_animation_end=on_animation_end,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
+        ScrollableControl.__init__(
+            self,
+            auto_scroll=auto_scroll,
+            on_scroll_interval=on_scroll_interval,
+            on_scroll=on_scroll,
+        )
+
         self.__controls: List[Control] = []
         self.controls = controls
         self.horizontal = horizontal
         self.runs_count = runs_count
         self.max_extent = max_extent
         self.spacing = spacing
         self.run_spacing = run_spacing
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/haptic_feedback.py` & `flet_core-0.7.0.dev1395/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/icon.py` & `flet_core-0.7.0.dev1395/src/flet_core/icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     Online docs: https://flet.dev/docs/controls/icon
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         rotate: RotateValue = None,
         scale: ScaleValue = None,
         offset: OffsetValue = None,
         aspect_ratio: OptionalNumber = None,
@@ -67,18 +68,18 @@
         data: Any = None,
         #
         # Specific
         #
         color: Optional[str] = None,
         size: OptionalNumber = None,
     ):
-
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             expand=expand,
             col=col,
             opacity=opacity,
             rotate=rotate,
             scale=scale,
             offset=offset,
             aspect_ratio=aspect_ratio,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/icon_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/icon_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     Online docs: https://flet.dev/docs/controls/iconbutton
     """
 
     def __init__(
         self,
         icon: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -98,14 +99,15 @@
         on_click=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/icons.py` & `flet_core-0.7.0.dev1395/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/image.py` & `flet_core-0.7.0.dev1395/src/flet_core/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     Online docs: https://flet.dev/docs/controls/image
     """
 
     def __init__(
         self,
         src: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -88,18 +89,18 @@
         fit: Optional[ImageFit] = None,
         border_radius: BorderRadiusValue = None,
         color: Optional[str] = None,
         color_blend_mode: BlendMode = BlendMode.NONE,
         gapless_playback: Optional[bool] = None,
         semantics_label: Optional[str] = None,
     ):
-
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/list_tile.py` & `flet_core-0.7.0.dev1395/src/flet_core/list_tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     Online docs: https://flet.dev/docs/controls/listtile
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -97,14 +98,15 @@
         url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/list_view.py` & `flet_core-0.7.0.dev1395/src/flet_core/list_view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Any, List, Optional, Union
 
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
+from flet_core.scrollable_control import ScrollableControl
 from flet_core.types import (
     AnimationValue,
     OffsetValue,
     PaddingValue,
     ResponsiveNumber,
     RotateValue,
     ScaleValue,
+    ScrollMode,
 )
 
 
-class ListView(ConstrainedControl):
+class ListView(ConstrainedControl, ScrollableControl):
     """
     A scrollable list of controls arranged linearly.
 
     ListView is the most commonly used scrolling control. It displays its children one after another in the scroll direction. In the cross axis, the children are required to fill the ListView.
 
     Example:
 
@@ -52,14 +54,15 @@
     Online docs: https://flet.dev/docs/controls/listview
     """
 
     def __init__(
         self,
         controls: Optional[List[Control]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -76,27 +79,33 @@
         animate_scale: AnimationValue = None,
         animate_offset: AnimationValue = None,
         on_animation_end=None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
+        # ScrollableControl specific
+        #
+        auto_scroll: Optional[bool] = None,
+        on_scroll_interval: OptionalNumber = None,
+        on_scroll: Any = None,
+        #
         # Specific
         #
         horizontal: Optional[bool] = None,
         spacing: OptionalNumber = None,
         item_extent: OptionalNumber = None,
         first_item_prototype: Optional[bool] = None,
         divider_thickness: OptionalNumber = None,
         padding: PaddingValue = None,
-        auto_scroll: Optional[bool] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -114,23 +123,29 @@
             animate_offset=animate_offset,
             on_animation_end=on_animation_end,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
+        ScrollableControl.__init__(
+            self,
+            auto_scroll=auto_scroll,
+            on_scroll_interval=on_scroll_interval,
+            on_scroll=on_scroll,
+        )
+
         self.__controls: List[Control] = []
         self.controls = controls
         self.horizontal = horizontal
         self.spacing = spacing
         self.divider_thickness = divider_thickness
         self.item_extent = item_extent
         self.first_item_prototype = first_item_prototype
         self.padding = padding
-        self.auto_scroll = auto_scroll
 
     def _get_control_name(self):
         return "listview"
 
     def _before_build_command(self):
         super()._before_build_command()
         self._set_attr_json("padding", self.__padding)
@@ -204,16 +219,7 @@
     @property
     def controls(self):
         return self.__controls
 
     @controls.setter
     def controls(self, value):
         self.__controls = value if value is not None else []
-
-    # auto_scroll
-    @property
-    def auto_scroll(self) -> Optional[bool]:
-        return self._get_attr("autoScroll")
-
-    @auto_scroll.setter
-    def auto_scroll(self, value: Optional[bool]):
-        self._set_attr("autoScroll", value)
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/local_connection.py` & `flet_core-0.7.0.dev1395/src/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/margin.py` & `flet_core-0.7.0.dev1395/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/markdown.py` & `flet_core-0.7.0.dev1395/src/flet_core/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     Online docs: https://flet.dev/docs/controls/markdown
     """
 
     def __init__(
         self,
         value: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -77,14 +78,15 @@
         auto_follow_links: Optional[bool] = None,
         auto_follow_links_target: Optional[str] = None,
         on_tap_link=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/matplotlib_chart.py` & `flet_core-0.7.0.dev1395/src/flet_core/matplotlib_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     Online docs: https://flet.dev/docs/controls/matplotlibchart
     """
 
     def __init__(
         self,
         figure: Optional[Figure] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         rotate: RotateValue = None,
         scale: ScaleValue = None,
         offset: OffsetValue = None,
         aspect_ratio: OptionalNumber = None,
@@ -90,18 +91,18 @@
         #
         # Specific
         #
         isolated: bool = False,
         original_size: bool = False,
         transparent: bool = False,
     ):
-
         Container.__init__(
             self,
             ref=ref,
+            key=key,
             expand=expand,
             col=col,
             opacity=opacity,
             rotate=rotate,
             scale=scale,
             offset=offset,
             aspect_ratio=aspect_ratio,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/navigation_bar.py` & `flet_core-0.7.0.dev1395/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/navigation_rail.py` & `flet_core-0.7.0.dev1395/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/outlined_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/outlined_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Online docs: https://flet.dev/docs/controls/outlinedbutton
     """
 
     def __init__(
         self,
         text: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -80,14 +81,15 @@
         on_hover=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/padding.py` & `flet_core-0.7.0.dev1395/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/page.py` & `flet_core-0.7.0.dev1395/src/flet_core/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 import uuid
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 from urllib.parse import urlparse
 
 import flet_core
+from flet_core.animation import AnimationCurve
 from flet_core.app_bar import AppBar
 from flet_core.banner import Banner
 from flet_core.client_storage import ClientStorage
 from flet_core.clipboard import Clipboard
 from flet_core.connection import Connection
 from flet_core.control import Control, OptionalNumber
 from flet_core.control_event import ControlEvent
@@ -806,14 +807,38 @@
 
     def window_to_front(self):
         self.invoke_method("windowToFront")
 
     async def window_to_front_async(self):
         await self.invoke_method_async("windowToFront")
 
+    def scroll_to(
+        self,
+        offset: Optional[float] = None,
+        delta: Optional[float] = None,
+        key: Optional[str] = None,
+        duration: Optional[int] = None,
+        curve: Optional[AnimationCurve] = None,
+    ):
+        self.__default_view.scroll_to(
+            offset=offset, delta=delta, key=key, duration=duration, curve=curve
+        )
+
+    async def scroll_to_async(
+        self,
+        offset: Optional[float] = None,
+        delta: Optional[float] = None,
+        key: Optional[str] = None,
+        duration: Optional[int] = None,
+        curve: Optional[AnimationCurve] = None,
+    ):
+        await self.__default_view.scroll_to_async(
+            offset=offset, delta=delta, key=key, duration=duration, curve=curve
+        )
+
     def invoke_method(
         self,
         method_name: str,
         arguments: Optional[Dict[str, str]] = None,
         wait_for_result: bool = False,
     ) -> Optional[str]:
         method_id = uuid.uuid4().hex
@@ -1512,14 +1537,23 @@
     def window_visible(self) -> Optional[bool]:
         return self._get_attr("windowVisible", data_type="bool")
 
     @window_visible.setter
     def window_visible(self, value: Optional[bool]):
         self._set_attr("windowVisible", value)
 
+    # on_scroll_interval
+    @property
+    def on_scroll_interval(self) -> OptionalNumber:
+        return self.__default_view.on_scroll_interval
+
+    @on_scroll_interval.setter
+    def on_scroll_interval(self, value: OptionalNumber):
+        self.__default_view.on_scroll_interval
+
     # on_close
     @property
     def on_close(self):
         return self.__on_close
 
     @on_close.setter
     def on_close(self, handler):
@@ -1611,23 +1645,31 @@
     def on_error(self):
         return self.__on_error
 
     @on_error.setter
     def on_error(self, handler):
         self.__on_error.subscribe(handler)
 
+    # on_scroll
+    @property
+    def on_scroll(self):
+        return self.__default_view.on_scroll
+
+    @on_scroll.setter
+    def on_scroll(self, handler):
+        self.__default_view.on_scroll
+
 
 class Offstage(Control):
     def __init__(
         self,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
     ):
-
         Control.__init__(
             self,
             visible=visible,
             disabled=disabled,
             data=data,
         )
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/painting.py` & `flet_core-0.7.0.dev1395/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/plotly_chart.py` & `flet_core-0.7.0.dev1395/src/flet_core/plotly_chart.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     Online docs: https://flet.dev/docs/controls/plotlychart
     """
 
     def __init__(
         self,
         figure: Optional[Figure] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         rotate: RotateValue = None,
         scale: ScaleValue = None,
         offset: OffsetValue = None,
         aspect_ratio: OptionalNumber = None,
@@ -72,18 +73,18 @@
         data: Any = None,
         #
         # Specific
         #
         isolated: bool = False,
         original_size: bool = False,
     ):
-
         Container.__init__(
             self,
             ref=ref,
+            key=key,
             expand=expand,
             col=col,
             opacity=opacity,
             rotate=rotate,
             scale=scale,
             offset=offset,
             aspect_ratio=aspect_ratio,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/popup_menu_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/popup_menu_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     Online docs: https://flet.dev/docs/controls/popupmenubutton
     """
 
     def __init__(
         self,
         content: Optional[Control] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -161,18 +162,18 @@
         data: Any = None,
         #
         # PopupMenuButton-specific
         items: Optional[List[PopupMenuItem]] = None,
         icon: Optional[str] = None,
         on_cancelled=None,
     ):
-
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/progress_bar.py` & `flet_core-0.7.0.dev1395/src/flet_core/progress_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     Online docs: https://flet.dev/docs/controls/progressbar
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -82,14 +83,15 @@
         bar_height: OptionalNumber = None,
         color: Optional[str] = None,
         bgcolor: Optional[str] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/progress_ring.py` & `flet_core-0.7.0.dev1395/src/flet_core/progress_ring.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     Online docs: https://flet.dev/docs/controls/progressring
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -84,14 +85,15 @@
         stroke_width: OptionalNumber = None,
         color: Optional[str] = None,
         bgcolor: Optional[str] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/protocol.py` & `flet_core-0.7.0.dev1395/src/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/querystring.py` & `flet_core-0.7.0.dev1395/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/radio.py` & `flet_core-0.7.0.dev1395/src/flet_core/radio.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     Online docs: https://flet.dev/docs/controls/radio
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -87,14 +88,15 @@
         fill_color: Union[None, str, Dict[MaterialState, str]] = None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -125,15 +127,15 @@
         self.on_blur = on_blur
 
     def _get_control_name(self):
         return "radio"
 
     def _before_build_command(self):
         super()._before_build_command()
-        self._set_attr_json("fillColor", self._wrap_attr_dict(self.__fill_color))
+        self._set_attr_json("fillColor", self.__fill_color)
 
     # value
     @property
     def value(self) -> Optional[str]:
         return self._get_attr("value", def_value="")
 
     @value.setter
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/radio_group.py` & `flet_core-0.7.0.dev1395/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/responsive_row.py` & `flet_core-0.7.0.dev1395/src/flet_core/responsive_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     Online docs: https://flet.dev/docs/controls/responsiverow
     """
 
     def __init__(
         self,
         controls: Optional[List[Control]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -83,14 +84,15 @@
         vertical_alignment: CrossAxisAlignment = CrossAxisAlignment.NONE,
         spacing: Optional[ResponsiveNumber] = None,
         run_spacing: Optional[ResponsiveNumber] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -120,17 +122,17 @@
         self.columns = columns
 
     def _get_control_name(self):
         return "responsiverow"
 
     def _before_build_command(self):
         super()._before_build_command()
-        self._set_attr_json("columns", self._wrap_attr_dict(self.__columns))
-        self._set_attr_json("spacing", self._wrap_attr_dict(self.__spacing))
-        self._set_attr_json("runSpacing", self._wrap_attr_dict(self.__run_spacing))
+        self._set_attr_json("columns", self.__columns)
+        self._set_attr_json("spacing", self.__spacing)
+        self._set_attr_json("runSpacing", self.__run_spacing)
 
     def _get_children(self):
         return self.__controls
 
     def clean(self):
         super().clean()
         self.__controls.clear()
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/row.py` & `flet_core-0.7.0.dev1395/src/flet_core/column.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, List, Optional, Union
 
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
+from flet_core.scrollable_control import ScrollableControl
 from flet_core.types import (
     AnimationValue,
     CrossAxisAlignment,
     CrossAxisAlignmentString,
     MainAxisAlignment,
     MainAxisAlignmentString,
     OffsetValue,
@@ -14,57 +15,55 @@
     RotateValue,
     ScaleValue,
     ScrollMode,
     ScrollModeString,
 )
 
 
-class Row(ConstrainedControl):
+class Column(ConstrainedControl, ScrollableControl):
     """
-    A control that displays its children in a horizontal array.
-
-    To cause a child control to expand and fill the available horizontal space, set its `expand` property.
+    Container allows to decorate a control with background color and border and position it with padding, margin and alignment.
 
     Example:
 
     ```
     import flet as ft
 
-
     def main(page: ft.Page):
-        page.title = "Row example"
+        page.title = "Column example"
 
         page.add(
-            ft.Row(
+            ft.Column(
+                expand=True,
                 controls=[
                     ft.Container(
                         expand=1,
                         content=ft.Text("Container 1"),
                         bgcolor=ft.colors.GREEN_100,
                     ),
                     ft.Container(
                         expand=2, content=ft.Text("Container 2"), bgcolor=ft.colors.RED_100
                     ),
                 ],
             ),
         ),
 
-
     ft.app(target=main)
     ```
 
     -----
 
-    Online docs: https://flet.dev/docs/controls/row
+    Online docs: https://flet.dev/docs/controls/column
     """
 
     def __init__(
         self,
         controls: Optional[List[Control]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -81,28 +80,34 @@
         animate_scale: AnimationValue = None,
         animate_offset: AnimationValue = None,
         on_animation_end=None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
-        # Row specific
+        # ScrollableControl specific
+        #
+        scroll: Optional[ScrollMode] = None,
+        auto_scroll: Optional[bool] = None,
+        on_scroll_interval: OptionalNumber = None,
+        on_scroll: Any = None,
+        #
+        # Column specific
         #
         alignment: MainAxisAlignment = MainAxisAlignment.NONE,
-        vertical_alignment: CrossAxisAlignment = CrossAxisAlignment.NONE,
+        horizontal_alignment: CrossAxisAlignment = CrossAxisAlignment.NONE,
         spacing: OptionalNumber = None,
         tight: Optional[bool] = None,
         wrap: Optional[bool] = None,
         run_spacing: OptionalNumber = None,
-        scroll: Optional[ScrollMode] = None,
-        auto_scroll: Optional[bool] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -120,26 +125,32 @@
             animate_offset=animate_offset,
             on_animation_end=on_animation_end,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
+        ScrollableControl.__init__(
+            self,
+            scroll=scroll,
+            auto_scroll=auto_scroll,
+            on_scroll_interval=on_scroll_interval,
+            on_scroll=on_scroll,
+        )
+
         self.controls = controls
+        self.horizontal_alignment = horizontal_alignment
         self.alignment = alignment
-        self.vertical_alignment = vertical_alignment
         self.spacing = spacing
         self.tight = tight
         self.wrap = wrap
         self.run_spacing = run_spacing
-        self.scroll = scroll
-        self.auto_scroll = auto_scroll
 
     def _get_control_name(self):
-        return "row"
+        return "column"
 
     def _get_children(self):
         return self.__controls
 
     def clean(self):
         super().clean()
         self.__controls.clear()
@@ -153,15 +164,15 @@
     def tight(self) -> Optional[bool]:
         return self._get_attr("tight", data_type="bool", def_value=False)
 
     @tight.setter
     def tight(self, value: Optional[bool]):
         self._set_attr("tight", value)
 
-    # horizontal_alignment
+    # alignment
     @property
     def alignment(self) -> MainAxisAlignment:
         return self.__alignment
 
     @alignment.setter
     def alignment(self, value: MainAxisAlignment):
         self.__alignment = value
@@ -169,29 +180,29 @@
             self._set_attr("alignment", value.value)
         else:
             self.__set_alignment(value)
 
     def __set_alignment(self, value: MainAxisAlignmentString):
         self._set_attr("alignment", value)
 
-    # vertical_alignment
+    # horizontal_alignment
     @property
-    def vertical_alignment(self) -> CrossAxisAlignment:
-        return self.__vertical_alignment
+    def horizontal_alignment(self) -> CrossAxisAlignment:
+        return self.__horizontal_alignment
 
-    @vertical_alignment.setter
-    def vertical_alignment(self, value: CrossAxisAlignment):
-        self.__vertical_alignment = value
+    @horizontal_alignment.setter
+    def horizontal_alignment(self, value: CrossAxisAlignment):
+        self.__horizontal_alignment = value
         if isinstance(value, CrossAxisAlignment):
-            self._set_attr("verticalAlignment", value.value)
+            self._set_attr("horizontalAlignment", value.value)
         else:
-            self.__set_vertical_alignment(value)
+            self.__set_horizontal_alignment(value)
 
-    def __set_vertical_alignment(self, value: CrossAxisAlignmentString):
-        self._set_attr("verticalAlignment", value)
+    def __set_horizontal_alignment(self, value: CrossAxisAlignmentString):
+        self._set_attr("horizontalAlignment", value)
 
     # spacing
     @property
     def spacing(self) -> OptionalNumber:
         return self._get_attr("spacing")
 
     @spacing.setter
@@ -212,43 +223,14 @@
     def run_spacing(self) -> OptionalNumber:
         return self._get_attr("runSpacing")
 
     @run_spacing.setter
     def run_spacing(self, value: OptionalNumber):
         self._set_attr("runSpacing", value)
 
-    # scroll
-    @property
-    def scroll(self) -> Optional[ScrollMode]:
-        return self.__scroll
-
-    @scroll.setter
-    def scroll(self, value: Optional[ScrollMode]):
-        self.__scroll = value
-        if isinstance(value, ScrollMode):
-            self._set_attr("scroll", value.value)
-        else:
-            self.__set_scroll(value)
-
-    def __set_scroll(self, value: Optional[ScrollModeString]):
-        if value is True:
-            value = "auto"
-        elif value is False:
-            value = None
-        self._set_attr("scroll", value)
-
-    # auto_scroll
-    @property
-    def auto_scroll(self) -> Optional[bool]:
-        return self._get_attr("autoScroll")
-
-    @auto_scroll.setter
-    def auto_scroll(self, value: Optional[bool]):
-        self._set_attr("autoScroll", value)
-
     # controls
     @property
     def controls(self):
         return self.__controls
 
     @controls.setter
     def controls(self, value: Optional[List[Control]]):
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/semantics.py` & `flet_core-0.7.0.dev1395/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/session_storage.py` & `flet_core-0.7.0.dev1395/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/shader_mask.py` & `flet_core-0.7.0.dev1395/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/shadow.py` & `flet_core-0.7.0.dev1395/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/shake_detector.py` & `flet_core-0.7.0.dev1395/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/slider.py` & `flet_core-0.7.0.dev1395/src/flet_core/slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     Online docs: https://flet.dev/docs/controls/slider
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -82,14 +83,15 @@
         on_change_end=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/snack_bar.py` & `flet_core-0.7.0.dev1395/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/stack.py` & `flet_core-0.7.0.dev1395/src/flet_core/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     Online docs: https://flet.dev/docs/controls/stack
     """
 
     def __init__(
         self,
         controls: Optional[List[Control]] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -99,14 +100,15 @@
         # Stack-specific
         #
         clip_behavior: Optional[ClipBehavior] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/switch.py` & `flet_core-0.7.0.dev1395/src/flet_core/switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     Online docs: https://flet.dev/docs/controls/switch
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -97,14 +98,15 @@
         on_change=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -141,16 +143,16 @@
         self.on_blur = on_blur
 
     def _get_control_name(self):
         return "switch"
 
     def _before_build_command(self):
         super()._before_build_command()
-        self._set_attr_json("thumbColor", self._wrap_attr_dict(self.__thumb_color))
-        self._set_attr_json("trackColor", self._wrap_attr_dict(self.__track_color))
+        self._set_attr_json("thumbColor", self.__thumb_color)
+        self._set_attr_json("trackColor", self.__track_color)
 
     # value
     @property
     def value(self) -> Optional[bool]:
         return self._get_attr("value", data_type="bool", def_value=False)
 
     @value.setter
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/tabs.py` & `flet_core-0.7.0.dev1395/src/flet_core/tabs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
+from flet_core.border import BorderSide
+from flet_core.border_radius import BorderRadius
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
 from flet_core.types import (
     AnimationValue,
+    BorderRadiusValue,
+    MaterialState,
     OffsetValue,
+    PaddingValue,
     ResponsiveNumber,
     RotateValue,
     ScaleValue,
 )
 
 
 class Tab(Control):
@@ -124,14 +129,15 @@
 
     Online docs: https://flet.dev/docs/controls/tabs
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -153,20 +159,29 @@
         data: Any = None,
         #
         # Tabs-specific
         tabs: Optional[List[Tab]] = None,
         selected_index: Optional[int] = None,
         scrollable: Optional[bool] = None,
         animation_duration: Optional[int] = None,
+        divider_color: Optional[str] = None,
+        indicator_color: Optional[str] = None,
+        indicator_border_radius: BorderRadiusValue = None,
+        indicator_border_side: Optional[BorderSide] = None,
+        indicator_padding: PaddingValue = None,
+        indicator_tab_size: Optional[bool] = None,
+        label_color: Optional[str] = None,
+        unselected_label_color: Optional[str] = None,
+        overlay_color: Union[None, str, Dict[MaterialState, str]] = None,
         on_change=None,
     ):
-
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
@@ -188,19 +203,35 @@
             data=data,
         )
 
         self.tabs = tabs
         self.selected_index = selected_index
         self.scrollable = scrollable
         self.animation_duration = animation_duration
+        self.divider_color = divider_color
+        self.label_color = label_color
+        self.unselected_label_color = unselected_label_color
+        self.indicator_color = indicator_color
+        self.indicator_border_radius = indicator_border_radius
+        self.indicator_border_side = indicator_border_side
+        self.indicator_padding = indicator_padding
+        self.indicator_tab_size = indicator_tab_size
+        self.overlay_color = overlay_color
         self.on_change = on_change
 
     def _get_control_name(self):
         return "tabs"
 
+    def _before_build_command(self):
+        super()._before_build_command()
+        self._set_attr_json("overlayColor", self.__overlay_color)
+        self._set_attr_json("indicatorBorderRadius", self.__indicator_border_radius)
+        self._set_attr_json("indicatorBorderSide", self.__indicator_border_side)
+        self._set_attr_json("indicatorPadding", self.__indicator_padding)
+
     def _get_children(self):
         return self.__tabs
 
     # tabs
     @property
     def tabs(self) -> Optional[List[Tab]]:
         return self.__tabs
@@ -240,7 +271,88 @@
     @property
     def animation_duration(self) -> Optional[int]:
         return self._get_attr("animationDuration")
 
     @animation_duration.setter
     def animation_duration(self, value: Optional[int]):
         self._set_attr("animationDuration", value)
+
+    # divider_color
+    @property
+    def divider_color(self) -> Optional[str]:
+        return self._get_attr("dividerColor")
+
+    @divider_color.setter
+    def divider_color(self, value: Optional[str]):
+        self._set_attr("dividerColor", value)
+
+    # indicator_color
+    @property
+    def indicator_color(self) -> Optional[str]:
+        return self._get_attr("indicatorColor")
+
+    @indicator_color.setter
+    def indicator_color(self, value: Optional[str]):
+        self._set_attr("indicatorColor", value)
+
+    # indicator_border_radius
+    @property
+    def indicator_border_radius(self) -> BorderRadiusValue:
+        return self.__indicator_border_radius
+
+    @indicator_border_radius.setter
+    def indicator_border_radius(self, value: BorderRadiusValue):
+        self.__indicator_border_radius = value
+
+    # indicator_border_side
+    @property
+    def indicator_border_side(self) -> Optional[BorderSide]:
+        return self.__indicator_border_side
+
+    @indicator_border_side.setter
+    def indicator_border_side(self, value: Optional[BorderSide]):
+        self.__indicator_border_side = value
+
+    # indicator_padding
+    @property
+    def indicator_padding(self) -> PaddingValue:
+        return self.__indicator_padding
+
+    @indicator_padding.setter
+    def indicator_padding(self, value: PaddingValue):
+        self.__indicator_padding = value
+
+    # indicator_tab_size
+    @property
+    def indicator_tab_size(self) -> Optional[bool]:
+        return self._get_attr("indicatorTabSize", data_type="bool", def_value=False)
+
+    @indicator_tab_size.setter
+    def indicator_tab_size(self, value: Optional[bool]):
+        self._set_attr("indicatorTabSize", value)
+
+    # label_color
+    @property
+    def label_color(self) -> Optional[str]:
+        return self._get_attr("labelColor")
+
+    @label_color.setter
+    def label_color(self, value: Optional[str]):
+        self._set_attr("labelColor", value)
+
+    # unselected_label_color
+    @property
+    def unselected_label_color(self) -> Optional[str]:
+        return self._get_attr("unselectedLabelColor")
+
+    @unselected_label_color.setter
+    def unselected_label_color(self, value: Optional[str]):
+        self._set_attr("unselectedLabelColor", value)
+
+    # overlay_color
+    @property
+    def overlay_color(self) -> Union[None, str, Dict[MaterialState, str]]:
+        return self.__overlay_color
+
+    @overlay_color.setter
+    def overlay_color(self, value: Union[None, str, Dict[MaterialState, str]]):
+        self.__overlay_color = value
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/template_route.py` & `flet_core-0.7.0.dev1395/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/text.py` & `flet_core-0.7.0.dev1395/src/flet_core/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     Online docs: https://flet.dev/docs/controls/text
     """
 
     def __init__(
         self,
         value: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -144,14 +145,15 @@
         color: Optional[str] = None,
         bgcolor: Optional[str] = None,
         semantics_label: Optional[str] = None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/text_button.py` & `flet_core-0.7.0.dev1395/src/flet_core/text_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Online docs: https://flet.dev/docs/controls/textbutton
     """
 
     def __init__(
         self,
         text: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
         bottom: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
@@ -80,14 +81,15 @@
         on_hover=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             left=left,
             top=top,
             right=right,
             bottom=bottom,
             expand=expand,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/text_span.py` & `flet_core-0.7.0.dev1395/src/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/text_style.py` & `flet_core-0.7.0.dev1395/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/textfield.py` & `flet_core-0.7.0.dev1395/src/flet_core/textfield.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 
     Online docs: https://flet.dev/docs/controls/textfield
     """
 
     def __init__(
         self,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         expand: Union[None, bool, int] = None,
         col: Optional[ResponsiveNumber] = None,
         opacity: OptionalNumber = None,
         rotate: RotateValue = None,
         scale: ScaleValue = None,
@@ -178,14 +179,15 @@
         on_submit=None,
         on_focus=None,
         on_blur=None,
     ):
         FormFieldControl.__init__(
             self,
             ref=ref,
+            key=key,
             width=width,
             height=height,
             expand=expand,
             col=col,
             opacity=opacity,
             rotate=rotate,
             scale=scale,
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/tooltip.py` & `flet_core-0.7.0.dev1395/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/transform.py` & `flet_core-0.7.0.dev1395/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/transparent_pointer.py` & `flet_core-0.7.0.dev1395/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/types.py` & `flet_core-0.7.0.dev1395/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/user_control.py` & `flet_core-0.7.0.dev1395/src/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/vertical_divider.py` & `flet_core-0.7.0.dev1395/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/view.py` & `flet_core-0.7.0.dev1395/src/flet_core/view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from flet_core import Control
 from flet_core.app_bar import AppBar
 from flet_core.control import OptionalNumber
 from flet_core.floating_action_button import FloatingActionButton
 from flet_core.navigation_bar import NavigationBar
+from flet_core.scrollable_control import ScrollableControl
 from flet_core.types import (
     CrossAxisAlignment,
     CrossAxisAlignmentString,
     MainAxisAlignment,
     MainAxisAlignmentString,
     PaddingValue,
     ScrollMode,
     ScrollModeString,
 )
 
 
-class View(Control):
+class View(ScrollableControl):
     """
     View is the top most container for all other controls.
 
     A root view is automatically created when a new user session started. From layout perspective the View represents a `Column`(https://flet.dev/docs/controls/column/) control, so it has a similar behavior and shares same properties.
 
     -----
 
@@ -35,19 +36,32 @@
         floating_action_button: Optional[FloatingActionButton] = None,
         navigation_bar: Optional[NavigationBar] = None,
         vertical_alignment: MainAxisAlignment = MainAxisAlignment.NONE,
         horizontal_alignment: CrossAxisAlignment = CrossAxisAlignment.NONE,
         spacing: OptionalNumber = None,
         padding: PaddingValue = None,
         bgcolor: Optional[str] = None,
+        #
+        # ScrollableControl specific
+        #
         scroll: Optional[ScrollMode] = None,
         auto_scroll: Optional[bool] = None,
+        on_scroll_interval: OptionalNumber = None,
+        on_scroll: Any = None,
     ):
         Control.__init__(self)
 
+        ScrollableControl.__init__(
+            self,
+            scroll=scroll,
+            auto_scroll=auto_scroll,
+            on_scroll_interval=on_scroll_interval,
+            on_scroll=on_scroll,
+        )
+
         self.controls = controls if controls is not None else []
         self.route = route
         self.appbar = appbar
         self.navigation_bar = navigation_bar
         self.floating_action_button = floating_action_button
         self.vertical_alignment = vertical_alignment
         self.horizontal_alignment = horizontal_alignment
@@ -174,36 +188,7 @@
     @property
     def bgcolor(self):
         return self._get_attr("bgcolor")
 
     @bgcolor.setter
     def bgcolor(self, value):
         self._set_attr("bgcolor", value)
-
-    # scroll
-    @property
-    def scroll(self) -> Optional[ScrollMode]:
-        return self.__scroll
-
-    @scroll.setter
-    def scroll(self, value: Optional[ScrollMode]):
-        self.__scroll = value
-        if isinstance(value, ScrollMode):
-            self._set_attr("scroll", value.value)
-        else:
-            self.__set_scroll(value)
-
-    def __set_scroll(self, value: Optional[ScrollModeString]):
-        if value is True:
-            value = "auto"
-        elif value is False:
-            value = None
-        self._set_attr("scroll", value)
-
-    # auto_scroll
-    @property
-    def auto_scroll(self) -> Optional[bool]:
-        return self._get_attr("autoScroll")
-
-    @auto_scroll.setter
-    def auto_scroll(self, value: Optional[bool]):
-        self._set_attr("autoScroll", value)
```

### Comparing `flet_core-0.7.0.dev1372/src/flet_core/window_drag_area.py` & `flet_core-0.7.0.dev1395/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.7.0.dev1372/PKG-INFO` & `flet_core-0.7.0.dev1395/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-core
-Version: 0.7.0.dev1372
+Version: 0.7.0.dev1395
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

